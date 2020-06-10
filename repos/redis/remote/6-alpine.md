## `redis:6-alpine`

```console
$ docker pull redis@sha256:b7561e4e994ab52cb2062b9c3e943ab2af3287caf9d9aeb6719acc77013769a5
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
$ docker pull redis@sha256:4ad74bee4b84a7592ee5259f49633f38cd483708c340ad513c8633587524e6cf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.6 MB (10578272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b546e82a6d0eceb411b424487643c8d5224cb12a74b6175469991ce2e78c42d1`
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
# Wed, 10 Jun 2020 09:46:57 GMT
ENV REDIS_VERSION=6.0.5
# Wed, 10 Jun 2020 09:46:57 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.5.tar.gz
# Wed, 10 Jun 2020 09:46:57 GMT
ENV REDIS_DOWNLOAD_SHA=42cf86a114d2a451b898fcda96acd4d01062a7dbaaad2801d9164a36f898f596
# Wed, 10 Jun 2020 09:47:55 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Wed, 10 Jun 2020 09:47:56 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 10 Jun 2020 09:47:56 GMT
VOLUME [/data]
# Wed, 10 Jun 2020 09:47:56 GMT
WORKDIR /data
# Wed, 10 Jun 2020 09:47:56 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Wed, 10 Jun 2020 09:47:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Jun 2020 09:47:57 GMT
EXPOSE 6379
# Wed, 10 Jun 2020 09:47:57 GMT
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
	-	`sha256:18cbc0ec1809e3eaf7385a5cfab30fde97ee9d3dea7b36b09887cfc58d5aa227`  
		Last Modified: Wed, 10 Jun 2020 09:48:36 GMT  
		Size: 7.4 MB (7398335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ec7a0dc6d885d4d980018127fd9ea8ee5cc98770af746f0adb0864f2236944`  
		Last Modified: Wed, 10 Jun 2020 09:48:34 GMT  
		Size: 99.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cefbc91f729f5741ab4f1b04a8d3b66785a58149332496cbfed607e9445e29`  
		Last Modified: Wed, 10 Jun 2020 09:48:34 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine` - linux; arm variant v6

```console
$ docker pull redis@sha256:b602c0551173a14df3db4e5d2ec758580ba09a279494860d118ee80c02823c62
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.3 MB (10270606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13c00c05c95a15a6a3e48934b2741a39317235376f414dbd8665bd9b919c3463`
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
# Tue, 09 Jun 2020 22:40:56 GMT
ENV REDIS_VERSION=6.0.5
# Tue, 09 Jun 2020 22:40:57 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.5.tar.gz
# Tue, 09 Jun 2020 22:40:58 GMT
ENV REDIS_DOWNLOAD_SHA=42cf86a114d2a451b898fcda96acd4d01062a7dbaaad2801d9164a36f898f596
# Tue, 09 Jun 2020 22:41:51 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Tue, 09 Jun 2020 22:41:54 GMT
RUN mkdir /data && chown redis:redis /data
# Tue, 09 Jun 2020 22:41:56 GMT
VOLUME [/data]
# Tue, 09 Jun 2020 22:41:57 GMT
WORKDIR /data
# Tue, 09 Jun 2020 22:41:58 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Tue, 09 Jun 2020 22:41:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Jun 2020 22:42:00 GMT
EXPOSE 6379
# Tue, 09 Jun 2020 22:42:01 GMT
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
	-	`sha256:2101694971779e05094b1fea74b740d2e9c8f4d6e0d5b93fe7c2892dbedd1741`  
		Last Modified: Tue, 09 Jun 2020 22:42:29 GMT  
		Size: 7.3 MB (7281512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55b5a6403bc5044ba266d5895b9e8969e47c166166501f96a444732d6048ea05`  
		Last Modified: Tue, 09 Jun 2020 22:42:26 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db2634e9202ad589653192bec8af71e535a3c82984ed1d7be0d6cb080353857`  
		Last Modified: Tue, 09 Jun 2020 22:42:26 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine` - linux; arm variant v7

```console
$ docker pull redis@sha256:f68a5595c59b859acd4c1a66268440170631efa7667d2c28f4f7f68a2c08e749
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9938315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f20577baaee80faac6e7726933469c80db9d2a4cae6f93a9e0a3a8d087be81f`
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
# Wed, 10 Jun 2020 04:21:27 GMT
ENV REDIS_VERSION=6.0.5
# Wed, 10 Jun 2020 04:21:29 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.5.tar.gz
# Wed, 10 Jun 2020 04:21:30 GMT
ENV REDIS_DOWNLOAD_SHA=42cf86a114d2a451b898fcda96acd4d01062a7dbaaad2801d9164a36f898f596
# Wed, 10 Jun 2020 04:22:19 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Wed, 10 Jun 2020 04:22:21 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 10 Jun 2020 04:22:22 GMT
VOLUME [/data]
# Wed, 10 Jun 2020 04:22:22 GMT
WORKDIR /data
# Wed, 10 Jun 2020 04:22:23 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Wed, 10 Jun 2020 04:22:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Jun 2020 04:22:24 GMT
EXPOSE 6379
# Wed, 10 Jun 2020 04:22:25 GMT
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
	-	`sha256:8a222119e47d449748e21695f88dbea630877f4f18c6c192f5883599963395b3`  
		Last Modified: Wed, 10 Jun 2020 04:23:17 GMT  
		Size: 7.2 MB (7152153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f4248b4d7ca7f72565af888ed45b6354077cb9253bedf088f23365d5615003`  
		Last Modified: Wed, 10 Jun 2020 04:23:16 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324f9b7a5371f70e184982603d81d51affea3acea97ab68dd08f364ce9c20ccf`  
		Last Modified: Wed, 10 Jun 2020 04:23:16 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:a0ef5159e5cf82837215238642d989a85404452dd710e8a6df8411b2d2df75ed
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.5 MB (10485315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:053e2fff24b852097aaf5c1059014b7e95884041c564ea5bd305a6c9d87d1016`
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
# Wed, 10 Jun 2020 06:18:04 GMT
ENV REDIS_VERSION=6.0.5
# Wed, 10 Jun 2020 06:18:05 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.5.tar.gz
# Wed, 10 Jun 2020 06:18:05 GMT
ENV REDIS_DOWNLOAD_SHA=42cf86a114d2a451b898fcda96acd4d01062a7dbaaad2801d9164a36f898f596
# Wed, 10 Jun 2020 06:18:54 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Wed, 10 Jun 2020 06:18:56 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 10 Jun 2020 06:18:57 GMT
VOLUME [/data]
# Wed, 10 Jun 2020 06:18:57 GMT
WORKDIR /data
# Wed, 10 Jun 2020 06:18:58 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Wed, 10 Jun 2020 06:18:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Jun 2020 06:18:59 GMT
EXPOSE 6379
# Wed, 10 Jun 2020 06:19:00 GMT
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
	-	`sha256:50de19f7bf7b06f7e1635eca69e0f362a908490475b297d26d0d72a8abfc9762`  
		Last Modified: Wed, 10 Jun 2020 06:19:53 GMT  
		Size: 7.4 MB (7392471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57be62b993a575b8f96cb26073ccfd77592e03c14b785c62877cfa5eeee5256f`  
		Last Modified: Wed, 10 Jun 2020 06:19:50 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641e13c5b89607d6abf87e26205816bfdc35ae9f8588ffbfc7e5a2bc29b7851e`  
		Last Modified: Wed, 10 Jun 2020 06:19:50 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine` - linux; 386

```console
$ docker pull redis@sha256:5d49b9e41e41538c64db8a8de542dc885c00b43bc6ccd4e7db1a707f2d5bfd2f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.3 MB (10253024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8220c85e125781e04c748bb18f52f3c5d30116515a65df326e39532d7ab77875`
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
# Wed, 10 Jun 2020 00:37:05 GMT
ENV REDIS_VERSION=6.0.5
# Wed, 10 Jun 2020 00:37:06 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.5.tar.gz
# Wed, 10 Jun 2020 00:37:06 GMT
ENV REDIS_DOWNLOAD_SHA=42cf86a114d2a451b898fcda96acd4d01062a7dbaaad2801d9164a36f898f596
# Wed, 10 Jun 2020 00:39:29 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Wed, 10 Jun 2020 00:39:31 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 10 Jun 2020 00:39:31 GMT
VOLUME [/data]
# Wed, 10 Jun 2020 00:39:31 GMT
WORKDIR /data
# Wed, 10 Jun 2020 00:39:32 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Wed, 10 Jun 2020 00:39:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Jun 2020 00:39:33 GMT
EXPOSE 6379
# Wed, 10 Jun 2020 00:39:33 GMT
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
	-	`sha256:e6d3bc67e1805280f53de1f224f91e9510511b154b0384be75e37224c0e8f328`  
		Last Modified: Wed, 10 Jun 2020 00:41:01 GMT  
		Size: 7.1 MB (7072808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8088253aad333a97ab19a338da3d2d2d036d39bbf89a49853631139fccc3533`  
		Last Modified: Wed, 10 Jun 2020 00:40:58 GMT  
		Size: 99.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6e2618d87da1456ea363224e3a10f4b11d283a219861ca8ea142ab2c381bed1`  
		Last Modified: Wed, 10 Jun 2020 00:40:58 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine` - linux; ppc64le

```console
$ docker pull redis@sha256:4cfc207c3eeaada887cb09efd809fe36ff03cfa30cf4207e76325f1b2df8dbd0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.1 MB (11092533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0db67e4365ae10f249d15b3e19aa1c3feb244a8b60e94c645a163fe612bf92f3`
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
# Wed, 10 Jun 2020 12:08:43 GMT
ENV REDIS_VERSION=6.0.5
# Wed, 10 Jun 2020 12:08:46 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.5.tar.gz
# Wed, 10 Jun 2020 12:08:52 GMT
ENV REDIS_DOWNLOAD_SHA=42cf86a114d2a451b898fcda96acd4d01062a7dbaaad2801d9164a36f898f596
# Wed, 10 Jun 2020 12:09:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Wed, 10 Jun 2020 12:09:52 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 10 Jun 2020 12:09:54 GMT
VOLUME [/data]
# Wed, 10 Jun 2020 12:09:58 GMT
WORKDIR /data
# Wed, 10 Jun 2020 12:09:59 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Wed, 10 Jun 2020 12:10:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Jun 2020 12:10:02 GMT
EXPOSE 6379
# Wed, 10 Jun 2020 12:10:06 GMT
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
	-	`sha256:5015edbec4bd8927750452197232a5d7201124e438b2e07ca69ebe50a86be0a6`  
		Last Modified: Wed, 10 Jun 2020 12:11:37 GMT  
		Size: 7.9 MB (7897895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5e37d60859c4b9484e9a426c652ddb1589611c14d74815949b8bb5c3cfec5c3`  
		Last Modified: Wed, 10 Jun 2020 12:11:34 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28bcfc4c09a1087314ed96a795cfffe6f9a6cef19f694d5b5da727475b9ea86f`  
		Last Modified: Wed, 10 Jun 2020 12:11:34 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine` - linux; s390x

```console
$ docker pull redis@sha256:d9d38daf8bdcd9d3bd3695d72a81ea198f0fa7b730921eaf77b6f6f91a975f5f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.6 MB (10609163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1017030a4d1b4f13938c721f4927b80f63e8323863b1e8e97d7c37722eb9d30d`
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
# Tue, 09 Jun 2020 22:24:18 GMT
ENV REDIS_VERSION=6.0.5
# Tue, 09 Jun 2020 22:24:19 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.5.tar.gz
# Tue, 09 Jun 2020 22:24:19 GMT
ENV REDIS_DOWNLOAD_SHA=42cf86a114d2a451b898fcda96acd4d01062a7dbaaad2801d9164a36f898f596
# Tue, 09 Jun 2020 22:25:05 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Tue, 09 Jun 2020 22:25:07 GMT
RUN mkdir /data && chown redis:redis /data
# Tue, 09 Jun 2020 22:25:08 GMT
VOLUME [/data]
# Tue, 09 Jun 2020 22:25:08 GMT
WORKDIR /data
# Tue, 09 Jun 2020 22:25:09 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Tue, 09 Jun 2020 22:25:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Jun 2020 22:25:10 GMT
EXPOSE 6379
# Tue, 09 Jun 2020 22:25:10 GMT
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
	-	`sha256:3454704292ca9802dc4f62309a18602ad922ebd03329e6a45e4621beba81ee90`  
		Last Modified: Tue, 09 Jun 2020 22:25:56 GMT  
		Size: 7.7 MB (7655672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4710e9d69862433e637e71513628df5207903ab537763335f493ee23a7d04d82`  
		Last Modified: Tue, 09 Jun 2020 22:25:59 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b26e2e2c99c5cb69bae7b68df2c04b4ef12b7ac0c374a0aa4e7ca2240b55b01`  
		Last Modified: Tue, 09 Jun 2020 22:25:54 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
