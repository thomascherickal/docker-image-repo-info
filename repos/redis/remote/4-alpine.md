## `redis:4-alpine`

```console
$ docker pull redis@sha256:0103d97c355ca11341618d3dd5a450bba2f4603be4ffea321abe5d38376a8e07
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

### `redis:4-alpine` - linux; amd64

```console
$ docker pull redis@sha256:db4a5cfb5fe5ef2ce941a1fef14442b9eaa44033170f9c575b9eb555b99a899f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7708901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1191e27509ec13c94162e68cd45af10fa33bd64bdc07649e447d9b6bd186768d`
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
# Sat, 18 Jan 2020 04:18:00 GMT
ENV REDIS_VERSION=4.0.14
# Sat, 18 Jan 2020 04:18:00 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-4.0.14.tar.gz
# Sat, 18 Jan 2020 04:18:01 GMT
ENV REDIS_DOWNLOAD_SHA=1e1e18420a86cfb285933123b04a82e1ebda20bfb0a289472745a087587e93a7
# Sat, 18 Jan 2020 04:18:30 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Sat, 18 Jan 2020 04:18:30 GMT
RUN mkdir /data && chown redis:redis /data
# Sat, 18 Jan 2020 04:18:31 GMT
VOLUME [/data]
# Sat, 18 Jan 2020 04:18:31 GMT
WORKDIR /data
# Sat, 18 Jan 2020 04:18:31 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Sat, 18 Jan 2020 04:18:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 04:18:31 GMT
EXPOSE 6379
# Sat, 18 Jan 2020 04:18:31 GMT
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
	-	`sha256:ec5dd1f9ae1c236f9736ce95fc294687d180ba211fb9e0c745a57c03d28577d2`  
		Last Modified: Sat, 18 Jan 2020 04:19:35 GMT  
		Size: 4.5 MB (4501637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5d9202626639f82a2e086e3cef6608e055b29ffaa80cd0ff7ed4068f7146351`  
		Last Modified: Sat, 18 Jan 2020 04:19:34 GMT  
		Size: 99.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ce699e4a1c76289bd8b45c8be37078f722d5a2901ffc01c770be37d154a47c`  
		Last Modified: Sat, 18 Jan 2020 04:19:34 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:4-alpine` - linux; arm variant v6

```console
$ docker pull redis@sha256:1d096739b8d820b46f534227a34dcbf753a3d45e5c3b89cc8f26c02c95398835
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.4 MB (7355932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef44ccc9f6bcf851b4c9fc7153ee28b4504ff158b3366adb0432f3622d1b9bfb`
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
# Sat, 18 Jan 2020 03:36:43 GMT
ENV REDIS_VERSION=4.0.14
# Sat, 18 Jan 2020 03:36:44 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-4.0.14.tar.gz
# Sat, 18 Jan 2020 03:36:47 GMT
ENV REDIS_DOWNLOAD_SHA=1e1e18420a86cfb285933123b04a82e1ebda20bfb0a289472745a087587e93a7
# Sat, 18 Jan 2020 03:37:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Sat, 18 Jan 2020 03:37:19 GMT
RUN mkdir /data && chown redis:redis /data
# Sat, 18 Jan 2020 03:37:20 GMT
VOLUME [/data]
# Sat, 18 Jan 2020 03:37:21 GMT
WORKDIR /data
# Sat, 18 Jan 2020 03:37:21 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Sat, 18 Jan 2020 03:37:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 03:37:23 GMT
EXPOSE 6379
# Sat, 18 Jan 2020 03:37:24 GMT
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
	-	`sha256:42121219bc4df6e10bcbfc347ea1be88c94d8363a9763a77464533912b69c515`  
		Last Modified: Sat, 18 Jan 2020 03:38:18 GMT  
		Size: 4.3 MB (4330768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3db2867f0889d58d2f0d371a12af2805fdbde73edc49f214e9c917550185e7a`  
		Last Modified: Sat, 18 Jan 2020 03:38:18 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5089b74c426466629256b2ea4ba251ca38421b5704a3fccda04117a1cd8ed62a`  
		Last Modified: Sat, 18 Jan 2020 03:38:18 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:4-alpine` - linux; arm variant v7

```console
$ docker pull redis@sha256:5fd80f1b1e3318b335f8c26d14167a6a427680a6fb54d02fee83357e022d848c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7075755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e252e30f48bb89ad7251386577b565595d5f7a726cbb22a6a2f5e7cc7c5c7142`
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
# Sat, 18 Jan 2020 03:24:30 GMT
ENV REDIS_VERSION=4.0.14
# Sat, 18 Jan 2020 03:24:32 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-4.0.14.tar.gz
# Sat, 18 Jan 2020 03:24:33 GMT
ENV REDIS_DOWNLOAD_SHA=1e1e18420a86cfb285933123b04a82e1ebda20bfb0a289472745a087587e93a7
# Sat, 18 Jan 2020 03:24:59 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Sat, 18 Jan 2020 03:25:01 GMT
RUN mkdir /data && chown redis:redis /data
# Sat, 18 Jan 2020 03:25:01 GMT
VOLUME [/data]
# Sat, 18 Jan 2020 03:25:02 GMT
WORKDIR /data
# Sat, 18 Jan 2020 03:25:03 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Sat, 18 Jan 2020 03:25:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 03:25:06 GMT
EXPOSE 6379
# Sat, 18 Jan 2020 03:25:08 GMT
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
	-	`sha256:b5e4b546a93e27d4979da603e6d95a54e31617ea5e95b9bc0fe587d8868b194a`  
		Last Modified: Sat, 18 Jan 2020 03:26:08 GMT  
		Size: 4.3 MB (4254620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f30c53192f2cb882e729ca8c7c06e1f79f5942cd02d1584074c1b6f46cb9692e`  
		Last Modified: Sat, 18 Jan 2020 03:26:07 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da0b075b8585d5730753c166fdf30c8dcc32cec06d3f3578c407fce379b9188`  
		Last Modified: Sat, 18 Jan 2020 03:26:07 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:4-alpine` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:bda7253a930cdd1fe330248c3087e698be5df500fcd60da39124ccc7ac83da29
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7532308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a89386f34b387f55ff56f491e86b3dfd8a95ce38a3dfee5fa7befb5cc9888264`
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
# Sat, 18 Jan 2020 04:38:10 GMT
ENV REDIS_VERSION=4.0.14
# Sat, 18 Jan 2020 04:38:13 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-4.0.14.tar.gz
# Sat, 18 Jan 2020 04:38:16 GMT
ENV REDIS_DOWNLOAD_SHA=1e1e18420a86cfb285933123b04a82e1ebda20bfb0a289472745a087587e93a7
# Sat, 18 Jan 2020 04:38:53 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Sat, 18 Jan 2020 04:39:04 GMT
RUN mkdir /data && chown redis:redis /data
# Sat, 18 Jan 2020 04:39:06 GMT
VOLUME [/data]
# Sat, 18 Jan 2020 04:39:09 GMT
WORKDIR /data
# Sat, 18 Jan 2020 04:39:12 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Sat, 18 Jan 2020 04:39:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 04:39:17 GMT
EXPOSE 6379
# Sat, 18 Jan 2020 04:39:21 GMT
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
	-	`sha256:f09b08b3808f3733a779a373e464c8e3853f0efb32caa8ebcaa41eaffa2288c6`  
		Last Modified: Sat, 18 Jan 2020 04:40:44 GMT  
		Size: 4.4 MB (4402766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0538450caa005c461bbb8408e2681c043ffd3bc52366b05640c794f8cd97a440`  
		Last Modified: Sat, 18 Jan 2020 04:40:43 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee944227d3696243130b8177067e9260ed57ea57185700f08daa67bb05401c0f`  
		Last Modified: Sat, 18 Jan 2020 04:40:43 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:4-alpine` - linux; 386

```console
$ docker pull redis@sha256:31ea21f88df58204d683b763c96ef808bde59f272f2cca7685c9399323af8843
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.5 MB (7475340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:793e76b0aec2e27981933c4245737c9064e9a43fa974c7ac60aef07ee1467958`
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
# Sat, 18 Jan 2020 09:50:19 GMT
ENV REDIS_VERSION=4.0.14
# Sat, 18 Jan 2020 09:50:19 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-4.0.14.tar.gz
# Sat, 18 Jan 2020 09:50:19 GMT
ENV REDIS_DOWNLOAD_SHA=1e1e18420a86cfb285933123b04a82e1ebda20bfb0a289472745a087587e93a7
# Sat, 18 Jan 2020 09:50:54 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Sat, 18 Jan 2020 09:50:55 GMT
RUN mkdir /data && chown redis:redis /data
# Sat, 18 Jan 2020 09:50:55 GMT
VOLUME [/data]
# Sat, 18 Jan 2020 09:50:55 GMT
WORKDIR /data
# Sat, 18 Jan 2020 09:50:55 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Sat, 18 Jan 2020 09:50:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 09:50:56 GMT
EXPOSE 6379
# Sat, 18 Jan 2020 09:50:56 GMT
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
	-	`sha256:ae839848a00534273983a88073a89529987f3f4ebf6bc6db730617f925d0146b`  
		Last Modified: Sat, 18 Jan 2020 09:51:58 GMT  
		Size: 4.3 MB (4259136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a531c21b8f559f4e312dcf2bf61e09be3f4cc8ad4f202fb6daee28dec70561`  
		Last Modified: Sat, 18 Jan 2020 09:51:57 GMT  
		Size: 99.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e30bc35953c321c605c675eedad6e76f0dc61a4737ed12a606330a3c195f11f`  
		Last Modified: Sat, 18 Jan 2020 09:51:57 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:4-alpine` - linux; ppc64le

```console
$ docker pull redis@sha256:b7cd99c8a26e897f9254b041223fcbdfe7f00f603cba0bb95c8100a6018823aa
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.9 MB (7916927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c48b76389ea6d913fd75c1da7d297e38ca4c03450c3e81062e8c3aa7ca42cda`
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
# Sat, 18 Jan 2020 02:41:01 GMT
ENV REDIS_VERSION=4.0.14
# Sat, 18 Jan 2020 02:41:04 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-4.0.14.tar.gz
# Sat, 18 Jan 2020 02:41:06 GMT
ENV REDIS_DOWNLOAD_SHA=1e1e18420a86cfb285933123b04a82e1ebda20bfb0a289472745a087587e93a7
# Sat, 18 Jan 2020 02:41:35 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Sat, 18 Jan 2020 02:41:42 GMT
RUN mkdir /data && chown redis:redis /data
# Sat, 18 Jan 2020 02:41:45 GMT
VOLUME [/data]
# Sat, 18 Jan 2020 02:41:48 GMT
WORKDIR /data
# Sat, 18 Jan 2020 02:41:49 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Sat, 18 Jan 2020 02:41:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 02:41:52 GMT
EXPOSE 6379
# Sat, 18 Jan 2020 02:41:54 GMT
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
	-	`sha256:22a7ad6d80a9e4e7013f2ce702c43f70da36d87033d42d7092bdd05a7f2f5604`  
		Last Modified: Sat, 18 Jan 2020 02:43:52 GMT  
		Size: 4.7 MB (4683109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e48ca63908c23d082bd156d611d64a52dbf985f78a479b1050da3e9ef380bafa`  
		Last Modified: Sat, 18 Jan 2020 02:43:51 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83865f79075ad408f148278569c59a787682763e4dabfc23e061bbbd2a09a51f`  
		Last Modified: Sat, 18 Jan 2020 02:43:51 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:4-alpine` - linux; s390x

```console
$ docker pull redis@sha256:40ee192e1556502d51508aa7bd25ac844747df278116216825886f888945fcac
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.6 MB (7555914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:475a274acc6eb04786c9cf3cd515ac87e5cf41c67ca0fb0cad07997a9da7354a`
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
# Sat, 18 Jan 2020 02:48:45 GMT
ENV REDIS_VERSION=4.0.14
# Sat, 18 Jan 2020 02:48:45 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-4.0.14.tar.gz
# Sat, 18 Jan 2020 02:48:45 GMT
ENV REDIS_DOWNLOAD_SHA=1e1e18420a86cfb285933123b04a82e1ebda20bfb0a289472745a087587e93a7
# Sat, 18 Jan 2020 02:49:07 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Sat, 18 Jan 2020 02:49:08 GMT
RUN mkdir /data && chown redis:redis /data
# Sat, 18 Jan 2020 02:49:08 GMT
VOLUME [/data]
# Sat, 18 Jan 2020 02:49:09 GMT
WORKDIR /data
# Sat, 18 Jan 2020 02:49:09 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Sat, 18 Jan 2020 02:49:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 02:49:09 GMT
EXPOSE 6379
# Sat, 18 Jan 2020 02:49:10 GMT
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
	-	`sha256:1bcc501a902e4194a070e393969f34627ba39b17fb49fb97ed26896b73176c1c`  
		Last Modified: Sat, 18 Jan 2020 02:49:54 GMT  
		Size: 4.6 MB (4564776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf4fc08c11ac1acfa7406c896658961cb088b31214a6285b3b51860cb0e79a1`  
		Last Modified: Sat, 18 Jan 2020 02:49:54 GMT  
		Size: 99.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc6c6ec6b77b54d4f5c7ec743b6fe408e2ad9a7a37635accbca5a595c61e1e84`  
		Last Modified: Sat, 18 Jan 2020 02:49:54 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
