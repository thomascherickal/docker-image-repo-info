## `redis:6-alpine3.12`

```console
$ docker pull redis@sha256:b7a605df2fcdc2d7a2d977f70a955e39cc0a9897dc56129eae3d32d533a72b44
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

### `redis:6-alpine3.12` - linux; amd64

```console
$ docker pull redis@sha256:4920debee18fad71841ce101a7867743ff8fe7d47e6191b750c3edcfffc1cb18
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.6 MB (10616443 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f731cd48185c2bc96057d5bc76e2cdb398dee800c7608bc3ec52e423d27e0f0a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 16:25:16 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Fri, 11 Dec 2020 16:25:18 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Fri, 11 Dec 2020 16:25:18 GMT
ENV REDIS_VERSION=6.0.9
# Fri, 11 Dec 2020 16:25:18 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.9.tar.gz
# Fri, 11 Dec 2020 16:25:18 GMT
ENV REDIS_DOWNLOAD_SHA=dc2bdcf81c620e9f09cfd12e85d3bc631c897b2db7a55218fd8a65eaa37f86dd
# Fri, 11 Dec 2020 16:26:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 11 Dec 2020 16:26:16 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 11 Dec 2020 16:26:17 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 16:26:17 GMT
WORKDIR /data
# Fri, 11 Dec 2020 16:26:17 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 11 Dec 2020 16:26:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 16:26:17 GMT
EXPOSE 6379
# Fri, 11 Dec 2020 16:26:18 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c9d57a1c7f4bb594339d259d1485b48bd5b81e9e6f662b4791b1dadc5d4daf`  
		Last Modified: Fri, 11 Dec 2020 16:30:52 GMT  
		Size: 1.2 KB (1229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccd033d7ec061821df52b64df5078b36d1f755a2f02e4b6b578e3ebd739313dd`  
		Last Modified: Fri, 11 Dec 2020 16:30:53 GMT  
		Size: 381.5 KB (381504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ff79b059f9901008744218e40a0c2cc2194b860cb44d9c5a7f37a9b3f6c9c1b`  
		Last Modified: Fri, 11 Dec 2020 16:30:54 GMT  
		Size: 7.4 MB (7436255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d91237314b7702f9f49259aadffd895f5e5da9ecf2ed189279bc80a38fad2c99`  
		Last Modified: Fri, 11 Dec 2020 16:30:53 GMT  
		Size: 99.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47d41ba6aa87a9d0622f389d6d86f94c8f9eaec54e6b6aed0f87f9f675f0b35`  
		Last Modified: Fri, 11 Dec 2020 16:30:55 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine3.12` - linux; arm variant v6

```console
$ docker pull redis@sha256:1f3a06f1bf62780d2f81ee6ce7952cc3bc354efabb5012905e39fb7f919c9737
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.3 MB (10298529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d066ee281e4401396a80e77d8430f5700066c397fb9ef302aaa904874f2f25aa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Fri, 11 Dec 2020 02:17:15 GMT
ADD file:1a9c0a67560d338c0c0e7005d8915d998fc9cf3e9f53bfd7e42e8391f0a39bce in / 
# Fri, 11 Dec 2020 02:17:15 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:10:34 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Fri, 11 Dec 2020 05:10:43 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Fri, 11 Dec 2020 05:10:44 GMT
ENV REDIS_VERSION=6.0.9
# Fri, 11 Dec 2020 05:10:46 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.9.tar.gz
# Fri, 11 Dec 2020 05:10:47 GMT
ENV REDIS_DOWNLOAD_SHA=dc2bdcf81c620e9f09cfd12e85d3bc631c897b2db7a55218fd8a65eaa37f86dd
# Fri, 11 Dec 2020 05:11:45 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 11 Dec 2020 05:11:48 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 11 Dec 2020 05:11:49 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 05:11:51 GMT
WORKDIR /data
# Fri, 11 Dec 2020 05:11:53 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 11 Dec 2020 05:11:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:11:56 GMT
EXPOSE 6379
# Fri, 11 Dec 2020 05:11:57 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:f1c16df8fee33d421d08790b17ca2af67a3fe49e77b6b991dd0c30631f5d1baf`  
		Last Modified: Fri, 11 Dec 2020 02:17:57 GMT  
		Size: 2.6 MB (2601992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:447a76a74c6810b07663d685dcd2f99da1fc67cf7824495b6f04910e7723f678`  
		Last Modified: Fri, 11 Dec 2020 05:13:24 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c23f37f74eda655a638a407067de4a279a1536b0fa95d392a642008f7ca9504c`  
		Last Modified: Fri, 11 Dec 2020 05:13:24 GMT  
		Size: 384.9 KB (384903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376c02a72867d551dccf4d126de821cbf525915f4a2134bdd9ac64efc356dfa5`  
		Last Modified: Fri, 11 Dec 2020 05:13:27 GMT  
		Size: 7.3 MB (7309830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2841ac26cd6d92532b6b078236ac00325878be691b4b4c6b8ff7e243c60299a`  
		Last Modified: Fri, 11 Dec 2020 05:13:24 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6bbb6f08c45dc43c49d843e77355eeb67b2f639b2de072cf7d1c88c5179ccfa`  
		Last Modified: Fri, 11 Dec 2020 05:13:24 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine3.12` - linux; arm variant v7

```console
$ docker pull redis@sha256:e0cafbbd3012fd1ec61eb0c08d763e9e6ebaf8005bdcae3c9e9e06c889a550d5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (9975285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d507472c7a727bfdcd9dd573d8c7cb23e062a175c0d1a5d1dd75b5fd9c2f1575`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Fri, 11 Dec 2020 02:20:33 GMT
ADD file:0e85952ec585d17378d9bb15a94ddc10c3ed8f766f275cf50fb36be1126f35d2 in / 
# Fri, 11 Dec 2020 02:20:34 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 15:47:37 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Fri, 11 Dec 2020 15:47:41 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Fri, 11 Dec 2020 15:47:42 GMT
ENV REDIS_VERSION=6.0.9
# Fri, 11 Dec 2020 15:47:43 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.9.tar.gz
# Fri, 11 Dec 2020 15:47:44 GMT
ENV REDIS_DOWNLOAD_SHA=dc2bdcf81c620e9f09cfd12e85d3bc631c897b2db7a55218fd8a65eaa37f86dd
# Fri, 11 Dec 2020 15:48:35 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 11 Dec 2020 15:48:39 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 11 Dec 2020 15:48:40 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 15:48:40 GMT
WORKDIR /data
# Fri, 11 Dec 2020 15:48:41 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 11 Dec 2020 15:48:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 15:48:43 GMT
EXPOSE 6379
# Fri, 11 Dec 2020 15:48:45 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:f70c74f2e22556cebd0cbbff78c03d4f0560d76979bf799d67730340a639aa57`  
		Last Modified: Fri, 11 Dec 2020 02:21:18 GMT  
		Size: 2.4 MB (2405692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bdac81f68b558d3a5d368f3b955dc55a67a9c6cfb03221be0d3dfaee25d087e`  
		Last Modified: Fri, 11 Dec 2020 15:53:27 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce249ae19ee7cfd52424c42faa2e50309438aebacb9a43947eb1fdec74bf031`  
		Last Modified: Fri, 11 Dec 2020 15:53:26 GMT  
		Size: 378.5 KB (378477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e495ee124e93fe4c9ab62137c66e4842ae31642a5db511527dd3c0a9e7d1ae4a`  
		Last Modified: Fri, 11 Dec 2020 15:53:28 GMT  
		Size: 7.2 MB (7189311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7375900d77eef3a72f6eaf54d0f65b42d5daa4a7f58411c5a96038b99523ee`  
		Last Modified: Fri, 11 Dec 2020 15:53:26 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a29218c610a3176586033c660089935fa5d7c712c6abb8b8d73659482ec45f2b`  
		Last Modified: Fri, 11 Dec 2020 15:53:27 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine3.12` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:3c2f4c6f2198353515645e8f26579ecb784d5dbc482a09f64fd75fa356bbaded
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.5 MB (10538961 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be1387a3afff9818204a65b266441831e38fb404b96454c6806e2fa14cc40a8b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 15:02:17 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Fri, 11 Dec 2020 15:02:27 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Fri, 11 Dec 2020 15:02:27 GMT
ENV REDIS_VERSION=6.0.9
# Fri, 11 Dec 2020 15:02:29 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.9.tar.gz
# Fri, 11 Dec 2020 15:02:30 GMT
ENV REDIS_DOWNLOAD_SHA=dc2bdcf81c620e9f09cfd12e85d3bc631c897b2db7a55218fd8a65eaa37f86dd
# Fri, 11 Dec 2020 15:03:29 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 11 Dec 2020 15:03:35 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 11 Dec 2020 15:03:37 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 15:03:38 GMT
WORKDIR /data
# Fri, 11 Dec 2020 15:03:39 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 11 Dec 2020 15:03:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 15:03:41 GMT
EXPOSE 6379
# Fri, 11 Dec 2020 15:03:41 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:644769aa9380d3217180aef39343466a8888ab65d032d49b2e0d076e1ae64439`  
		Last Modified: Fri, 11 Dec 2020 15:08:09 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d71757449c7064c22fec07fcdc49bb7e35eb87d73ea3bf8c27d1a905d48919d`  
		Last Modified: Fri, 11 Dec 2020 15:08:09 GMT  
		Size: 383.9 KB (383919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3cd5f021d563a6ee7aa62d867017fd12906672c59780e893f251b32c352cf9c`  
		Last Modified: Fri, 11 Dec 2020 15:08:12 GMT  
		Size: 7.4 MB (7446615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1e5adad9c79ea2144deca62b13ee827c6e6215c5bf2c78ea0cb65547c6830e`  
		Last Modified: Fri, 11 Dec 2020 15:08:09 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0306f453b38c725ecca92c6919b0d3a5a2adcb43433fdf0dd6f5c521c9251a4b`  
		Last Modified: Fri, 11 Dec 2020 15:08:09 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine3.12` - linux; 386

```console
$ docker pull redis@sha256:11c668c42354850a57e763dfaf466377160b4b7f8ca8a3386d1fe7635ad49925
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.2 MB (10165934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bcf50494a811f099981ffb562f6420f004af9e7268dd20f26d9d56b806b7423c`
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
# Tue, 27 Oct 2020 18:52:31 GMT
ENV REDIS_VERSION=6.0.9
# Tue, 27 Oct 2020 18:52:31 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.9.tar.gz
# Tue, 27 Oct 2020 18:52:31 GMT
ENV REDIS_DOWNLOAD_SHA=dc2bdcf81c620e9f09cfd12e85d3bc631c897b2db7a55218fd8a65eaa37f86dd
# Tue, 27 Oct 2020 18:53:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Tue, 27 Oct 2020 18:53:49 GMT
RUN mkdir /data && chown redis:redis /data
# Tue, 27 Oct 2020 18:53:49 GMT
VOLUME [/data]
# Tue, 27 Oct 2020 18:53:50 GMT
WORKDIR /data
# Tue, 27 Oct 2020 18:53:50 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Tue, 27 Oct 2020 18:53:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 27 Oct 2020 18:53:50 GMT
EXPOSE 6379
# Tue, 27 Oct 2020 18:53:50 GMT
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
	-	`sha256:a4c0228bd36855a7879a83900f726d9955f38132fa9c4690301c80d2c9d1aaef`  
		Last Modified: Tue, 27 Oct 2020 18:57:03 GMT  
		Size: 7.1 MB (7111402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3277e25fd087e30209de55960dd41c90bc1bbfa5d634136e19377eeed64f25a1`  
		Last Modified: Tue, 27 Oct 2020 18:57:01 GMT  
		Size: 100.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932ded4edc680655c90a182a5a432d03093494b0a20a773a7a35c48719e4f798`  
		Last Modified: Tue, 27 Oct 2020 18:57:01 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine3.12` - linux; ppc64le

```console
$ docker pull redis@sha256:73fc4a15e734570f71ef64171fb6c18f6fd77b2600a7ff11c79add47d4a5c2e5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.0 MB (11005565 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9365a495cb6714971706629a98af83b5eeaac607aca058d09edff23427f76f4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 22 Oct 2020 11:00:06 GMT
ADD file:176e047fab2c1828575bffa6b14773efa297b7ecf312d86103c5dd4f78ec8027 in / 
# Thu, 22 Oct 2020 11:00:17 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 22:35:47 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Thu, 22 Oct 2020 22:35:57 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Tue, 27 Oct 2020 18:23:42 GMT
ENV REDIS_VERSION=6.0.9
# Tue, 27 Oct 2020 18:23:45 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.9.tar.gz
# Tue, 27 Oct 2020 18:23:47 GMT
ENV REDIS_DOWNLOAD_SHA=dc2bdcf81c620e9f09cfd12e85d3bc631c897b2db7a55218fd8a65eaa37f86dd
# Tue, 27 Oct 2020 18:24:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Tue, 27 Oct 2020 18:24:55 GMT
RUN mkdir /data && chown redis:redis /data
# Tue, 27 Oct 2020 18:24:56 GMT
VOLUME [/data]
# Tue, 27 Oct 2020 18:25:03 GMT
WORKDIR /data
# Tue, 27 Oct 2020 18:25:04 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Tue, 27 Oct 2020 18:25:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 27 Oct 2020 18:25:15 GMT
EXPOSE 6379
# Tue, 27 Oct 2020 18:25:19 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:692a9d763e196c85d79fc3e45b316b1bb557c93ba88a3c8ebf679a585d1efe73`  
		Last Modified: Thu, 22 Oct 2020 11:02:06 GMT  
		Size: 2.8 MB (2803218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e48583f52640e5f838d8293b8b84eb715c9495d35e0d2b59baa879a3032d2434`  
		Last Modified: Thu, 22 Oct 2020 22:40:43 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11a4e4c49b0451515cfa0d5ae9c61c767794ff7b4c305a3b44dd4cb912d7f9e4`  
		Last Modified: Thu, 22 Oct 2020 22:40:43 GMT  
		Size: 263.3 KB (263288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba269da8b2fee4f0cbc5770d9484045809d2705311f7bed9787b386e011a5ff`  
		Last Modified: Tue, 27 Oct 2020 18:32:05 GMT  
		Size: 7.9 MB (7937247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b95388c9dfb7854ecfef02bcd403d91584d51c8c631b7123da9e4ba0937b7f0`  
		Last Modified: Tue, 27 Oct 2020 18:32:03 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9e572f20c03f6da1157ff8f273f89176e4580bd2e838db5fbfda02c4094ff02`  
		Last Modified: Tue, 27 Oct 2020 18:32:03 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine3.12` - linux; s390x

```console
$ docker pull redis@sha256:bbf1f9f38bf7a7de0b66bfd58cc5a3c33173eb4b0158094325989b5098db2d0e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.7 MB (10680833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26ffcc2424bfaf187f9b73252367da2d9a4c4e709aa104a5ca6038525fd1ab80`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Fri, 11 Dec 2020 02:09:52 GMT
ADD file:c9395a36a4e03768aabd282eb1f31705cc00181d3147222d9c940eaa5a8fd511 in / 
# Fri, 11 Dec 2020 02:09:53 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 13:58:32 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Fri, 11 Dec 2020 13:58:35 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Fri, 11 Dec 2020 13:58:36 GMT
ENV REDIS_VERSION=6.0.9
# Fri, 11 Dec 2020 13:58:37 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.9.tar.gz
# Fri, 11 Dec 2020 13:58:37 GMT
ENV REDIS_DOWNLOAD_SHA=dc2bdcf81c620e9f09cfd12e85d3bc631c897b2db7a55218fd8a65eaa37f86dd
# Fri, 11 Dec 2020 13:59:58 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 11 Dec 2020 14:00:01 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 11 Dec 2020 14:00:02 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 14:00:03 GMT
WORKDIR /data
# Fri, 11 Dec 2020 14:00:03 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 11 Dec 2020 14:00:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 14:00:04 GMT
EXPOSE 6379
# Fri, 11 Dec 2020 14:00:05 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:7c2470fe3d16cb70fca0826168095a96838b1322a8cd1502b28284ee8561b491`  
		Last Modified: Fri, 11 Dec 2020 02:10:27 GMT  
		Size: 2.6 MB (2565988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f9fd6145aff29902d4fd018025ad260fe864cbe9f06627b6964ba58e33a2aa7`  
		Last Modified: Fri, 11 Dec 2020 14:04:21 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7732b2116381efd347a216d9f6b13848bbe0ece877b2e04b99db18bb895ef06b`  
		Last Modified: Fri, 11 Dec 2020 14:04:21 GMT  
		Size: 386.4 KB (386378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93837edc854160e5d352064021ef0643dc8853c08ef6a7db54c7d26826f4d159`  
		Last Modified: Fri, 11 Dec 2020 14:04:22 GMT  
		Size: 7.7 MB (7726663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e10d717a8b160df9b2308b85e3b790ee5928f5f5ca285f3f13604550f182d5`  
		Last Modified: Fri, 11 Dec 2020 14:04:21 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a38ca9da3526b4b2c13acede2462a69c5e8139a5324a5e340a8cb9469e6998b7`  
		Last Modified: Fri, 11 Dec 2020 14:04:21 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
