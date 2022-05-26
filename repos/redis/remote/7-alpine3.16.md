## `redis:7-alpine3.16`

```console
$ docker pull redis@sha256:558d0845026fe0bf091a00c0ad647ffacf9df385d780d433ca70661f7276f834
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

### `redis:7-alpine3.16` - linux; amd64

```console
$ docker pull redis@sha256:8bd5e4aae7ec87e5833b38353fc11eb43d1a88a7aad8aef0f3efb673984e1885
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.8 MB (11832470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3ea2db12504cefdd7ce39289971cee44301906441d49ba9026d3be60945a059`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 22:04:39 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Wed, 25 May 2022 22:04:40 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Wed, 25 May 2022 22:04:40 GMT
ENV REDIS_VERSION=7.0.0
# Wed, 25 May 2022 22:04:40 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.0.0.tar.gz
# Wed, 25 May 2022 22:04:40 GMT
ENV REDIS_DOWNLOAD_SHA=284d8bd1fd85d6a55a05ee4e7c31c31977ad56cbf344ed83790beeb148baa720
# Wed, 25 May 2022 22:05:41 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Wed, 25 May 2022 22:05:42 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 25 May 2022 22:05:42 GMT
VOLUME [/data]
# Wed, 25 May 2022 22:05:42 GMT
WORKDIR /data
# Wed, 25 May 2022 22:05:42 GMT
COPY file:a9e7249f657e2eec627bb4be492ad18aae3e5e1f0e47d22644eaf1ef2138c0ce in /usr/local/bin/ 
# Wed, 25 May 2022 22:05:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 25 May 2022 22:05:42 GMT
EXPOSE 6379
# Wed, 25 May 2022 22:05:42 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90389148883be3c6500b090644113cf690b528e6f057515568a36bfd0b0d87c`  
		Last Modified: Wed, 25 May 2022 22:09:41 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c08b6ea4d56366e32f458bcaeb9933840882cfa4ac9073d0d42649e34d1a16`  
		Last Modified: Wed, 25 May 2022 22:09:41 GMT  
		Size: 406.2 KB (406166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b344356131fc0a2f86f1838624745711fa46073d07430b0876b636312d48e0`  
		Last Modified: Wed, 25 May 2022 22:09:42 GMT  
		Size: 8.6 MB (8625432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dbe7dca7b464b3007aab230a3e043d41f91d377b95091983a07a8a025fbafbd`  
		Last Modified: Wed, 25 May 2022 22:09:40 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dc883bc6e9416a43c5d8931046e71932641e94da6531a0165581b1a25407505`  
		Last Modified: Wed, 25 May 2022 22:09:41 GMT  
		Size: 579.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:7-alpine3.16` - linux; arm variant v6

```console
$ docker pull redis@sha256:29b72312f688d35175c34b2ebdecac56dc9c366c249f8b9fdfbade4e48ad39a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.8 MB (11759967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d062c61a27722606f2f087b0b493be9deadf4a48434554e328e9349bbbe52c07`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Mon, 23 May 2022 19:49:32 GMT
ADD file:f7cee617575b5e5a7672d298a519bb8d8b5098efb90aa2a5d7b0510003457d52 in / 
# Mon, 23 May 2022 19:49:33 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 23:49:59 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Wed, 25 May 2022 23:50:02 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Wed, 25 May 2022 23:50:03 GMT
ENV REDIS_VERSION=7.0.0
# Wed, 25 May 2022 23:50:03 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.0.0.tar.gz
# Wed, 25 May 2022 23:50:04 GMT
ENV REDIS_DOWNLOAD_SHA=284d8bd1fd85d6a55a05ee4e7c31c31977ad56cbf344ed83790beeb148baa720
# Wed, 25 May 2022 23:51:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Wed, 25 May 2022 23:51:30 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 25 May 2022 23:51:30 GMT
VOLUME [/data]
# Wed, 25 May 2022 23:51:31 GMT
WORKDIR /data
# Wed, 25 May 2022 23:51:31 GMT
COPY file:a9e7249f657e2eec627bb4be492ad18aae3e5e1f0e47d22644eaf1ef2138c0ce in /usr/local/bin/ 
# Wed, 25 May 2022 23:51:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 25 May 2022 23:51:32 GMT
EXPOSE 6379
# Wed, 25 May 2022 23:51:32 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:79a25ccaf940855872635c06e7614d9b27dd38ffb5a8adfdb9274dfdc0ea0d87`  
		Last Modified: Mon, 23 May 2022 19:08:47 GMT  
		Size: 2.6 MB (2606142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fa0ad1182fac92be0203541ebed1ed824b228bb8931f84fd331fc2f5e69e26b`  
		Last Modified: Wed, 25 May 2022 23:58:12 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af04e825a985a118c21a144eaa95bdea91b0a9087403f5edb9bc52c7f1238b9a`  
		Last Modified: Wed, 25 May 2022 23:58:13 GMT  
		Size: 410.4 KB (410362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e785471f6ab39dc5a754c6b6650fe840d0ccb4b0639b6532e09075a17ae07972`  
		Last Modified: Wed, 25 May 2022 23:58:17 GMT  
		Size: 8.7 MB (8741484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41edfba2ba32032ea73edbb684392a07aa8058bc20360af3a12f402c16613d5f`  
		Last Modified: Wed, 25 May 2022 23:58:12 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e372dd9950173e147e7199ca3d16f385f8ce629034978262118cdd4a3afbec4`  
		Last Modified: Wed, 25 May 2022 23:58:12 GMT  
		Size: 579.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:7-alpine3.16` - linux; arm variant v7

```console
$ docker pull redis@sha256:40dd2859e30681ce9cf3c847be2add984f02074cc48e5556c4278f50d1c04001
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.4 MB (11433095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0c71e6db353b56887fcc9907d7d9ac2e8ea9b8857df94f82de0c48820191103`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Mon, 23 May 2022 18:57:46 GMT
ADD file:72698cc08524b911ebaacf992490707e5a951ddd2fe6edb3fb598e9dc7155049 in / 
# Mon, 23 May 2022 18:57:47 GMT
CMD ["/bin/sh"]
# Thu, 26 May 2022 01:06:31 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Thu, 26 May 2022 01:06:35 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Thu, 26 May 2022 01:06:35 GMT
ENV REDIS_VERSION=7.0.0
# Thu, 26 May 2022 01:06:35 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.0.0.tar.gz
# Thu, 26 May 2022 01:06:36 GMT
ENV REDIS_DOWNLOAD_SHA=284d8bd1fd85d6a55a05ee4e7c31c31977ad56cbf344ed83790beeb148baa720
# Thu, 26 May 2022 01:07:58 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Thu, 26 May 2022 01:07:59 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 26 May 2022 01:08:00 GMT
VOLUME [/data]
# Thu, 26 May 2022 01:08:00 GMT
WORKDIR /data
# Thu, 26 May 2022 01:08:00 GMT
COPY file:a9e7249f657e2eec627bb4be492ad18aae3e5e1f0e47d22644eaf1ef2138c0ce in /usr/local/bin/ 
# Thu, 26 May 2022 01:08:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 May 2022 01:08:01 GMT
EXPOSE 6379
# Thu, 26 May 2022 01:08:02 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:6366ba92f08e2418e90171f1e34bd86ecd50fdc95953b3f33b8943c143518eca`  
		Last Modified: Mon, 23 May 2022 18:59:17 GMT  
		Size: 2.4 MB (2411648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c95dd4ea78393dcf27dfa1aa64dea763e0fc045eaa38376f2a799ced22b8fc3`  
		Last Modified: Thu, 26 May 2022 01:17:43 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cf2b46cefeffc1fbcaae2f439cd8a4063ddd994bf5e57cd4b4e34cc9307a99f`  
		Last Modified: Thu, 26 May 2022 01:17:44 GMT  
		Size: 404.1 KB (404098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2129658c7943bd6a8d3f209353c69ad5f991106bdf6cdd8c6a3b0171360e0a28`  
		Last Modified: Thu, 26 May 2022 01:17:48 GMT  
		Size: 8.6 MB (8615364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8f71d34c329c0abfd29f09284aced06e0b9d8bde15a2761db372d0680fb452`  
		Last Modified: Thu, 26 May 2022 01:17:43 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01f06dcda8c3e69e6fa12776f3c599306fd5e496c46285ef2dd8e53d648f2d40`  
		Last Modified: Thu, 26 May 2022 01:17:43 GMT  
		Size: 579.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:7-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:ef35b4fb296565b594a37dc55a4ec1d5335d977d73d52664122810de2b86bbed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.9 MB (11864667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d368b6a2bc5e569e10b12e91e6f7cc02b0cc260f51de4cce1dc22a9bae8205c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 23:41:51 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Wed, 25 May 2022 23:41:53 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Wed, 25 May 2022 23:41:54 GMT
ENV REDIS_VERSION=7.0.0
# Wed, 25 May 2022 23:41:55 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.0.0.tar.gz
# Wed, 25 May 2022 23:41:56 GMT
ENV REDIS_DOWNLOAD_SHA=284d8bd1fd85d6a55a05ee4e7c31c31977ad56cbf344ed83790beeb148baa720
# Wed, 25 May 2022 23:43:32 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Wed, 25 May 2022 23:43:33 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 25 May 2022 23:43:34 GMT
VOLUME [/data]
# Wed, 25 May 2022 23:43:35 GMT
WORKDIR /data
# Wed, 25 May 2022 23:43:37 GMT
COPY file:a9e7249f657e2eec627bb4be492ad18aae3e5e1f0e47d22644eaf1ef2138c0ce in /usr/local/bin/ 
# Wed, 25 May 2022 23:43:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 25 May 2022 23:43:38 GMT
EXPOSE 6379
# Wed, 25 May 2022 23:43:39 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9cb7a578000254e0dc90b6df14e94881632ece9dd85884b400a508492be5d9b`  
		Last Modified: Wed, 25 May 2022 23:51:01 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9052ca636db21d422f2e940c13fa5d300d6e2cf7f86f0f73ea58fab01feedb63`  
		Last Modified: Wed, 25 May 2022 23:51:01 GMT  
		Size: 407.2 KB (407213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aefe99c0fcabff07e81b58c833b741b11c38b4074c0b422eb52efaa95b837550`  
		Last Modified: Wed, 25 May 2022 23:51:03 GMT  
		Size: 8.8 MB (8761071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1df16d43d38c3b549ea3ca0a893a827be9e84ac512ff0ff1f94a79d0e794323`  
		Last Modified: Wed, 25 May 2022 23:51:01 GMT  
		Size: 99.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c80a0547a5ff0a69df3b32081c99c26669a720080097ea9a7293afb86f700dc`  
		Last Modified: Wed, 25 May 2022 23:51:01 GMT  
		Size: 580.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:7-alpine3.16` - linux; 386

```console
$ docker pull redis@sha256:28cc1ff12329de238e2521d2ebcfa32b89a47fd2fa34f6b0effefda414cf1ba2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.5 MB (11479754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:366c7ea7a63fe3817bcfe8365aed63a5554902df5167a98665b9d1a448a75659`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Mon, 23 May 2022 19:38:20 GMT
ADD file:1750ccfabfe93636015070d51a6e824cbd738056223421c69d8aaabc38041b18 in / 
# Mon, 23 May 2022 19:38:20 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 22:12:12 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Wed, 25 May 2022 22:12:14 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Wed, 25 May 2022 22:12:14 GMT
ENV REDIS_VERSION=7.0.0
# Wed, 25 May 2022 22:12:15 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.0.0.tar.gz
# Wed, 25 May 2022 22:12:16 GMT
ENV REDIS_DOWNLOAD_SHA=284d8bd1fd85d6a55a05ee4e7c31c31977ad56cbf344ed83790beeb148baa720
# Wed, 25 May 2022 22:13:17 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Wed, 25 May 2022 22:13:17 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 25 May 2022 22:13:18 GMT
VOLUME [/data]
# Wed, 25 May 2022 22:13:19 GMT
WORKDIR /data
# Wed, 25 May 2022 22:13:21 GMT
COPY file:a9e7249f657e2eec627bb4be492ad18aae3e5e1f0e47d22644eaf1ef2138c0ce in /usr/local/bin/ 
# Wed, 25 May 2022 22:13:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 25 May 2022 22:13:22 GMT
EXPOSE 6379
# Wed, 25 May 2022 22:13:23 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:bb638a3869eed698f88775c7a48f36f8e22e7c6bbaa98fa1d5678966b619b859`  
		Last Modified: Mon, 23 May 2022 19:09:25 GMT  
		Size: 2.8 MB (2801887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5606fb113d21aa033df3c08bd7a75a5a81b2bdcd6f07088d5361b11a25a30f6`  
		Last Modified: Wed, 25 May 2022 22:19:30 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01878a6bc72011373f1316d7c82f835278bc12d26b93301da233a8499ea2f239`  
		Last Modified: Wed, 25 May 2022 22:19:30 GMT  
		Size: 413.6 KB (413593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8f4198d30aa5e00d12eab1e2a1ba961959f2402f1a74f20d9cd3a81194ed5cd`  
		Last Modified: Wed, 25 May 2022 22:19:31 GMT  
		Size: 8.3 MB (8262355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:530b37b013ff8d73efd73a958b2aaf82d891d087a078ffcbb29759d76ff86dac`  
		Last Modified: Wed, 25 May 2022 22:19:30 GMT  
		Size: 100.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70a12c7410c55064c57c155f66e42e713bd627d3e9e62e92a637fc70eff8156e`  
		Last Modified: Wed, 25 May 2022 22:19:29 GMT  
		Size: 580.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:7-alpine3.16` - linux; ppc64le

```console
$ docker pull redis@sha256:0b752c29c21f26ccbb913ffe7f7f93d8b7fb482bed3f76852a733ac2e10fb575
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **12.4 MB (12443519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c682a113952a2868e3b97f1b1f39fdbbeff72b39d25d53d423a5a3a45aff95ab`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Mon, 23 May 2022 19:16:51 GMT
ADD file:6a5450c8a7cee3ceda59e7cb350c54df4139b0f7b7cf49c8b31bb9c01646c3cd in / 
# Mon, 23 May 2022 19:16:53 GMT
CMD ["/bin/sh"]
# Thu, 26 May 2022 00:20:18 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Thu, 26 May 2022 00:20:34 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Thu, 26 May 2022 00:20:42 GMT
ENV REDIS_VERSION=7.0.0
# Thu, 26 May 2022 00:20:49 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.0.0.tar.gz
# Thu, 26 May 2022 00:20:54 GMT
ENV REDIS_DOWNLOAD_SHA=284d8bd1fd85d6a55a05ee4e7c31c31977ad56cbf344ed83790beeb148baa720
# Thu, 26 May 2022 00:22:23 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Thu, 26 May 2022 00:22:35 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 26 May 2022 00:22:40 GMT
VOLUME [/data]
# Thu, 26 May 2022 00:22:45 GMT
WORKDIR /data
# Thu, 26 May 2022 00:22:48 GMT
COPY file:a9e7249f657e2eec627bb4be492ad18aae3e5e1f0e47d22644eaf1ef2138c0ce in /usr/local/bin/ 
# Thu, 26 May 2022 00:22:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 May 2022 00:23:01 GMT
EXPOSE 6379
# Thu, 26 May 2022 00:23:08 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:d3deabf2a506ef6f5fa7c2a68bf27047574cef9908b30a97ff2d01ae539b089a`  
		Last Modified: Mon, 23 May 2022 19:09:13 GMT  
		Size: 2.8 MB (2789745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:829eb500d899e72e6b49a33db765f361e3f6b6e9f8f7022cbd62988a36011b69`  
		Last Modified: Thu, 26 May 2022 00:35:11 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ac73a539d726ff67c63af0126efb487ef797bdc2b4f487a546b9babfe784f6`  
		Last Modified: Thu, 26 May 2022 00:35:11 GMT  
		Size: 413.6 KB (413623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16aa4e526eead8d64331e92a011435415a1e0feada830e80abe85d4e533ac892`  
		Last Modified: Thu, 26 May 2022 00:35:13 GMT  
		Size: 9.2 MB (9238154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d9961ea48fbbedefc53a0c822ddf4fd50b17fb297b7eb3e605733d3c9e4d1e`  
		Last Modified: Thu, 26 May 2022 00:35:11 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a08f86f164470408704b84af98f92412e8428218f757c632dbdea15daabe4f97`  
		Last Modified: Thu, 26 May 2022 00:35:11 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:7-alpine3.16` - linux; s390x

```console
$ docker pull redis@sha256:8e845b2ad2eec813a04896d4e2e5588827e49d5394579c95f3651f0cb11c1cb0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.9 MB (11882532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6176fb10199ce7ddbf18f9ddbf372f12cbf7935de592fde07c0981d77097d9a3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Mon, 23 May 2022 19:41:59 GMT
ADD file:e1852d8ef555a0d3ef6d0b74a898720c82bb9f491430b06a0dd0499497ce118e in / 
# Mon, 23 May 2022 19:42:10 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 23:23:38 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Wed, 25 May 2022 23:23:39 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Wed, 25 May 2022 23:23:40 GMT
ENV REDIS_VERSION=7.0.0
# Wed, 25 May 2022 23:23:40 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.0.0.tar.gz
# Wed, 25 May 2022 23:23:40 GMT
ENV REDIS_DOWNLOAD_SHA=284d8bd1fd85d6a55a05ee4e7c31c31977ad56cbf344ed83790beeb148baa720
# Wed, 25 May 2022 23:24:36 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Wed, 25 May 2022 23:24:37 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 25 May 2022 23:24:38 GMT
VOLUME [/data]
# Wed, 25 May 2022 23:24:38 GMT
WORKDIR /data
# Wed, 25 May 2022 23:24:38 GMT
COPY file:a9e7249f657e2eec627bb4be492ad18aae3e5e1f0e47d22644eaf1ef2138c0ce in /usr/local/bin/ 
# Wed, 25 May 2022 23:24:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 25 May 2022 23:24:39 GMT
EXPOSE 6379
# Wed, 25 May 2022 23:24:39 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:af1ac1a73384e058591d04d19bc05a06781cc32d52d4593b468d6cb95eda9858`  
		Last Modified: Mon, 23 May 2022 19:43:36 GMT  
		Size: 2.6 MB (2580494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:152aae9522a42ef726a16c3f39fadb0aa74325b74a43efad7ee7605b4ff68a7b`  
		Last Modified: Wed, 25 May 2022 23:30:19 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2e02fe158318d41fa93857ee7ac8c3f7fbe37d1d58f47858c6cb9839fba2210`  
		Last Modified: Wed, 25 May 2022 23:30:19 GMT  
		Size: 410.9 KB (410950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b74c6b75d858557c2a389e2f788e7b571a745b303c588935307ba1ecb113aee2`  
		Last Modified: Wed, 25 May 2022 23:30:20 GMT  
		Size: 8.9 MB (8889111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743b1029f72357bee3605d1053f50909cd3c1fd70cf0cf3a486f38010a7f125d`  
		Last Modified: Wed, 25 May 2022 23:30:20 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca577a120e9d416542b86c654fd19a8dc95dbe4d0f4c9bd73160c6653e35e1d4`  
		Last Modified: Wed, 25 May 2022 23:30:19 GMT  
		Size: 578.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
