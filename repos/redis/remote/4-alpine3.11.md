## `redis:4-alpine3.11`

```console
$ docker pull redis@sha256:ea116c3743cd96877e7cee1c0b6ddbf4df9e0abc2f765a378d5adb3116a89c3a
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

### `redis:4-alpine3.11` - linux; amd64

```console
$ docker pull redis@sha256:73c82ede3e0a3786ad0b490a1dc93b38f051d1440c8bb9fe86d1438fbe8e5a5e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.2 MB (9173356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e97349d974ede62c535c4e8bda13df358b94c976cf0462dfb956500e6549f47c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Tue, 24 Dec 2019 19:20:12 GMT
ADD file:36fdc8cb08228a87093fb227736f4ce1d4d6c15366326dea541fbbd863976ee5 in / 
# Tue, 24 Dec 2019 19:20:12 GMT
CMD ["/bin/sh"]
# Tue, 24 Dec 2019 20:14:58 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Tue, 24 Dec 2019 20:15:01 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Tue, 24 Dec 2019 20:19:52 GMT
ENV REDIS_VERSION=4.0.14
# Tue, 24 Dec 2019 20:19:52 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-4.0.14.tar.gz
# Tue, 24 Dec 2019 20:19:53 GMT
ENV REDIS_DOWNLOAD_SHA=1e1e18420a86cfb285933123b04a82e1ebda20bfb0a289472745a087587e93a7
# Fri, 03 Jan 2020 01:33:47 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 03 Jan 2020 01:33:48 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 03 Jan 2020 01:33:48 GMT
VOLUME [/data]
# Fri, 03 Jan 2020 01:33:48 GMT
WORKDIR /data
# Fri, 03 Jan 2020 01:33:48 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 03 Jan 2020 01:33:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Jan 2020 01:33:49 GMT
EXPOSE 6379
# Fri, 03 Jan 2020 01:33:49 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:e6b0cf9c0882fb079c9d35361d12ff4691f916b6d825061247d1bd0b26d7cf3f`  
		Last Modified: Tue, 24 Dec 2019 19:20:40 GMT  
		Size: 2.8 MB (2801778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c5ff11edca67531e0937045954dac7484778b96d3e77f5a0d6056cca7f4ab90`  
		Last Modified: Tue, 24 Dec 2019 20:22:23 GMT  
		Size: 1.2 KB (1225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14fa80ee947360e5477d9d5904bdbce44e47c2f8716d1f87ecc3b7a754071db8`  
		Last Modified: Tue, 24 Dec 2019 20:22:23 GMT  
		Size: 402.6 KB (402555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1e6142008d9a656b24f2280f7646df3b41495b99f213f6fb873913974beef95`  
		Last Modified: Fri, 03 Jan 2020 01:35:48 GMT  
		Size: 6.0 MB (5967286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79ac60f31746bf406e80ac1bced49304049e10c93429501a8c3fc89c1489a552`  
		Last Modified: Fri, 03 Jan 2020 01:35:47 GMT  
		Size: 100.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c823fabb4f303d4d31a0ed3c6fcea243f44dd9e380377d93332aad4e56d0ec3`  
		Last Modified: Fri, 03 Jan 2020 01:35:47 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:4-alpine3.11` - linux; arm variant v6

```console
$ docker pull redis@sha256:ccf7003b14d1249e6eb5489d10a8ea0d8d3d8a3c35424c1315bcfaa785af13b4
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8581864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:662d77118d62ce9fe5c4df2cb6301273c1ab848402856815dd540186bd46464c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Tue, 24 Dec 2019 18:49:41 GMT
ADD file:c4f944e24d0f2e758363506e8b98b3b53973ec18dd4dd23da3f09520ef22c65c in / 
# Tue, 24 Dec 2019 18:49:42 GMT
CMD ["/bin/sh"]
# Tue, 24 Dec 2019 20:06:32 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Tue, 24 Dec 2019 20:06:35 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Tue, 24 Dec 2019 20:09:22 GMT
ENV REDIS_VERSION=4.0.14
# Tue, 24 Dec 2019 20:09:23 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-4.0.14.tar.gz
# Tue, 24 Dec 2019 20:09:24 GMT
ENV REDIS_DOWNLOAD_SHA=1e1e18420a86cfb285933123b04a82e1ebda20bfb0a289472745a087587e93a7
# Fri, 03 Jan 2020 01:58:11 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 03 Jan 2020 01:58:13 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 03 Jan 2020 01:58:14 GMT
VOLUME [/data]
# Fri, 03 Jan 2020 01:58:15 GMT
WORKDIR /data
# Fri, 03 Jan 2020 01:58:15 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 03 Jan 2020 01:58:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Jan 2020 01:58:16 GMT
EXPOSE 6379
# Fri, 03 Jan 2020 01:58:17 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:546eec1e02ac5f4494868d8b22e8ced00773a2fba8e25b3edd30002889874299`  
		Last Modified: Tue, 24 Dec 2019 18:50:07 GMT  
		Size: 2.6 MB (2612021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6690ebdbfaabe4d222e0989fa8663a736e4d4fcb9172c9bfc7ebf5866172bf5a`  
		Last Modified: Tue, 24 Dec 2019 20:10:13 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a8fc7c7c940bf5b9b6c72b079564f927090d1ac1b8c983fc63187cd5a0ee85`  
		Last Modified: Tue, 24 Dec 2019 20:10:13 GMT  
		Size: 405.8 KB (405793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e54db2d3c6cf0e59242648ed81865902edf0f1ee8b619adc39c77375916a842`  
		Last Modified: Fri, 03 Jan 2020 01:59:06 GMT  
		Size: 5.6 MB (5562247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b7c1e0cb2405fe74acad2591c617cf13c511f96287521f46743ad020fc3ea6`  
		Last Modified: Fri, 03 Jan 2020 01:59:05 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7663ecd02996b90a4c028cab9c72e5fc8e4efa3153b1163969283f26f1c5cfae`  
		Last Modified: Fri, 03 Jan 2020 01:59:04 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:4-alpine3.11` - linux; arm variant v7

```console
$ docker pull redis@sha256:ae37b60ea06db0e8d37e2d71462b925ab476b111191fd5fe054060adc84e4cbd
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.2 MB (8230782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e6c60c6f6f64fc2d496c130222e98e91cfdfa8a74fba6701b8baffb6ccdba6d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Tue, 24 Dec 2019 18:59:09 GMT
ADD file:caf7ca25875eddd2bfa2d1e56663bb52d278a85f6ee1314f9ccf01dc4da8070a in / 
# Tue, 24 Dec 2019 18:59:10 GMT
CMD ["/bin/sh"]
# Tue, 24 Dec 2019 20:44:33 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Tue, 24 Dec 2019 20:44:40 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Tue, 24 Dec 2019 20:47:30 GMT
ENV REDIS_VERSION=4.0.14
# Tue, 24 Dec 2019 20:47:30 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-4.0.14.tar.gz
# Tue, 24 Dec 2019 20:47:31 GMT
ENV REDIS_DOWNLOAD_SHA=1e1e18420a86cfb285933123b04a82e1ebda20bfb0a289472745a087587e93a7
# Fri, 03 Jan 2020 01:12:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 03 Jan 2020 01:12:39 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 03 Jan 2020 01:12:40 GMT
VOLUME [/data]
# Fri, 03 Jan 2020 01:12:40 GMT
WORKDIR /data
# Fri, 03 Jan 2020 01:12:41 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 03 Jan 2020 01:12:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Jan 2020 01:12:42 GMT
EXPOSE 6379
# Fri, 03 Jan 2020 01:12:43 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:3922e475e500b2739b5e74787fc80622853325822f71f8bd3de7e5b09654d60f`  
		Last Modified: Tue, 24 Dec 2019 18:59:33 GMT  
		Size: 2.4 MB (2416691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb845f4a68f07a520a518f5d1ffd397679ad8af7fa5e53d0c647f26ad5c9fd02`  
		Last Modified: Tue, 24 Dec 2019 20:48:30 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1df621bbb71ea946244d3e8863368412b46b3e06c4e846a7178fb2b8efb6e17f`  
		Last Modified: Tue, 24 Dec 2019 20:48:30 GMT  
		Size: 399.8 KB (399775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26661058f56ebd9fd81dabfda34f9bd829ab1f6d63ca875bb3b61df7485aec6f`  
		Last Modified: Fri, 03 Jan 2020 01:14:32 GMT  
		Size: 5.4 MB (5412512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2939bab2bbc37ce83dca96b8ca52509bb7252db4f46ffebb62f16de801eb3863`  
		Last Modified: Fri, 03 Jan 2020 01:14:31 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45b3f71b0e039ae09d7020453a91c33633a2a89e1d8bd4bc66dea3a7f8e70e1`  
		Last Modified: Fri, 03 Jan 2020 01:14:30 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:4-alpine3.11` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:de847947793f777e43f6649037fb35420a39e7a98bc2e8589645b6f52132666f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.9 MB (8887855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3eb9a713f9525fbc82ae071f1ee94590239c7325806fb9973a5b7a48adbd058`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Tue, 24 Dec 2019 20:26:15 GMT
ADD file:d6c3db0313ab0c6201770c7248d1bac964011a1c08f1a9b434442b7c21efef87 in / 
# Tue, 24 Dec 2019 20:26:24 GMT
CMD ["/bin/sh"]
# Tue, 24 Dec 2019 21:36:53 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Tue, 24 Dec 2019 21:36:55 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Tue, 24 Dec 2019 21:39:12 GMT
ENV REDIS_VERSION=4.0.14
# Tue, 24 Dec 2019 21:39:13 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-4.0.14.tar.gz
# Tue, 24 Dec 2019 21:39:14 GMT
ENV REDIS_DOWNLOAD_SHA=1e1e18420a86cfb285933123b04a82e1ebda20bfb0a289472745a087587e93a7
# Fri, 03 Jan 2020 01:57:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 03 Jan 2020 01:57:14 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 03 Jan 2020 01:57:15 GMT
VOLUME [/data]
# Fri, 03 Jan 2020 01:57:15 GMT
WORKDIR /data
# Fri, 03 Jan 2020 01:57:16 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 03 Jan 2020 01:57:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Jan 2020 01:57:18 GMT
EXPOSE 6379
# Fri, 03 Jan 2020 01:57:18 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:cde5963f3b93eec667cad527c99d80402a5a91a7a1381f7ffe562f215aec0c50`  
		Last Modified: Tue, 24 Dec 2019 20:26:52 GMT  
		Size: 2.7 MB (2719182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91e5527b2c4228c8cae1dea3684631a5b3320e665960c29c0aa4a5fce854198c`  
		Last Modified: Tue, 24 Dec 2019 21:40:08 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b34c2c544f18db3904a205c7d612b06f7cb3618ae089403278b5a5edcfade03`  
		Last Modified: Tue, 24 Dec 2019 21:40:08 GMT  
		Size: 404.7 KB (404658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ff8f65d6c2cc279f96e3966fac0d1562b810e3557e936b09bfbb3db48743a79`  
		Last Modified: Fri, 03 Jan 2020 01:59:13 GMT  
		Size: 5.8 MB (5762211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfa2800fdf843ec090fc809aba9c9bb4ff77508e6fa518b7a1ab76e11ebecab9`  
		Last Modified: Fri, 03 Jan 2020 01:59:11 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c02cd5cda9e3b2c0551dda95aee9dcd18702362d1931c8f574bf821db0082fa7`  
		Last Modified: Fri, 03 Jan 2020 01:59:11 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:4-alpine3.11` - linux; 386

```console
$ docker pull redis@sha256:1e2f827b51e674cad405b2b9ab81f14e1919a46ebdbca17d6ec5266ad1777b5d
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.9 MB (8943648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1d080933ce61dc9c694e2421bbf2418e063b1aa987b60bf7d9ab5f9f8b0c1df`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Tue, 24 Dec 2019 19:38:57 GMT
ADD file:d0127a9692e8445993a88163cb741dbb23fa25436dd65289e76b08484264b397 in / 
# Tue, 24 Dec 2019 19:38:57 GMT
CMD ["/bin/sh"]
# Tue, 24 Dec 2019 22:37:05 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Tue, 24 Dec 2019 22:37:07 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Tue, 24 Dec 2019 22:39:56 GMT
ENV REDIS_VERSION=4.0.14
# Tue, 24 Dec 2019 22:39:56 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-4.0.14.tar.gz
# Tue, 24 Dec 2019 22:39:56 GMT
ENV REDIS_DOWNLOAD_SHA=1e1e18420a86cfb285933123b04a82e1ebda20bfb0a289472745a087587e93a7
# Fri, 03 Jan 2020 01:51:39 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 03 Jan 2020 01:51:39 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 03 Jan 2020 01:51:40 GMT
VOLUME [/data]
# Fri, 03 Jan 2020 01:51:40 GMT
WORKDIR /data
# Fri, 03 Jan 2020 01:51:40 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 03 Jan 2020 01:51:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Jan 2020 01:51:40 GMT
EXPOSE 6379
# Fri, 03 Jan 2020 01:51:41 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:57bbc6f150623b3e4f01930af4ab2efa6ed5df02319341a08b1ce0bbd7e4afdf`  
		Last Modified: Tue, 24 Dec 2019 19:39:19 GMT  
		Size: 2.8 MB (2805146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89cbe0acfe3faf3101d7c8daddebef28303450f801a706b4b586db7490b2c11a`  
		Last Modified: Tue, 24 Dec 2019 22:41:04 GMT  
		Size: 1.2 KB (1229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2a90697d0698d45923f3cd38872000eaf66147ef07aaf2766fe4e1982b4912`  
		Last Modified: Tue, 24 Dec 2019 22:41:04 GMT  
		Size: 407.9 KB (407911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a45618e4558513d188bbfcb28bd6d00f4ecb360b5aed8ba9f97886161fda28af`  
		Last Modified: Fri, 03 Jan 2020 01:52:53 GMT  
		Size: 5.7 MB (5728850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d8492bacd0df05ebaf1ba205be8abc839f98dc71bc57cb5c253e4c2149ea66a`  
		Last Modified: Fri, 03 Jan 2020 01:52:52 GMT  
		Size: 100.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a889914eee9f26b98b11a0550a8a3e45ba6606e3378ed3365f232509c1d7d06f`  
		Last Modified: Fri, 03 Jan 2020 01:52:52 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:4-alpine3.11` - linux; ppc64le

```console
$ docker pull redis@sha256:2e3feccd82de97e0916d72016af599c66277c3cf50a148f551ddc2b224a56309
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9323245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:980d93c59feb966941360d8489160e9600c7e25261ed1fbbe4da06e9c4f01c1c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Tue, 24 Dec 2019 19:28:37 GMT
ADD file:4d85451a651e236d899cd849617594eb6babf24079f9b2269134ad06d89bdecc in / 
# Tue, 24 Dec 2019 19:28:38 GMT
CMD ["/bin/sh"]
# Tue, 24 Dec 2019 20:30:45 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Tue, 24 Dec 2019 20:30:57 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Tue, 24 Dec 2019 20:35:21 GMT
ENV REDIS_VERSION=4.0.14
# Tue, 24 Dec 2019 20:35:25 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-4.0.14.tar.gz
# Tue, 24 Dec 2019 20:35:29 GMT
ENV REDIS_DOWNLOAD_SHA=1e1e18420a86cfb285933123b04a82e1ebda20bfb0a289472745a087587e93a7
# Fri, 03 Jan 2020 01:35:22 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 03 Jan 2020 01:35:27 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 03 Jan 2020 01:35:29 GMT
VOLUME [/data]
# Fri, 03 Jan 2020 01:35:32 GMT
WORKDIR /data
# Fri, 03 Jan 2020 01:35:36 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 03 Jan 2020 01:35:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Jan 2020 01:35:44 GMT
EXPOSE 6379
# Fri, 03 Jan 2020 01:35:47 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:a5dee701e1e87430161d8fce67e77ee5e132bdbafe165c52490a36df654c7660`  
		Last Modified: Tue, 24 Dec 2019 19:29:09 GMT  
		Size: 2.8 MB (2816482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec98a815652651227cde929032b86b4e74b97f25c96435f5f938a388ea821608`  
		Last Modified: Tue, 24 Dec 2019 20:38:02 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d541bbafc448828f3fe8671379551e915de8ee4752aea51ff6b90b6a89a59e5d`  
		Last Modified: Tue, 24 Dec 2019 20:38:03 GMT  
		Size: 409.9 KB (409873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b33af92554dff2b2eb3c572203fe88854b61275f78966305686fb28eac0c18`  
		Last Modified: Fri, 03 Jan 2020 01:38:42 GMT  
		Size: 6.1 MB (6095081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6f0c3e283e9bf9c21ea9958c67fe42872331359d45d7e1e33abbef37439b09`  
		Last Modified: Fri, 03 Jan 2020 01:38:39 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55609ecb167445dd150dd5fed1b832ecdd89dcc0c259eea13487dd97eab2b589`  
		Last Modified: Fri, 03 Jan 2020 01:38:39 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:4-alpine3.11` - linux; s390x

```console
$ docker pull redis@sha256:6654ab227c8ff3056e8e2d442a24a5ec23ac885b6a64d2f62f1d2b0c20225f4f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8755303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92fef3e6a1e6e3da67d4ba8694d6316b959a8c72a82b4c190a42bcf14fdec827`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Tue, 24 Dec 2019 20:16:56 GMT
ADD file:d26fbcd308b78da175af74382b16ee1f7a3370ab9d618b306d604d292e72c560 in / 
# Tue, 24 Dec 2019 20:16:56 GMT
CMD ["/bin/sh"]
# Tue, 24 Dec 2019 20:40:18 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Tue, 24 Dec 2019 20:40:19 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Tue, 24 Dec 2019 20:41:43 GMT
ENV REDIS_VERSION=4.0.14
# Tue, 24 Dec 2019 20:41:43 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-4.0.14.tar.gz
# Tue, 24 Dec 2019 20:41:43 GMT
ENV REDIS_DOWNLOAD_SHA=1e1e18420a86cfb285933123b04a82e1ebda20bfb0a289472745a087587e93a7
# Fri, 03 Jan 2020 01:56:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 03 Jan 2020 01:56:29 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 03 Jan 2020 01:56:29 GMT
VOLUME [/data]
# Fri, 03 Jan 2020 01:56:29 GMT
WORKDIR /data
# Fri, 03 Jan 2020 01:56:30 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 03 Jan 2020 01:56:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 03 Jan 2020 01:56:30 GMT
EXPOSE 6379
# Fri, 03 Jan 2020 01:56:30 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:bca389ebb9be8103bf737251d68f962104771b2f9c1fff1f7ae0207458fa4c86`  
		Last Modified: Tue, 24 Dec 2019 20:17:18 GMT  
		Size: 2.6 MB (2579591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e07ee4313a681359a7a34cb7e38cf1ab1203a05bdb0c31199de86bb63c77e2`  
		Last Modified: Tue, 24 Dec 2019 20:42:18 GMT  
		Size: 1.2 KB (1229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea8e178bc6600fcf408e03744a3727dde9be59c3b4cc3b212a2f8562dd20259d`  
		Last Modified: Tue, 24 Dec 2019 20:42:18 GMT  
		Size: 407.4 KB (407361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac617499b65e0320f8848e185d33fafd1d86dc6738bee875f3e9820055b7ed10`  
		Last Modified: Fri, 03 Jan 2020 01:57:38 GMT  
		Size: 5.8 MB (5766609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c78892fa19566b1d85e59986e52172b6c29ccf50c4b83d9c80288cb967b72cb7`  
		Last Modified: Fri, 03 Jan 2020 01:57:37 GMT  
		Size: 100.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c917d2bc1064d2572fd6b1f9f68e1f359ad2168a2440a7757678d65ae7ad21b9`  
		Last Modified: Fri, 03 Jan 2020 01:57:36 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
