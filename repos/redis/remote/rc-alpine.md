## `redis:rc-alpine`

```console
$ docker pull redis@sha256:d8bc279440fa6564ede832c579d435e90f9d0437aab6f699c52d376d0ab76efa
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

### `redis:rc-alpine` - linux; amd64

```console
$ docker pull redis@sha256:641817e4de52818d8c712760a12852d7bd07a66b9daa42ebd2dd0d9ba28068d8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.9 MB (10879568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bca63d382f81801f11ed9b04f8b1099edde8bcd39fb60be410345e7250f484c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 12:53:24 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Thu, 17 Dec 2020 12:53:25 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Thu, 17 Dec 2020 12:53:25 GMT
ENV REDIS_VERSION=6.2-rc1
# Thu, 17 Dec 2020 12:53:26 GMT
ENV REDIS_DOWNLOAD_URL=https://github.com/redis/redis/archive/6.2-rc1.tar.gz
# Thu, 17 Dec 2020 12:53:26 GMT
ENV REDIS_DOWNLOAD_SHA=bb7b18aaed17d70efce77ae56d2f7211dd077bcd0e2b94897188eed3e2484c78
# Thu, 17 Dec 2020 12:55:17 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Thu, 17 Dec 2020 12:55:19 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 17 Dec 2020 12:55:20 GMT
VOLUME [/data]
# Thu, 17 Dec 2020 12:55:20 GMT
WORKDIR /data
# Thu, 17 Dec 2020 12:55:21 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Thu, 17 Dec 2020 12:55:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 12:55:21 GMT
EXPOSE 6379
# Thu, 17 Dec 2020 12:55:22 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a8d0188e48174d9e60f943c4e463c23268b864ed4f146041bee8d79710cc359`  
		Last Modified: Thu, 17 Dec 2020 13:00:14 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a3f5c4e0176ac6c0887cb55795f7ffd12376b33d546a11bb4f5c306133e7606`  
		Last Modified: Thu, 17 Dec 2020 13:00:14 GMT  
		Size: 381.5 KB (381525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9af23bab33d0b044adf2a7763f82025fa8eceb77b1e95fe61ed0763303d05f6`  
		Last Modified: Thu, 17 Dec 2020 13:00:16 GMT  
		Size: 7.7 MB (7697231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e24b8f34bba1bd53a1b7ae940af1e87704e21760c7f3ab6c0ca55b6a62a4629`  
		Last Modified: Thu, 17 Dec 2020 13:00:15 GMT  
		Size: 100.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d216621fb7bbb6dc6c91dd2fc645af6bc216cdd50a2f5220352f280fbe4567`  
		Last Modified: Thu, 17 Dec 2020 13:00:14 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:rc-alpine` - linux; arm variant v6

```console
$ docker pull redis@sha256:d96c2dfb4fc0456dcc44e6e4163745fbd1b3a8092b0f5b5d25c585e89656d0e3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.6 MB (10602486 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d04f5515f1c80b85bb821456d7f821f13850f3c4f344eca0bdab7253e0a0e03`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 07:46:58 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Thu, 17 Dec 2020 07:47:01 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Wed, 13 Jan 2021 00:54:56 GMT
ENV REDIS_VERSION=6.2-rc2
# Wed, 13 Jan 2021 00:54:57 GMT
ENV REDIS_DOWNLOAD_URL=https://github.com/redis/redis/archive/6.2-rc2.tar.gz
# Wed, 13 Jan 2021 00:54:58 GMT
ENV REDIS_DOWNLOAD_SHA=9b48819edd2823dfb71395cc4e63079df2c13a5cc8ffb61bb896d4847a7023e7
# Wed, 13 Jan 2021 00:55:53 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Wed, 13 Jan 2021 00:55:56 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 13 Jan 2021 00:55:58 GMT
VOLUME [/data]
# Wed, 13 Jan 2021 00:56:00 GMT
WORKDIR /data
# Wed, 13 Jan 2021 00:56:01 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Wed, 13 Jan 2021 00:56:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jan 2021 00:56:03 GMT
EXPOSE 6379
# Wed, 13 Jan 2021 00:56:05 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40124c0d73f95636123785ccdb99c93a3454329868c5537721760fba0d5e99c9`  
		Last Modified: Thu, 17 Dec 2020 07:50:47 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd139e1646613b396219f74e964daafa46866e4b8c2126479be9e0723bc92fc`  
		Last Modified: Thu, 17 Dec 2020 07:50:50 GMT  
		Size: 384.9 KB (384906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ebb55b74af1af59236810c91b2fbd455735f4722a72841fa6959f2c2df52e7b`  
		Last Modified: Wed, 13 Jan 2021 00:58:02 GMT  
		Size: 7.6 MB (7611609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b678cdad9dc3e712ae4aed85c954227294c56fadfdf729c006b5063d5aa95e6d`  
		Last Modified: Wed, 13 Jan 2021 00:58:01 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b3a6ae1a2aa887f578a5273836900184e6222f63e2339dbaf0a9280cbecb0b`  
		Last Modified: Wed, 13 Jan 2021 00:58:00 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:rc-alpine` - linux; arm variant v7

```console
$ docker pull redis@sha256:250d596fbef60ba89ab7cdda75a25b10ecf78d7a42e2031c5f05311bd70387e0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.3 MB (10268587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f727cc142144e6b4d2bc0ba1ba10896933ddd6ec3a734582d079289cdad5c16e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 06:01:41 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Thu, 17 Dec 2020 06:01:46 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Wed, 13 Jan 2021 02:58:17 GMT
ENV REDIS_VERSION=6.2-rc2
# Wed, 13 Jan 2021 02:58:17 GMT
ENV REDIS_DOWNLOAD_URL=https://github.com/redis/redis/archive/6.2-rc2.tar.gz
# Wed, 13 Jan 2021 02:58:18 GMT
ENV REDIS_DOWNLOAD_SHA=9b48819edd2823dfb71395cc4e63079df2c13a5cc8ffb61bb896d4847a7023e7
# Wed, 13 Jan 2021 02:59:05 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Wed, 13 Jan 2021 02:59:07 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 13 Jan 2021 02:59:08 GMT
VOLUME [/data]
# Wed, 13 Jan 2021 02:59:08 GMT
WORKDIR /data
# Wed, 13 Jan 2021 02:59:09 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Wed, 13 Jan 2021 02:59:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jan 2021 02:59:11 GMT
EXPOSE 6379
# Wed, 13 Jan 2021 02:59:11 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:016dc30bee1352371169f899cf6dadeffe365c1216856983c92d32c8bc0838db`  
		Last Modified: Thu, 17 Dec 2020 06:06:17 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77141b34d8205444d6a790020e004ece4dce84a015044e30f7764314baabe163`  
		Last Modified: Thu, 17 Dec 2020 06:06:17 GMT  
		Size: 378.5 KB (378466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d166357add3ff929e3d1e9002eb2a8414d7ef6a0e6b8cfbaa301b7013dbfd3f`  
		Last Modified: Wed, 13 Jan 2021 03:03:23 GMT  
		Size: 7.5 MB (7480758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78088e128e5faaee437754b8a0058ae39ceb66770bf62c2d1301af61c5e105a0`  
		Last Modified: Wed, 13 Jan 2021 03:03:19 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f4b6e476d42d87aaf3f1770200a2bd4a9286d8f64eb1223df409f04b5ac65e5`  
		Last Modified: Wed, 13 Jan 2021 03:03:19 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:rc-alpine` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:0b23dbaf740ab5e25623f853ece6e2473efef2a3becbac44fa46c53bf669d645
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.8 MB (10796886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d774d3bae490986ebdf97fa40b983a625254cbfdece82e973f7cb2f3721f06c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 04:31:21 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Thu, 17 Dec 2020 04:31:30 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Thu, 17 Dec 2020 04:31:32 GMT
ENV REDIS_VERSION=6.2-rc1
# Thu, 17 Dec 2020 04:31:34 GMT
ENV REDIS_DOWNLOAD_URL=https://github.com/redis/redis/archive/6.2-rc1.tar.gz
# Thu, 17 Dec 2020 04:31:36 GMT
ENV REDIS_DOWNLOAD_SHA=bb7b18aaed17d70efce77ae56d2f7211dd077bcd0e2b94897188eed3e2484c78
# Thu, 17 Dec 2020 04:32:41 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Thu, 17 Dec 2020 04:32:44 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 17 Dec 2020 04:32:45 GMT
VOLUME [/data]
# Thu, 17 Dec 2020 04:32:47 GMT
WORKDIR /data
# Thu, 17 Dec 2020 04:32:47 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Thu, 17 Dec 2020 04:32:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 04:32:49 GMT
EXPOSE 6379
# Thu, 17 Dec 2020 04:32:50 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db34f812ca31140e369d56b86750ffc993f48a2c7f3d918faa1656c9ee2091ed`  
		Last Modified: Thu, 17 Dec 2020 04:37:14 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d1078d6539f84db18283766b6f742be80c0aa5f711f32c629d8da00076e1a5`  
		Last Modified: Thu, 17 Dec 2020 04:37:15 GMT  
		Size: 383.9 KB (383926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9f8c359b877102fcfeeb4080aab0bb083e5e172746bd509ec075c52efdf4e10`  
		Last Modified: Thu, 17 Dec 2020 04:37:17 GMT  
		Size: 7.7 MB (7702106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a6d66fb781adccf1920d60592a28be04b0c63807c6131aa56f61fd03cefa12e`  
		Last Modified: Thu, 17 Dec 2020 04:37:14 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d4041c8c48d4bcba6dca02f290e009a76a894e3952c68a76abd5a894a6cdc0`  
		Last Modified: Thu, 17 Dec 2020 04:37:14 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:rc-alpine` - linux; 386

```console
$ docker pull redis@sha256:6340c00e8d323c70a317787854d84fbca8b06133291963ec3874793db0364b56
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.6 MB (10595061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78b7b6ede1d35f5eff3974c10257398d0f3a7ea38da7612a7951341d40470fb0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 17 Dec 2020 00:38:32 GMT
ADD file:de33fda50a142403e842620d20bc4404e66fc4ace16edc6946c4539e8a797458 in / 
# Thu, 17 Dec 2020 00:38:32 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 07:18:27 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Thu, 17 Dec 2020 07:18:28 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Wed, 13 Jan 2021 00:49:22 GMT
ENV REDIS_VERSION=6.2-rc2
# Wed, 13 Jan 2021 00:49:22 GMT
ENV REDIS_DOWNLOAD_URL=https://github.com/redis/redis/archive/6.2-rc2.tar.gz
# Wed, 13 Jan 2021 00:49:22 GMT
ENV REDIS_DOWNLOAD_SHA=9b48819edd2823dfb71395cc4e63079df2c13a5cc8ffb61bb896d4847a7023e7
# Wed, 13 Jan 2021 00:51:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Wed, 13 Jan 2021 00:51:54 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 13 Jan 2021 00:51:54 GMT
VOLUME [/data]
# Wed, 13 Jan 2021 00:51:55 GMT
WORKDIR /data
# Wed, 13 Jan 2021 00:51:55 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Wed, 13 Jan 2021 00:51:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jan 2021 00:51:56 GMT
EXPOSE 6379
# Wed, 13 Jan 2021 00:51:56 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:455793c72b878001f0905634ed52a2524ba51796e7377bf00683a85123f7dce9`  
		Last Modified: Thu, 17 Dec 2020 00:39:18 GMT  
		Size: 2.8 MB (2794130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:158c4edad6eb4817abd5e3c2b06b2f1aa5ad7811d33774f2942ab00b34314135`  
		Last Modified: Thu, 17 Dec 2020 07:23:09 GMT  
		Size: 1.2 KB (1229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:facc0878898feba5ee198462ea38c2d03a502f33710c7d24234c5f944cef7d49`  
		Last Modified: Thu, 17 Dec 2020 07:23:09 GMT  
		Size: 387.0 KB (386952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e72e2c3326b455c8b17acf9fb3e96a4e99701fae39fe6968ba2b3c818eb145ad`  
		Last Modified: Wed, 13 Jan 2021 00:59:09 GMT  
		Size: 7.4 MB (7412233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2880380140353027673abe29cd0bcf4449d6d58f7428ef8d02ac2717938b15e9`  
		Last Modified: Wed, 13 Jan 2021 00:59:12 GMT  
		Size: 99.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:683f45c2bdae758499fdb4ace0a28bce7119dbcba8827802ff664c46b21949f4`  
		Last Modified: Wed, 13 Jan 2021 00:59:05 GMT  
		Size: 418.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:rc-alpine` - linux; ppc64le

```console
$ docker pull redis@sha256:5bc3a439bb684225b5dc8e54c60c0f3833ebb9bdeb2ed425c265dacc4d2b555d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.4 MB (11406911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89b8279a571c96232122410462682dc947d1c1a998b56d52c88a441220159e7b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 17 Dec 2020 00:20:42 GMT
ADD file:0a38c9b4955f8faa79627c166fca80ef342e443a16ce2925a30eeae317bbd786 in / 
# Thu, 17 Dec 2020 00:20:48 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 09:29:31 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Thu, 17 Dec 2020 09:29:37 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Thu, 17 Dec 2020 09:29:39 GMT
ENV REDIS_VERSION=6.2-rc1
# Thu, 17 Dec 2020 09:29:43 GMT
ENV REDIS_DOWNLOAD_URL=https://github.com/redis/redis/archive/6.2-rc1.tar.gz
# Thu, 17 Dec 2020 09:29:46 GMT
ENV REDIS_DOWNLOAD_SHA=bb7b18aaed17d70efce77ae56d2f7211dd077bcd0e2b94897188eed3e2484c78
# Thu, 17 Dec 2020 09:30:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Thu, 17 Dec 2020 09:30:51 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 17 Dec 2020 09:30:55 GMT
VOLUME [/data]
# Thu, 17 Dec 2020 09:31:01 GMT
WORKDIR /data
# Thu, 17 Dec 2020 09:31:04 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Thu, 17 Dec 2020 09:31:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 09:31:08 GMT
EXPOSE 6379
# Thu, 17 Dec 2020 09:31:11 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:a9d343b7bcc225fe7ac17d96a81329510ab7f31a50472311cafe7168d3107317`  
		Last Modified: Thu, 17 Dec 2020 00:21:33 GMT  
		Size: 2.8 MB (2805226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e8d0d5e19985959d65a37003a438fb8943b89e582ca7917c449835c614db5df`  
		Last Modified: Thu, 17 Dec 2020 09:35:20 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9969035389a56309d4cff14d9854eb67648a92d7aa151bce27238b926d851034`  
		Last Modified: Thu, 17 Dec 2020 09:35:20 GMT  
		Size: 388.4 KB (388384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dfa720485044ef67584b4e2fc807ef9bf1db77b70d53965ddf93bd8d7008905`  
		Last Modified: Thu, 17 Dec 2020 09:35:21 GMT  
		Size: 8.2 MB (8211488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f20dc69c10f16c4b16d535b1823a75c1bf3f57c8bf4f33336edb7191ca656372`  
		Last Modified: Thu, 17 Dec 2020 09:35:19 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14d60103e0607d561c6ff0eeba1bb32ec52e365d889ef4292d593d426d3e8ae0`  
		Last Modified: Thu, 17 Dec 2020 09:35:20 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:rc-alpine` - linux; s390x

```console
$ docker pull redis@sha256:5f4c7d12c15d7744355b2b0ee130799c8d76ce0d30b8d7aa2d00dcee0bf7e7c2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.9 MB (10944047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d54bfdd98d3a58f89af3dc23a80e8a3a76fb5974953f934e53cfeb5a51848bc2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 16 Dec 2020 23:41:37 GMT
ADD file:3ad3856d165e8760af85574a8ffa75ca44b7e1b97b64d1d6d4608445efa4b860 in / 
# Wed, 16 Dec 2020 23:41:37 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 09:36:53 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Thu, 17 Dec 2020 09:36:56 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Thu, 17 Dec 2020 09:36:57 GMT
ENV REDIS_VERSION=6.2-rc1
# Thu, 17 Dec 2020 09:36:57 GMT
ENV REDIS_DOWNLOAD_URL=https://github.com/redis/redis/archive/6.2-rc1.tar.gz
# Thu, 17 Dec 2020 09:36:58 GMT
ENV REDIS_DOWNLOAD_SHA=bb7b18aaed17d70efce77ae56d2f7211dd077bcd0e2b94897188eed3e2484c78
# Thu, 17 Dec 2020 09:38:06 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Thu, 17 Dec 2020 09:38:08 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 17 Dec 2020 09:38:09 GMT
VOLUME [/data]
# Thu, 17 Dec 2020 09:38:10 GMT
WORKDIR /data
# Thu, 17 Dec 2020 09:38:10 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Thu, 17 Dec 2020 09:38:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 09:38:12 GMT
EXPOSE 6379
# Thu, 17 Dec 2020 09:38:13 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:ee52640a49e15b8b7c8edb66c2d048b26abdee8d828d6e5ef4e10a28cb15a84f`  
		Last Modified: Wed, 16 Dec 2020 23:42:15 GMT  
		Size: 2.6 MB (2567018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2007345c0ef6eac7083589d387182c4b51ad9e1f4e573a54992689c51ccdbc50`  
		Last Modified: Thu, 17 Dec 2020 09:42:33 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd649604246bf9f7e6ebfe3c3772a714e12c1734f4da680e97933eacd340cd7d`  
		Last Modified: Thu, 17 Dec 2020 09:42:32 GMT  
		Size: 386.4 KB (386399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a746912ac65804b9650d5e5efa813f41b7629ce487c26744185b46a77aa6b4ef`  
		Last Modified: Thu, 17 Dec 2020 09:42:35 GMT  
		Size: 8.0 MB (7988820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62e1c4eaa5237593e9353b0433b005ac0b6b8fd28a19501b77262d98d4199fbf`  
		Last Modified: Thu, 17 Dec 2020 09:42:33 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d87de7d46b029979e898b3fda4e9b27cfb6a8f9b52e3b543a2eb88bf9c9d8f7`  
		Last Modified: Thu, 17 Dec 2020 09:42:33 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
