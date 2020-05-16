## `redis:6-alpine3.11`

```console
$ docker pull redis@sha256:5f7869cb705fc567053e9ff2fac25d6bca2a680c2528dc8f224873758f17c248
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

### `redis:6-alpine3.11` - linux; amd64

```console
$ docker pull redis@sha256:e5146a61518fef302756bd0bf226ac530fc23d7537097fa378cc50fcb5778b64
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.6 MB (10615454 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4ceee5c3fa3cea2607d5e2bcc54d019be616e322979be8fc7a8d0d78b59a1f1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 19:19:42 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Fri, 24 Apr 2020 19:19:43 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Sat, 16 May 2020 02:13:46 GMT
ENV REDIS_VERSION=6.0.2
# Sat, 16 May 2020 02:13:46 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.2.tar.gz
# Sat, 16 May 2020 02:13:46 GMT
ENV REDIS_DOWNLOAD_SHA=9c37cd4228a57e82e7037094751c63349302b0b86c5e30b778a63a802dfd0109
# Sat, 16 May 2020 02:15:35 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Sat, 16 May 2020 02:15:36 GMT
RUN mkdir /data && chown redis:redis /data
# Sat, 16 May 2020 02:15:36 GMT
VOLUME [/data]
# Sat, 16 May 2020 02:15:37 GMT
WORKDIR /data
# Sat, 16 May 2020 02:15:37 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Sat, 16 May 2020 02:15:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 May 2020 02:15:38 GMT
EXPOSE 6379
# Sat, 16 May 2020 02:15:38 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0373118a0d956ca0ee963e307457f45f073db9096f7c6f87c10251d071f0dc`  
		Last Modified: Fri, 24 Apr 2020 19:23:01 GMT  
		Size: 1.2 KB (1228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd369fe62565d644723bfdb734c4ecb2a96191366ec08424146aa9c5ff6b308`  
		Last Modified: Fri, 24 Apr 2020 19:23:02 GMT  
		Size: 402.6 KB (402568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d862fc04e31c48831cc75b3b3868126e27f4e51c45bdcddb6ffc7c94b9205a76`  
		Last Modified: Sat, 16 May 2020 02:20:31 GMT  
		Size: 7.4 MB (7397830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbb087a9da0889770a90077b54e12441d375e7027b377997f98a5e6d827ab3fe`  
		Last Modified: Sat, 16 May 2020 02:20:29 GMT  
		Size: 99.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be29dc118a7a01cd97bac04e83376259dee6d48d1cf35a94a8d26d3a73159bb`  
		Last Modified: Sat, 16 May 2020 02:20:30 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine3.11` - linux; arm variant v6

```console
$ docker pull redis@sha256:4057fbe62d49d301734916e4d6d7dd8f9c2d06ebfdad741698aa18ff152b642c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.3 MB (10312873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00275d208cadbfe750c573429cfd2721a47e1b792b022432d241395fbe82dbb5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 22:30:17 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Thu, 23 Apr 2020 22:30:20 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Fri, 15 May 2020 23:24:21 GMT
ENV REDIS_VERSION=6.0.2
# Fri, 15 May 2020 23:24:22 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.2.tar.gz
# Fri, 15 May 2020 23:24:23 GMT
ENV REDIS_DOWNLOAD_SHA=9c37cd4228a57e82e7037094751c63349302b0b86c5e30b778a63a802dfd0109
# Fri, 15 May 2020 23:25:22 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 15 May 2020 23:25:28 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 15 May 2020 23:25:30 GMT
VOLUME [/data]
# Fri, 15 May 2020 23:25:31 GMT
WORKDIR /data
# Fri, 15 May 2020 23:25:33 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 15 May 2020 23:25:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 15 May 2020 23:25:36 GMT
EXPOSE 6379
# Fri, 15 May 2020 23:25:37 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ab5b04292d1974b3feedf74dddf563efe3ba5b5c38239a49e8adf0ac8140028`  
		Last Modified: Thu, 23 Apr 2020 22:33:41 GMT  
		Size: 1.3 KB (1253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af20f6a7bee5bf869254b4964c1a5d8dd5ef1353ac48081a885920682312555b`  
		Last Modified: Thu, 23 Apr 2020 22:33:41 GMT  
		Size: 405.8 KB (405799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82cd828ef5be835bbd932776269cc78fa20d6597c5286a8301d9712ca6ba27e1`  
		Last Modified: Fri, 15 May 2020 23:26:27 GMT  
		Size: 7.3 MB (7285336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62363baf5a298c4aecde09c629388197091d261f20fd00863a1693c8847cc34`  
		Last Modified: Fri, 15 May 2020 23:26:27 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0e939b10f701fd67e6400e3d0193f9dbafde2f4bc53215a7305a7c7352bdcb`  
		Last Modified: Fri, 15 May 2020 23:26:25 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine3.11` - linux; arm variant v7

```console
$ docker pull redis@sha256:a9395e60f632ac5808d01ff562ddafcccf44d254f634164eef079f86f0e4fcd3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (9972279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2af28cbbd6cfbc59e7a5f1a1855dd7caa878b4fd03a749db7b3e51823a58c6b7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 08:51:32 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Fri, 24 Apr 2020 08:51:36 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Sat, 16 May 2020 06:33:17 GMT
ENV REDIS_VERSION=6.0.2
# Sat, 16 May 2020 06:33:18 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.2.tar.gz
# Sat, 16 May 2020 06:33:20 GMT
ENV REDIS_DOWNLOAD_SHA=9c37cd4228a57e82e7037094751c63349302b0b86c5e30b778a63a802dfd0109
# Sat, 16 May 2020 06:34:11 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Sat, 16 May 2020 06:34:13 GMT
RUN mkdir /data && chown redis:redis /data
# Sat, 16 May 2020 06:34:14 GMT
VOLUME [/data]
# Sat, 16 May 2020 06:34:15 GMT
WORKDIR /data
# Sat, 16 May 2020 06:34:16 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Sat, 16 May 2020 06:34:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 May 2020 06:34:17 GMT
EXPOSE 6379
# Sat, 16 May 2020 06:34:18 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0765e03c998449baf4c76a1011cf80e6ab974db3d5d8da3a361bfeeb875d96db`  
		Last Modified: Fri, 24 Apr 2020 08:55:16 GMT  
		Size: 1.3 KB (1254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc07fda5f4761823162fa661b4466f517ad5db025d9689c123221af67af9b53f`  
		Last Modified: Fri, 24 Apr 2020 08:55:16 GMT  
		Size: 399.8 KB (399779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b80e8aaba692112e559076be6bb0334a707afdf5e98838a1871caa0866a8c0e`  
		Last Modified: Sat, 16 May 2020 06:35:45 GMT  
		Size: 7.1 MB (7148634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a87bac8f769e16dcbd264fba3220e6015ebc7ade1c9dbbeaaf05826b5a181b86`  
		Last Modified: Sat, 16 May 2020 06:35:46 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fb4e2186895e529da275fc0432b79e52a0bb9857639493ec62bcf3bf168531a`  
		Last Modified: Sat, 16 May 2020 06:35:45 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine3.11` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:1961f4617f243f9e5277fbdda907572aa587f6aae12444b30b6a19645b635f32
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.5 MB (10510509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d30379a22856a9b2b69c3adc7a2bd61aa73bb2230f99162172b71a006b141fdd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 12:45:10 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Fri, 24 Apr 2020 12:45:13 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Sat, 02 May 2020 01:42:43 GMT
ENV REDIS_VERSION=6.0.1
# Sat, 02 May 2020 01:42:44 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.1.tar.gz
# Sat, 02 May 2020 01:42:44 GMT
ENV REDIS_DOWNLOAD_SHA=b8756e430479edc162ba9c44dc89ac394316cd482f2dc6b91bcd5fe12593f273
# Sat, 02 May 2020 01:43:36 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Sat, 02 May 2020 01:43:38 GMT
RUN mkdir /data && chown redis:redis /data
# Sat, 02 May 2020 01:43:39 GMT
VOLUME [/data]
# Sat, 02 May 2020 01:43:40 GMT
WORKDIR /data
# Sat, 02 May 2020 01:43:40 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Sat, 02 May 2020 01:43:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 02 May 2020 01:43:42 GMT
EXPOSE 6379
# Sat, 02 May 2020 01:43:42 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c7050d23898adae8e4a2e0ab67eaeab9f9a9ec0fa5b88b128eeff4de1570877`  
		Last Modified: Fri, 24 Apr 2020 12:48:50 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8982b178d819b1f2f10c3375b2c7ed054157cc5e711b58b6a2dcb376686e5d59`  
		Last Modified: Fri, 24 Apr 2020 12:48:50 GMT  
		Size: 404.7 KB (404661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc865bafaa411d274a5d06d9baa2dbe66c6457ec9cc74ae2a19e0319080acf9c`  
		Last Modified: Sat, 02 May 2020 01:44:33 GMT  
		Size: 7.4 MB (7379619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92ad23622f528f7c78240673322e87edcc8eb3c86c5895b4a5b552458d6fc996`  
		Last Modified: Sat, 02 May 2020 01:44:31 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd5700fcef1ec7c82744aff73a55942e494726d6198e0b5836021b4c5c8031d3`  
		Last Modified: Sat, 02 May 2020 01:44:31 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine3.11` - linux; 386

```console
$ docker pull redis@sha256:bbfdc448dafad37023ae75c4fcfbd5d1ec7bd78aad8e769b62753c36c31757b3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.3 MB (10290082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b34322bf2334fed58c9521a918064a594354d513fbeec9b4b637dd5be45e8b84`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:04 GMT
ADD file:63bd8a316cba8c404cc2e32a5120406c24aee8db3224c469a6077b941d900863 in / 
# Thu, 23 Apr 2020 21:16:04 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 05:49:36 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Fri, 24 Apr 2020 05:49:38 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Sat, 16 May 2020 00:09:40 GMT
ENV REDIS_VERSION=6.0.2
# Sat, 16 May 2020 00:09:41 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.2.tar.gz
# Sat, 16 May 2020 00:09:41 GMT
ENV REDIS_DOWNLOAD_SHA=9c37cd4228a57e82e7037094751c63349302b0b86c5e30b778a63a802dfd0109
# Sat, 16 May 2020 00:11:08 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Sat, 16 May 2020 00:11:09 GMT
RUN mkdir /data && chown redis:redis /data
# Sat, 16 May 2020 00:11:09 GMT
VOLUME [/data]
# Sat, 16 May 2020 00:11:10 GMT
WORKDIR /data
# Sat, 16 May 2020 00:11:10 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Sat, 16 May 2020 00:11:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 May 2020 00:11:10 GMT
EXPOSE 6379
# Sat, 16 May 2020 00:11:11 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:2826c1e79865da7e0da0a993a2a38db61c3911e05b5df617439a86d4deac90fb`  
		Last Modified: Thu, 23 Apr 2020 21:16:32 GMT  
		Size: 2.8 MB (2808418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4eb71d5f124b9b51684034d7d96fba6399ff6892995e51137d0c0617a11fb9`  
		Last Modified: Fri, 24 Apr 2020 05:53:39 GMT  
		Size: 1.2 KB (1229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7685edc32d5ef38faf3beb4310c119862b1dfa18ea58edb0dbca84e9417b267`  
		Last Modified: Fri, 24 Apr 2020 05:53:39 GMT  
		Size: 407.9 KB (407901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c02f4cc0a73447e7af4c367a8efe6a3fe2e6b6cdf92088abd4c2b8f99f980af`  
		Last Modified: Sat, 16 May 2020 00:14:01 GMT  
		Size: 7.1 MB (7072021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd586489393880a99bcea0f145202694e2d8e8c438c7d6b44741073ea6d2c16`  
		Last Modified: Sat, 16 May 2020 00:13:59 GMT  
		Size: 100.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dd50ae8a09e8979660d44015b05f83ff9419212dcd16c1dd9372263dfadaff9`  
		Last Modified: Sat, 16 May 2020 00:13:59 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine3.11` - linux; ppc64le

```console
$ docker pull redis@sha256:cfba805e8e322ce58dab2b9b4b858f37f7302e0e2f6cda93544aea5f6b65672a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.1 MB (11119089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:616d6a9d879f69164d4b78badb5f026795f41523df81f13ca70fb7db44af3c15`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 20:39:04 GMT
ADD file:1aaebe252dfb1885e066fcbc84aaa915bae149c3608f19600855ad1d4f7450c1 in / 
# Thu, 23 Apr 2020 20:39:06 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 09:02:06 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Fri, 24 Apr 2020 09:02:13 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Sat, 02 May 2020 01:39:11 GMT
ENV REDIS_VERSION=6.0.1
# Sat, 02 May 2020 01:39:15 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.1.tar.gz
# Sat, 02 May 2020 01:39:18 GMT
ENV REDIS_DOWNLOAD_SHA=b8756e430479edc162ba9c44dc89ac394316cd482f2dc6b91bcd5fe12593f273
# Sat, 02 May 2020 01:40:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Sat, 02 May 2020 01:40:24 GMT
RUN mkdir /data && chown redis:redis /data
# Sat, 02 May 2020 01:40:26 GMT
VOLUME [/data]
# Sat, 02 May 2020 01:40:32 GMT
WORKDIR /data
# Sat, 02 May 2020 01:40:33 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Sat, 02 May 2020 01:40:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 02 May 2020 01:40:45 GMT
EXPOSE 6379
# Sat, 02 May 2020 01:40:52 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:9a8fdc5b698322331ee7eba7dd6f66f3a4e956554db22dd1e834d519415b4f8e`  
		Last Modified: Thu, 23 Apr 2020 20:41:33 GMT  
		Size: 2.8 MB (2821843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dc79e36a18515157312416d029cb35887ee8668b53b6c0e3867a4d0dd8dd231`  
		Last Modified: Fri, 24 Apr 2020 09:06:56 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb83078862453fa1de07d734ccc5b995c92cd74710488c11d066ad752e3402d`  
		Last Modified: Fri, 24 Apr 2020 09:06:57 GMT  
		Size: 409.9 KB (409875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9024d4e75c53ef1953ae3a78f8ad86bbe92518fb99180971de1094d47df89a61`  
		Last Modified: Sat, 02 May 2020 01:42:05 GMT  
		Size: 7.9 MB (7885566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c68a8681cb0eb950f0b784e7af7e325f5e33abeb97efa1552be604661f62a9b0`  
		Last Modified: Sat, 02 May 2020 01:42:02 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcf07fa05cd4bf9799620ac107ef4670f3b0cc1d147ad2af58ea414f055ece71`  
		Last Modified: Sat, 02 May 2020 01:42:02 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine3.11` - linux; s390x

```console
$ docker pull redis@sha256:7e87f23ad9c129bc30f56aa8881568fd3bae9fdcf1aca09f9fd15a145a8a78bf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.6 MB (10647559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd9dc6fb128105420046bfd04554e6dd0f328c259824417652aef3ff4986b8df`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 17:50:57 GMT
ADD file:a59a30c2fd43c9f3b820751a6f5a54688c14440a1ddace1ab255475f46e6ba2d in / 
# Thu, 23 Apr 2020 17:50:58 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 07:02:35 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Fri, 24 Apr 2020 07:02:36 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Fri, 15 May 2020 22:42:24 GMT
ENV REDIS_VERSION=6.0.2
# Fri, 15 May 2020 22:42:25 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.2.tar.gz
# Fri, 15 May 2020 22:42:25 GMT
ENV REDIS_DOWNLOAD_SHA=9c37cd4228a57e82e7037094751c63349302b0b86c5e30b778a63a802dfd0109
# Fri, 15 May 2020 22:43:00 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 15 May 2020 22:43:01 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 15 May 2020 22:43:02 GMT
VOLUME [/data]
# Fri, 15 May 2020 22:43:02 GMT
WORKDIR /data
# Fri, 15 May 2020 22:43:02 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 15 May 2020 22:43:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 15 May 2020 22:43:03 GMT
EXPOSE 6379
# Fri, 15 May 2020 22:43:03 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:7184c046fdf17da4c16ca482e5ede36e1f2d41ac8cea9c036e488fd149d6e8e7`  
		Last Modified: Thu, 23 Apr 2020 17:51:38 GMT  
		Size: 2.6 MB (2582859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2da1b54f68b54cfd646e4cf510a14593b857e3c6e7732985b5a3bc5e213a72a`  
		Last Modified: Fri, 24 Apr 2020 07:04:54 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41f0a46f7a997ac6f05cd804b3a0f56c74348f25fd9e164c66ab7c5c4a6a2c82`  
		Last Modified: Fri, 24 Apr 2020 07:04:54 GMT  
		Size: 407.4 KB (407392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7d280287c062cfd9d589ad117076ba536339a11933f5cc8c50679b99a7d5a33`  
		Last Modified: Fri, 15 May 2020 22:43:59 GMT  
		Size: 7.7 MB (7655503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f8cd36de079748236b7e47e5540b2968095a52c1e3eb820750e1eb95c3cf282`  
		Last Modified: Fri, 15 May 2020 22:43:57 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c5e784b212d08809045f9af3f7675dd7d74d224be6831c0bedaf3512f2d204`  
		Last Modified: Fri, 15 May 2020 22:43:57 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
