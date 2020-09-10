## `redis:alpine`

```console
$ docker pull redis@sha256:328b8c7fc82e6d13bf3ff442a84d27c2972e6f98f4b606704657d6516ee69e80
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

### `redis:alpine` - linux; amd64

```console
$ docker pull redis@sha256:a6e7c197527f8f73a3f37f3b1a3e77c95530359ce1f1a572f940f4bd1843f53b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.0 MB (10986001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd71e6db4a54eb70734ea6c7792f701328cc9001fce5a9e0941a2ad9a6bc6d29`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Thu, 04 Jun 2020 22:33:29 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Thu, 04 Jun 2020 22:33:30 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Thu, 10 Sep 2020 19:14:26 GMT
ENV REDIS_VERSION=6.0.8
# Thu, 10 Sep 2020 19:14:26 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.8.tar.gz
# Thu, 10 Sep 2020 19:14:26 GMT
ENV REDIS_DOWNLOAD_SHA=04fa1fddc39bd1aecb6739dd5dd73858a3515b427acd1e2947a66dadce868d68
# Thu, 10 Sep 2020 19:15:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Thu, 10 Sep 2020 19:15:45 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 10 Sep 2020 19:15:45 GMT
VOLUME [/data]
# Thu, 10 Sep 2020 19:15:45 GMT
WORKDIR /data
# Thu, 10 Sep 2020 19:15:46 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Thu, 10 Sep 2020 19:15:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Sep 2020 19:15:46 GMT
EXPOSE 6379
# Thu, 10 Sep 2020 19:15:46 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b8c029ceab510ffd36b89e8ddb97a446ab5700dd954eeecd02e500e6dec4852`  
		Last Modified: Thu, 04 Jun 2020 22:36:07 GMT  
		Size: 1.2 KB (1227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e983a1eb737a9b9ab5e8c2846e18b0cda41703c68bc7e47a8482b4011a78592c`  
		Last Modified: Thu, 04 Jun 2020 22:36:07 GMT  
		Size: 380.7 KB (380655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de9de2cb6149eafb96b3084de239660a2b9ccd6fe875174746c51a529c7fd5d8`  
		Last Modified: Thu, 10 Sep 2020 19:18:58 GMT  
		Size: 7.8 MB (7806064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a04900c891eb6f7481831116ace8fde5eccfc61e7ed7f820ecf79d8a68c08e7`  
		Last Modified: Thu, 10 Sep 2020 19:18:56 GMT  
		Size: 100.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be5e938aa8ffe1560c9778f21147f73ee43a3271cfba78a5900efba06a5d2fde`  
		Last Modified: Thu, 10 Sep 2020 19:18:57 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:alpine` - linux; arm variant v6

```console
$ docker pull redis@sha256:f4a6209a87ee505bc69440582b301b1b8a3bf1f4155bdd0acb00f522047c0a71
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.7 MB (10675570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0a9a658fbeafd5bf0d5c103e59ee02f8d68f109247aa7e84b24676f0fd0b0e4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Thu, 04 Jun 2020 22:55:15 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Thu, 04 Jun 2020 22:55:18 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Thu, 10 Sep 2020 17:57:15 GMT
ENV REDIS_VERSION=6.0.8
# Thu, 10 Sep 2020 17:57:21 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.8.tar.gz
# Thu, 10 Sep 2020 17:57:24 GMT
ENV REDIS_DOWNLOAD_SHA=04fa1fddc39bd1aecb6739dd5dd73858a3515b427acd1e2947a66dadce868d68
# Thu, 10 Sep 2020 17:58:36 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Thu, 10 Sep 2020 17:58:56 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 10 Sep 2020 17:59:01 GMT
VOLUME [/data]
# Thu, 10 Sep 2020 17:59:04 GMT
WORKDIR /data
# Thu, 10 Sep 2020 17:59:08 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Thu, 10 Sep 2020 17:59:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Sep 2020 17:59:14 GMT
EXPOSE 6379
# Thu, 10 Sep 2020 17:59:17 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2491f7cfcf9c696e17ac4e1826543b0841d1a6d4067364396768b07a5ed10d2d`  
		Last Modified: Thu, 04 Jun 2020 22:57:54 GMT  
		Size: 1.3 KB (1253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6dc1c58292fd74a4a2f0afcf684683f24d2c84aff9c8e60f1b79ab451e15c19`  
		Last Modified: Thu, 04 Jun 2020 22:57:54 GMT  
		Size: 384.0 KB (384009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a682f20ccd048f15042b0795ad86c53dcbda31f43c11433ccc322fa606efc35`  
		Last Modified: Thu, 10 Sep 2020 17:59:44 GMT  
		Size: 7.7 MB (7686469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d81098731454adddc735ccce337449a13a85fddfa5769c295ae8e18c61423e6f`  
		Last Modified: Thu, 10 Sep 2020 17:59:42 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f384c5506f420a142502bc1cb16db626a349b6374e55b2dc9a1bc3b9b4bd3d51`  
		Last Modified: Thu, 10 Sep 2020 17:59:42 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:alpine` - linux; arm variant v7

```console
$ docker pull redis@sha256:7aef6cbf11ed78660db387330b97ced46cf75073310f17bcf0320d585133845f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.3 MB (10315770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bd2a94610818a6f2b4f327bb74c98e118f47900d8852e916c9a4df162e440d9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Thu, 04 Jun 2020 21:58:41 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Thu, 04 Jun 2020 21:58:44 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Thu, 10 Sep 2020 18:06:00 GMT
ENV REDIS_VERSION=6.0.8
# Thu, 10 Sep 2020 18:06:08 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.8.tar.gz
# Thu, 10 Sep 2020 18:06:14 GMT
ENV REDIS_DOWNLOAD_SHA=04fa1fddc39bd1aecb6739dd5dd73858a3515b427acd1e2947a66dadce868d68
# Thu, 10 Sep 2020 18:07:35 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Thu, 10 Sep 2020 18:08:02 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 10 Sep 2020 18:08:10 GMT
VOLUME [/data]
# Thu, 10 Sep 2020 18:08:19 GMT
WORKDIR /data
# Thu, 10 Sep 2020 18:08:31 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Thu, 10 Sep 2020 18:08:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Sep 2020 18:08:53 GMT
EXPOSE 6379
# Thu, 10 Sep 2020 18:09:05 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84e032461d169a86565d092c6a802fca065f93a26a09f8863354d32847f9e3ff`  
		Last Modified: Thu, 04 Jun 2020 22:01:06 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b3deaa50a54fd0aba551155315c34af4ebfcd8f651178f1992540a5f0a024a`  
		Last Modified: Thu, 04 Jun 2020 22:01:08 GMT  
		Size: 377.6 KB (377597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d9cf6897e045e3396dbcf2c5550be8ffdd14a1517f4a912423064d923303ee`  
		Last Modified: Thu, 10 Sep 2020 18:15:18 GMT  
		Size: 7.5 MB (7529602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b923e4a6c876402b2658b57da0e034f6779c89f98543d4c59f6807aef57b5ae`  
		Last Modified: Thu, 10 Sep 2020 18:15:15 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb668df52637a7e06e40dfbc8a3ccc1ef1d73e0c308570ea4c981f7ace38689e`  
		Last Modified: Thu, 10 Sep 2020 18:15:15 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:alpine` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:55813df4e251324a7adedbceb03b816cb171e4f5af9affe29bf1420827538d8b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.9 MB (10900275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80fba8f7d3f9572b344c89d91ab3241e4f78e2e607388a64fe96d3d525a77d93`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Thu, 04 Jun 2020 22:52:14 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Thu, 04 Jun 2020 22:52:17 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Thu, 10 Sep 2020 19:37:29 GMT
ENV REDIS_VERSION=6.0.8
# Thu, 10 Sep 2020 19:37:30 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.8.tar.gz
# Thu, 10 Sep 2020 19:37:31 GMT
ENV REDIS_DOWNLOAD_SHA=04fa1fddc39bd1aecb6739dd5dd73858a3515b427acd1e2947a66dadce868d68
# Thu, 10 Sep 2020 19:38:23 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Thu, 10 Sep 2020 19:38:26 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 10 Sep 2020 19:38:27 GMT
VOLUME [/data]
# Thu, 10 Sep 2020 19:38:28 GMT
WORKDIR /data
# Thu, 10 Sep 2020 19:38:29 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Thu, 10 Sep 2020 19:38:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Sep 2020 19:38:31 GMT
EXPOSE 6379
# Thu, 10 Sep 2020 19:38:32 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4ce967624268d2fc70fda2e1a83da9d436c27153f185bdd30342587b2456a8c`  
		Last Modified: Thu, 04 Jun 2020 22:55:00 GMT  
		Size: 1.3 KB (1254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbfc97b74d7061059d7d0ea2b506592ca4d39cf2462555b9d96de62bbdacb419`  
		Last Modified: Thu, 04 Jun 2020 22:55:00 GMT  
		Size: 383.1 KB (383077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:853be217661793e1d32b22cd3c0adca419cd4f583eb796db9d106b78f38ebbb7`  
		Last Modified: Thu, 10 Sep 2020 19:41:39 GMT  
		Size: 7.8 MB (7807431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:792981fe6267b6eed3b23d0c46a0275bd235aea564551e377e54b16fc5544a2c`  
		Last Modified: Thu, 10 Sep 2020 19:41:36 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ddc4636cc530017b1e4d4637014e113a9cf81e7019c17804cb9299ee4f235ae`  
		Last Modified: Thu, 10 Sep 2020 19:41:36 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:alpine` - linux; 386

```console
$ docker pull redis@sha256:ce524b38924f44cbf873c5eff4da397b2fd21172c10f290ae7f60f32b442d54f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.7 MB (10651321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf56f55a82f84f855d6c8528f06c840b2c4d92233c491b3faa139234b8c53c9b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Thu, 04 Jun 2020 22:44:17 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Thu, 04 Jun 2020 22:44:19 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Thu, 10 Sep 2020 21:39:22 GMT
ENV REDIS_VERSION=6.0.8
# Thu, 10 Sep 2020 21:39:22 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.8.tar.gz
# Thu, 10 Sep 2020 21:39:22 GMT
ENV REDIS_DOWNLOAD_SHA=04fa1fddc39bd1aecb6739dd5dd73858a3515b427acd1e2947a66dadce868d68
# Thu, 10 Sep 2020 21:41:45 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Thu, 10 Sep 2020 21:41:47 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 10 Sep 2020 21:41:47 GMT
VOLUME [/data]
# Thu, 10 Sep 2020 21:41:48 GMT
WORKDIR /data
# Thu, 10 Sep 2020 21:41:48 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Thu, 10 Sep 2020 21:41:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Sep 2020 21:41:49 GMT
EXPOSE 6379
# Thu, 10 Sep 2020 21:41:49 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b628b8d7bee24f7032c92603ba89a235d5945514d906c4848a75669b0f787ab8`  
		Last Modified: Thu, 04 Jun 2020 22:47:17 GMT  
		Size: 1.2 KB (1227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ca4f94d24ace225a77b0d0ba2ee230994a7f23f01bc896f54dc8ea152dbdfd9`  
		Last Modified: Thu, 04 Jun 2020 22:47:17 GMT  
		Size: 386.2 KB (386181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4ae258c5f255d66074b581a760e38fcdad650dbf11b2aee2f32e731086c0d45`  
		Last Modified: Thu, 10 Sep 2020 21:43:00 GMT  
		Size: 7.5 MB (7471100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c81db9595bae0523b6eb44843c4cfe3933897858e6a675e16a89b738d1f49ed0`  
		Last Modified: Thu, 10 Sep 2020 21:42:57 GMT  
		Size: 100.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2abac4824ba72316df56a71f26a82df3f6d787865e25bde36c9e17accd05fe5`  
		Last Modified: Thu, 10 Sep 2020 21:42:57 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:alpine` - linux; ppc64le

```console
$ docker pull redis@sha256:9cdc08f8aea75904c146174a69ad7ab565c4553ef5f11abc1bceac29a0e25c29
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.5 MB (11497299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24ed6992c4e88114bebfef52af43be2cc0a295f804c7391eb3e6fe860fbbf094`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Thu, 04 Jun 2020 22:32:42 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Thu, 04 Jun 2020 22:32:53 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Wed, 02 Sep 2020 03:17:02 GMT
ENV REDIS_VERSION=6.0.7
# Wed, 02 Sep 2020 03:17:09 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.7.tar.gz
# Wed, 02 Sep 2020 03:17:13 GMT
ENV REDIS_DOWNLOAD_SHA=c2aaa1a4c7e72c70adedf976fdd5e1d34d395989283dab9d7840e0a304bb2393
# Wed, 02 Sep 2020 03:18:08 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Wed, 02 Sep 2020 03:18:22 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 02 Sep 2020 03:18:26 GMT
VOLUME [/data]
# Wed, 02 Sep 2020 03:18:32 GMT
WORKDIR /data
# Wed, 02 Sep 2020 03:18:34 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Wed, 02 Sep 2020 03:18:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Sep 2020 03:18:40 GMT
EXPOSE 6379
# Wed, 02 Sep 2020 03:18:45 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0a4eed06b46f74c11d91aa424485bad52c09b5607c232345340403d82d43992`  
		Last Modified: Thu, 04 Jun 2020 22:37:30 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705f70508e8f57ad781a7cbe3d67807948e3219d2118cf0c0f191ed66345d1d3`  
		Last Modified: Thu, 04 Jun 2020 22:37:31 GMT  
		Size: 387.6 KB (387630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9407a96f08af26031174ea91a8052cf5163acdd4f8ebbd667d106f2c55770264`  
		Last Modified: Wed, 02 Sep 2020 03:19:58 GMT  
		Size: 8.3 MB (8302660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:695bbb49dc0c42b1bc4e50c691691dc3b95635451d11491adc9200c2936a85b4`  
		Last Modified: Wed, 02 Sep 2020 03:19:56 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d76c99943af4ab262712956a885e0ab83668c1f3f205c2e8f1f8666fdff61f4`  
		Last Modified: Wed, 02 Sep 2020 03:19:56 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:alpine` - linux; s390x

```console
$ docker pull redis@sha256:3db38803536a7550b18dd03d4a40321619103e73dc2ff89bec2b7a6797ffeac2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.0 MB (11027244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4aedd08fbe281f75c3e1b78736f485ab4eac6d09f9f7441d990a549e4e356ebe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Thu, 04 Jun 2020 22:49:22 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Thu, 04 Jun 2020 22:49:23 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Thu, 10 Sep 2020 17:43:09 GMT
ENV REDIS_VERSION=6.0.8
# Thu, 10 Sep 2020 17:43:09 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.8.tar.gz
# Thu, 10 Sep 2020 17:43:09 GMT
ENV REDIS_DOWNLOAD_SHA=04fa1fddc39bd1aecb6739dd5dd73858a3515b427acd1e2947a66dadce868d68
# Thu, 10 Sep 2020 17:43:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Thu, 10 Sep 2020 17:43:43 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 10 Sep 2020 17:43:43 GMT
VOLUME [/data]
# Thu, 10 Sep 2020 17:43:43 GMT
WORKDIR /data
# Thu, 10 Sep 2020 17:43:43 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Thu, 10 Sep 2020 17:43:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Sep 2020 17:43:44 GMT
EXPOSE 6379
# Thu, 10 Sep 2020 17:43:44 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c338feeb97fe0a2fb1ad44e709e15721daf32f3607235e92e8c6189725da76`  
		Last Modified: Thu, 04 Jun 2020 22:50:55 GMT  
		Size: 1.3 KB (1253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3e4b07b0ef1066cf476f86bb29ccfc959007a13fed6acef2b2b9ea50b112945`  
		Last Modified: Thu, 04 Jun 2020 22:50:55 GMT  
		Size: 385.5 KB (385498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef47eb6249a5bfb7044711856b643ccb8029f34aef2acd8a3399d90f62338a1e`  
		Last Modified: Thu, 10 Sep 2020 17:44:29 GMT  
		Size: 8.1 MB (8073754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:214c3688f3dc0841edfb41c37f10fbeb76ba98aa6bf14a98a17b68f65b6ad880`  
		Last Modified: Thu, 10 Sep 2020 17:44:27 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4fdcd063ee4d1040672e72ee19a818fcfdf0ab641fbc27bd1a911750928f2ff`  
		Last Modified: Thu, 10 Sep 2020 17:44:28 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
