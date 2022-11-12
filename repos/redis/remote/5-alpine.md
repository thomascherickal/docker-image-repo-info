## `redis:5-alpine`

```console
$ docker pull redis@sha256:afe7ad17688ab96d9cdf99388d3c75a5323c85ff3a73b4c4e6432d58067283c3
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
$ docker pull redis@sha256:1b24e5253e866e60e320446bd588407df499936bdc7d89fa52cd2772a4e3a162
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9639703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7558bc54e8a27a73a00084ee5b1615354b010a23174e3a917b9388eb750f5afe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:07:37 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Sat, 12 Nov 2022 08:07:39 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Sat, 12 Nov 2022 08:10:21 GMT
ENV REDIS_VERSION=5.0.14
# Sat, 12 Nov 2022 08:10:21 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.14.tar.gz
# Sat, 12 Nov 2022 08:10:21 GMT
ENV REDIS_DOWNLOAD_SHA=3ea5024766d983249e80d4aa9457c897a9f079957d0fb1f35682df233f997f32
# Sat, 12 Nov 2022 08:10:58 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Sat, 12 Nov 2022 08:10:59 GMT
RUN mkdir /data && chown redis:redis /data
# Sat, 12 Nov 2022 08:10:59 GMT
VOLUME [/data]
# Sat, 12 Nov 2022 08:10:59 GMT
WORKDIR /data
# Sat, 12 Nov 2022 08:10:59 GMT
COPY file:a9e7249f657e2eec627bb4be492ad18aae3e5e1f0e47d22644eaf1ef2138c0ce in /usr/local/bin/ 
# Sat, 12 Nov 2022 08:10:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 08:10:59 GMT
EXPOSE 6379
# Sat, 12 Nov 2022 08:10:59 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83276aa4de36d9be316b90e13568d2867c44a7d18385402135386d4c6d6e39e6`  
		Last Modified: Sat, 12 Nov 2022 08:11:51 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:731cc432e6da70180e8680fcd2b301187354fb21b7da299939ee5fce5e212504`  
		Last Modified: Sat, 12 Nov 2022 08:11:52 GMT  
		Size: 386.7 KB (386730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67999d49aa905421e5eef5634ca77ff0b32489a88a95d4904adf144af01f597`  
		Last Modified: Sat, 12 Nov 2022 08:13:00 GMT  
		Size: 6.4 MB (6444719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf1ab41b1708ffad1febf99297af653669b850b2b8aae54ef32af3ba4406655`  
		Last Modified: Sat, 12 Nov 2022 08:12:59 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18a7dec11639171d7df563840e7ad2443f63930ec6d5e79645d793a76140ee91`  
		Last Modified: Sat, 12 Nov 2022 08:12:59 GMT  
		Size: 578.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-alpine` - linux; arm variant v6

```console
$ docker pull redis@sha256:07c1af9c7de7b1744f8dd10b6cde737769fdc01d0cfe161b4082cae111a4a457
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9588996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:119c8e401e9f7cf1ea9acd33c7c76e455ddd5b6c89866e67427d700ea5eb4f26`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Sat, 12 Nov 2022 03:49:18 GMT
ADD file:493290ed8856fa13463defe63da0d30ab3de5dde042c87ef7c0701d66ebb8892 in / 
# Sat, 12 Nov 2022 03:49:18 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:05:40 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Sat, 12 Nov 2022 08:05:41 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Sat, 12 Nov 2022 08:08:26 GMT
ENV REDIS_VERSION=5.0.14
# Sat, 12 Nov 2022 08:08:26 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.14.tar.gz
# Sat, 12 Nov 2022 08:08:26 GMT
ENV REDIS_DOWNLOAD_SHA=3ea5024766d983249e80d4aa9457c897a9f079957d0fb1f35682df233f997f32
# Sat, 12 Nov 2022 08:09:03 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Sat, 12 Nov 2022 08:09:04 GMT
RUN mkdir /data && chown redis:redis /data
# Sat, 12 Nov 2022 08:09:04 GMT
VOLUME [/data]
# Sat, 12 Nov 2022 08:09:04 GMT
WORKDIR /data
# Sat, 12 Nov 2022 08:09:04 GMT
COPY file:a9e7249f657e2eec627bb4be492ad18aae3e5e1f0e47d22644eaf1ef2138c0ce in /usr/local/bin/ 
# Sat, 12 Nov 2022 08:09:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 08:09:04 GMT
EXPOSE 6379
# Sat, 12 Nov 2022 08:09:04 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:9616ea8c1de4a90b1a50591336485e88ae5c2346e0d778bdbe69b00647bf8e39`  
		Last Modified: Sat, 12 Nov 2022 03:50:12 GMT  
		Size: 2.6 MB (2615105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e57376876736ea81b0b30a9390e8de4e16127f9ce8391ea10c9080a138fab1f0`  
		Last Modified: Sat, 12 Nov 2022 08:10:15 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a0398a226a864481262608a098172816548bc07b2faf82eb13a0088e0d058a`  
		Last Modified: Sat, 12 Nov 2022 08:10:16 GMT  
		Size: 391.5 KB (391460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51b018407ff7d0980eb2e3509887a5d8b317e45b1a7c9404bf2eed7cc9a20ccd`  
		Last Modified: Sat, 12 Nov 2022 08:11:40 GMT  
		Size: 6.6 MB (6580511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccd1577795e059526508d055902d81e675dcc8eb2a08b67874e821a95616f640`  
		Last Modified: Sat, 12 Nov 2022 08:11:38 GMT  
		Size: 100.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66498064c5e62703b5c6c1a30e88969ea82d0f880e806da307cfbaaca6ddf8e3`  
		Last Modified: Sat, 12 Nov 2022 08:11:38 GMT  
		Size: 578.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-alpine` - linux; arm variant v7

```console
$ docker pull redis@sha256:8a05f227e96bad2dae2cd0fc451184668df8ff2a73a82ac6013de58041c264a9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9293582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35600c67ce510876bdb166a396ded728dd95b7337c36fe25cbc7bbded74f3186`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Sat, 12 Nov 2022 03:57:24 GMT
ADD file:0b4a628f529226f5ec9d357ca63138bd2d22411a889c780ac8d395d761e07b2c in / 
# Sat, 12 Nov 2022 03:57:24 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 07:40:46 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Sat, 12 Nov 2022 07:40:48 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Sat, 12 Nov 2022 07:44:07 GMT
ENV REDIS_VERSION=5.0.14
# Sat, 12 Nov 2022 07:44:07 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.14.tar.gz
# Sat, 12 Nov 2022 07:44:07 GMT
ENV REDIS_DOWNLOAD_SHA=3ea5024766d983249e80d4aa9457c897a9f079957d0fb1f35682df233f997f32
# Sat, 12 Nov 2022 07:44:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Sat, 12 Nov 2022 07:44:46 GMT
RUN mkdir /data && chown redis:redis /data
# Sat, 12 Nov 2022 07:44:46 GMT
VOLUME [/data]
# Sat, 12 Nov 2022 07:44:46 GMT
WORKDIR /data
# Sat, 12 Nov 2022 07:44:47 GMT
COPY file:a9e7249f657e2eec627bb4be492ad18aae3e5e1f0e47d22644eaf1ef2138c0ce in /usr/local/bin/ 
# Sat, 12 Nov 2022 07:44:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 07:44:47 GMT
EXPOSE 6379
# Sat, 12 Nov 2022 07:44:47 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:e44ba29d168a7f7c9e914f3724614df9e070aa6ef9b9ba5c9004db3c071f403a`  
		Last Modified: Sat, 12 Nov 2022 03:58:16 GMT  
		Size: 2.4 MB (2418788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39f9cb9b18701b22e7c9736238d068843b2c63aa2da9111d82b8a7d66e645c74`  
		Last Modified: Sat, 12 Nov 2022 07:47:10 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d30a6c1644a9524c717986690f4a17768535c172e9834975c6a79aff151c060`  
		Last Modified: Sat, 12 Nov 2022 07:47:10 GMT  
		Size: 384.7 KB (384677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd10522c86ca19e74a6c5701089630db73f32b967aed97a4ffe21d7b706d4436`  
		Last Modified: Sat, 12 Nov 2022 07:48:46 GMT  
		Size: 6.5 MB (6488200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c09c6837a55cf6ee882560322b74bf173c324da8274d4746508267cb776dcff6`  
		Last Modified: Sat, 12 Nov 2022 07:48:44 GMT  
		Size: 100.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136f0bb41f2fe4e5713e8415eed6d87e66c3b2896eac6b42be639b2ca0b8b45d`  
		Last Modified: Sat, 12 Nov 2022 07:48:44 GMT  
		Size: 575.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-alpine` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:4777db34db362acf1d107d113a6552b1528aac109999363b5529b4b290e031a9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.4 MB (11440189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f06db87632d226e9f7268abe5a30aa322dbb839d33a0302e8b5aec027dc0d1e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Thu, 10 Nov 2022 20:39:41 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 04:57:48 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Fri, 11 Nov 2022 04:57:49 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Fri, 11 Nov 2022 04:59:50 GMT
ENV REDIS_VERSION=5.0.14
# Fri, 11 Nov 2022 04:59:50 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.14.tar.gz
# Fri, 11 Nov 2022 04:59:50 GMT
ENV REDIS_DOWNLOAD_SHA=3ea5024766d983249e80d4aa9457c897a9f079957d0fb1f35682df233f997f32
# Fri, 11 Nov 2022 05:00:19 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 11 Nov 2022 05:00:19 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 11 Nov 2022 05:00:19 GMT
VOLUME [/data]
# Fri, 11 Nov 2022 05:00:19 GMT
WORKDIR /data
# Fri, 11 Nov 2022 05:00:19 GMT
COPY file:a9e7249f657e2eec627bb4be492ad18aae3e5e1f0e47d22644eaf1ef2138c0ce in /usr/local/bin/ 
# Fri, 11 Nov 2022 05:00:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Nov 2022 05:00:19 GMT
EXPOSE 6379
# Fri, 11 Nov 2022 05:00:20 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78e59348074813e352b5624fd1835fde9f2fddaf5ae7ab2797dca8e9163ecd0b`  
		Last Modified: Fri, 11 Nov 2022 05:01:15 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e214d0d969b6e533cf1e7e12088fc5c8daed7d233a984bfba8ce35b0b2700fea`  
		Last Modified: Fri, 11 Nov 2022 05:01:15 GMT  
		Size: 388.1 KB (388070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:737e98adabe276adeb4e37304ee0f535f0a44f377a75e44492d82142d7dcc285`  
		Last Modified: Fri, 11 Nov 2022 05:02:30 GMT  
		Size: 8.3 MB (8342470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d9582513e083aaec608c71ca1cba51db706ce52368d643552f949e1d2e4c635`  
		Last Modified: Fri, 11 Nov 2022 05:02:28 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:453830061328b1835760de2bebcd3d3d979e5a1e5889e6d3e63f6485be901c41`  
		Last Modified: Fri, 11 Nov 2022 05:02:28 GMT  
		Size: 580.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-alpine` - linux; 386

```console
$ docker pull redis@sha256:239263aec1e3f6b540e73b82b0602476fa5c11c2e19c9eb90a3aef5cda6e9c0b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9442901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ee7e6bfd38376e997ae50157593a9396cad01b662173ef9bdcce5e4ab40ed31`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Sat, 12 Nov 2022 03:38:23 GMT
ADD file:561637cbdd23fdd69f555dbc938902d79be2b123eb244d2cfd35b337878b63df in / 
# Sat, 12 Nov 2022 03:38:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 07:02:15 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Sat, 12 Nov 2022 07:02:17 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Sat, 12 Nov 2022 07:05:48 GMT
ENV REDIS_VERSION=5.0.14
# Sat, 12 Nov 2022 07:05:49 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.14.tar.gz
# Sat, 12 Nov 2022 07:05:50 GMT
ENV REDIS_DOWNLOAD_SHA=3ea5024766d983249e80d4aa9457c897a9f079957d0fb1f35682df233f997f32
# Sat, 12 Nov 2022 07:06:31 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Sat, 12 Nov 2022 07:06:32 GMT
RUN mkdir /data && chown redis:redis /data
# Sat, 12 Nov 2022 07:06:33 GMT
VOLUME [/data]
# Sat, 12 Nov 2022 07:06:34 GMT
WORKDIR /data
# Sat, 12 Nov 2022 07:06:36 GMT
COPY file:a9e7249f657e2eec627bb4be492ad18aae3e5e1f0e47d22644eaf1ef2138c0ce in /usr/local/bin/ 
# Sat, 12 Nov 2022 07:06:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 07:06:37 GMT
EXPOSE 6379
# Sat, 12 Nov 2022 07:06:38 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:0c10ccf9426f4a034c81b9e1a0fa81fc5cd957d8a4e0ea545ee33f4cd59f227b`  
		Last Modified: Sat, 12 Nov 2022 03:39:07 GMT  
		Size: 2.8 MB (2808348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78fd914527e66e21c74c8d2a25cfa28f5a4d39243f6d46f20fb778950b1b08f0`  
		Last Modified: Sat, 12 Nov 2022 07:08:27 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0c12a978af39fd1b16ada46c659cb471e1adcc439fdfb7a4aee108a23eb329`  
		Last Modified: Sat, 12 Nov 2022 07:08:27 GMT  
		Size: 394.5 KB (394546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d62a2178d016d49e46ae142ab1febbb077a6b5c25a1b26a911a96cbca3db4d9`  
		Last Modified: Sat, 12 Nov 2022 07:09:53 GMT  
		Size: 6.2 MB (6238091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbd5ca317a33f5b052259c10e30d944d9816bcf0790e160c3a6b51ad3639c7d3`  
		Last Modified: Sat, 12 Nov 2022 07:09:52 GMT  
		Size: 100.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b9082deac8001415a580186c34dcc6911c3c9d230b28c616b20aa46740482cc`  
		Last Modified: Sat, 12 Nov 2022 07:09:52 GMT  
		Size: 575.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-alpine` - linux; ppc64le

```console
$ docker pull redis@sha256:422391984be9f2d302194ef29bbe732a8f5a3bdd7d7f50dae607158b747db96f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.3 MB (10269400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:228905f511d36f59ada3d41eb147c890bb32f069afa8dd2901e576a009d9d225`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 06:53:34 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Fri, 07 Oct 2022 06:53:37 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Fri, 07 Oct 2022 06:57:38 GMT
ENV REDIS_VERSION=5.0.14
# Fri, 07 Oct 2022 06:57:38 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.14.tar.gz
# Fri, 07 Oct 2022 06:57:38 GMT
ENV REDIS_DOWNLOAD_SHA=3ea5024766d983249e80d4aa9457c897a9f079957d0fb1f35682df233f997f32
# Fri, 07 Oct 2022 06:58:29 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 07 Oct 2022 06:58:31 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 07 Oct 2022 06:58:31 GMT
VOLUME [/data]
# Fri, 07 Oct 2022 06:58:31 GMT
WORKDIR /data
# Fri, 07 Oct 2022 06:58:31 GMT
COPY file:a9e7249f657e2eec627bb4be492ad18aae3e5e1f0e47d22644eaf1ef2138c0ce in /usr/local/bin/ 
# Fri, 07 Oct 2022 06:58:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Oct 2022 06:58:32 GMT
EXPOSE 6379
# Fri, 07 Oct 2022 06:58:32 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a40cf9cbcba26de4ca6c60a1af02dfa33aaf568aa79bebaed1e686245b267d4`  
		Last Modified: Fri, 07 Oct 2022 07:00:21 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04762a605fa4de733e39087992868566a08896e7b6956799265cb96da6c75cf5`  
		Last Modified: Fri, 07 Oct 2022 07:00:21 GMT  
		Size: 405.7 KB (405686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd5248cd917ec80a4213bee083c9df2dd76bef1039ff88ab74f7228f97b7eb0d`  
		Last Modified: Fri, 07 Oct 2022 07:01:59 GMT  
		Size: 7.1 MB (7058406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35f26b211dbd64900ebe40ad741a04f857323b2dbc1932fb66c48309f211d8d1`  
		Last Modified: Fri, 07 Oct 2022 07:01:57 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5411051a0ff265ce5d7b7b344433e2ed4d5945230e2aafa49ebc6e385cd65f`  
		Last Modified: Fri, 07 Oct 2022 07:01:57 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-alpine` - linux; s390x

```console
$ docker pull redis@sha256:b6de7f891e40a2dca2f495b08906e48f1b26e56bbc1e438191c52e298db91de7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.8 MB (9755836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:055be5fd09a8c84646408e7378d018e4b544e357ee3858d99c4d646e3adc8b5d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Sat, 12 Nov 2022 03:42:05 GMT
ADD file:b78ae95cbacd853e398f187adaf3be51d9e301a66de8f7a4b6c60a9733075cb5 in / 
# Sat, 12 Nov 2022 03:42:06 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:24:44 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Sat, 12 Nov 2022 08:24:46 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Sat, 12 Nov 2022 08:28:08 GMT
ENV REDIS_VERSION=5.0.14
# Sat, 12 Nov 2022 08:28:08 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.14.tar.gz
# Sat, 12 Nov 2022 08:28:09 GMT
ENV REDIS_DOWNLOAD_SHA=3ea5024766d983249e80d4aa9457c897a9f079957d0fb1f35682df233f997f32
# Sat, 12 Nov 2022 08:28:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Sat, 12 Nov 2022 08:28:47 GMT
RUN mkdir /data && chown redis:redis /data
# Sat, 12 Nov 2022 08:28:47 GMT
VOLUME [/data]
# Sat, 12 Nov 2022 08:28:48 GMT
WORKDIR /data
# Sat, 12 Nov 2022 08:28:48 GMT
COPY file:a9e7249f657e2eec627bb4be492ad18aae3e5e1f0e47d22644eaf1ef2138c0ce in /usr/local/bin/ 
# Sat, 12 Nov 2022 08:28:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Nov 2022 08:28:48 GMT
EXPOSE 6379
# Sat, 12 Nov 2022 08:28:49 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:cff16a5ffe2df97bc1d10b021c5ceb98bdb36a18a1d70395590444ac204a9b2b`  
		Last Modified: Sat, 12 Nov 2022 03:43:06 GMT  
		Size: 2.6 MB (2591126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f0cfe0d0e1cb48d94dd5ea1498fa6d7e94a6b4dbba4ae54ce0bb2ffc82581bf`  
		Last Modified: Sat, 12 Nov 2022 08:30:32 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b6b515bf7b943e6c1d3be874757da2917c30076d122141c0045f3130aacfb23`  
		Last Modified: Sat, 12 Nov 2022 08:30:32 GMT  
		Size: 391.9 KB (391857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c326889bdf9c166bf02ee18497fd52343e368ae5b4167a1527ef1db2a28499a2`  
		Last Modified: Sat, 12 Nov 2022 08:31:32 GMT  
		Size: 6.8 MB (6770871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43df2a1590715bb043771e76ea6cd28ddea0594f641a63aea0a811551b31fada`  
		Last Modified: Sat, 12 Nov 2022 08:31:31 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1fe30388350c924ab38b16bedeec9545ee3c7feaff392cb56b182eb4b9d9a5`  
		Last Modified: Sat, 12 Nov 2022 08:31:31 GMT  
		Size: 578.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
