## `redis:5-alpine`

```console
$ docker pull redis@sha256:6777532d6a8e0124c592111372339476792a40cebb130cf522863d19c2cc6e63
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

### `redis:5-alpine` - linux; amd64

```console
$ docker pull redis@sha256:853fde116bec7df75a6f7c50f09396d0eccc15c605f91565c2c637e40885c7bf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9870744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb57d37ad39e1355b0c0d81fe7e66428c6e64ce40f7ad2236677bb3a6bbd6937`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 17 Mar 2022 04:01:58 GMT
ADD file:cf4b631a115c2bbfbd81cad2d3041bceb64a8136aac92ba8a63b6c51d60af764 in / 
# Thu, 17 Mar 2022 04:01:59 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 05:52:05 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Fri, 18 Mar 2022 05:52:07 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Fri, 18 Mar 2022 06:03:22 GMT
ENV REDIS_VERSION=5.0.14
# Fri, 18 Mar 2022 06:03:22 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.14.tar.gz
# Fri, 18 Mar 2022 06:03:22 GMT
ENV REDIS_DOWNLOAD_SHA=3ea5024766d983249e80d4aa9457c897a9f079957d0fb1f35682df233f997f32
# Fri, 18 Mar 2022 06:04:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 18 Mar 2022 06:04:22 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 18 Mar 2022 06:04:22 GMT
VOLUME [/data]
# Fri, 18 Mar 2022 06:04:22 GMT
WORKDIR /data
# Fri, 18 Mar 2022 06:04:22 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 18 Mar 2022 06:04:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 06:04:22 GMT
EXPOSE 6379
# Fri, 18 Mar 2022 06:04:22 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:3d243047344378e9b7136d552d48feb7ea8b6fe14ce0990e0cc011d5e369626a`  
		Last Modified: Thu, 17 Mar 2022 04:02:41 GMT  
		Size: 2.8 MB (2812636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5dbe74b9b57a68635e01eecc3ff361880863fcd89c000379ef23229ec1f07f0`  
		Last Modified: Fri, 18 Mar 2022 06:05:56 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b16015c185cbd247a89249e61b942a2601b416fc38ca621107ec4e1cc7b191cc`  
		Last Modified: Fri, 18 Mar 2022 06:05:56 GMT  
		Size: 406.3 KB (406323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e28b56ee1e9a60b8ef418de16979630d2f70b3ff5bf78cb29b18db250df0b468`  
		Last Modified: Fri, 18 Mar 2022 06:08:32 GMT  
		Size: 6.6 MB (6649970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc223657e928a3438789542db0f601c1f2df9f3123e9e32a493e3c6b9cac4beb`  
		Last Modified: Fri, 18 Mar 2022 06:08:31 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe43b584da53a76c09e58dd4adf8e401e1f442069c4fde7688358d0e472d104`  
		Last Modified: Fri, 18 Mar 2022 06:08:31 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-alpine` - linux; arm variant v6

```console
$ docker pull redis@sha256:1bb34fbf1da4e4e1ed34dba28b63ebc851baab546d8ba2458032473502ca7d39
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9614309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42772410438570f820d96d8d1bd4f06340fec038f0f5e3252f61640dd396d5fe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 17 Mar 2022 02:26:45 GMT
ADD file:9c8618405ef54d562132919ffe49c862d014b402e0e4813b87bf01574fa04c0e in / 
# Thu, 17 Mar 2022 02:26:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 10:18:30 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Thu, 17 Mar 2022 10:18:33 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Thu, 17 Mar 2022 10:23:27 GMT
ENV REDIS_VERSION=5.0.14
# Thu, 17 Mar 2022 10:23:27 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.14.tar.gz
# Thu, 17 Mar 2022 10:23:27 GMT
ENV REDIS_DOWNLOAD_SHA=3ea5024766d983249e80d4aa9457c897a9f079957d0fb1f35682df233f997f32
# Thu, 17 Mar 2022 10:24:32 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Thu, 17 Mar 2022 10:24:33 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 17 Mar 2022 10:24:34 GMT
VOLUME [/data]
# Thu, 17 Mar 2022 10:24:34 GMT
WORKDIR /data
# Thu, 17 Mar 2022 10:24:34 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Thu, 17 Mar 2022 10:24:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 10:24:35 GMT
EXPOSE 6379
# Thu, 17 Mar 2022 10:24:36 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:787f016efa9bc7812361be134f731e845b97fba19169cf3615e7048c0412380e`  
		Last Modified: Thu, 17 Mar 2022 02:28:24 GMT  
		Size: 2.6 MB (2624973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50806cda018687498cbd7c69c295daee4ebe97e116c0106b7ef9f8ba14523dd7`  
		Last Modified: Thu, 17 Mar 2022 10:26:33 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36f33eb49213759d7d6fd6c50029e8fa0eb322ca9180f41fb1e0313d075c50c4`  
		Last Modified: Thu, 17 Mar 2022 10:26:33 GMT  
		Size: 410.3 KB (410290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11992e6dcd0e4c95945cd58836c87a26de27f8d487676b896f6a383ed51fbaa4`  
		Last Modified: Thu, 17 Mar 2022 10:28:04 GMT  
		Size: 6.6 MB (6577228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ac465501ad640809ba32d023ddbfcf8f4be26742e3e230b276e9d89e045ad1`  
		Last Modified: Thu, 17 Mar 2022 10:28:00 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21f5d1546d1c6007547b300c03d273a0b6c591fda8ddec46b65a8337d8a7778c`  
		Last Modified: Thu, 17 Mar 2022 10:28:00 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-alpine` - linux; arm variant v7

```console
$ docker pull redis@sha256:876042dfa369fd50109ff63b8a913053fe44d47de85ee705561e7fb199910fe3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9305561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce39da9ec1f91fe1f2fdbd680368869c99d1f760acf7860b4bd0f64e3d8c6ed2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 17 Mar 2022 09:26:34 GMT
ADD file:01e87d7f83dfb32fd8a1b7b889b923432c2e0516d79a4196e01ad0ad15e33d68 in / 
# Thu, 17 Mar 2022 09:26:35 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 12:11:27 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Fri, 18 Mar 2022 12:11:32 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Fri, 18 Mar 2022 12:23:04 GMT
ENV REDIS_VERSION=5.0.14
# Fri, 18 Mar 2022 12:23:04 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.14.tar.gz
# Fri, 18 Mar 2022 12:23:04 GMT
ENV REDIS_DOWNLOAD_SHA=3ea5024766d983249e80d4aa9457c897a9f079957d0fb1f35682df233f997f32
# Fri, 18 Mar 2022 12:24:06 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 18 Mar 2022 12:24:08 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 18 Mar 2022 12:24:08 GMT
VOLUME [/data]
# Fri, 18 Mar 2022 12:24:09 GMT
WORKDIR /data
# Fri, 18 Mar 2022 12:24:09 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 18 Mar 2022 12:24:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 12:24:10 GMT
EXPOSE 6379
# Fri, 18 Mar 2022 12:24:10 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:205cbce5da6d59acc17b2db4c1af7903ca3497b99d4bedb94ef66ace17303808`  
		Last Modified: Thu, 17 Mar 2022 09:28:11 GMT  
		Size: 2.4 MB (2427136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a8e157a1170daae834602ee5f747668e412f7609b2b3d154f66761627156366`  
		Last Modified: Fri, 18 Mar 2022 12:28:16 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9639c0daea0b1bec7878e31cd2aad4c3472123568cf1da5254de4ed38651fe3`  
		Last Modified: Fri, 18 Mar 2022 12:28:17 GMT  
		Size: 404.4 KB (404398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e66700593884dbd5d6ccf04defa785bf683d7a66e76b6f266d8f49ecee89e5c1`  
		Last Modified: Fri, 18 Mar 2022 12:31:37 GMT  
		Size: 6.5 MB (6472212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d2af4380b87b847b6419bac8fb0ab9d217774491465df7b88680b9872ada02`  
		Last Modified: Fri, 18 Mar 2022 12:31:33 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee3904f496bbb05a5c3d3e95d1052f33c7438876f4ca59de9ab6b320a4f55fd`  
		Last Modified: Fri, 18 Mar 2022 12:31:33 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-alpine` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:6d988657dd6b64c9be0a56571cbe5527baea27d9de26fc6457a7bdac62e96605
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.8 MB (9793215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa8ced7db4728acda231c5e74a61c637eeee89b2aa55ce0281c0c7493ecaf568`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 17 Mar 2022 03:19:52 GMT
ADD file:cd7d91362950471ca4678cf3833dc47119ab519dea51424c847bbbb21e1649d4 in / 
# Thu, 17 Mar 2022 03:19:52 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 19:59:12 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Thu, 17 Mar 2022 19:59:14 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Thu, 17 Mar 2022 20:05:22 GMT
ENV REDIS_VERSION=5.0.14
# Thu, 17 Mar 2022 20:05:23 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.14.tar.gz
# Thu, 17 Mar 2022 20:05:24 GMT
ENV REDIS_DOWNLOAD_SHA=3ea5024766d983249e80d4aa9457c897a9f079957d0fb1f35682df233f997f32
# Thu, 17 Mar 2022 20:06:00 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Thu, 17 Mar 2022 20:06:01 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 17 Mar 2022 20:06:02 GMT
VOLUME [/data]
# Thu, 17 Mar 2022 20:06:03 GMT
WORKDIR /data
# Thu, 17 Mar 2022 20:06:05 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Thu, 17 Mar 2022 20:06:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 20:06:06 GMT
EXPOSE 6379
# Thu, 17 Mar 2022 20:06:07 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:148d739a8e6b9342daa1f5b428d3a3c6118f340f21df28c16e06f918ef150147`  
		Last Modified: Thu, 17 Mar 2022 03:20:45 GMT  
		Size: 2.7 MB (2714807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92115e67ee868c75637e30d95c19d9cea7fc508b7b7dbc6f3ce7d67874916867`  
		Last Modified: Thu, 17 Mar 2022 20:07:54 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85acff92d17c7a624a43c3870e1b7d34a678851c4ad3db8dd70140d790460d55`  
		Last Modified: Thu, 17 Mar 2022 20:07:54 GMT  
		Size: 407.2 KB (407234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:486c63ab8b159f9f7cd86b253a4aa9dcd2f663155a7dcf92527553dc00028187`  
		Last Modified: Thu, 17 Mar 2022 20:10:19 GMT  
		Size: 6.7 MB (6669425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c56f4431768848f3692c0e8295b10dfa00aef47388bbccdc04de7f746423d6`  
		Last Modified: Thu, 17 Mar 2022 20:10:17 GMT  
		Size: 98.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61cf7e418b0d8cb8f1f60cf6d2ef34f655c5be679591467792222bb5f8c85809`  
		Last Modified: Thu, 17 Mar 2022 20:10:17 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-alpine` - linux; 386

```console
$ docker pull redis@sha256:bb9b7b3ad840282c6e8ab9c441c0d305ed266ff15bab7bb8e11a0ad951184a7c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9603230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ef18dbb92df82dd2e54953079cf8e0ed33e9f02ece268c3cf8724febc9695ce`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 17 Mar 2022 08:13:03 GMT
ADD file:22216bc654d9177244235f242fa83cae3b283b3c145cad7ccf11c0d29f5f0ff2 in / 
# Thu, 17 Mar 2022 08:13:03 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 19:43:31 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Thu, 17 Mar 2022 19:43:34 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Thu, 17 Mar 2022 19:56:22 GMT
ENV REDIS_VERSION=5.0.14
# Thu, 17 Mar 2022 19:56:22 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.14.tar.gz
# Thu, 17 Mar 2022 19:56:22 GMT
ENV REDIS_DOWNLOAD_SHA=3ea5024766d983249e80d4aa9457c897a9f079957d0fb1f35682df233f997f32
# Thu, 17 Mar 2022 19:58:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Thu, 17 Mar 2022 19:58:17 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 17 Mar 2022 19:58:17 GMT
VOLUME [/data]
# Thu, 17 Mar 2022 19:58:17 GMT
WORKDIR /data
# Thu, 17 Mar 2022 19:58:18 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Thu, 17 Mar 2022 19:58:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 19:58:18 GMT
EXPOSE 6379
# Thu, 17 Mar 2022 19:58:18 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:93317a1f65ec94b67aefe728a598022610246404e3a68d391c76cd0e5244a2a0`  
		Last Modified: Thu, 17 Mar 2022 08:13:56 GMT  
		Size: 2.8 MB (2821789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b24f62ee1b8f3c513a4a4c434b03862ad8380bd9c5e41990d204c4e279e58cf`  
		Last Modified: Thu, 17 Mar 2022 20:01:08 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef53db642e1bf4fbe88a9bdf20dfdc6ab61b2e17b023a88fb3a87d1ad24471be`  
		Last Modified: Thu, 17 Mar 2022 20:01:08 GMT  
		Size: 413.0 KB (412982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c42d66d0f463e39898c69016865c1cb363d85f2aa2b4f8afac35b8f84a4c152a`  
		Last Modified: Thu, 17 Mar 2022 20:04:11 GMT  
		Size: 6.4 MB (6366646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ecc50782b59e739ab97f2f0057cf2fe699f95d67f7cecaaf1900aec139c17c3`  
		Last Modified: Thu, 17 Mar 2022 20:04:09 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f977078f6bb695e7b483018f6670191132f3b1325d18dbd22b6a073b6ab66dd`  
		Last Modified: Thu, 17 Mar 2022 20:04:09 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-alpine` - linux; ppc64le

```console
$ docker pull redis@sha256:f3d3d58608d2cda7ca6404f7e36c12ce31dc37d575e5e6de8d47c8c449b52427
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.4 MB (10353051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:261218aca3062bd31fece4e91625b9e54a3806d14fbb56f2d938d8c86c86ddd0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 24 Nov 2021 20:20:16 GMT
ADD file:57115dca2eb707f46b6301e75174e6aa316fb02ac28643b91429b75be51bd8c8 in / 
# Wed, 24 Nov 2021 20:20:20 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 00:58:13 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Tue, 30 Nov 2021 00:58:19 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Tue, 30 Nov 2021 01:02:42 GMT
ENV REDIS_VERSION=5.0.14
# Tue, 30 Nov 2021 01:02:44 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.14.tar.gz
# Tue, 30 Nov 2021 01:02:47 GMT
ENV REDIS_DOWNLOAD_SHA=3ea5024766d983249e80d4aa9457c897a9f079957d0fb1f35682df233f997f32
# Tue, 30 Nov 2021 01:03:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Tue, 30 Nov 2021 01:03:54 GMT
RUN mkdir /data && chown redis:redis /data
# Tue, 30 Nov 2021 01:03:58 GMT
VOLUME [/data]
# Tue, 30 Nov 2021 01:04:05 GMT
WORKDIR /data
# Tue, 30 Nov 2021 01:04:07 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Tue, 30 Nov 2021 01:04:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 30 Nov 2021 01:04:15 GMT
EXPOSE 6379
# Tue, 30 Nov 2021 01:04:18 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:159b5dcb1717c815c76ff5ea1db730e18e8609c9090238e43282856db9e71f47`  
		Last Modified: Wed, 24 Nov 2021 20:21:14 GMT  
		Size: 2.8 MB (2814780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fdebffe4e42fede349f1e45bd57bfe6cb93bda55d5dccf5e53d5a6061db63db`  
		Last Modified: Tue, 30 Nov 2021 01:05:47 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5101e39ab1eefa195df978720311d2e325f05e8b4d282e6e8487eed9f6caabf0`  
		Last Modified: Tue, 30 Nov 2021 01:05:48 GMT  
		Size: 413.0 KB (412952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4640f2fc177bb415b92c16cdf39797deeff99c4a9643f5f999f9603de56041`  
		Last Modified: Tue, 30 Nov 2021 01:06:52 GMT  
		Size: 7.1 MB (7123497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4d2cbe95739a5f7ea65defbe09db4e37d8f89b5a8db73ea870cf7d6928b566`  
		Last Modified: Tue, 30 Nov 2021 01:06:50 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4cf4e6018746c49575516dde6316706087bea778c428b6ce9af86145821b4ec`  
		Last Modified: Tue, 30 Nov 2021 01:06:50 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-alpine` - linux; s390x

```console
$ docker pull redis@sha256:6cd58d75cef3a2708bc604a0e27f396098e9d350844c35668cf6538a9b00e96d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (9960670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34d49139a53966aeec6f8f0ea0fc7435f428dc83d04da23c00b1ad946cfb6fb7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 17 Mar 2022 03:04:28 GMT
ADD file:f623c69acb1859b41ef29e8f20f4e6c7072d9c6d7210d745afc615251bfe418f in / 
# Thu, 17 Mar 2022 03:04:28 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 15:37:21 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Thu, 17 Mar 2022 15:37:22 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Thu, 17 Mar 2022 15:41:59 GMT
ENV REDIS_VERSION=5.0.14
# Thu, 17 Mar 2022 15:41:59 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.14.tar.gz
# Thu, 17 Mar 2022 15:42:00 GMT
ENV REDIS_DOWNLOAD_SHA=3ea5024766d983249e80d4aa9457c897a9f079957d0fb1f35682df233f997f32
# Thu, 17 Mar 2022 15:42:33 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Thu, 17 Mar 2022 15:42:33 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 17 Mar 2022 15:42:34 GMT
VOLUME [/data]
# Thu, 17 Mar 2022 15:42:34 GMT
WORKDIR /data
# Thu, 17 Mar 2022 15:42:34 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Thu, 17 Mar 2022 15:42:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 15:42:34 GMT
EXPOSE 6379
# Thu, 17 Mar 2022 15:42:34 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:d51040c5bfbf434887bfed2557335a411e6ef760d04cc178d455d1c3ec1b721c`  
		Last Modified: Thu, 17 Mar 2022 03:05:26 GMT  
		Size: 2.6 MB (2601715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fff5030e3f42ca4bbffb08fe3a5b040f5c529e596b39f49a3c82569e31fcf72`  
		Last Modified: Thu, 17 Mar 2022 15:44:20 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c3c5fb50d004d642c4b2a46a3aa675c6ea2f35c124a4e1fc9a14a2b226bb44`  
		Last Modified: Thu, 17 Mar 2022 15:44:21 GMT  
		Size: 410.9 KB (410902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59fb8186d59c91c3e46fd399c5e74cc6067e4069c29659c735fbb8b3b4c1235`  
		Last Modified: Thu, 17 Mar 2022 15:45:52 GMT  
		Size: 6.9 MB (6946238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b332cc5aaef70dc9238c5700cacd1392b0b0489d63e6e61edd35efffe27968db`  
		Last Modified: Thu, 17 Mar 2022 15:45:50 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b34a67aad70c8e707fd1f030b5e19e70e00c7288526fd054ef0435b34f996240`  
		Last Modified: Thu, 17 Mar 2022 15:45:51 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
