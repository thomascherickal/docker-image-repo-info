## `redis:alpine`

```console
$ docker pull redis@sha256:b0fa8a1a94f8556ca4a526a135730e9eb25c046dc38c7520d145a4604dc10c5b
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
$ docker pull redis@sha256:bfc2818d0367c9771b79fa5850933c0129d6da2dba9c56e6ebffe697bc16ec0b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.0 MB (10969988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7b388ce3d39eb5558af143a66ab79016e851a2e6cf04ba09100b33e23c4e396`
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
# Wed, 22 Jul 2020 01:22:13 GMT
ENV REDIS_VERSION=6.0.6
# Wed, 22 Jul 2020 01:22:14 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.6.tar.gz
# Wed, 22 Jul 2020 01:22:14 GMT
ENV REDIS_DOWNLOAD_SHA=12ad49b163af5ef39466e8d2f7d212a58172116e5b441eebecb4e6ca22363d94
# Wed, 22 Jul 2020 01:24:11 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Wed, 22 Jul 2020 01:24:13 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 22 Jul 2020 01:24:13 GMT
VOLUME [/data]
# Wed, 22 Jul 2020 01:24:14 GMT
WORKDIR /data
# Wed, 22 Jul 2020 01:24:14 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Wed, 22 Jul 2020 01:24:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 01:24:15 GMT
EXPOSE 6379
# Wed, 22 Jul 2020 01:24:15 GMT
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
	-	`sha256:660ad543c5fcdf05cfe4c188017b80587aa4c56dc27b14fbf09c65256721c284`  
		Last Modified: Wed, 22 Jul 2020 01:27:30 GMT  
		Size: 7.8 MB (7790052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823cbe4f5025627f7c303d30925645c8e11c22fa2ec2eba4f1e3337125a696e4`  
		Last Modified: Wed, 22 Jul 2020 01:27:28 GMT  
		Size: 99.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3dd0c30e1c8e144888490e76c9c7ed6397d9d800d8695fc91951de5e0dadb2b`  
		Last Modified: Wed, 22 Jul 2020 01:27:28 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:alpine` - linux; arm variant v6

```console
$ docker pull redis@sha256:33505b074d4b48dffa997855f6bec4a865c1ae01c66b49dbea613d566ec70f90
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.7 MB (10661036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5a8a290a3928930ad754bcea7386d1ba8bbf38f25d78e60835e5e84bfa17064`
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
# Tue, 21 Jul 2020 23:29:51 GMT
ENV REDIS_VERSION=6.0.6
# Tue, 21 Jul 2020 23:29:52 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.6.tar.gz
# Tue, 21 Jul 2020 23:29:53 GMT
ENV REDIS_DOWNLOAD_SHA=12ad49b163af5ef39466e8d2f7d212a58172116e5b441eebecb4e6ca22363d94
# Tue, 21 Jul 2020 23:30:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Tue, 21 Jul 2020 23:30:45 GMT
RUN mkdir /data && chown redis:redis /data
# Tue, 21 Jul 2020 23:30:46 GMT
VOLUME [/data]
# Tue, 21 Jul 2020 23:30:48 GMT
WORKDIR /data
# Tue, 21 Jul 2020 23:30:49 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Tue, 21 Jul 2020 23:30:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Jul 2020 23:30:53 GMT
EXPOSE 6379
# Tue, 21 Jul 2020 23:30:54 GMT
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
	-	`sha256:473199eb9d3be10eb63f89c36ab6c5115693ea95d744a9845dbc1476f841f39b`  
		Last Modified: Tue, 21 Jul 2020 23:33:08 GMT  
		Size: 7.7 MB (7671938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c256f417029671b534f58dc2f665f0d5863028e68c4373068a90b1e69edf7f5`  
		Last Modified: Tue, 21 Jul 2020 23:33:06 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9230cc619eb842a033ee0a8a19966c2e9ef54b9d677389d4e68a404d3562189`  
		Last Modified: Tue, 21 Jul 2020 23:33:06 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:alpine` - linux; arm variant v7

```console
$ docker pull redis@sha256:32beaff27c543fc8787d06e552602f9459110b23be3241ee84ecbf52ef7547f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.3 MB (10303476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a3bfc351f4a5e7583aba901f130b98935cfcce5f233fdf2e8ed7e1f42b53568`
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
# Wed, 22 Jul 2020 00:22:45 GMT
ENV REDIS_VERSION=6.0.6
# Wed, 22 Jul 2020 00:22:45 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.6.tar.gz
# Wed, 22 Jul 2020 00:22:46 GMT
ENV REDIS_DOWNLOAD_SHA=12ad49b163af5ef39466e8d2f7d212a58172116e5b441eebecb4e6ca22363d94
# Wed, 22 Jul 2020 00:23:32 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Wed, 22 Jul 2020 00:23:34 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 22 Jul 2020 00:23:35 GMT
VOLUME [/data]
# Wed, 22 Jul 2020 00:23:35 GMT
WORKDIR /data
# Wed, 22 Jul 2020 00:23:36 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Wed, 22 Jul 2020 00:23:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 00:23:37 GMT
EXPOSE 6379
# Wed, 22 Jul 2020 00:23:38 GMT
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
	-	`sha256:b5c8616b8c57bcece63f9d60eb32abd9db74ae9898f465f7fab03277f9377f99`  
		Last Modified: Wed, 22 Jul 2020 00:25:31 GMT  
		Size: 7.5 MB (7517310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270e2484d52cee8912e86828dde5119637d2aa88548f97b6d43be8f7f29dd6f2`  
		Last Modified: Wed, 22 Jul 2020 00:25:28 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b3097fb9d4bae7b869189d654263becf0be6c63175d3f07c3af7fa705248450`  
		Last Modified: Wed, 22 Jul 2020 00:25:28 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:alpine` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:d8e196ceda25bdb3cc76ed528f94f9f4c6adf6a9c2be566767dca4b2873f095e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.9 MB (10881785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25c2f3bdf63c1ff68b593d596f51c43befb60bc005a899341aba68c047d15725`
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
# Wed, 22 Jul 2020 00:05:38 GMT
ENV REDIS_VERSION=6.0.6
# Wed, 22 Jul 2020 00:05:39 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.6.tar.gz
# Wed, 22 Jul 2020 00:05:41 GMT
ENV REDIS_DOWNLOAD_SHA=12ad49b163af5ef39466e8d2f7d212a58172116e5b441eebecb4e6ca22363d94
# Wed, 22 Jul 2020 00:06:32 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Wed, 22 Jul 2020 00:06:35 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 22 Jul 2020 00:06:36 GMT
VOLUME [/data]
# Wed, 22 Jul 2020 00:06:38 GMT
WORKDIR /data
# Wed, 22 Jul 2020 00:06:39 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Wed, 22 Jul 2020 00:06:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 00:06:40 GMT
EXPOSE 6379
# Wed, 22 Jul 2020 00:06:41 GMT
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
	-	`sha256:2e7e0b09507610ddcfc0db519f67dea00ae27ae891cb2f09a95fdd24b7ce5ba1`  
		Last Modified: Wed, 22 Jul 2020 00:09:20 GMT  
		Size: 7.8 MB (7788942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:086ac853329b27e6045965453c1cbbdce01fdd7224c909a7ef27dc6d60ae2820`  
		Last Modified: Wed, 22 Jul 2020 00:09:15 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:548fb98385301185df27623df62ff36e35d4d95679acf2cbf6775dccdeda6e18`  
		Last Modified: Wed, 22 Jul 2020 00:09:15 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:alpine` - linux; 386

```console
$ docker pull redis@sha256:9efcf2d4a3a3d21b54d1f9942664c4741fed147d455315e5b3f78a61bf1dc5d6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.6 MB (10649871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce6e4fa9639e9c0658bfd21d3bcedc7da0cfdb8f6bc918f3caf01a4e0912b658`
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
# Tue, 01 Sep 2020 21:40:31 GMT
ENV REDIS_VERSION=6.0.7
# Tue, 01 Sep 2020 21:40:31 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.7.tar.gz
# Tue, 01 Sep 2020 21:40:32 GMT
ENV REDIS_DOWNLOAD_SHA=c2aaa1a4c7e72c70adedf976fdd5e1d34d395989283dab9d7840e0a304bb2393
# Tue, 01 Sep 2020 21:41:59 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Tue, 01 Sep 2020 21:42:01 GMT
RUN mkdir /data && chown redis:redis /data
# Tue, 01 Sep 2020 21:42:01 GMT
VOLUME [/data]
# Tue, 01 Sep 2020 21:42:01 GMT
WORKDIR /data
# Tue, 01 Sep 2020 21:42:02 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Tue, 01 Sep 2020 21:42:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Sep 2020 21:42:03 GMT
EXPOSE 6379
# Tue, 01 Sep 2020 21:42:03 GMT
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
	-	`sha256:1af891067e51ef39400fa2cc69bae0b96f8857f7303779dcab7ef6af951cb729`  
		Last Modified: Tue, 01 Sep 2020 21:42:50 GMT  
		Size: 7.5 MB (7469648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1527543b45ddd9e5cb1670f4f9708312676d1af05acec3572494cdcbf226634c`  
		Last Modified: Tue, 01 Sep 2020 21:42:48 GMT  
		Size: 99.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f81bf33082a4eb587713a42b604ebfec5c3cb21653f9115a56fa9751d39125b1`  
		Last Modified: Tue, 01 Sep 2020 21:42:48 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:alpine` - linux; ppc64le

```console
$ docker pull redis@sha256:f064ab9a888c556f2dcc79478c6c4a5d210d786f92be6bbce6bd10935bd36550
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.5 MB (11483904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee09524c0f4dd7d68ebde961c99ff219969be48226a0a58bc281e5b713544b47`
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
# Wed, 22 Jul 2020 01:45:34 GMT
ENV REDIS_VERSION=6.0.6
# Wed, 22 Jul 2020 01:45:36 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.6.tar.gz
# Wed, 22 Jul 2020 01:45:38 GMT
ENV REDIS_DOWNLOAD_SHA=12ad49b163af5ef39466e8d2f7d212a58172116e5b441eebecb4e6ca22363d94
# Wed, 22 Jul 2020 01:46:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Wed, 22 Jul 2020 01:46:48 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 22 Jul 2020 01:46:51 GMT
VOLUME [/data]
# Wed, 22 Jul 2020 01:47:02 GMT
WORKDIR /data
# Wed, 22 Jul 2020 01:47:05 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Wed, 22 Jul 2020 01:47:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jul 2020 01:47:21 GMT
EXPOSE 6379
# Wed, 22 Jul 2020 01:47:24 GMT
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
	-	`sha256:c0b156d64f477f6318c9a07306a30c65306dd6df98e8f61e3aed81acba598ee6`  
		Last Modified: Wed, 22 Jul 2020 01:50:26 GMT  
		Size: 8.3 MB (8289265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5b08bac6cd6cc2bac474103ab9195e1ed33bfd2b53dd1784bb283b16d2a5d3`  
		Last Modified: Wed, 22 Jul 2020 01:50:24 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b3d539bb36ffa37c2f536ffbdb40ae55c68da2a388687dec692b5487cc33fb8`  
		Last Modified: Wed, 22 Jul 2020 01:50:23 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:alpine` - linux; s390x

```console
$ docker pull redis@sha256:b91e20e3e316e3ec818257ee25adb724c11bde25935a986ebd2050eba71a55ce
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.0 MB (11025412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4bd0026fd69616a6587c12b7a8abb6a7407dc73baf56e50d03d4921185aae02`
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
# Tue, 01 Sep 2020 21:42:43 GMT
ENV REDIS_VERSION=6.0.7
# Tue, 01 Sep 2020 21:42:43 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.7.tar.gz
# Tue, 01 Sep 2020 21:42:44 GMT
ENV REDIS_DOWNLOAD_SHA=c2aaa1a4c7e72c70adedf976fdd5e1d34d395989283dab9d7840e0a304bb2393
# Tue, 01 Sep 2020 21:43:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Tue, 01 Sep 2020 21:43:30 GMT
RUN mkdir /data && chown redis:redis /data
# Tue, 01 Sep 2020 21:43:30 GMT
VOLUME [/data]
# Tue, 01 Sep 2020 21:43:31 GMT
WORKDIR /data
# Tue, 01 Sep 2020 21:43:31 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Tue, 01 Sep 2020 21:43:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Sep 2020 21:43:32 GMT
EXPOSE 6379
# Tue, 01 Sep 2020 21:43:32 GMT
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
	-	`sha256:e2f6e6374f84abac9f6f76a7b42f0a40e99cc1c5c6bded656be43298538373ff`  
		Last Modified: Tue, 01 Sep 2020 21:44:21 GMT  
		Size: 8.1 MB (8071922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bec737f4476c6e7f10842648c8c582e762b9cb90c6ecbfe2ec7a8b918d7070f`  
		Last Modified: Tue, 01 Sep 2020 21:44:19 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1c2a7ae99040f4191c5b1c33a68eada94c62ac04298843dce2c310b4c3b46b`  
		Last Modified: Tue, 01 Sep 2020 21:44:19 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
