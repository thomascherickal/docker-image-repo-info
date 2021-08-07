## `redis:6-alpine3.14`

```console
$ docker pull redis@sha256:c8612cb52f56304c895c5e346cc79a9459990074797bea8a549df573b41a4cd3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `redis:6-alpine3.14` - linux; amd64

```console
$ docker pull redis@sha256:324faae103b6af6dd7085748ca8ea99b9e32785a0f3f80f62ce6f2d5185aeaaa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.9 MB (10895186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:814803e951a7ff04c8f7dfd366b4cc6de6859ac159e185f9ecbe9db82c9e9388`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Fri, 06 Aug 2021 17:19:45 GMT
ADD file:34eb5c40aa00028921a224d1764ae1b1f3ef710d191e4dfc7df55e0594aa7217 in / 
# Fri, 06 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 22:07:59 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Fri, 06 Aug 2021 22:08:02 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Fri, 06 Aug 2021 22:08:02 GMT
ENV REDIS_VERSION=6.2.5
# Fri, 06 Aug 2021 22:08:02 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.5.tar.gz
# Fri, 06 Aug 2021 22:08:03 GMT
ENV REDIS_DOWNLOAD_SHA=4b9a75709a1b74b3785e20a6c158cab94cf52298aa381eea947a678a60d551ae
# Fri, 06 Aug 2021 22:10:02 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 06 Aug 2021 22:10:03 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 06 Aug 2021 22:10:04 GMT
VOLUME [/data]
# Fri, 06 Aug 2021 22:10:04 GMT
WORKDIR /data
# Fri, 06 Aug 2021 22:10:04 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 06 Aug 2021 22:10:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 22:10:05 GMT
EXPOSE 6379
# Fri, 06 Aug 2021 22:10:06 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:29291e31a76a7e560b9b7ad3cada56e8c18d50a96cca8a2573e4f4689d7aca77`  
		Last Modified: Thu, 05 Aug 2021 15:56:25 GMT  
		Size: 2.8 MB (2813006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16bbd9479e910eabc5de34a71d51574b0a02cf7a90456d94377af78b3aa6726d`  
		Last Modified: Fri, 06 Aug 2021 22:14:20 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4bb2b90a23b5e3f3871306be4f92344b08c2568b3c4166b61238f576f592cb7`  
		Last Modified: Fri, 06 Aug 2021 22:14:21 GMT  
		Size: 384.5 KB (384463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:011b05d94792ae5064f3c23625eee73c924c5a37c9d9ef8ce0cde6a7059ea611`  
		Last Modified: Fri, 06 Aug 2021 22:14:22 GMT  
		Size: 7.7 MB (7695902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a615fd1f2fd070050e2a5181c0334d55efdd7e2a85adb7c4bd159838125ade4`  
		Last Modified: Fri, 06 Aug 2021 22:14:20 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd76b8efa6e93f9e401fa5e2e138617b6f0e13a2d4e81236131c927bb3ab58c3`  
		Last Modified: Fri, 06 Aug 2021 22:14:20 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine3.14` - linux; arm variant v6

```console
$ docker pull redis@sha256:e839f4d7410934866e6593f9444805e36a1dfa63bc347f091ccb175c36934125
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.6 MB (10592500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:934fb9490a8906fda34b0bfb502f28a62cb83edf95669d240388cc5d5ce750c2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Fri, 06 Aug 2021 17:49:32 GMT
ADD file:7f2c7deda009eabdcbbdccb11e854043d32c498e64e7e1ca02165d7bb4261d39 in / 
# Fri, 06 Aug 2021 17:49:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 23:44:24 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Fri, 06 Aug 2021 23:44:27 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Fri, 06 Aug 2021 23:44:28 GMT
ENV REDIS_VERSION=6.2.5
# Fri, 06 Aug 2021 23:44:28 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.5.tar.gz
# Fri, 06 Aug 2021 23:44:28 GMT
ENV REDIS_DOWNLOAD_SHA=4b9a75709a1b74b3785e20a6c158cab94cf52298aa381eea947a678a60d551ae
# Fri, 06 Aug 2021 23:45:38 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 06 Aug 2021 23:45:40 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 06 Aug 2021 23:45:40 GMT
VOLUME [/data]
# Fri, 06 Aug 2021 23:45:41 GMT
WORKDIR /data
# Fri, 06 Aug 2021 23:45:41 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 06 Aug 2021 23:45:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 23:45:42 GMT
EXPOSE 6379
# Fri, 06 Aug 2021 23:45:43 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:f465bb3e9fcd0c42f936ecc566c6e40353c00f3089b2b2c2ea1663c30f89d3ab`  
		Last Modified: Fri, 06 Aug 2021 17:51:00 GMT  
		Size: 2.6 MB (2626350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea02c10e7c391f7906fcf7ab9b98c53997b8b591aab9fb9baa13ca3d3a756541`  
		Last Modified: Fri, 06 Aug 2021 23:50:16 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45559cdce8ead418b97cd9dac623de212c53a763344dc043e7bf7b3fe5f5d636`  
		Last Modified: Fri, 06 Aug 2021 23:50:17 GMT  
		Size: 388.5 KB (388466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6546d2495c0c6b69b098e5bcc47a13a3a722206a1dee25d57aac986c9ff3670b`  
		Last Modified: Fri, 06 Aug 2021 23:50:21 GMT  
		Size: 7.6 MB (7575866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cef4596ea425517d2244aff609c65cf91add15f09ccc46ac88a9d74bb3dcce23`  
		Last Modified: Fri, 06 Aug 2021 23:50:16 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75733dd86aa3d9d456e216e5f2189b07a37d5c92525b1f87d489ed7d933d5a19`  
		Last Modified: Fri, 06 Aug 2021 23:50:17 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine3.14` - linux; arm variant v7

```console
$ docker pull redis@sha256:350c39df8aaddf9176d96b569bdb5630ab9234d57478ec3ecfd347f83536b7c3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.3 MB (10273038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a58198aa926418ce588e2b62ed464dbd20e886c08055eb023df10516796b15c0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Fri, 06 Aug 2021 17:57:32 GMT
ADD file:3a35ff3ac0d80289d419a4d6d8319610c38e1936d296addafb9aaf506946230f in / 
# Fri, 06 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 23:27:22 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Fri, 06 Aug 2021 23:27:25 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Fri, 06 Aug 2021 23:27:26 GMT
ENV REDIS_VERSION=6.2.5
# Fri, 06 Aug 2021 23:27:26 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.5.tar.gz
# Fri, 06 Aug 2021 23:27:27 GMT
ENV REDIS_DOWNLOAD_SHA=4b9a75709a1b74b3785e20a6c158cab94cf52298aa381eea947a678a60d551ae
# Fri, 06 Aug 2021 23:28:36 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 06 Aug 2021 23:28:37 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 06 Aug 2021 23:28:38 GMT
VOLUME [/data]
# Fri, 06 Aug 2021 23:28:38 GMT
WORKDIR /data
# Fri, 06 Aug 2021 23:28:39 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 06 Aug 2021 23:28:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Aug 2021 23:28:40 GMT
EXPOSE 6379
# Fri, 06 Aug 2021 23:28:40 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:4ee0caa23b369b04827640a4be298bf4ff7bacd030c77e915f5d7fb8f987594a`  
		Last Modified: Fri, 06 Aug 2021 17:58:57 GMT  
		Size: 2.4 MB (2429359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:157f86a12cf9f88c46f2b23f86a5b473982490de10b04db824b29a10e8e0a125`  
		Last Modified: Fri, 06 Aug 2021 23:35:01 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7673623305275567982c76a112a4de4a737203241e26b21d3f48b5610165410f`  
		Last Modified: Fri, 06 Aug 2021 23:35:02 GMT  
		Size: 383.2 KB (383228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c971746929065ae7647a0f92bfbabf10b3f8bd26d45beb3141161909556a6a58`  
		Last Modified: Fri, 06 Aug 2021 23:35:06 GMT  
		Size: 7.5 MB (7458636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9858721b824412f363d7e0527bb1b8e97fa355308daa27263f7a476091672a8d`  
		Last Modified: Fri, 06 Aug 2021 23:35:01 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b926e6c98f2c949d5746718df0391616b5d1c48978c6731f7d8accb255bf87a`  
		Last Modified: Fri, 06 Aug 2021 23:35:01 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:fc856014691d52258a64ab4ef05bf835ce416eb552576264d98309ec92949aba
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.8 MB (10801344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4b2ec2d149ef8ecec1790fed380d1dbff92336e1666489e31adb29a3c9ade01`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Fri, 06 Aug 2021 17:39:26 GMT
ADD file:1a8fd1066485e1261462e689c1a072f010c1d3be904b73ef2b84128fac652951 in / 
# Fri, 06 Aug 2021 17:39:27 GMT
CMD ["/bin/sh"]
# Sat, 07 Aug 2021 00:57:58 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Sat, 07 Aug 2021 00:57:59 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Sat, 07 Aug 2021 00:58:00 GMT
ENV REDIS_VERSION=6.2.5
# Sat, 07 Aug 2021 00:58:00 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.5.tar.gz
# Sat, 07 Aug 2021 00:58:00 GMT
ENV REDIS_DOWNLOAD_SHA=4b9a75709a1b74b3785e20a6c158cab94cf52298aa381eea947a678a60d551ae
# Sat, 07 Aug 2021 00:58:56 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Sat, 07 Aug 2021 00:58:57 GMT
RUN mkdir /data && chown redis:redis /data
# Sat, 07 Aug 2021 00:58:57 GMT
VOLUME [/data]
# Sat, 07 Aug 2021 00:58:57 GMT
WORKDIR /data
# Sat, 07 Aug 2021 00:58:57 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Sat, 07 Aug 2021 00:58:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 07 Aug 2021 00:58:58 GMT
EXPOSE 6379
# Sat, 07 Aug 2021 00:58:58 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:fd3acdcea5682abced546ec19fb6ebee725c5184e5d91614c469c0a79e67f2d0`  
		Last Modified: Fri, 06 Aug 2021 17:40:12 GMT  
		Size: 2.7 MB (2710613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b620df9971e1dcd03b770001b4056c90d73c4664eddb54df7aea8a95e96a6b0`  
		Last Modified: Sat, 07 Aug 2021 01:02:47 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6d728099fba6b7543bfe7e9efd6780bab86d257adb204801290346ff514d6d`  
		Last Modified: Sat, 07 Aug 2021 01:02:47 GMT  
		Size: 386.2 KB (386219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:971159ded50a4f7345cafc80f2148686a6ed3b75261accc6e90e6d09c0baedeb`  
		Last Modified: Sat, 07 Aug 2021 01:02:49 GMT  
		Size: 7.7 MB (7702696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:049846f7b180e81f1355d40f34e10a674a358d6bdc1416843a526828421b3551`  
		Last Modified: Sat, 07 Aug 2021 01:02:47 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa2317e201c9a11508ce91654d1c69e51a60267fd1182d3b49a803071591396`  
		Last Modified: Sat, 07 Aug 2021 01:02:47 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine3.14` - linux; 386

```console
$ docker pull redis@sha256:6edcbc387edd866a080491c015c029b458f49678152dfe364ad50383620c3215
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.6 MB (10557130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e783a072e8ad0e8c3e68c87f419f6df6b2572289c79b0fd4448357e425225d1a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Fri, 06 Aug 2021 17:38:26 GMT
ADD file:bafaec4a54d6cef99b5f3660d074a3d2251e4d4bd09df9ea65f33e9bffb7d88d in / 
# Fri, 06 Aug 2021 17:38:26 GMT
CMD ["/bin/sh"]
# Sat, 07 Aug 2021 02:26:05 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Sat, 07 Aug 2021 02:26:07 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Sat, 07 Aug 2021 02:26:08 GMT
ENV REDIS_VERSION=6.2.5
# Sat, 07 Aug 2021 02:26:08 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.5.tar.gz
# Sat, 07 Aug 2021 02:26:08 GMT
ENV REDIS_DOWNLOAD_SHA=4b9a75709a1b74b3785e20a6c158cab94cf52298aa381eea947a678a60d551ae
# Sat, 07 Aug 2021 02:27:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Sat, 07 Aug 2021 02:27:35 GMT
RUN mkdir /data && chown redis:redis /data
# Sat, 07 Aug 2021 02:27:35 GMT
VOLUME [/data]
# Sat, 07 Aug 2021 02:27:36 GMT
WORKDIR /data
# Sat, 07 Aug 2021 02:27:36 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Sat, 07 Aug 2021 02:27:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 07 Aug 2021 02:27:36 GMT
EXPOSE 6379
# Sat, 07 Aug 2021 02:27:37 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:935703e1179e32e201e4a36d5664d58299dc8e7bcac197b70c295c0a59216db1`  
		Last Modified: Fri, 06 Aug 2021 17:39:15 GMT  
		Size: 2.8 MB (2821910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb7d3d912e0a00c38ab24725f690fb87d01c80af611b515f2b44b7cfd2add60b`  
		Last Modified: Sat, 07 Aug 2021 02:32:17 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80747572cb14554b8336b84ff50d75513afbf7a619826259fe572651239a68b3`  
		Last Modified: Sat, 07 Aug 2021 02:32:18 GMT  
		Size: 390.8 KB (390832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a66cdc655ea4b4bf9bf88f4177baed0a270cfb01144f95aca4bdb70db1da327`  
		Last Modified: Sat, 07 Aug 2021 02:32:19 GMT  
		Size: 7.3 MB (7342570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a7e0e7bcf112da16f97fd724d1d84d247ba66ecda2ace88006122a218b613fe`  
		Last Modified: Sat, 07 Aug 2021 02:32:17 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f66c9d880ed07fd1b6e9e46158e621d905854fe3b3f9203c436fb5d0235e0aec`  
		Last Modified: Sat, 07 Aug 2021 02:32:17 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine3.14` - linux; ppc64le

```console
$ docker pull redis@sha256:97875d43e60dee45e12182688a3ee7172bf7829c85c5fbcc6b4658d63aaaadfe
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.4 MB (11410206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59d30ca0ed277abe9036bb2b1271a2d50a2ed1549e6feb4463165bd50baefb7a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Fri, 06 Aug 2021 18:28:28 GMT
ADD file:40f3b617d7ff269d92f0ffcf8aad561b5f2c0626ef519a7f584f1ba0182b3188 in / 
# Fri, 06 Aug 2021 18:28:35 GMT
CMD ["/bin/sh"]
# Sat, 07 Aug 2021 01:50:18 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Sat, 07 Aug 2021 01:50:31 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Sat, 07 Aug 2021 01:50:36 GMT
ENV REDIS_VERSION=6.2.5
# Sat, 07 Aug 2021 01:50:41 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.5.tar.gz
# Sat, 07 Aug 2021 01:50:45 GMT
ENV REDIS_DOWNLOAD_SHA=4b9a75709a1b74b3785e20a6c158cab94cf52298aa381eea947a678a60d551ae
# Sat, 07 Aug 2021 01:51:54 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Sat, 07 Aug 2021 01:52:03 GMT
RUN mkdir /data && chown redis:redis /data
# Sat, 07 Aug 2021 01:52:05 GMT
VOLUME [/data]
# Sat, 07 Aug 2021 01:52:09 GMT
WORKDIR /data
# Sat, 07 Aug 2021 01:52:11 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Sat, 07 Aug 2021 01:52:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 07 Aug 2021 01:52:22 GMT
EXPOSE 6379
# Sat, 07 Aug 2021 01:52:26 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:0ff902055236f70c4694c806877243e1dd52c513825a2a3ecc7eba8f5202acc8`  
		Last Modified: Fri, 06 Aug 2021 18:29:33 GMT  
		Size: 2.8 MB (2811152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:080f179058a55d84d9a58e9143697539308305bc62d793a4dbf5e9c714fbf97f`  
		Last Modified: Sat, 07 Aug 2021 01:58:11 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d14d309a9f0336abe66a29b88217d74075bf2b6ebc8c1dec75d8a0bdf38f160`  
		Last Modified: Sat, 07 Aug 2021 01:58:11 GMT  
		Size: 391.1 KB (391069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef9ccbcad7f5ac939e478f95824dfbfc8270142b8b91c9ddfc8c7b94a2c6b00`  
		Last Modified: Sat, 07 Aug 2021 01:58:13 GMT  
		Size: 8.2 MB (8206162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f75eb3267c1150ccbebffb2e8e6e68c393bd8dfabbb69ea141778cf83f1b6000`  
		Last Modified: Sat, 07 Aug 2021 01:58:11 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977f0d719f8308cf8b842d6ecd386d05841cf385cc47a05dfc9e338f90249082`  
		Last Modified: Sat, 07 Aug 2021 01:58:11 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
