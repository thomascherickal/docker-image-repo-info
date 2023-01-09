## `redis:6-alpine`

```console
$ docker pull redis@sha256:7fee7daf81b016d8bf0338d77bbe9ae8e2e0ed63fc1edf4d754491f03a89575a
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

### `redis:6-alpine` - linux; amd64

```console
$ docker pull redis@sha256:e23bc4f8f94da81e54b5c9b6f0b843c8b579c88a0f62823634de091d79fdd6ad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.2 MB (11245207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e76fcf02160312d184b00f8cb1181e5b167eb915af30847214bfc0e9973fa37e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 20:04:34 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Mon, 09 Jan 2023 20:04:35 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Mon, 09 Jan 2023 20:05:23 GMT
ENV REDIS_VERSION=6.2.8
# Mon, 09 Jan 2023 20:05:23 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.8.tar.gz
# Mon, 09 Jan 2023 20:05:23 GMT
ENV REDIS_DOWNLOAD_SHA=f91ab24bcb42673cb853292eb5d43c2017d11d659854808ed6a529c97297fdfe
# Mon, 09 Jan 2023 20:06:01 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Mon, 09 Jan 2023 20:06:02 GMT
RUN mkdir /data && chown redis:redis /data
# Mon, 09 Jan 2023 20:06:02 GMT
VOLUME [/data]
# Mon, 09 Jan 2023 20:06:02 GMT
WORKDIR /data
# Mon, 09 Jan 2023 20:06:02 GMT
COPY file:a9e7249f657e2eec627bb4be492ad18aae3e5e1f0e47d22644eaf1ef2138c0ce in /usr/local/bin/ 
# Mon, 09 Jan 2023 20:06:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 20:06:03 GMT
EXPOSE 6379
# Mon, 09 Jan 2023 20:06:03 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa0a0152d355cb21f10a6599c8f7b6423492c2afa3ecfb516b49e649ad2b0aa1`  
		Last Modified: Mon, 09 Jan 2023 20:07:37 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:402c460b24b7cb3db325fd375d404548e0faf1b2115355f3bad7182317090eeb`  
		Last Modified: Mon, 09 Jan 2023 20:07:38 GMT  
		Size: 347.7 KB (347680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae243dcb2b477b00de558d499adf07a2309e201aab6075753803eb1112371ce`  
		Last Modified: Mon, 09 Jan 2023 20:08:04 GMT  
		Size: 7.5 MB (7524924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a31b336515a3bde75fe92ea66634d2ba6d61da1f5ba26a828643e48ceb0cef`  
		Last Modified: Mon, 09 Jan 2023 20:08:03 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddab3d6d3afc840ddd90af17d3f7333d89891123d67547a35e1351c2745ceee3`  
		Last Modified: Mon, 09 Jan 2023 20:08:03 GMT  
		Size: 574.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine` - linux; arm variant v6

```console
$ docker pull redis@sha256:d0d1087df99da5331bbcf36880000d2e3f4380fbeaa19b34d732ae2efebf94c9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.0 MB (11027538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0639f2cd9ca0a3c75ea58a1084c4e6e574d2c6202b9cbd92a36ffaf193e742b8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Tue, 22 Nov 2022 22:55:46 GMT
ADD file:132c76d7f7dae2f51f589ee460f1870a2cec6e9dc7ff8e38e88fcee2cfbe70da in / 
# Tue, 22 Nov 2022 22:55:46 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 23:51:31 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Thu, 01 Dec 2022 23:51:33 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Mon, 12 Dec 2022 23:23:04 GMT
ENV REDIS_VERSION=6.2.8
# Mon, 12 Dec 2022 23:23:04 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.8.tar.gz
# Mon, 12 Dec 2022 23:23:04 GMT
ENV REDIS_DOWNLOAD_SHA=f91ab24bcb42673cb853292eb5d43c2017d11d659854808ed6a529c97297fdfe
# Mon, 12 Dec 2022 23:23:51 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Mon, 12 Dec 2022 23:23:51 GMT
RUN mkdir /data && chown redis:redis /data
# Mon, 12 Dec 2022 23:23:52 GMT
VOLUME [/data]
# Mon, 12 Dec 2022 23:23:52 GMT
WORKDIR /data
# Mon, 12 Dec 2022 23:23:52 GMT
COPY file:a9e7249f657e2eec627bb4be492ad18aae3e5e1f0e47d22644eaf1ef2138c0ce in /usr/local/bin/ 
# Mon, 12 Dec 2022 23:23:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Dec 2022 23:23:52 GMT
EXPOSE 6379
# Mon, 12 Dec 2022 23:23:53 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:c2eb4db52fbe1266a78d8c185d33544a2916faa7d82fb5f50909fe233e0579da`  
		Last Modified: Tue, 22 Nov 2022 22:56:39 GMT  
		Size: 3.1 MB (3107138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b91688d0a8d4b6e99c48c41f5fe1a16e0f9b3f2aa685d708c6193c02690525bc`  
		Last Modified: Thu, 01 Dec 2022 23:54:44 GMT  
		Size: 1.2 KB (1238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050c2c061cfa4c7fd9f8755ec721a5fa2fda537b2d82bba53ef33835f5cc28d2`  
		Last Modified: Thu, 01 Dec 2022 23:54:44 GMT  
		Size: 347.8 KB (347780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:121bd7d4df72498702ed52cb561f8203bc98e68dcecadf5220785157d05eb790`  
		Last Modified: Mon, 12 Dec 2022 23:25:33 GMT  
		Size: 7.6 MB (7570701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8c3f37f47622040af67e92e309f0957a1c7074996c4e0488aae1f2fbcefcbb`  
		Last Modified: Mon, 12 Dec 2022 23:25:31 GMT  
		Size: 99.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b636f65bc24c52ebb20dad4d58990c30fc06da10182169b0b129f94aa5b65c6`  
		Last Modified: Mon, 12 Dec 2022 23:25:31 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine` - linux; arm variant v7

```console
$ docker pull redis@sha256:3701537fe1ce2d29a061b47d53d1818ca8e1c274e6b124c7b2cc62adb6e5fd98
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.7 MB (10671556 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd6a9c904f7037d43323cf2d2c825c95477cac87f4c0d7b6408e3eeb9aa94935`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Tue, 22 Nov 2022 22:57:20 GMT
ADD file:080010d9005e8e0dae3e98c7f9afff3e3a40ed32579ca01946efc6ede8316bad in / 
# Tue, 22 Nov 2022 22:57:20 GMT
CMD ["/bin/sh"]
# Fri, 02 Dec 2022 00:01:13 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Fri, 02 Dec 2022 00:01:15 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Mon, 12 Dec 2022 23:58:20 GMT
ENV REDIS_VERSION=6.2.8
# Mon, 12 Dec 2022 23:58:20 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.8.tar.gz
# Mon, 12 Dec 2022 23:58:20 GMT
ENV REDIS_DOWNLOAD_SHA=f91ab24bcb42673cb853292eb5d43c2017d11d659854808ed6a529c97297fdfe
# Mon, 12 Dec 2022 23:58:56 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Mon, 12 Dec 2022 23:58:56 GMT
RUN mkdir /data && chown redis:redis /data
# Mon, 12 Dec 2022 23:58:56 GMT
VOLUME [/data]
# Mon, 12 Dec 2022 23:58:56 GMT
WORKDIR /data
# Mon, 12 Dec 2022 23:58:56 GMT
COPY file:a9e7249f657e2eec627bb4be492ad18aae3e5e1f0e47d22644eaf1ef2138c0ce in /usr/local/bin/ 
# Mon, 12 Dec 2022 23:58:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Dec 2022 23:58:57 GMT
EXPOSE 6379
# Mon, 12 Dec 2022 23:58:57 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:cb2ec849933dd31db64abae3fdcb6923c490d9795577bee1ee1be04eab0376ee`  
		Last Modified: Tue, 22 Nov 2022 22:58:12 GMT  
		Size: 2.9 MB (2865346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef2eb8d5aa57e030bf1ddee4aa613ecca25cd292516e78214cf4bc28434cd74`  
		Last Modified: Fri, 02 Dec 2022 00:05:28 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:959709b3ec332ce2d9e6b098114c0624343032d61ecee79a38f70c4a951db9d7`  
		Last Modified: Fri, 02 Dec 2022 00:05:29 GMT  
		Size: 347.6 KB (347604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21b6d795e3697cfd6a9bf64615a1e406ab2222f7ff9ec33c71aa1178a3f29855`  
		Last Modified: Tue, 13 Dec 2022 00:02:23 GMT  
		Size: 7.5 MB (7456688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327b2b70576b9f3ed5ab1bd08bc356099cd918d174d4bc14fe48ac81c2fd322b`  
		Last Modified: Tue, 13 Dec 2022 00:02:22 GMT  
		Size: 97.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e533dcec5b36a446cd2372e21275c5c4eadb74d3d5c807cba815d6395794c316`  
		Last Modified: Tue, 13 Dec 2022 00:02:22 GMT  
		Size: 578.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:496eeed59ae76f792c1a7f4296f6ed84c36375b874df6f8afb782104cc767541
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.2 MB (11202543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98891aef65eaf867371ecfaaac5b0b28251b1067be0d3b53dc4b495ee07d8bad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 21:43:40 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Mon, 09 Jan 2023 21:43:41 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Mon, 09 Jan 2023 21:44:21 GMT
ENV REDIS_VERSION=6.2.8
# Mon, 09 Jan 2023 21:44:21 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.8.tar.gz
# Mon, 09 Jan 2023 21:44:21 GMT
ENV REDIS_DOWNLOAD_SHA=f91ab24bcb42673cb853292eb5d43c2017d11d659854808ed6a529c97297fdfe
# Mon, 09 Jan 2023 21:44:49 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Mon, 09 Jan 2023 21:44:50 GMT
RUN mkdir /data && chown redis:redis /data
# Mon, 09 Jan 2023 21:44:50 GMT
VOLUME [/data]
# Mon, 09 Jan 2023 21:44:50 GMT
WORKDIR /data
# Mon, 09 Jan 2023 21:44:50 GMT
COPY file:a9e7249f657e2eec627bb4be492ad18aae3e5e1f0e47d22644eaf1ef2138c0ce in /usr/local/bin/ 
# Mon, 09 Jan 2023 21:44:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 21:44:50 GMT
EXPOSE 6379
# Mon, 09 Jan 2023 21:44:50 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60c5bfc4515ca45a1d7e0f19ba442639a014baa29ae89f3ecad5389c2cd2295`  
		Last Modified: Mon, 09 Jan 2023 21:46:09 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b470822c93ffb73ecf0da151fab720a45366613d2db952375c3d90ea75dea3`  
		Last Modified: Mon, 09 Jan 2023 21:46:09 GMT  
		Size: 347.9 KB (347897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a2ded22cac09cdd0f59301805392a3a9f37a310e55f9f08dce2832c8522327`  
		Last Modified: Mon, 09 Jan 2023 21:46:36 GMT  
		Size: 7.6 MB (7593430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8820b5f9f94899bf3226eb6eb0e21799630a2973c0c1958c959a126669768fd`  
		Last Modified: Mon, 09 Jan 2023 21:46:34 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ccd6cf20b5114a1ef517d09b6d90eb57ad51b07eccd5ebf83022e88a50a155b`  
		Last Modified: Mon, 09 Jan 2023 21:46:34 GMT  
		Size: 578.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine` - linux; 386

```console
$ docker pull redis@sha256:f9d1bd8b0ec7452eadbbdd49f031583dc9e5892f05ae535e29a4e883ba7c689d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.0 MB (11012633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:197cee5df8855e3df605e31579407d428a8e33093e1a3286bef1aec4208a4fe6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:00 GMT
ADD file:d03619a0ef81726c34189e849b80cc92da908eb36e116f28275d5765e6d0919a in / 
# Mon, 09 Jan 2023 17:05:00 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 18:30:47 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Mon, 09 Jan 2023 18:30:50 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Mon, 09 Jan 2023 18:31:51 GMT
ENV REDIS_VERSION=6.2.8
# Mon, 09 Jan 2023 18:31:52 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.8.tar.gz
# Mon, 09 Jan 2023 18:31:53 GMT
ENV REDIS_DOWNLOAD_SHA=f91ab24bcb42673cb853292eb5d43c2017d11d659854808ed6a529c97297fdfe
# Mon, 09 Jan 2023 18:32:30 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Mon, 09 Jan 2023 18:32:31 GMT
RUN mkdir /data && chown redis:redis /data
# Mon, 09 Jan 2023 18:32:32 GMT
VOLUME [/data]
# Mon, 09 Jan 2023 18:32:33 GMT
WORKDIR /data
# Mon, 09 Jan 2023 18:32:35 GMT
COPY file:a9e7249f657e2eec627bb4be492ad18aae3e5e1f0e47d22644eaf1ef2138c0ce in /usr/local/bin/ 
# Mon, 09 Jan 2023 18:32:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 18:32:36 GMT
EXPOSE 6379
# Mon, 09 Jan 2023 18:32:37 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:40e5b0b2e2bde18974628cadecd8a2f190f45f06c32846c16885d69b2908bf68`  
		Last Modified: Mon, 09 Jan 2023 17:05:42 GMT  
		Size: 3.4 MB (3408318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e95f02e6879af0d16422eb9bf76a7b8b339bf3b6bae98bacc9ea332c51e28c`  
		Last Modified: Mon, 09 Jan 2023 18:34:50 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0708ca46fe9205b44f1ccec5a22ae0c1ad7d57d53d74beea2b79cac54241d9a`  
		Last Modified: Mon, 09 Jan 2023 18:34:51 GMT  
		Size: 347.6 KB (347605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78267af2660e37bcb401c53870ce214733ee68722b51aab98928590c92b3aa67`  
		Last Modified: Mon, 09 Jan 2023 18:35:24 GMT  
		Size: 7.3 MB (7254796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9a5cf053cfb308ce4a58c2638b5a00b5ef0ca36b2e291d168e6f97ada373850`  
		Last Modified: Mon, 09 Jan 2023 18:35:23 GMT  
		Size: 99.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:392b15e52071e21334cf61fc74b92e9c83e201d3eb46d92d87b24e31573d51e7`  
		Last Modified: Mon, 09 Jan 2023 18:35:23 GMT  
		Size: 576.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine` - linux; ppc64le

```console
$ docker pull redis@sha256:66b9289dc3e9a4a461f2243fd95aa97785ba549d5a6132c35cda65935e507eea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.9 MB (11868647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af7f773ebf6097c050c4d772a8cbd965b760f1580f8f352221d31523de78abd4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 23 Nov 2022 00:18:18 GMT
ADD file:a8e68f93c597f70ce637ef578c72c9b41b4b8d80b552b8e5570d4efcc1d02ff5 in / 
# Wed, 23 Nov 2022 00:18:18 GMT
CMD ["/bin/sh"]
# Fri, 02 Dec 2022 00:19:09 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Fri, 02 Dec 2022 00:19:13 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Mon, 12 Dec 2022 22:12:35 GMT
ENV REDIS_VERSION=6.2.8
# Mon, 12 Dec 2022 22:12:35 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.8.tar.gz
# Mon, 12 Dec 2022 22:12:35 GMT
ENV REDIS_DOWNLOAD_SHA=f91ab24bcb42673cb853292eb5d43c2017d11d659854808ed6a529c97297fdfe
# Mon, 12 Dec 2022 22:13:23 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Mon, 12 Dec 2022 22:13:24 GMT
RUN mkdir /data && chown redis:redis /data
# Mon, 12 Dec 2022 22:13:24 GMT
VOLUME [/data]
# Mon, 12 Dec 2022 22:13:25 GMT
WORKDIR /data
# Mon, 12 Dec 2022 22:13:25 GMT
COPY file:a9e7249f657e2eec627bb4be492ad18aae3e5e1f0e47d22644eaf1ef2138c0ce in /usr/local/bin/ 
# Mon, 12 Dec 2022 22:13:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Dec 2022 22:13:26 GMT
EXPOSE 6379
# Mon, 12 Dec 2022 22:13:26 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:69314845b945e4b33e4ee552d0e4156645f71c81b6cb71108c1e32e139aec052`  
		Last Modified: Wed, 23 Nov 2022 00:19:02 GMT  
		Size: 3.4 MB (3384500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67cfdac3009c2f827e7dc6432edc1f3726b1ba8a8f35b7ff173284e78a7516ed`  
		Last Modified: Fri, 02 Dec 2022 00:23:51 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3786223a169388cd0603f29896b77f4deff5978199f9db1783b026551007d3`  
		Last Modified: Fri, 02 Dec 2022 00:23:50 GMT  
		Size: 347.9 KB (347932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a75dc8926edb3ff0d652d7b55fb8dc306a51575a00e504b5606aaa0ca7fdb979`  
		Last Modified: Mon, 12 Dec 2022 22:16:35 GMT  
		Size: 8.1 MB (8134233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c316b8bbdfb5170371d8cafe2c83563d90ae8db67fd6c1336bf3b609209e6134`  
		Last Modified: Mon, 12 Dec 2022 22:16:32 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c1fd4deeac2e1f6a191e4e02aa989f35b351cfb0e00d61185a0c25bd1a169a`  
		Last Modified: Mon, 12 Dec 2022 22:16:32 GMT  
		Size: 578.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine` - linux; s390x

```console
$ docker pull redis@sha256:a781dbacd0b4cbf08cf01d2e0264ae284d9f289361e8eb19bf085b1116c22f20
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.3 MB (11341438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:571310f8d90017392d1665b441bd29cc6e9497f8c65db01267209f2165f674e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Tue, 22 Nov 2022 22:47:02 GMT
ADD file:d8cbd162b64e4b7a8b83086be37ef5ee69e955ac955ebbe59e70c6be2a2d1a9f in / 
# Tue, 22 Nov 2022 22:47:03 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 23:46:57 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Thu, 01 Dec 2022 23:46:58 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Mon, 12 Dec 2022 23:04:51 GMT
ENV REDIS_VERSION=6.2.8
# Mon, 12 Dec 2022 23:04:51 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.8.tar.gz
# Mon, 12 Dec 2022 23:04:51 GMT
ENV REDIS_DOWNLOAD_SHA=f91ab24bcb42673cb853292eb5d43c2017d11d659854808ed6a529c97297fdfe
# Mon, 12 Dec 2022 23:05:32 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Mon, 12 Dec 2022 23:05:33 GMT
RUN mkdir /data && chown redis:redis /data
# Mon, 12 Dec 2022 23:05:33 GMT
VOLUME [/data]
# Mon, 12 Dec 2022 23:05:33 GMT
WORKDIR /data
# Mon, 12 Dec 2022 23:05:34 GMT
COPY file:a9e7249f657e2eec627bb4be492ad18aae3e5e1f0e47d22644eaf1ef2138c0ce in /usr/local/bin/ 
# Mon, 12 Dec 2022 23:05:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Dec 2022 23:05:34 GMT
EXPOSE 6379
# Mon, 12 Dec 2022 23:05:34 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:844b8973ca9523380e35625da9a5fd2d50338c403129146541e13d0722c056f7`  
		Last Modified: Tue, 22 Nov 2022 22:47:59 GMT  
		Size: 3.2 MB (3170814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db1be814075d1274a0e9bcb59929c7021970d8964094b5e2ad21d1d9d97776bb`  
		Last Modified: Thu, 01 Dec 2022 23:51:08 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44c07df67a06c981699be9f591dda0031fe1c1680c39d733f9f4b22de636d128`  
		Last Modified: Thu, 01 Dec 2022 23:51:08 GMT  
		Size: 347.7 KB (347658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81761d43cbe4f9c09d998ae4b0bdcc2a1f6e39da23ebc809270646ae7b6e683c`  
		Last Modified: Mon, 12 Dec 2022 23:07:57 GMT  
		Size: 7.8 MB (7820987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35f156163e29c913d6a1e9bc6bdb6d6a08db866ad5c05f0bc03693b7ffe68d1c`  
		Last Modified: Mon, 12 Dec 2022 23:07:56 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46aeef5b80ac516c3f46508c8f66a9005dc77dcf41097a155d9cc2f9c99e58b2`  
		Last Modified: Mon, 12 Dec 2022 23:07:56 GMT  
		Size: 577.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
