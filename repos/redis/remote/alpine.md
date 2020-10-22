## `redis:alpine`

```console
$ docker pull redis@sha256:7a958b10a7b71bc36c578fa1b325f3f6a7d75ee2f481dccd57d67e570cd03c21
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
$ docker pull redis@sha256:1d7b34908bbad6c2d323f5449e1402d32cddd6158e1a590f42f1fca0d11f9071
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.5 MB (10478670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d1b562adb1c2721aa4735f9e0911bb14b97b5d957d9d82f25db31b0875d406a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 07:39:57 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Thu, 22 Oct 2020 07:39:58 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Thu, 22 Oct 2020 07:39:59 GMT
ENV REDIS_VERSION=6.0.8
# Thu, 22 Oct 2020 07:39:59 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.8.tar.gz
# Thu, 22 Oct 2020 07:39:59 GMT
ENV REDIS_DOWNLOAD_SHA=04fa1fddc39bd1aecb6739dd5dd73858a3515b427acd1e2947a66dadce868d68
# Thu, 22 Oct 2020 07:40:57 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Thu, 22 Oct 2020 07:40:58 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 22 Oct 2020 07:40:58 GMT
VOLUME [/data]
# Thu, 22 Oct 2020 07:40:58 GMT
WORKDIR /data
# Thu, 22 Oct 2020 07:40:59 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Thu, 22 Oct 2020 07:40:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 07:40:59 GMT
EXPOSE 6379
# Thu, 22 Oct 2020 07:40:59 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb6015f7c791c1d4df482321bc1d3e195417941c34d5b5c5785384e3442c4562`  
		Last Modified: Thu, 22 Oct 2020 07:42:43 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8890a096979561e03a70f99509191517058ad64aa71d16a956b7da5ec218e35`  
		Last Modified: Thu, 22 Oct 2020 07:42:43 GMT  
		Size: 256.5 KB (256467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7933daa80bd544ef99ad5fdccbf4224ae2830fee4a2747e54c086d6c2ca6202`  
		Last Modified: Thu, 22 Oct 2020 07:42:45 GMT  
		Size: 7.4 MB (7423600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8651e291ae1c7e82ce8c5ee092a86a48e0594289c86db434681f821c482231af`  
		Last Modified: Thu, 22 Oct 2020 07:42:43 GMT  
		Size: 100.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a466f5107c933bec123433b1e92c51cddbde374b1055a4f17d9d781a0196cf90`  
		Last Modified: Thu, 22 Oct 2020 07:42:43 GMT  
		Size: 413.0 B  
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
$ docker pull redis@sha256:6b2845b6653e5621055b84a3d0f5251d62749f552bc29759a85da949af671eb9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.8 MB (9837738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f01c20a1653cfb6c4aedbef7556e96e607467274d49aa3e519866695be763102`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 08:51:59 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Thu, 22 Oct 2020 08:52:03 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Thu, 22 Oct 2020 08:52:04 GMT
ENV REDIS_VERSION=6.0.8
# Thu, 22 Oct 2020 08:52:05 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.8.tar.gz
# Thu, 22 Oct 2020 08:52:07 GMT
ENV REDIS_DOWNLOAD_SHA=04fa1fddc39bd1aecb6739dd5dd73858a3515b427acd1e2947a66dadce868d68
# Thu, 22 Oct 2020 08:52:57 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Thu, 22 Oct 2020 08:52:59 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 22 Oct 2020 08:53:00 GMT
VOLUME [/data]
# Thu, 22 Oct 2020 08:53:01 GMT
WORKDIR /data
# Thu, 22 Oct 2020 08:53:01 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Thu, 22 Oct 2020 08:53:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 08:53:03 GMT
EXPOSE 6379
# Thu, 22 Oct 2020 08:53:04 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b9671ff75b12bc0664c454ab69ea8d357979c28433884f0367d8bc1cf77cc52`  
		Last Modified: Thu, 22 Oct 2020 08:54:43 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9657e73a4e39cdaf3b69292ee79d8cacb08259e0d6ae66b0c098e21bb140985`  
		Last Modified: Thu, 22 Oct 2020 08:54:41 GMT  
		Size: 253.3 KB (253343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2747c3bcaf25b79c76924ee1b53acd2199a9b516681e642d523b1b8cd55d7d7e`  
		Last Modified: Thu, 22 Oct 2020 08:54:44 GMT  
		Size: 7.2 MB (7176912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a134ff96cad0b7a6d365c06c98e960f3b5ac25d66422aaeedf95afcc74aee192`  
		Last Modified: Thu, 22 Oct 2020 08:54:41 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:668b51dc3bd09401e585d7015ed1bc65aa4cd910a9965a482161f19aae194d50`  
		Last Modified: Thu, 22 Oct 2020 08:54:43 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:alpine` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:bc93daf2cfb6ece163e1081f737a3c54a493fe41f28b91af82312776a90b1f0c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.4 MB (10384741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97689dbf307334225778f6337c16984e2436aee4a4c67bf10bc0e3cf000c023e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 08:10:41 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Thu, 22 Oct 2020 08:10:48 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Thu, 22 Oct 2020 08:10:49 GMT
ENV REDIS_VERSION=6.0.8
# Thu, 22 Oct 2020 08:10:50 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.8.tar.gz
# Thu, 22 Oct 2020 08:10:50 GMT
ENV REDIS_DOWNLOAD_SHA=04fa1fddc39bd1aecb6739dd5dd73858a3515b427acd1e2947a66dadce868d68
# Thu, 22 Oct 2020 08:11:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Thu, 22 Oct 2020 08:11:51 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 22 Oct 2020 08:11:52 GMT
VOLUME [/data]
# Thu, 22 Oct 2020 08:11:53 GMT
WORKDIR /data
# Thu, 22 Oct 2020 08:11:53 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Thu, 22 Oct 2020 08:11:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 08:11:55 GMT
EXPOSE 6379
# Thu, 22 Oct 2020 08:11:56 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20a8898a6fdbbf78bbcfc31cb918a901d03750502127e173205c711128b2a68`  
		Last Modified: Thu, 22 Oct 2020 08:13:34 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c0074f6fc2ab9db7b4f65cb010fd63a0be77906d3ac127dbfe8a85677e838f4`  
		Last Modified: Thu, 22 Oct 2020 08:13:33 GMT  
		Size: 258.5 KB (258498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e897a4cf9f36fb0f68e41ab1a925e7b4fcaf8881aceb535de8a6dc5c76b25419`  
		Last Modified: Thu, 22 Oct 2020 08:13:36 GMT  
		Size: 7.4 MB (7417888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c55314d34a6da6b2cda456ba05b3e0ecb9373853cba27ba6c29bb119bca86cb7`  
		Last Modified: Thu, 22 Oct 2020 08:13:34 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf77d829365d2ec2780d96ca57b1c12d53db63a7225b4f0085c3be17687237c`  
		Last Modified: Thu, 22 Oct 2020 08:13:34 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:alpine` - linux; 386

```console
$ docker pull redis@sha256:a2cc4dfe6b765749c2b8fc4437dd77525ba411356f92effe3f86a88315e71f51
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.2 MB (10151702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b935995dc8fb1b715baa58a9a9ceef1f6eef1809f1d1711f73773b5826ea0ca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 05:26:45 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Thu, 22 Oct 2020 05:26:47 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Thu, 22 Oct 2020 05:26:48 GMT
ENV REDIS_VERSION=6.0.8
# Thu, 22 Oct 2020 05:26:48 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.8.tar.gz
# Thu, 22 Oct 2020 05:26:48 GMT
ENV REDIS_DOWNLOAD_SHA=04fa1fddc39bd1aecb6739dd5dd73858a3515b427acd1e2947a66dadce868d68
# Thu, 22 Oct 2020 05:28:59 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Thu, 22 Oct 2020 05:29:00 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 22 Oct 2020 05:29:00 GMT
VOLUME [/data]
# Thu, 22 Oct 2020 05:29:01 GMT
WORKDIR /data
# Thu, 22 Oct 2020 05:29:01 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Thu, 22 Oct 2020 05:29:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 05:29:01 GMT
EXPOSE 6379
# Thu, 22 Oct 2020 05:29:01 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e56191a325dfbb700a740ca5d50b18b47cada55e2a160eba04f310d426371cf9`  
		Last Modified: Thu, 22 Oct 2020 05:31:05 GMT  
		Size: 1.2 KB (1228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c130f6497e095cd8ed8ffb5c25fe3fa3a9f1d2dd2e4bf1f8a08b419c7b775a3f`  
		Last Modified: Thu, 22 Oct 2020 05:31:06 GMT  
		Size: 261.4 KB (261385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a94268fc8a17ad0181850adb600371df480807538126ce959748565c1543bb7`  
		Last Modified: Thu, 22 Oct 2020 05:31:07 GMT  
		Size: 7.1 MB (7097171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1987a9a54657346a102dde1051b52fe1f634688292832b4577cd34cf48a055d`  
		Last Modified: Thu, 22 Oct 2020 05:31:05 GMT  
		Size: 99.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b0de7ee95a0e86c268d26ec934b9de09cd6e81ec2939de1a54451148bb10e8`  
		Last Modified: Thu, 22 Oct 2020 05:31:05 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:alpine` - linux; ppc64le

```console
$ docker pull redis@sha256:0260a7102e959ceda41070dd7ca11caf9386c6a3fffad391cccb6aa01b8cdae8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.5 MB (11498544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5779e996507f275daf4d4a2e3b11ef6d9d82b4ee7eb1f4e33fe74bae1c7d93e`
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
# Fri, 11 Sep 2020 18:35:08 GMT
ENV REDIS_VERSION=6.0.8
# Fri, 11 Sep 2020 18:35:13 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.8.tar.gz
# Fri, 11 Sep 2020 18:35:19 GMT
ENV REDIS_DOWNLOAD_SHA=04fa1fddc39bd1aecb6739dd5dd73858a3515b427acd1e2947a66dadce868d68
# Fri, 11 Sep 2020 18:36:31 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 11 Sep 2020 18:36:43 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 11 Sep 2020 18:36:50 GMT
VOLUME [/data]
# Fri, 11 Sep 2020 18:36:58 GMT
WORKDIR /data
# Fri, 11 Sep 2020 18:37:11 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 11 Sep 2020 18:37:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Sep 2020 18:37:24 GMT
EXPOSE 6379
# Fri, 11 Sep 2020 18:37:33 GMT
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
	-	`sha256:d9d3970ec596ba4c349c24115d239a25429d58f1403606d7fa72e4f20f45736e`  
		Last Modified: Fri, 11 Sep 2020 18:39:14 GMT  
		Size: 8.3 MB (8303903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66d266c05763962f82f44666e320930fddffc6f3fed6c383abf35d18e8cfc9de`  
		Last Modified: Fri, 11 Sep 2020 18:39:11 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30cc7d92bed6ce1cee6c7db9acca7a4dcf150ae27572e678edea2644aecf9075`  
		Last Modified: Fri, 11 Sep 2020 18:39:11 GMT  
		Size: 416.0 B  
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
