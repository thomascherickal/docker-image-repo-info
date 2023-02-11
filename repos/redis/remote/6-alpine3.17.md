## `redis:6-alpine3.17`

```console
$ docker pull redis@sha256:ab80f389d36d2199dd569f521d392154887378beab0512cacdd813b0e081b31e
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

### `redis:6-alpine3.17` - linux; amd64

```console
$ docker pull redis@sha256:6536c76c861b30f2f64b38c391330813ef187cef5f773dc58b5646230cc0afc5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.2 MB (11244891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb7aa3675db47d71cba6b8d9848de9a84d84bc62d310c217778e66c06a992c7a`
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
# Tue, 17 Jan 2023 21:15:49 GMT
ENV REDIS_VERSION=6.2.10
# Tue, 17 Jan 2023 21:15:49 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.10.tar.gz
# Tue, 17 Jan 2023 21:15:49 GMT
ENV REDIS_DOWNLOAD_SHA=22684f66d272379b91e3e53693918b535e2a6e54b9d14e1cad171658e0eefeca
# Tue, 17 Jan 2023 21:16:25 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Tue, 17 Jan 2023 21:16:26 GMT
RUN mkdir /data && chown redis:redis /data
# Tue, 17 Jan 2023 21:16:26 GMT
VOLUME [/data]
# Tue, 17 Jan 2023 21:16:26 GMT
WORKDIR /data
# Tue, 17 Jan 2023 21:16:26 GMT
COPY file:a9e7249f657e2eec627bb4be492ad18aae3e5e1f0e47d22644eaf1ef2138c0ce in /usr/local/bin/ 
# Tue, 17 Jan 2023 21:16:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 17 Jan 2023 21:16:26 GMT
EXPOSE 6379
# Tue, 17 Jan 2023 21:16:26 GMT
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
	-	`sha256:d261588b2353caaa78b77a6006bf919f4d273e3afa3c2b472a2643d2e3e13726`  
		Last Modified: Tue, 17 Jan 2023 21:19:40 GMT  
		Size: 7.5 MB (7524609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c77101e06792d1793c29fc07cf2c843ab78a8c7809fabdd55a553c7b455832c`  
		Last Modified: Tue, 17 Jan 2023 21:19:38 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2b5d7bf021d648249da2189f928fc348f992293ac66fbdf306058bb5ccf5f0`  
		Last Modified: Tue, 17 Jan 2023 21:19:38 GMT  
		Size: 575.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine3.17` - linux; arm variant v6

```console
$ docker pull redis@sha256:0b2306d8b1d15e712f3cced6d72f7e45ec3c44c1f102e0782741d186fd7af0a2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.0 MB (11031780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9798e204ea84c3d1c9b843f860d8ebc77349855bd2ca33831a07dc09375ae6af`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:28 GMT
ADD file:d825d9aef59df0df23c0140a490998407ee0a62a051699b5c050aef7cb03f042 in / 
# Fri, 10 Feb 2023 20:49:28 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 06:46:24 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Sat, 11 Feb 2023 06:46:25 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Sat, 11 Feb 2023 06:47:15 GMT
ENV REDIS_VERSION=6.2.10
# Sat, 11 Feb 2023 06:47:15 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.10.tar.gz
# Sat, 11 Feb 2023 06:47:16 GMT
ENV REDIS_DOWNLOAD_SHA=22684f66d272379b91e3e53693918b535e2a6e54b9d14e1cad171658e0eefeca
# Sat, 11 Feb 2023 06:47:55 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Sat, 11 Feb 2023 06:47:56 GMT
RUN mkdir /data && chown redis:redis /data
# Sat, 11 Feb 2023 06:47:56 GMT
VOLUME [/data]
# Sat, 11 Feb 2023 06:47:56 GMT
WORKDIR /data
# Sat, 11 Feb 2023 06:47:56 GMT
COPY file:a9e7249f657e2eec627bb4be492ad18aae3e5e1f0e47d22644eaf1ef2138c0ce in /usr/local/bin/ 
# Sat, 11 Feb 2023 06:47:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 06:47:57 GMT
EXPOSE 6379
# Sat, 11 Feb 2023 06:47:57 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:6a6e4ab63e54442e16400f69d37f662d60cbd67565631eff6bf59b4176e482c3`  
		Last Modified: Fri, 10 Feb 2023 20:50:22 GMT  
		Size: 3.1 MB (3110885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ccb4337f56ba5ece8e733c304874b2145fcc96ee68497e99821553340f52e9b`  
		Last Modified: Sat, 11 Feb 2023 06:49:47 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d89a58f66533b43d2d910954d229cbf1c7605172b9d491850c9a82439e6344d`  
		Last Modified: Sat, 11 Feb 2023 06:49:47 GMT  
		Size: 347.8 KB (347792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38ebf2c168469fafa374ddace8d1d3010888e329cc187026ac7dcf05a4a82a30`  
		Last Modified: Sat, 11 Feb 2023 06:50:21 GMT  
		Size: 7.6 MB (7571182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:306b8da1f739a3d1a8ead099481f38c24cb63d620e06e633181265391e2c2eb9`  
		Last Modified: Sat, 11 Feb 2023 06:50:20 GMT  
		Size: 100.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b0d73dbbef5b409cbf416920072771e17cea94d99ae17037fe48c097977efd`  
		Last Modified: Sat, 11 Feb 2023 06:50:20 GMT  
		Size: 580.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine3.17` - linux; arm variant v7

```console
$ docker pull redis@sha256:875c4509f67fd6b506c6f422e1c2654a0713d68e08af8bfd553ab77925797c79
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.7 MB (10674865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40405e6ae1d8172e76e56a69122db5a4e6a38ae21907e78131cc014f2afe5f9c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:31 GMT
ADD file:143b601fcc6b5d7d95d3e5ccad3fec7081191a47e28d4f9294a7fb2499cab1af in / 
# Fri, 10 Feb 2023 21:51:31 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 06:00:15 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Sat, 11 Feb 2023 06:00:17 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Sat, 11 Feb 2023 06:01:12 GMT
ENV REDIS_VERSION=6.2.10
# Sat, 11 Feb 2023 06:01:12 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.10.tar.gz
# Sat, 11 Feb 2023 06:01:12 GMT
ENV REDIS_DOWNLOAD_SHA=22684f66d272379b91e3e53693918b535e2a6e54b9d14e1cad171658e0eefeca
# Sat, 11 Feb 2023 06:01:49 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Sat, 11 Feb 2023 06:01:50 GMT
RUN mkdir /data && chown redis:redis /data
# Sat, 11 Feb 2023 06:01:50 GMT
VOLUME [/data]
# Sat, 11 Feb 2023 06:01:50 GMT
WORKDIR /data
# Sat, 11 Feb 2023 06:01:50 GMT
COPY file:a9e7249f657e2eec627bb4be492ad18aae3e5e1f0e47d22644eaf1ef2138c0ce in /usr/local/bin/ 
# Sat, 11 Feb 2023 06:01:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 06:01:51 GMT
EXPOSE 6379
# Sat, 11 Feb 2023 06:01:51 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:6fb81ff47bd6d7db0ed86c9b951ad6417ec73ab60af6d22daa604076a902629c`  
		Last Modified: Fri, 10 Feb 2023 21:52:33 GMT  
		Size: 2.9 MB (2868494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46188b9a7e8840a4033301af52ee767ea7e81ba8d1c58eb83b12a52763c06dd6`  
		Last Modified: Sat, 11 Feb 2023 06:04:21 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04df0708a961a8c68657fcc3638726aae0f3fab7b2fe2eeadfe2c2717bb96871`  
		Last Modified: Sat, 11 Feb 2023 06:04:21 GMT  
		Size: 347.6 KB (347609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f6603d9c9c9dae43a4a10efc23ec706d002acf420c86b1c61fda0e70dde1d6`  
		Last Modified: Sat, 11 Feb 2023 06:04:59 GMT  
		Size: 7.5 MB (7456844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4462856c95ed8b283ff85ecea173db49165ac605fc5d18f9bb8be618eb343c0`  
		Last Modified: Sat, 11 Feb 2023 06:04:57 GMT  
		Size: 100.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa650132b2027e26424efcedc7f82d3bd958145a728588039558765ba8ebd90`  
		Last Modified: Sat, 11 Feb 2023 06:04:57 GMT  
		Size: 576.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine3.17` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:0f6e66e179fcde71149229191dd4c1b3e4a747c133cf2657334f758e0cbf41ab
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.2 MB (11205121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7be3d544e807883671dcc6c0f406141f68de5c61d25aba516248903a4c91ef7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 05:18:20 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Sat, 11 Feb 2023 05:18:22 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Sat, 11 Feb 2023 05:19:02 GMT
ENV REDIS_VERSION=6.2.10
# Sat, 11 Feb 2023 05:19:02 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.10.tar.gz
# Sat, 11 Feb 2023 05:19:02 GMT
ENV REDIS_DOWNLOAD_SHA=22684f66d272379b91e3e53693918b535e2a6e54b9d14e1cad171658e0eefeca
# Sat, 11 Feb 2023 05:19:30 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Sat, 11 Feb 2023 05:19:31 GMT
RUN mkdir /data && chown redis:redis /data
# Sat, 11 Feb 2023 05:19:31 GMT
VOLUME [/data]
# Sat, 11 Feb 2023 05:19:31 GMT
WORKDIR /data
# Sat, 11 Feb 2023 05:19:31 GMT
COPY file:a9e7249f657e2eec627bb4be492ad18aae3e5e1f0e47d22644eaf1ef2138c0ce in /usr/local/bin/ 
# Sat, 11 Feb 2023 05:19:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 05:19:31 GMT
EXPOSE 6379
# Sat, 11 Feb 2023 05:19:31 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5015c79ed515bf1c31986bf0c02f0058deb7f938811749567bfb8d1263a5e8d2`  
		Last Modified: Sat, 11 Feb 2023 05:20:47 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca28624189f688cb7e78c078bfbc4a0ebf1688dddf9fcf0a2ac7754818decf6`  
		Last Modified: Sat, 11 Feb 2023 05:20:47 GMT  
		Size: 347.9 KB (347907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04081bc5daa9de244d19dc91315518046e2f3591ea96c3e67a8e065de972ee30`  
		Last Modified: Sat, 11 Feb 2023 05:21:13 GMT  
		Size: 7.6 MB (7593277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab6c10025118f45e558b2e96f54886927712b3d58d774ce0ba21227fbec3d379`  
		Last Modified: Sat, 11 Feb 2023 05:21:12 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36bcb5f16c4b8f8e4e8c2f30fb0bf82b81af6c87f22beb0049e5f2b4d08c7c5d`  
		Last Modified: Sat, 11 Feb 2023 05:21:12 GMT  
		Size: 577.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine3.17` - linux; 386

```console
$ docker pull redis@sha256:c85b533bfde000d327d73c57e0dbb61fef5505843b107ae8a74abd286d8f8b07
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.0 MB (11016808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:770948d51920bb0b84fafef64e130839b01b9dbbb3be3293437a93fbf7fc551e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:23 GMT
ADD file:125f3514520a5cd29df2830a409aa026a2bc06a77a7a5d150133436404b33d41 in / 
# Fri, 10 Feb 2023 21:24:24 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 02:42:13 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Sat, 11 Feb 2023 02:42:15 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Sat, 11 Feb 2023 02:43:17 GMT
ENV REDIS_VERSION=6.2.10
# Sat, 11 Feb 2023 02:43:18 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.10.tar.gz
# Sat, 11 Feb 2023 02:43:19 GMT
ENV REDIS_DOWNLOAD_SHA=22684f66d272379b91e3e53693918b535e2a6e54b9d14e1cad171658e0eefeca
# Sat, 11 Feb 2023 02:43:56 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Sat, 11 Feb 2023 02:43:57 GMT
RUN mkdir /data && chown redis:redis /data
# Sat, 11 Feb 2023 02:43:58 GMT
VOLUME [/data]
# Sat, 11 Feb 2023 02:43:59 GMT
WORKDIR /data
# Sat, 11 Feb 2023 02:44:01 GMT
COPY file:a9e7249f657e2eec627bb4be492ad18aae3e5e1f0e47d22644eaf1ef2138c0ce in /usr/local/bin/ 
# Sat, 11 Feb 2023 02:44:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 02:44:02 GMT
EXPOSE 6379
# Sat, 11 Feb 2023 02:44:03 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:b3e346c15c2377ec0e75cc9efa98baecd58b0e9bb92f0ec07eeda0bcc7e67fc7`  
		Last Modified: Fri, 10 Feb 2023 21:25:13 GMT  
		Size: 3.4 MB (3412353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed33790235ed12bfc39c6015e39ac603eef3c97869474228fd55cd8884d39408`  
		Last Modified: Sat, 11 Feb 2023 02:46:17 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55cdd52ff76f5b537420062fd9a7c0315832fd0ef807068e828af1f6d63ed35d`  
		Last Modified: Sat, 11 Feb 2023 02:46:17 GMT  
		Size: 347.6 KB (347596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8f6fc87688141bd0d9760c097d993586caa84677212a5bfcdf8b2646658f1c7`  
		Last Modified: Sat, 11 Feb 2023 02:46:50 GMT  
		Size: 7.3 MB (7254943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e33d5be86c8069c84f9a581c87a1991760f3a9c643abea4833d2c0c7dc91bac`  
		Last Modified: Sat, 11 Feb 2023 02:46:49 GMT  
		Size: 99.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7695b445733ce5c67ce05c189bfcaf7f5d9807a71f9fd611aee7504b5cd220`  
		Last Modified: Sat, 11 Feb 2023 02:46:49 GMT  
		Size: 577.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine3.17` - linux; ppc64le

```console
$ docker pull redis@sha256:90e50411b998b7b927703c6fb020fcde7764e145a578500de859984cd1728b44
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.9 MB (11875435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:499a7f6bd584a6b7ff957da9cfab610a59e4752d2523c1d50750aa96021199d4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:36 GMT
ADD file:ec037a0d4b462d12963ac20d9ec49bb73b4bcaf84d4bc7b364ebf93667e585b0 in / 
# Fri, 10 Feb 2023 21:20:36 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 00:35:51 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Sat, 11 Feb 2023 00:35:56 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Sat, 11 Feb 2023 00:37:20 GMT
ENV REDIS_VERSION=6.2.10
# Sat, 11 Feb 2023 00:37:20 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.10.tar.gz
# Sat, 11 Feb 2023 00:37:21 GMT
ENV REDIS_DOWNLOAD_SHA=22684f66d272379b91e3e53693918b535e2a6e54b9d14e1cad171658e0eefeca
# Sat, 11 Feb 2023 00:38:11 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Sat, 11 Feb 2023 00:38:13 GMT
RUN mkdir /data && chown redis:redis /data
# Sat, 11 Feb 2023 00:38:14 GMT
VOLUME [/data]
# Sat, 11 Feb 2023 00:38:14 GMT
WORKDIR /data
# Sat, 11 Feb 2023 00:38:15 GMT
COPY file:a9e7249f657e2eec627bb4be492ad18aae3e5e1f0e47d22644eaf1ef2138c0ce in /usr/local/bin/ 
# Sat, 11 Feb 2023 00:38:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 00:38:16 GMT
EXPOSE 6379
# Sat, 11 Feb 2023 00:38:16 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:aa3c56f9c6f127b6c8f628c95db165741ca400d19bdaef2752d80f093e47451e`  
		Last Modified: Fri, 10 Feb 2023 21:21:37 GMT  
		Size: 3.4 MB (3390750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b984eda205048e12763406d5bba006c9cdd29c0a96716b8eb19b6341ea87a136`  
		Last Modified: Sat, 11 Feb 2023 00:40:55 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1596dbb042b71d9d2f99fa35647d78556855f99b031224641dcc4e3921c6ab46`  
		Last Modified: Sat, 11 Feb 2023 00:40:56 GMT  
		Size: 347.9 KB (347920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b529fc18f5c6c95a140822b35af3b2119e27db536fea17b8740a700e1b175ae3`  
		Last Modified: Sat, 11 Feb 2023 00:41:36 GMT  
		Size: 8.1 MB (8134781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fe54e7b0deaff9e18679e58a69e2a45b1c55bfe8d63188a43c7f7cc9c7d0099`  
		Last Modified: Sat, 11 Feb 2023 00:41:33 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07484f488db67157cfc067625d6251972127a18d67f137222e9b10d7b2128b42`  
		Last Modified: Sat, 11 Feb 2023 00:41:34 GMT  
		Size: 577.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine3.17` - linux; s390x

```console
$ docker pull redis@sha256:a4dba2df2f3cab29ab39b738d33de150a10abd4bbbbc8204d2ee42a362803333
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.3 MB (11346684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:882600f167a690b2f8aa1315270c7d67005e212e464ba73582067afd6419fc7e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:25 GMT
ADD file:03b2fb4d732a294329449ff55c5d84f7d2735e6510985718979469994f3a607b in / 
# Fri, 10 Feb 2023 21:41:26 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 05:14:39 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Sat, 11 Feb 2023 05:14:40 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Sat, 11 Feb 2023 05:15:41 GMT
ENV REDIS_VERSION=6.2.10
# Sat, 11 Feb 2023 05:15:41 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.10.tar.gz
# Sat, 11 Feb 2023 05:15:41 GMT
ENV REDIS_DOWNLOAD_SHA=22684f66d272379b91e3e53693918b535e2a6e54b9d14e1cad171658e0eefeca
# Sat, 11 Feb 2023 05:16:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Sat, 11 Feb 2023 05:16:16 GMT
RUN mkdir /data && chown redis:redis /data
# Sat, 11 Feb 2023 05:16:16 GMT
VOLUME [/data]
# Sat, 11 Feb 2023 05:16:16 GMT
WORKDIR /data
# Sat, 11 Feb 2023 05:16:17 GMT
COPY file:a9e7249f657e2eec627bb4be492ad18aae3e5e1f0e47d22644eaf1ef2138c0ce in /usr/local/bin/ 
# Sat, 11 Feb 2023 05:16:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 05:16:17 GMT
EXPOSE 6379
# Sat, 11 Feb 2023 05:16:17 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:24c4f8de3549a39c64b0edc2cfa68769b373f35138d0f13725100160bb32d4e2`  
		Last Modified: Fri, 10 Feb 2023 21:42:16 GMT  
		Size: 3.2 MB (3175116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:498875fea887faca6923f24eb01071d9726f31e2190602d0d5f4a95460615a66`  
		Last Modified: Sat, 11 Feb 2023 05:18:35 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:701202efffcf5330e98381a4555776e1d78fb6ef4cd5eaa611ea7870d1554420`  
		Last Modified: Sat, 11 Feb 2023 05:18:35 GMT  
		Size: 347.6 KB (347644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a1857fafb41a1fd2725e8b58a2281e396c31c21050a2ba2432cbebbc14daaf`  
		Last Modified: Sat, 11 Feb 2023 05:18:59 GMT  
		Size: 7.8 MB (7821942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f070ef2113bf4cb9c1cf807092e2648389e72f6e9a36318d043c0313f9e07c1`  
		Last Modified: Sat, 11 Feb 2023 05:18:58 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c904f0b9243390f9e21d67042cabe697fe460fa5f25b5c2e6eef5d38c9c8dc6`  
		Last Modified: Sat, 11 Feb 2023 05:18:58 GMT  
		Size: 579.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
