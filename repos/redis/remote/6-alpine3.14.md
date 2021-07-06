## `redis:6-alpine3.14`

```console
$ docker pull redis@sha256:8c00f0db8eae7a75ac128404a96bdbe042bf01da7b927b3225fe859d61c5fb1f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; 386

### `redis:6-alpine3.14` - linux; amd64

```console
$ docker pull redis@sha256:8061ca607db2a0c80010aeb5fc9bed0253448bc68711eaa14253a392f6c48280
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.9 MB (10891270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:500703a12fa42704f1901f244f3cb4feb74fb1ca550b2eff4bb22e765eb10971`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Tue, 06 Jul 2021 17:54:35 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Tue, 06 Jul 2021 17:54:36 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Tue, 06 Jul 2021 17:54:36 GMT
ENV REDIS_VERSION=6.2.4
# Tue, 06 Jul 2021 17:54:37 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.4.tar.gz
# Tue, 06 Jul 2021 17:54:37 GMT
ENV REDIS_DOWNLOAD_SHA=ba32c406a10fc2c09426e2be2787d74ff204eb3a2e496d87cff76a476b6ae16e
# Tue, 06 Jul 2021 17:55:45 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Tue, 06 Jul 2021 17:55:46 GMT
RUN mkdir /data && chown redis:redis /data
# Tue, 06 Jul 2021 17:55:46 GMT
VOLUME [/data]
# Tue, 06 Jul 2021 17:55:46 GMT
WORKDIR /data
# Tue, 06 Jul 2021 17:55:46 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Tue, 06 Jul 2021 17:55:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Jul 2021 17:55:47 GMT
EXPOSE 6379
# Tue, 06 Jul 2021 17:55:47 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db2305878ef924f3ebdc23c7f93c84e1406eca01618c945f859736bccd4692d`  
		Last Modified: Tue, 06 Jul 2021 17:59:24 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3558750a1d54c99f919b839c9dde5afd8f769bd3afee3f0f6ec1b9b451fde5e7`  
		Last Modified: Tue, 06 Jul 2021 17:59:24 GMT  
		Size: 384.4 KB (384421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240d71d1acc751292d1017af4780c07ca4105656f96a627dc2362e5f924f96d9`  
		Last Modified: Tue, 06 Jul 2021 17:59:26 GMT  
		Size: 7.7 MB (7693556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a888d25337fd29fe874e5bfa2001e31469ccbc2391e515935079996031a2fa5`  
		Last Modified: Tue, 06 Jul 2021 17:59:24 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22e6fbce362aff5cd621f37ee0c4834dccc2f01545cc33a4d9f351215e830a3b`  
		Last Modified: Tue, 06 Jul 2021 17:59:24 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine3.14` - linux; arm variant v6

```console
$ docker pull redis@sha256:baac05fb2a56758d9c9385854d3eb3910350c122ba8baad4aee6051d56cf0802
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.6 MB (10587297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e05ea979ebe241e0e13e2b018a4925a00db2da968a6562c28b1723884f5c2a80`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:26 GMT
ADD file:c80bc2b093cbc0fc466582ef21cbed377de9fa874aedbf320079525ddacd1200 in / 
# Tue, 15 Jun 2021 22:57:26 GMT
CMD ["/bin/sh"]
# Tue, 06 Jul 2021 17:03:28 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Tue, 06 Jul 2021 17:03:31 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Tue, 06 Jul 2021 17:03:32 GMT
ENV REDIS_VERSION=6.2.4
# Tue, 06 Jul 2021 17:03:32 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.4.tar.gz
# Tue, 06 Jul 2021 17:03:33 GMT
ENV REDIS_DOWNLOAD_SHA=ba32c406a10fc2c09426e2be2787d74ff204eb3a2e496d87cff76a476b6ae16e
# Tue, 06 Jul 2021 17:04:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Tue, 06 Jul 2021 17:04:45 GMT
RUN mkdir /data && chown redis:redis /data
# Tue, 06 Jul 2021 17:04:45 GMT
VOLUME [/data]
# Tue, 06 Jul 2021 17:04:46 GMT
WORKDIR /data
# Tue, 06 Jul 2021 17:04:46 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Tue, 06 Jul 2021 17:04:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Jul 2021 17:04:47 GMT
EXPOSE 6379
# Tue, 06 Jul 2021 17:04:48 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:b4c9a0924271af3466de27804af26420eb58da1466e7eaaba127d178b380fea3`  
		Last Modified: Tue, 15 Jun 2021 22:58:47 GMT  
		Size: 2.6 MB (2624382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597047ceadae07829fd8b80127f94d3d69704d627c57bb16d7e83c9def767301`  
		Last Modified: Tue, 06 Jul 2021 17:09:20 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570997ff334916737428e81b30711552ca4fab99d9025f566edcf44c3e13ca1e`  
		Last Modified: Tue, 06 Jul 2021 17:09:21 GMT  
		Size: 388.4 KB (388435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e1e8306e3b4bbc1b97652acca93f28efe4d8ef59bb349f9fb186d13933580fe`  
		Last Modified: Tue, 06 Jul 2021 17:09:26 GMT  
		Size: 7.6 MB (7572664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc42ac49a9bae95a0eeb6b979923d96100b51899881f22c6e5002656e813fc4`  
		Last Modified: Tue, 06 Jul 2021 17:09:21 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a77a3205c0bc592d871be3abcd43a90718b0d33d3ea231c54f002a14bb96988`  
		Last Modified: Tue, 06 Jul 2021 17:09:20 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine3.14` - linux; arm variant v7

```console
$ docker pull redis@sha256:1cd809915c6360fc517a2bafe9c9c8cf7093fc6ce3b5a3deb384f424442d1b24
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.3 MB (10267591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a9305cf4248d7823122f31276c6f7cee0b928afdb38476e7354eb0df0a02835`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:05 GMT
ADD file:416a8b507abdc6bdcb22997a4be0a4170796c3f9f77e315b2dbff2b0a212bc68 in / 
# Tue, 15 Jun 2021 23:15:06 GMT
CMD ["/bin/sh"]
# Tue, 06 Jul 2021 18:09:03 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Tue, 06 Jul 2021 18:09:08 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Tue, 06 Jul 2021 18:09:09 GMT
ENV REDIS_VERSION=6.2.4
# Tue, 06 Jul 2021 18:09:10 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.4.tar.gz
# Tue, 06 Jul 2021 18:09:11 GMT
ENV REDIS_DOWNLOAD_SHA=ba32c406a10fc2c09426e2be2787d74ff204eb3a2e496d87cff76a476b6ae16e
# Tue, 06 Jul 2021 18:10:41 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Tue, 06 Jul 2021 18:10:44 GMT
RUN mkdir /data && chown redis:redis /data
# Tue, 06 Jul 2021 18:10:45 GMT
VOLUME [/data]
# Tue, 06 Jul 2021 18:10:47 GMT
WORKDIR /data
# Tue, 06 Jul 2021 18:10:48 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Tue, 06 Jul 2021 18:10:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Jul 2021 18:10:50 GMT
EXPOSE 6379
# Tue, 06 Jul 2021 18:10:51 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:136482bf81d1fa351b424ebb8c7e34d15f2c5ed3fc0b66b544b8312bda3d52d9`  
		Last Modified: Tue, 15 Jun 2021 23:16:40 GMT  
		Size: 2.4 MB (2427917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e6ae5782522d489b98cc4cf0217b5ebdc53a69e00fb48e9f17256e53036e0c`  
		Last Modified: Tue, 06 Jul 2021 18:18:30 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66778e3445c034f863fc933b171106e21d3fcca76fe28d94af1b1f17aa19e5fd`  
		Last Modified: Tue, 06 Jul 2021 18:18:30 GMT  
		Size: 383.2 KB (383231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8f92ad6c30a9b158f5ed168ad32a137ef98e6a2b60fa58856a9480ff50f548b`  
		Last Modified: Tue, 06 Jul 2021 18:18:33 GMT  
		Size: 7.5 MB (7454623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cb40cda1f09aa27c99e8ff57f2b8dfb0e5c51400792f130dac7f2c37c40e6fd`  
		Last Modified: Tue, 06 Jul 2021 18:18:29 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8924d2578279ea87ae9fbf4b20f803d670e4f9edda7bc109dd5386a037c88df4`  
		Last Modified: Tue, 06 Jul 2021 18:18:29 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine3.14` - linux; 386

```console
$ docker pull redis@sha256:1d348fd324adc6d091a30775fd5216530a4bdfd659eef9acd2d1345ce641b668
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.6 MB (10553343 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ac08352e6df94f2cb7ecdeea2a99caa4f55b10061b4c68c8beeb1a239f5e569`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Tue, 15 Jun 2021 21:38:30 GMT
ADD file:3b0fe1454491bb05e218b090fd461f2fd39546aa4a53eb3f953ee8eae149ac57 in / 
# Tue, 15 Jun 2021 21:38:30 GMT
CMD ["/bin/sh"]
# Tue, 06 Jul 2021 17:58:37 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Tue, 06 Jul 2021 17:58:39 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Tue, 06 Jul 2021 17:58:39 GMT
ENV REDIS_VERSION=6.2.4
# Tue, 06 Jul 2021 17:58:40 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.4.tar.gz
# Tue, 06 Jul 2021 17:58:40 GMT
ENV REDIS_DOWNLOAD_SHA=ba32c406a10fc2c09426e2be2787d74ff204eb3a2e496d87cff76a476b6ae16e
# Tue, 06 Jul 2021 17:59:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Tue, 06 Jul 2021 17:59:53 GMT
RUN mkdir /data && chown redis:redis /data
# Tue, 06 Jul 2021 17:59:53 GMT
VOLUME [/data]
# Tue, 06 Jul 2021 17:59:54 GMT
WORKDIR /data
# Tue, 06 Jul 2021 17:59:54 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Tue, 06 Jul 2021 17:59:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Jul 2021 17:59:54 GMT
EXPOSE 6379
# Tue, 06 Jul 2021 17:59:54 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:be21df321efb39c5daf3151073ebff7688e15ea6cd5158878bc9559a5db76ac6`  
		Last Modified: Tue, 15 Jun 2021 21:39:16 GMT  
		Size: 2.8 MB (2820718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2551de8396d4fcd47753ef4d9beb999c0b7ea922e5a92009681b6f94f5c0506b`  
		Last Modified: Tue, 06 Jul 2021 18:04:37 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec7f9665c61bd95041cf22f6ce770b5e8bbbbbad420a7eb1f7566217c27198d8`  
		Last Modified: Tue, 06 Jul 2021 18:04:37 GMT  
		Size: 390.8 KB (390807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c97ee26a9e9d2e3a3f05fe1a59385214b8960bc7c7a56160bbc3da49e3cc03d`  
		Last Modified: Tue, 06 Jul 2021 18:04:39 GMT  
		Size: 7.3 MB (7340000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9955f04b1bb9f6bc2b57e90f8211208c35a7399364310042b3dd90f0f06147b7`  
		Last Modified: Tue, 06 Jul 2021 18:04:37 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:724c8a44bc78fff263c076b30ce22be9be213780c6c4b4f7cae21d216f49122a`  
		Last Modified: Tue, 06 Jul 2021 18:04:37 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
