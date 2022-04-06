## `redis:6-alpine3.15`

```console
$ docker pull redis@sha256:132337b9d7744ffee4fae83f51de53c3530935ad3ba528b7110f2d805f55cbf5
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

### `redis:6-alpine3.15` - linux; amd64

```console
$ docker pull redis@sha256:6c42cce2871e8dc5fb3e843ed5c4e7939d312faf5e53ff0ff4ca955a7e0b2b39
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.9 MB (10930105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34e1dc356a22aadc8d41f9335ad4b5fdcf9f4c1472df3523846ad2e73d7d6c41`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 10:42:26 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Tue, 05 Apr 2022 10:42:28 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Tue, 05 Apr 2022 10:43:51 GMT
ENV REDIS_VERSION=6.2.6
# Tue, 05 Apr 2022 10:43:51 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.6.tar.gz
# Tue, 05 Apr 2022 10:43:51 GMT
ENV REDIS_DOWNLOAD_SHA=5b2b8b7a50111ef395bf1c1d5be11e6e167ac018125055daa8b5c2317ae131ab
# Tue, 05 Apr 2022 10:44:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Tue, 05 Apr 2022 10:44:48 GMT
RUN mkdir /data && chown redis:redis /data
# Tue, 05 Apr 2022 10:44:48 GMT
VOLUME [/data]
# Tue, 05 Apr 2022 10:44:48 GMT
WORKDIR /data
# Tue, 05 Apr 2022 10:44:48 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Tue, 05 Apr 2022 10:44:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 10:44:49 GMT
EXPOSE 6379
# Tue, 05 Apr 2022 10:44:49 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:192e0352348275fe7c4099cf478959878b50bda7afe561ad71f1f239daa17d31`  
		Last Modified: Tue, 05 Apr 2022 10:47:59 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7151bccd2756efc52d97e3ec15c8053c4313a5bee00319382ba922c7a1cdf2aa`  
		Last Modified: Tue, 05 Apr 2022 10:47:59 GMT  
		Size: 406.4 KB (406358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e599fac432b220fe1c5ea089049eae50679a15e7a0256ec33c120dc28b41382d`  
		Last Modified: Tue, 05 Apr 2022 10:48:19 GMT  
		Size: 7.7 MB (7707366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:720d86c109236e95a044add74c942c8eef356caf1a4e667e8e8cbfcfd98db1d8`  
		Last Modified: Tue, 05 Apr 2022 10:48:18 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40911e48517b623f5392889e83a35fa77316c51937b7b1742b5bd846403cf099`  
		Last Modified: Tue, 05 Apr 2022 10:48:18 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine3.15` - linux; arm variant v6

```console
$ docker pull redis@sha256:9e26d922909c7b6e26f43af23943a5c34274ec011cc5c7dcfdc5618b013caf1c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.6 MB (10625031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52d48c5ba7c8d751adb03b82b8b21605077c4ea7f66d37221673dedb57c6dd90`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 13:02:08 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Tue, 05 Apr 2022 13:02:12 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Tue, 05 Apr 2022 13:03:57 GMT
ENV REDIS_VERSION=6.2.6
# Tue, 05 Apr 2022 13:03:57 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.6.tar.gz
# Tue, 05 Apr 2022 13:03:58 GMT
ENV REDIS_DOWNLOAD_SHA=5b2b8b7a50111ef395bf1c1d5be11e6e167ac018125055daa8b5c2317ae131ab
# Tue, 05 Apr 2022 13:05:08 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Tue, 05 Apr 2022 13:05:11 GMT
RUN mkdir /data && chown redis:redis /data
# Tue, 05 Apr 2022 13:05:11 GMT
VOLUME [/data]
# Tue, 05 Apr 2022 13:05:12 GMT
WORKDIR /data
# Tue, 05 Apr 2022 13:05:12 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Tue, 05 Apr 2022 13:05:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 13:05:13 GMT
EXPOSE 6379
# Tue, 05 Apr 2022 13:05:13 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4d9991d98fe184813ce2b5454f27c6dace6e9644f3c040dcb2cfa0bf916715`  
		Last Modified: Tue, 05 Apr 2022 13:10:01 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de7974bac14e30fdafb22f66f2b1e1ca4242a61cfa78c944d9b5387f85798833`  
		Last Modified: Tue, 05 Apr 2022 13:10:01 GMT  
		Size: 410.5 KB (410530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b9759607c8e0670bb8cbb730ba7ce59f0f21b8d7d8eea935296c7d7322d00e`  
		Last Modified: Tue, 05 Apr 2022 13:10:30 GMT  
		Size: 7.6 MB (7590711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b546f6621d2c5a4f347c5ab7cdd83b683823ee97673bfe3cb18e9799553a599d`  
		Last Modified: Tue, 05 Apr 2022 13:10:26 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11e7ad123f35f8a093ac9fe9ca2d9da77b457d8084832ccb4ed6e82242d0c2fb`  
		Last Modified: Tue, 05 Apr 2022 13:10:26 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine3.15` - linux; arm variant v7

```console
$ docker pull redis@sha256:eb1a0e37089a8e96ac239a8aa87b9e8bfba981a17147003fcab8bb9077d793a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.3 MB (10300557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:656433a0dcf3d93aefda2a42151d96aa457d3feec55b2376016d15d6607c4a1d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 16:05:20 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Tue, 05 Apr 2022 16:05:23 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Tue, 05 Apr 2022 16:07:25 GMT
ENV REDIS_VERSION=6.2.6
# Tue, 05 Apr 2022 16:07:25 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.6.tar.gz
# Tue, 05 Apr 2022 16:07:25 GMT
ENV REDIS_DOWNLOAD_SHA=5b2b8b7a50111ef395bf1c1d5be11e6e167ac018125055daa8b5c2317ae131ab
# Tue, 05 Apr 2022 16:08:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Tue, 05 Apr 2022 16:08:35 GMT
RUN mkdir /data && chown redis:redis /data
# Tue, 05 Apr 2022 16:08:36 GMT
VOLUME [/data]
# Tue, 05 Apr 2022 16:08:36 GMT
WORKDIR /data
# Tue, 05 Apr 2022 16:08:37 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Tue, 05 Apr 2022 16:08:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 16:08:37 GMT
EXPOSE 6379
# Tue, 05 Apr 2022 16:08:38 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2efbe042e3961fe37f11893d0a1dbf4b29b62079ae6626dcd1bafddd15b4315d`  
		Last Modified: Tue, 05 Apr 2022 16:17:13 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab97eb61d6fd7754a0bd0e13fa0bd4d4e3c05ddb1975c790e69745915c8845e4`  
		Last Modified: Tue, 05 Apr 2022 16:17:14 GMT  
		Size: 404.4 KB (404413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b769a6531d7b17cf98abf7f077819e67b8704145cf999b1c82e0e0046e85d255`  
		Last Modified: Tue, 05 Apr 2022 16:17:54 GMT  
		Size: 7.5 MB (7470006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2542d7a30a60fca0896618d1b2f1308f93dd235166c0b83a654bd42973e2af27`  
		Last Modified: Tue, 05 Apr 2022 16:17:49 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6920ac5de7a252d2cf24975a6537ea3d0341fa0ad22aaa3b567322590e062138`  
		Last Modified: Tue, 05 Apr 2022 16:17:49 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:b295bbc5b7e6dc9d62b68d70ca75f14f7add2197e25853ceb6c6fb7998111fe6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.8 MB (10835230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50bbab999a8710af814e2e66146444bc367f26c871153cc6554577385fed1058`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:09:56 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Tue, 05 Apr 2022 07:09:58 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Tue, 05 Apr 2022 07:11:15 GMT
ENV REDIS_VERSION=6.2.6
# Tue, 05 Apr 2022 07:11:16 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.6.tar.gz
# Tue, 05 Apr 2022 07:11:17 GMT
ENV REDIS_DOWNLOAD_SHA=5b2b8b7a50111ef395bf1c1d5be11e6e167ac018125055daa8b5c2317ae131ab
# Tue, 05 Apr 2022 07:11:58 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Tue, 05 Apr 2022 07:11:58 GMT
RUN mkdir /data && chown redis:redis /data
# Tue, 05 Apr 2022 07:11:59 GMT
VOLUME [/data]
# Tue, 05 Apr 2022 07:12:00 GMT
WORKDIR /data
# Tue, 05 Apr 2022 07:12:02 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Tue, 05 Apr 2022 07:12:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 07:12:03 GMT
EXPOSE 6379
# Tue, 05 Apr 2022 07:12:04 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d958ce1c7c3635737d6c3a700d8ef0133cd0c25eed686c65ad6bf3c1542c3385`  
		Last Modified: Tue, 05 Apr 2022 07:15:41 GMT  
		Size: 1.2 KB (1237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc31afb0d4b76e8ac99f0203c03a315991664d0baddbb7216a8e9497b59c8991`  
		Last Modified: Tue, 05 Apr 2022 07:15:42 GMT  
		Size: 407.3 KB (407312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a10ea637b73c27ed84b475598cf71384c0aa2260c45b68cbaf7a04155e04aff`  
		Last Modified: Tue, 05 Apr 2022 07:16:08 GMT  
		Size: 7.7 MB (7709692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05eebd03f36af3a8232eb5f67dfd30f7a575e7050efeecced4ac35749285b46b`  
		Last Modified: Tue, 05 Apr 2022 07:16:06 GMT  
		Size: 99.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c76fe238c311d640987029a09e0018f14a3115b88763604f0852fcff2f2db238`  
		Last Modified: Tue, 05 Apr 2022 07:16:07 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine3.15` - linux; 386

```console
$ docker pull redis@sha256:4603c4e6feda7f17efa7480e4c1191e78ee186c4362cad0480c06aa7bcd30c1e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.6 MB (10588813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb32dc126e1a0e92f7e37bbf2865e5da6fff68941ced60c6e65ba0a67697799a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:25 GMT
ADD file:7d51a0f8691eb78c9062fd31984423a93d276a67b4ed5d1a706e1c2cd9fea23a in / 
# Mon, 04 Apr 2022 23:38:25 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:34:57 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Tue, 05 Apr 2022 06:34:58 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Tue, 05 Apr 2022 06:36:16 GMT
ENV REDIS_VERSION=6.2.6
# Tue, 05 Apr 2022 06:36:17 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.6.tar.gz
# Tue, 05 Apr 2022 06:36:18 GMT
ENV REDIS_DOWNLOAD_SHA=5b2b8b7a50111ef395bf1c1d5be11e6e167ac018125055daa8b5c2317ae131ab
# Tue, 05 Apr 2022 06:36:58 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Tue, 05 Apr 2022 06:36:58 GMT
RUN mkdir /data && chown redis:redis /data
# Tue, 05 Apr 2022 06:36:59 GMT
VOLUME [/data]
# Tue, 05 Apr 2022 06:37:00 GMT
WORKDIR /data
# Tue, 05 Apr 2022 06:37:02 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Tue, 05 Apr 2022 06:37:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 06:37:03 GMT
EXPOSE 6379
# Tue, 05 Apr 2022 06:37:04 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:73b28a5955ec7fb46f2cf0434e4901a889f7dda3f8c9ec496300feb256c7eda8`  
		Last Modified: Mon, 04 Apr 2022 19:10:03 GMT  
		Size: 2.8 MB (2818974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68813003c3846d373740351e65ac66efe2a454dbc4b5fcebb3e55427c659a097`  
		Last Modified: Tue, 05 Apr 2022 06:40:41 GMT  
		Size: 1.2 KB (1238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76ceda6d7620e1692eddf9263515cdedbe8454709b8c75b23bba915ea0721b50`  
		Last Modified: Tue, 05 Apr 2022 06:40:41 GMT  
		Size: 412.8 KB (412810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33aace9bd49cd307446cef10200a57a7bd8a133a5bd2c06c8b2daa4d3e6a9272`  
		Last Modified: Tue, 05 Apr 2022 06:41:08 GMT  
		Size: 7.4 MB (7355279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e910667c7271fff8d8e7b64ddfe0db112baf981435b95c4f407dce4969f09fa`  
		Last Modified: Tue, 05 Apr 2022 06:41:06 GMT  
		Size: 99.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e5df03bfb0ad118f06992fcc558fe774dc03716183a3c1828cacd9e7d8dd52`  
		Last Modified: Tue, 05 Apr 2022 06:41:06 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine3.15` - linux; ppc64le

```console
$ docker pull redis@sha256:a62d18af82ab7bf099e62366d02c9115c5148ba8ecedde9231120d371d66193b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.4 MB (11446548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aef56858c31f0585a49a732a788a616452cbbada6fc5d5833a5510d67a658dbd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:30 GMT
ADD file:960cf6f9d3d1cfcb36c2d67dd4c3eaba7db1d0c7afe97968512248d7f234ad47 in / 
# Tue, 05 Apr 2022 00:23:32 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 19:45:47 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Tue, 05 Apr 2022 19:46:00 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Tue, 05 Apr 2022 19:48:33 GMT
ENV REDIS_VERSION=6.2.6
# Tue, 05 Apr 2022 19:48:39 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.6.tar.gz
# Tue, 05 Apr 2022 19:48:45 GMT
ENV REDIS_DOWNLOAD_SHA=5b2b8b7a50111ef395bf1c1d5be11e6e167ac018125055daa8b5c2317ae131ab
# Tue, 05 Apr 2022 19:49:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Tue, 05 Apr 2022 19:49:57 GMT
RUN mkdir /data && chown redis:redis /data
# Tue, 05 Apr 2022 19:50:00 GMT
VOLUME [/data]
# Tue, 05 Apr 2022 19:50:06 GMT
WORKDIR /data
# Tue, 05 Apr 2022 19:50:08 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Tue, 05 Apr 2022 19:50:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 19:50:18 GMT
EXPOSE 6379
# Tue, 05 Apr 2022 19:50:26 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:1877acf2d48ed8bcb5bd9756a95aca0c077457be7cf4fcef25807f4e9be88db1`  
		Last Modified: Mon, 04 Apr 2022 19:09:49 GMT  
		Size: 2.8 MB (2811186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2c000184e14c5aaba3e124988881ec3d1b1d2dd2463abde9556e9a6f22ba01`  
		Last Modified: Tue, 05 Apr 2022 19:56:26 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9acb8b4759f68baa5aab76b22f2774319ba63d6ff55709ee87803c59c5402cef`  
		Last Modified: Tue, 05 Apr 2022 19:56:27 GMT  
		Size: 413.2 KB (413158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6db5f6fdd8a2f1935ad7fe18d23ce490d86b4373032addb64307956196ed55c`  
		Last Modified: Tue, 05 Apr 2022 19:56:55 GMT  
		Size: 8.2 MB (8220387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1b89e4f510d602f3b8b7e7eac718c9922f0efff109bebff602782fadc51238`  
		Last Modified: Tue, 05 Apr 2022 19:56:53 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb64abcc215cab21cbd928a8e01f4eba193f75cbe113ca41ee3b431cb70db592`  
		Last Modified: Tue, 05 Apr 2022 19:56:53 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine3.15` - linux; s390x

```console
$ docker pull redis@sha256:135281a9fcd7f025dacc554b04a53d1428c3c89eb73e87a98eeb0ec339ee96ac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.0 MB (11043605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32885bd1aaa423de931d4a2eefd0f4e31f3bb9ac073e7c14438826da3c334d6d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:02:08 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Tue, 05 Apr 2022 06:02:09 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Tue, 05 Apr 2022 06:03:14 GMT
ENV REDIS_VERSION=6.2.6
# Tue, 05 Apr 2022 06:03:15 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.6.tar.gz
# Tue, 05 Apr 2022 06:03:15 GMT
ENV REDIS_DOWNLOAD_SHA=5b2b8b7a50111ef395bf1c1d5be11e6e167ac018125055daa8b5c2317ae131ab
# Tue, 05 Apr 2022 06:03:55 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Tue, 05 Apr 2022 06:03:57 GMT
RUN mkdir /data && chown redis:redis /data
# Tue, 05 Apr 2022 06:03:57 GMT
VOLUME [/data]
# Tue, 05 Apr 2022 06:03:58 GMT
WORKDIR /data
# Tue, 05 Apr 2022 06:03:58 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Tue, 05 Apr 2022 06:03:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 06:03:58 GMT
EXPOSE 6379
# Tue, 05 Apr 2022 06:03:59 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da88d1ec49321f32532a5dd885409190f63cadeea78e2169a0240dd718174226`  
		Last Modified: Tue, 05 Apr 2022 06:07:26 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b52dd08852521e579f2939dc00c60bf555e7708a9fa64afdbc8fed94542a71`  
		Last Modified: Tue, 05 Apr 2022 06:07:26 GMT  
		Size: 411.0 KB (410960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e5bc9cec375eb0b486de985438b2a72e7093ad8e2cc0dd91c9117e478a7ec2`  
		Last Modified: Tue, 05 Apr 2022 06:07:46 GMT  
		Size: 8.0 MB (8030456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67191c26c8c6fec4586050f0f33b05ea85bf8b0ed900a1793dabe52655893bc7`  
		Last Modified: Tue, 05 Apr 2022 06:07:44 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99b776f976bf24499015366eb8974ccfcbec3970465bb227fc380d1ab00a58f`  
		Last Modified: Tue, 05 Apr 2022 06:07:44 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
