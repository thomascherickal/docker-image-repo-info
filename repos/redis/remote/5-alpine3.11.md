## `redis:5-alpine3.11`

```console
$ docker pull redis@sha256:49a9889fc47003cc8b8d83bb008dacd3164f6f594caed5e7f1c6829f52c221a8
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

### `redis:5-alpine3.11` - linux; amd64

```console
$ docker pull redis@sha256:94d84454a412602eec64fc538cced0e08fbd5d37b3c99901ac79a13249f6a279
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.4 MB (10370266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8415a41514716648304d6d745ab46646375088770bea264ae4943f09eaaee1f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 04:15:28 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Sat, 18 Jan 2020 04:15:29 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Fri, 13 Mar 2020 20:22:29 GMT
ENV REDIS_VERSION=5.0.8
# Fri, 13 Mar 2020 20:22:29 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.8.tar.gz
# Fri, 13 Mar 2020 20:22:30 GMT
ENV REDIS_DOWNLOAD_SHA=f3c7eac42f433326a8d981b50dba0169fdfaf46abb23fcda2f933a7552ee4ed7
# Fri, 13 Mar 2020 20:23:23 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 13 Mar 2020 20:23:24 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 13 Mar 2020 20:23:24 GMT
VOLUME [/data]
# Fri, 13 Mar 2020 20:23:24 GMT
WORKDIR /data
# Fri, 13 Mar 2020 20:23:24 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 13 Mar 2020 20:23:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Mar 2020 20:23:25 GMT
EXPOSE 6379
# Fri, 13 Mar 2020 20:23:25 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dd5e7a0ba4adb7c7ae1c7d68b7d188015d166d9510d7439fd29ed78bbd95970`  
		Last Modified: Sat, 18 Jan 2020 04:19:10 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e20c1cdf5aefec6df08568a3dd0b1207350b1a877a5d50f494b05195159a82e9`  
		Last Modified: Sat, 18 Jan 2020 04:19:11 GMT  
		Size: 402.6 KB (402564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25131c35a099a911df583e1c31f2e689dea6c7bb4ee54525926ac000f675d20b`  
		Last Modified: Fri, 13 Mar 2020 20:24:16 GMT  
		Size: 7.2 MB (7163001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7c9740b22d5c916309bedc81636263b726294fe118128a4d3bdbba9d5d2331`  
		Last Modified: Fri, 13 Mar 2020 20:24:14 GMT  
		Size: 100.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f86850c30307fc7864c7da0454b16c5edc59f9deb663238cb7ac12a84225ac`  
		Last Modified: Fri, 13 Mar 2020 20:24:14 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-alpine3.11` - linux; arm variant v6

```console
$ docker pull redis@sha256:bee1cfb6e0cdb0521a978a7a4485448a1f4be6d41fd2f53c11e3571cec44dfc4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.1 MB (10100943 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab27ce5d2e1934a5b50384165ab5da2d0ad8cb60e42a483c4ef48ea9a13c76d5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 03:34:20 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Sat, 18 Jan 2020 03:34:23 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Fri, 13 Mar 2020 21:07:05 GMT
ENV REDIS_VERSION=5.0.8
# Fri, 13 Mar 2020 21:07:06 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.8.tar.gz
# Fri, 13 Mar 2020 21:07:07 GMT
ENV REDIS_DOWNLOAD_SHA=f3c7eac42f433326a8d981b50dba0169fdfaf46abb23fcda2f933a7552ee4ed7
# Fri, 13 Mar 2020 21:07:56 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 13 Mar 2020 21:07:58 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 13 Mar 2020 21:07:59 GMT
VOLUME [/data]
# Fri, 13 Mar 2020 21:08:00 GMT
WORKDIR /data
# Fri, 13 Mar 2020 21:08:00 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 13 Mar 2020 21:08:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Mar 2020 21:08:02 GMT
EXPOSE 6379
# Fri, 13 Mar 2020 21:08:02 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:832e07764099264ef96e50a1e5e41c52d6b0809bd054e29508a6878aa59d156d`  
		Last Modified: Sat, 18 Jan 2020 01:53:52 GMT  
		Size: 2.6 MB (2617562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:394e1ba208bc99e98b6e0f1a14d171c251bd7597b9f8d169ad10458d9019829d`  
		Last Modified: Sat, 18 Jan 2020 03:37:48 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c43c4e1907d314e253637bc464a11ab0c74455326617093a1c33bf2b218d2e78`  
		Last Modified: Sat, 18 Jan 2020 03:37:48 GMT  
		Size: 405.8 KB (405799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:868a9df35bc501a8fbb4c64ad8f341e2c25e4a7b994043135514897ff2e01f9f`  
		Last Modified: Fri, 13 Mar 2020 21:08:29 GMT  
		Size: 7.1 MB (7075778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8787ae50e721628d58c4bc199665ea569ebbd7f6c9191232db5f68238980c7c`  
		Last Modified: Fri, 13 Mar 2020 21:08:26 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e802e78c8f5ee6755eed9a62b60249999f0d4123ec94526e89a89ece97779a8`  
		Last Modified: Fri, 13 Mar 2020 21:08:26 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-alpine3.11` - linux; arm variant v7

```console
$ docker pull redis@sha256:953ff08a5bb9fa8b6f16517a7ac9bd8db2107ae162d867dc180bbcaea76bf3a5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9744110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baea0d3d3f4007f39ad78b1dbaa8a66267e7b1d5b9f4dbd3124b6ebddb8edd19`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Sat, 18 Jan 2020 02:03:19 GMT
ADD file:4c815f4461ff3b8d481f43d84eb2548cb1adbb3015d370cab86dd7f4d3d94279 in / 
# Sat, 18 Jan 2020 02:03:22 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 03:21:46 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Sat, 18 Jan 2020 03:21:49 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Fri, 13 Mar 2020 21:36:09 GMT
ENV REDIS_VERSION=5.0.8
# Fri, 13 Mar 2020 21:36:10 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.8.tar.gz
# Fri, 13 Mar 2020 21:36:10 GMT
ENV REDIS_DOWNLOAD_SHA=f3c7eac42f433326a8d981b50dba0169fdfaf46abb23fcda2f933a7552ee4ed7
# Fri, 13 Mar 2020 21:36:55 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 13 Mar 2020 21:36:57 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 13 Mar 2020 21:36:58 GMT
VOLUME [/data]
# Fri, 13 Mar 2020 21:36:58 GMT
WORKDIR /data
# Fri, 13 Mar 2020 21:36:59 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 13 Mar 2020 21:37:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Mar 2020 21:37:00 GMT
EXPOSE 6379
# Fri, 13 Mar 2020 21:37:01 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:3a2c5e3c37b2e3d749405512ef3793aa45a2f5c11615d9e9efa80179262cdf27`  
		Last Modified: Sat, 18 Jan 2020 02:04:05 GMT  
		Size: 2.4 MB (2419554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb4c25ff05240204c1b08c2fc7c9f092608801b1112a5563cc87c094d33b2610`  
		Last Modified: Sat, 18 Jan 2020 03:25:36 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a5180ac18cf5d41359489200210414611b31a360dba3115a321dcb0ee7d036`  
		Last Modified: Sat, 18 Jan 2020 03:25:36 GMT  
		Size: 399.8 KB (399774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a4ebee0300d4999ef78a28f5f56a947664d2bc86e427c2f16b3927e5c5a0026`  
		Last Modified: Fri, 13 Mar 2020 21:38:01 GMT  
		Size: 6.9 MB (6922975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd04793ea0f368c299fc801cf4286ca77ccc77d64aa2742c5cd2268fe159593e`  
		Last Modified: Fri, 13 Mar 2020 21:37:58 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a101b5036d43176b884b562c6cac57a4881094aaf7263e8b490f10928258617c`  
		Last Modified: Fri, 13 Mar 2020 21:37:59 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-alpine3.11` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:d8d5c0a8f203a49162a9c7e4e03607f9f4df34c27979faebb1702c2a67241712
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.3 MB (10307167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe65ba8057a29cb270ba8873eb3dd3d9776699233a446878047bb81ea0b8f7e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 04:33:18 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Sat, 18 Jan 2020 04:33:34 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Fri, 13 Mar 2020 21:06:36 GMT
ENV REDIS_VERSION=5.0.8
# Fri, 13 Mar 2020 21:06:37 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.8.tar.gz
# Fri, 13 Mar 2020 21:06:38 GMT
ENV REDIS_DOWNLOAD_SHA=f3c7eac42f433326a8d981b50dba0169fdfaf46abb23fcda2f933a7552ee4ed7
# Fri, 13 Mar 2020 21:07:26 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 13 Mar 2020 21:07:29 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 13 Mar 2020 21:07:31 GMT
VOLUME [/data]
# Fri, 13 Mar 2020 21:07:32 GMT
WORKDIR /data
# Fri, 13 Mar 2020 21:07:33 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 13 Mar 2020 21:07:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Mar 2020 21:07:35 GMT
EXPOSE 6379
# Fri, 13 Mar 2020 21:07:36 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:8fa90b21c985a6fcfff966bdfbde81cdd088de0aa8af38110057f6ac408f4408`  
		Last Modified: Sat, 18 Jan 2020 01:40:23 GMT  
		Size: 2.7 MB (2723075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b347d21af92f7fa1a81029304142b9a4f1fc27ab54133c379709546365755e28`  
		Last Modified: Sat, 18 Jan 2020 04:40:05 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7efbca486ea0050d3522c6bb7c903b3f18ad83367fca11182ef98e5fe857aa19`  
		Last Modified: Sat, 18 Jan 2020 04:40:04 GMT  
		Size: 404.7 KB (404659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54136fff4b7458384419b68c9d14a7fd1f07ab23b8cd47445af4849a95c80bd9`  
		Last Modified: Fri, 13 Mar 2020 21:08:34 GMT  
		Size: 7.2 MB (7177621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a4aa8bfd10eef359ce9f16a3f50f454b2f8ebf9186405e98144311e6b0712f`  
		Last Modified: Fri, 13 Mar 2020 21:08:31 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72a6b714b65b221bc72f6625343b213f257d5a100cccdea800a12fa94d7cca91`  
		Last Modified: Fri, 13 Mar 2020 21:08:31 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-alpine3.11` - linux; 386

```console
$ docker pull redis@sha256:6e5fc554ce234a2c0058fdb389bd07ce9514493c466fb8d83a6add243f2212fe
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.1 MB (10081613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:397a063d480ebded62e64d66ae10e3d889bd0fc083ab3ede8b6c0c28650993bb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Sat, 18 Jan 2020 01:38:44 GMT
ADD file:381b617b92fe699ad4ef4f30e0d9599f89e43e252883348c420ebe2a0cccbd63 in / 
# Sat, 18 Jan 2020 01:38:45 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 09:47:28 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Sat, 18 Jan 2020 09:47:30 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Fri, 13 Mar 2020 20:54:57 GMT
ENV REDIS_VERSION=5.0.8
# Fri, 13 Mar 2020 20:54:57 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.8.tar.gz
# Fri, 13 Mar 2020 20:54:57 GMT
ENV REDIS_DOWNLOAD_SHA=f3c7eac42f433326a8d981b50dba0169fdfaf46abb23fcda2f933a7552ee4ed7
# Fri, 13 Mar 2020 20:56:03 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 13 Mar 2020 20:56:03 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 13 Mar 2020 20:56:04 GMT
VOLUME [/data]
# Fri, 13 Mar 2020 20:56:04 GMT
WORKDIR /data
# Fri, 13 Mar 2020 20:56:04 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 13 Mar 2020 20:56:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Mar 2020 20:56:04 GMT
EXPOSE 6379
# Fri, 13 Mar 2020 20:56:05 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:f024b1263dc58db07a458b73ae1a2dca02ca55bef1ccd1fa3fd50656551fadf2`  
		Last Modified: Sat, 18 Jan 2020 01:39:18 GMT  
		Size: 2.8 MB (2806560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:919de76a1740b7c09172635adfe651ff8932cc9a10e907fe8c679f339d9d7f55`  
		Last Modified: Sat, 18 Jan 2020 09:51:38 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a79cec79577d23d585483773eb35aca3e0410ef04a2d46a680547bb670056f1`  
		Last Modified: Sat, 18 Jan 2020 09:51:38 GMT  
		Size: 407.9 KB (407903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a416e2442a2b4717c3d1403976e537e03c27b9c2b0fff4d77301111402093af`  
		Last Modified: Fri, 13 Mar 2020 20:56:40 GMT  
		Size: 6.9 MB (6865406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceebe93e821e9dcd147b557e3a7abe52cf28d543dc8a133e86dece53f65bb2d1`  
		Last Modified: Fri, 13 Mar 2020 20:56:39 GMT  
		Size: 100.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca1d43fb7afea342f85b38b7568a3ca6b84c12389d25f944a918398db2a2e972`  
		Last Modified: Fri, 13 Mar 2020 20:56:39 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-alpine3.11` - linux; ppc64le

```console
$ docker pull redis@sha256:edd295969b656b2d772707cf29360f360cdfe4aba0f03ed64e4f3bda22f3e428
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.9 MB (10881804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52069e8a4867da5c4167fa25b532bce6fd00371cf9a7036a2ec1862b5f25e5a4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Sat, 18 Jan 2020 02:20:41 GMT
ADD file:32ddb3d5255071cca51573ceee2464dd5a87c8d1cce514ae965b6e824d9ef24b in / 
# Sat, 18 Jan 2020 02:20:45 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 02:37:15 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Sat, 18 Jan 2020 02:37:22 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Fri, 13 Mar 2020 20:25:21 GMT
ENV REDIS_VERSION=5.0.8
# Fri, 13 Mar 2020 20:25:23 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.8.tar.gz
# Fri, 13 Mar 2020 20:25:27 GMT
ENV REDIS_DOWNLOAD_SHA=f3c7eac42f433326a8d981b50dba0169fdfaf46abb23fcda2f933a7552ee4ed7
# Fri, 13 Mar 2020 20:26:31 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 13 Mar 2020 20:26:51 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 13 Mar 2020 20:26:54 GMT
VOLUME [/data]
# Fri, 13 Mar 2020 20:26:59 GMT
WORKDIR /data
# Fri, 13 Mar 2020 20:27:00 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 13 Mar 2020 20:27:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Mar 2020 20:27:14 GMT
EXPOSE 6379
# Fri, 13 Mar 2020 20:27:20 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:cd95c8a93e39dcaa0634a65d5b86a88bcd5c3092adb1f96504a7030faa165123`  
		Last Modified: Sat, 18 Jan 2020 02:21:25 GMT  
		Size: 2.8 MB (2822125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01d4a026f522563a69e1816b228fd615d5a7657cf58fe1a874fac43b90023819`  
		Last Modified: Sat, 18 Jan 2020 02:42:55 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c965c69e1c9e4a92575fadc54f86389f10a46d5681a5ba6f1401679f22a6288`  
		Last Modified: Sat, 18 Jan 2020 02:42:55 GMT  
		Size: 409.9 KB (409883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16cabc3c9dea69fb1c149d13c6cb2056cc2ca301158d46a534e17d461e0079a6`  
		Last Modified: Fri, 13 Mar 2020 20:28:28 GMT  
		Size: 7.6 MB (7647984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7debcf4202fe534866eef974bd4b79e4923589c510651d2ee6ca7fe94725d8c`  
		Last Modified: Fri, 13 Mar 2020 20:28:27 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247814f7e79c1383d143814d2cfb72f80779f79456172da11f35c4c4ffd25c78`  
		Last Modified: Fri, 13 Mar 2020 20:28:27 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-alpine3.11` - linux; s390x

```console
$ docker pull redis@sha256:2d3796a0748bc691eadb706b7c9d8a149d44cdab3216ab13d095c63f5c5d6db1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.4 MB (10397239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fcc3c7893b9f9b66e45b162ea75c3573d6bb4a54ba6df7afff062698ecefc75`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Sat, 18 Jan 2020 01:41:33 GMT
ADD file:a6f8b7d4ba199527053ef1ac710b5e318135cb6903cb9ad6fae4fe42e6ad0bf7 in / 
# Sat, 18 Jan 2020 01:41:33 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 02:47:20 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Sat, 18 Jan 2020 02:47:21 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Fri, 13 Mar 2020 21:30:57 GMT
ENV REDIS_VERSION=5.0.8
# Fri, 13 Mar 2020 21:30:57 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.8.tar.gz
# Fri, 13 Mar 2020 21:30:58 GMT
ENV REDIS_DOWNLOAD_SHA=f3c7eac42f433326a8d981b50dba0169fdfaf46abb23fcda2f933a7552ee4ed7
# Fri, 13 Mar 2020 21:31:26 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 13 Mar 2020 21:31:27 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 13 Mar 2020 21:31:27 GMT
VOLUME [/data]
# Fri, 13 Mar 2020 21:31:28 GMT
WORKDIR /data
# Fri, 13 Mar 2020 21:31:28 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 13 Mar 2020 21:31:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Mar 2020 21:31:28 GMT
EXPOSE 6379
# Fri, 13 Mar 2020 21:31:28 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:176bad61a3a435da03ec603d2bd8f7a69286d92f21f447b17f21f0bc4e085bde`  
		Last Modified: Sat, 18 Jan 2020 01:41:59 GMT  
		Size: 2.6 MB (2582031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b87866e3e638ab9b00c8dc1f61818c0a0ce018124ee87bc5b563432dbb3ae216`  
		Last Modified: Sat, 18 Jan 2020 02:49:32 GMT  
		Size: 1.2 KB (1235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0904f8797d435556300db89f22f858b75552653853c9f674780fa46054a1a9f`  
		Last Modified: Sat, 18 Jan 2020 02:49:32 GMT  
		Size: 407.4 KB (407362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e933ca8994e9426395a2fd5d2f8191e0792b4afb93e031619fb54efd22a490`  
		Last Modified: Fri, 13 Mar 2020 21:32:16 GMT  
		Size: 7.4 MB (7406062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c85f3bb48ee620c57933e66814f0354706281f0377ad9ba9b32a58217b74a41`  
		Last Modified: Fri, 13 Mar 2020 21:32:20 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ade71db37ca97c5e95783965148be5cdccc051324d5c6e03b265bbfc7fd90ac`  
		Last Modified: Fri, 13 Mar 2020 21:32:30 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
