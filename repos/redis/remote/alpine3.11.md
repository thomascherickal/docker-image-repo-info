## `redis:alpine3.11`

```console
$ docker pull redis@sha256:2586f31f74ac1d7dc6f6c7eabca42f09bba5ec9911fc519d55fbd7508a9c4f01
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

### `redis:alpine3.11` - linux; amd64

```console
$ docker pull redis@sha256:dbf02fccdcd6251bed40e771690604e4d0da1b32515f0d4b961b6e4cfcacd7e8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.6 MB (10604748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:360360313017ecac5cb44a0cee3326cc25f6276d49166b6c0ca2d768cde55ac6`
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
# Sat, 02 May 2020 01:40:25 GMT
ENV REDIS_VERSION=6.0.1
# Sat, 02 May 2020 01:40:25 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.1.tar.gz
# Sat, 02 May 2020 01:40:25 GMT
ENV REDIS_DOWNLOAD_SHA=b8756e430479edc162ba9c44dc89ac394316cd482f2dc6b91bcd5fe12593f273
# Sat, 02 May 2020 01:41:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Sat, 02 May 2020 01:41:44 GMT
RUN mkdir /data && chown redis:redis /data
# Sat, 02 May 2020 01:41:44 GMT
VOLUME [/data]
# Sat, 02 May 2020 01:41:44 GMT
WORKDIR /data
# Sat, 02 May 2020 01:41:44 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Sat, 02 May 2020 01:41:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 02 May 2020 01:41:45 GMT
EXPOSE 6379
# Sat, 02 May 2020 01:41:45 GMT
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
	-	`sha256:e5396613619b6a2ebf845459a48420e49b8b471b5866f183451abc014f963f01`  
		Last Modified: Sat, 02 May 2020 01:42:28 GMT  
		Size: 7.4 MB (7387123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6809b5ad2cd452552a81bcb0c3922f84bfe88d4d94140aa49762ad10bdb8e704`  
		Last Modified: Sat, 02 May 2020 01:42:27 GMT  
		Size: 100.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:386ecfe54d06508fa3e2d52288b4e13f9f06c7b9ab1494f539ae45700f3c3fd0`  
		Last Modified: Sat, 02 May 2020 01:42:27 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:alpine3.11` - linux; arm variant v6

```console
$ docker pull redis@sha256:8afbe88a1bae6693ae973430a2f0f6652d668faaa18559fd1488913e18f6d0d6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.3 MB (10303204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24e0c84c8082e74a89417daaef6b270f8e919bbfdfa4d1688c7ac27660b50c6f`
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
# Sat, 02 May 2020 01:49:37 GMT
ENV REDIS_VERSION=6.0.1
# Sat, 02 May 2020 01:49:37 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.1.tar.gz
# Sat, 02 May 2020 01:49:38 GMT
ENV REDIS_DOWNLOAD_SHA=b8756e430479edc162ba9c44dc89ac394316cd482f2dc6b91bcd5fe12593f273
# Sat, 02 May 2020 01:50:31 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Sat, 02 May 2020 01:50:33 GMT
RUN mkdir /data && chown redis:redis /data
# Sat, 02 May 2020 01:50:34 GMT
VOLUME [/data]
# Sat, 02 May 2020 01:50:34 GMT
WORKDIR /data
# Sat, 02 May 2020 01:50:35 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Sat, 02 May 2020 01:50:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 02 May 2020 01:50:36 GMT
EXPOSE 6379
# Sat, 02 May 2020 01:50:37 GMT
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
	-	`sha256:35cea8ae723dc7cafd666daa44ecb12b0d65968c7aeea1a2467084943df8b143`  
		Last Modified: Sat, 02 May 2020 01:51:00 GMT  
		Size: 7.3 MB (7275669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7351c4f10e2ff4f2fd26a9c28d44a74a4d3ab192aed679054c585c5b67baf4`  
		Last Modified: Sat, 02 May 2020 01:50:57 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f20a953e196b16fa8573d9d91249ddfb941373fa9885dc9b557e4afe10be3bb`  
		Last Modified: Sat, 02 May 2020 01:50:57 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:alpine3.11` - linux; arm variant v7

```console
$ docker pull redis@sha256:128d43c9e3fc819b09bec95c89fd9e5960fedd8e1bb32f9614c237fd6aefc2ff
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (9964395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c998faf755d8c95bb2a656e9ab708c00395c4f5ee1d385dacfc87194358beb9a`
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
# Sat, 02 May 2020 01:08:45 GMT
ENV REDIS_VERSION=6.0.1
# Sat, 02 May 2020 01:08:46 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.1.tar.gz
# Sat, 02 May 2020 01:08:46 GMT
ENV REDIS_DOWNLOAD_SHA=b8756e430479edc162ba9c44dc89ac394316cd482f2dc6b91bcd5fe12593f273
# Sat, 02 May 2020 01:09:33 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Sat, 02 May 2020 01:09:34 GMT
RUN mkdir /data && chown redis:redis /data
# Sat, 02 May 2020 01:09:35 GMT
VOLUME [/data]
# Sat, 02 May 2020 01:09:36 GMT
WORKDIR /data
# Sat, 02 May 2020 01:09:36 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Sat, 02 May 2020 01:09:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 02 May 2020 01:09:38 GMT
EXPOSE 6379
# Sat, 02 May 2020 01:09:38 GMT
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
	-	`sha256:4cd80773e38739f61504827856c56fff1df3b934a7cf27576e905fd755d86324`  
		Last Modified: Sat, 02 May 2020 01:10:34 GMT  
		Size: 7.1 MB (7140750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c530d42bd44891a5c9e682f78d3f86feb27fb0a254499a7538396619a6734bdd`  
		Last Modified: Sat, 02 May 2020 01:10:32 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60d4db5f9c5ef7ef1d1f27fc21a9e2efd4310583d5fa8a4bf676a089cfd399a0`  
		Last Modified: Sat, 02 May 2020 01:10:32 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:alpine3.11` - linux; arm64 variant v8

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

### `redis:alpine3.11` - linux; 386

```console
$ docker pull redis@sha256:a002af578e24f00dd3f9025245f6b2e5d32f7772186caed168357babbe510a1e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.3 MB (10284553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d552fe7bd1e6f667b66ed482d4acc9cf4f4d06cf345200d90ed50b05205440e7`
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
# Sat, 02 May 2020 01:43:54 GMT
ENV REDIS_VERSION=6.0.1
# Sat, 02 May 2020 01:43:54 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.1.tar.gz
# Sat, 02 May 2020 01:43:54 GMT
ENV REDIS_DOWNLOAD_SHA=b8756e430479edc162ba9c44dc89ac394316cd482f2dc6b91bcd5fe12593f273
# Sat, 02 May 2020 01:45:23 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Sat, 02 May 2020 01:45:23 GMT
RUN mkdir /data && chown redis:redis /data
# Sat, 02 May 2020 01:45:24 GMT
VOLUME [/data]
# Sat, 02 May 2020 01:45:24 GMT
WORKDIR /data
# Sat, 02 May 2020 01:45:24 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Sat, 02 May 2020 01:45:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 02 May 2020 01:45:25 GMT
EXPOSE 6379
# Sat, 02 May 2020 01:45:25 GMT
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
	-	`sha256:caf182a1b6dd8149b47c9e196d6be21773878b8937a09282b20cf37480a58219`  
		Last Modified: Sat, 02 May 2020 01:46:14 GMT  
		Size: 7.1 MB (7066492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc7d3eaea7f7b112c3f59d2e3df1bc6aa521c0e84483a5817e95bd9ec1c014b2`  
		Last Modified: Sat, 02 May 2020 01:46:12 GMT  
		Size: 99.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee6e622001c7b99795490fd3f43d9324e8438eed8af737dbf7eca4e849128889`  
		Last Modified: Sat, 02 May 2020 01:46:12 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:alpine3.11` - linux; ppc64le

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

### `redis:alpine3.11` - linux; s390x

```console
$ docker pull redis@sha256:ae964572ae97f24165d01a13cdf1e717770d10f7a242fe210a71c628e518012c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.6 MB (10640477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:350c62fc7a80787ebae747d5817542f7fc43ffff9eb080c6f53525e9acf7de84`
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
# Sat, 02 May 2020 01:51:52 GMT
ENV REDIS_VERSION=6.0.1
# Sat, 02 May 2020 01:51:52 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.1.tar.gz
# Sat, 02 May 2020 01:51:53 GMT
ENV REDIS_DOWNLOAD_SHA=b8756e430479edc162ba9c44dc89ac394316cd482f2dc6b91bcd5fe12593f273
# Sat, 02 May 2020 01:52:24 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Sat, 02 May 2020 01:52:25 GMT
RUN mkdir /data && chown redis:redis /data
# Sat, 02 May 2020 01:52:25 GMT
VOLUME [/data]
# Sat, 02 May 2020 01:52:25 GMT
WORKDIR /data
# Sat, 02 May 2020 01:52:25 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Sat, 02 May 2020 01:52:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 02 May 2020 01:52:26 GMT
EXPOSE 6379
# Sat, 02 May 2020 01:52:26 GMT
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
	-	`sha256:73afbec9aa2c89b142f1aefeef8073efa3b6fec9d93b19222388b1a837bbc0aa`  
		Last Modified: Sat, 02 May 2020 01:53:06 GMT  
		Size: 7.6 MB (7648422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db9af4f6c49727ae3da752efa04b5dfaf9362be3b7ef768a1d458365d267de47`  
		Last Modified: Sat, 02 May 2020 01:53:04 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbe3ccf31704974427ead4064d6ff183bf1ad6c1c2f3ff4c8a7d42e7929278d8`  
		Last Modified: Sat, 02 May 2020 01:53:09 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
