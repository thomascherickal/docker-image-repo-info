## `redis:6-alpine`

```console
$ docker pull redis@sha256:909f81a3fb693e573cc8fdacc7bdb6c0fe40453126dd7cc28d6e773f7ee1cd62
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

### `redis:6-alpine` - linux; amd64

```console
$ docker pull redis@sha256:b84722fc8ed090f27b5e10274643d6f2ffc933c3f393ef744a52cc82d222cd1b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.6 MB (10605278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7277f03c430ea261baacd5b7acf3ea5de63f18873ad297d21f211b16f7162c23`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 19:19:42 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Fri, 24 Apr 2020 19:19:43 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Thu, 30 Apr 2020 19:37:50 GMT
ENV REDIS_VERSION=6.0.0
# Thu, 30 Apr 2020 19:37:50 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.0.tar.gz
# Thu, 30 Apr 2020 19:37:51 GMT
ENV REDIS_DOWNLOAD_SHA=16d13ec1c3255206deb4818ed444dca6dda1482b551736f0033253c211b788fc
# Thu, 30 Apr 2020 19:38:54 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Thu, 30 Apr 2020 19:38:54 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 30 Apr 2020 19:38:55 GMT
VOLUME [/data]
# Thu, 30 Apr 2020 19:38:55 GMT
WORKDIR /data
# Thu, 30 Apr 2020 19:38:55 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Thu, 30 Apr 2020 19:38:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Apr 2020 19:38:55 GMT
EXPOSE 6379
# Thu, 30 Apr 2020 19:38:56 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0373118a0d956ca0ee963e307457f45f073db9096f7c6f87c10251d071f0dc`  
		Last Modified: Fri, 24 Apr 2020 19:23:01 GMT  
		Size: 1.2 KB (1228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd369fe62565d644723bfdb734c4ecb2a96191366ec08424146aa9c5ff6b308`  
		Last Modified: Fri, 24 Apr 2020 19:23:02 GMT  
		Size: 402.6 KB (402568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db420843220f2ee6e3f050303ae5ab952c9453b6447228520e61ff61cd36edc6`  
		Last Modified: Thu, 30 Apr 2020 19:39:54 GMT  
		Size: 7.4 MB (7387653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02ac182be132e4b92684f4b88a18fc23e77a5f25455e0ab1af7c40462124bd6a`  
		Last Modified: Thu, 30 Apr 2020 19:39:47 GMT  
		Size: 100.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c5d252a4e797ebfb8b58c74f1bfcac29f4be85d8426fa0e6250807fe492e2c`  
		Last Modified: Thu, 30 Apr 2020 19:39:48 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine` - linux; arm variant v6

```console
$ docker pull redis@sha256:dc19e61b489399b96e94a6bbb868084fca25f474444f4b119f9b7c06041f5359
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.3 MB (10303396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adcd136038983b0d979d4fc8986ca79f7b04b1c75161be2fcfae69edab0af583`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 22:30:17 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Thu, 23 Apr 2020 22:30:20 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Thu, 30 Apr 2020 19:52:31 GMT
ENV REDIS_VERSION=6.0.0
# Thu, 30 Apr 2020 19:52:32 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.0.tar.gz
# Thu, 30 Apr 2020 19:52:33 GMT
ENV REDIS_DOWNLOAD_SHA=16d13ec1c3255206deb4818ed444dca6dda1482b551736f0033253c211b788fc
# Thu, 30 Apr 2020 19:53:41 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Thu, 30 Apr 2020 19:53:43 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 30 Apr 2020 19:53:44 GMT
VOLUME [/data]
# Thu, 30 Apr 2020 19:53:45 GMT
WORKDIR /data
# Thu, 30 Apr 2020 19:53:46 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Thu, 30 Apr 2020 19:53:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Apr 2020 19:53:47 GMT
EXPOSE 6379
# Thu, 30 Apr 2020 19:53:48 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ab5b04292d1974b3feedf74dddf563efe3ba5b5c38239a49e8adf0ac8140028`  
		Last Modified: Thu, 23 Apr 2020 22:33:41 GMT  
		Size: 1.3 KB (1253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af20f6a7bee5bf869254b4964c1a5d8dd5ef1353ac48081a885920682312555b`  
		Last Modified: Thu, 23 Apr 2020 22:33:41 GMT  
		Size: 405.8 KB (405799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7aece9b388f0488b21c04faa7be2a694b39f9067ef84b22d647a366a564d1b1`  
		Last Modified: Thu, 30 Apr 2020 19:54:23 GMT  
		Size: 7.3 MB (7275856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5167bae2551e025e3ec1fcb42d5d84a935da873e00f1eeab01183d4d1c928b9c`  
		Last Modified: Thu, 30 Apr 2020 19:54:17 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bdc323153e9a953c0956c82707f8db8af2cfc672ccd9db16ae3379b9703f176`  
		Last Modified: Thu, 30 Apr 2020 19:54:16 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine` - linux; arm variant v7

```console
$ docker pull redis@sha256:c0e44900acca77bbb599400e9b61f331db1b1dd899cab5de4cc933815255b04d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (9964701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed288e3ff72f1b0e810e30e15dcda2c7c4d2f4fc43be33e003bb3b575d80ee56`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 08:51:32 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Fri, 24 Apr 2020 08:51:36 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Thu, 30 Apr 2020 19:59:31 GMT
ENV REDIS_VERSION=6.0.0
# Thu, 30 Apr 2020 19:59:32 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.0.tar.gz
# Thu, 30 Apr 2020 19:59:33 GMT
ENV REDIS_DOWNLOAD_SHA=16d13ec1c3255206deb4818ed444dca6dda1482b551736f0033253c211b788fc
# Thu, 30 Apr 2020 20:00:18 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Thu, 30 Apr 2020 20:00:20 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 30 Apr 2020 20:00:21 GMT
VOLUME [/data]
# Thu, 30 Apr 2020 20:00:21 GMT
WORKDIR /data
# Thu, 30 Apr 2020 20:00:22 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Thu, 30 Apr 2020 20:00:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Apr 2020 20:00:23 GMT
EXPOSE 6379
# Thu, 30 Apr 2020 20:00:24 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0765e03c998449baf4c76a1011cf80e6ab974db3d5d8da3a361bfeeb875d96db`  
		Last Modified: Fri, 24 Apr 2020 08:55:16 GMT  
		Size: 1.3 KB (1254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc07fda5f4761823162fa661b4466f517ad5db025d9689c123221af67af9b53f`  
		Last Modified: Fri, 24 Apr 2020 08:55:16 GMT  
		Size: 399.8 KB (399779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:804e7af86c644d01f828ea49faddc66e7f2f53c27b9da50e77c95c4e8f1d4db9`  
		Last Modified: Thu, 30 Apr 2020 20:01:20 GMT  
		Size: 7.1 MB (7141056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98393a0ade1f39968fa4e054af8f2fda561ca07cd3e0af63e35f5b98e2b4b8d0`  
		Last Modified: Thu, 30 Apr 2020 20:01:18 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb5a20026dedfebefe5a9fda644ea41518462ebd300c93589c9405f02dfdc82e`  
		Last Modified: Thu, 30 Apr 2020 20:01:18 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:7407bb814866f3f85372dc1d36d9889cc23ca037697ed83bb8bd194954323784
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.5 MB (10510899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4af9d52e61b4cbb955a444ba03fcace7107c89aa00b961512bb65bc689223ff9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 12:45:10 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Fri, 24 Apr 2020 12:45:13 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Thu, 30 Apr 2020 19:50:08 GMT
ENV REDIS_VERSION=6.0.0
# Thu, 30 Apr 2020 19:50:09 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.0.tar.gz
# Thu, 30 Apr 2020 19:50:10 GMT
ENV REDIS_DOWNLOAD_SHA=16d13ec1c3255206deb4818ed444dca6dda1482b551736f0033253c211b788fc
# Thu, 30 Apr 2020 19:51:03 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Thu, 30 Apr 2020 19:51:06 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 30 Apr 2020 19:51:07 GMT
VOLUME [/data]
# Thu, 30 Apr 2020 19:51:08 GMT
WORKDIR /data
# Thu, 30 Apr 2020 19:51:08 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Thu, 30 Apr 2020 19:51:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Apr 2020 19:51:10 GMT
EXPOSE 6379
# Thu, 30 Apr 2020 19:51:10 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c7050d23898adae8e4a2e0ab67eaeab9f9a9ec0fa5b88b128eeff4de1570877`  
		Last Modified: Fri, 24 Apr 2020 12:48:50 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8982b178d819b1f2f10c3375b2c7ed054157cc5e711b58b6a2dcb376686e5d59`  
		Last Modified: Fri, 24 Apr 2020 12:48:50 GMT  
		Size: 404.7 KB (404661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68596a0ebf7ed7e6291ce88cb56b332f4f2b56319b9885dbc430d46ca089543e`  
		Last Modified: Thu, 30 Apr 2020 19:52:29 GMT  
		Size: 7.4 MB (7380008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3885b24cd247fd11eb7ee548337b37aa7abe67a747d4cf2e15c4720d9d43daa2`  
		Last Modified: Thu, 30 Apr 2020 19:52:23 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:476e538110ba6b162e72d775274dcab72c952c9f3d96f6c629a3fd3fc06c6fea`  
		Last Modified: Thu, 30 Apr 2020 19:52:24 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine` - linux; 386

```console
$ docker pull redis@sha256:0b387c6c8a1689f6e42472c54008c8e94148401222a97e4d3cd1bd01e2db08ff
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.3 MB (10284995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5baf2c4f6efd43152d81c73a4d75bf7b8da0964bd8c087b2edbe79eb0b8c62c2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:04 GMT
ADD file:63bd8a316cba8c404cc2e32a5120406c24aee8db3224c469a6077b941d900863 in / 
# Thu, 23 Apr 2020 21:16:04 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 05:49:36 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Fri, 24 Apr 2020 05:49:38 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Thu, 30 Apr 2020 19:42:10 GMT
ENV REDIS_VERSION=6.0.0
# Thu, 30 Apr 2020 19:42:10 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.0.tar.gz
# Thu, 30 Apr 2020 19:42:10 GMT
ENV REDIS_DOWNLOAD_SHA=16d13ec1c3255206deb4818ed444dca6dda1482b551736f0033253c211b788fc
# Thu, 30 Apr 2020 19:43:29 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Thu, 30 Apr 2020 19:43:29 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 30 Apr 2020 19:43:30 GMT
VOLUME [/data]
# Thu, 30 Apr 2020 19:43:30 GMT
WORKDIR /data
# Thu, 30 Apr 2020 19:43:30 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Thu, 30 Apr 2020 19:43:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Apr 2020 19:43:31 GMT
EXPOSE 6379
# Thu, 30 Apr 2020 19:43:31 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:2826c1e79865da7e0da0a993a2a38db61c3911e05b5df617439a86d4deac90fb`  
		Last Modified: Thu, 23 Apr 2020 21:16:32 GMT  
		Size: 2.8 MB (2808418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4eb71d5f124b9b51684034d7d96fba6399ff6892995e51137d0c0617a11fb9`  
		Last Modified: Fri, 24 Apr 2020 05:53:39 GMT  
		Size: 1.2 KB (1229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7685edc32d5ef38faf3beb4310c119862b1dfa18ea58edb0dbca84e9417b267`  
		Last Modified: Fri, 24 Apr 2020 05:53:39 GMT  
		Size: 407.9 KB (407901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29dc19d4fc83d03487f7dbabdaa135bcd9127b1cd4bf46250898386019adc0e6`  
		Last Modified: Thu, 30 Apr 2020 19:44:20 GMT  
		Size: 7.1 MB (7066931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:455ebc5ee2803c5d00b1a0df571ac01bef459447f938846b72c514a83b6f44cc`  
		Last Modified: Thu, 30 Apr 2020 19:44:08 GMT  
		Size: 101.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d69d2ef4be7a9a41e5e4a4cdc84b425e3de0cb6d9bc2e467900a659ee7911cd`  
		Last Modified: Thu, 30 Apr 2020 19:44:09 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine` - linux; ppc64le

```console
$ docker pull redis@sha256:e8acaced87453f680975346f5a047b4c96ab1de2f471991bf7a3659cde7ec637
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.1 MB (11119768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21508223f2fb6c1fceba138ebc3bec18abc737544a8de002a0234ffc138b4aff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 20:39:04 GMT
ADD file:1aaebe252dfb1885e066fcbc84aaa915bae149c3608f19600855ad1d4f7450c1 in / 
# Thu, 23 Apr 2020 20:39:06 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 09:02:06 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Fri, 24 Apr 2020 09:02:13 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Thu, 30 Apr 2020 21:10:35 GMT
ENV REDIS_VERSION=6.0.0
# Thu, 30 Apr 2020 21:10:37 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.0.tar.gz
# Thu, 30 Apr 2020 21:10:40 GMT
ENV REDIS_DOWNLOAD_SHA=16d13ec1c3255206deb4818ed444dca6dda1482b551736f0033253c211b788fc
# Thu, 30 Apr 2020 21:11:40 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Thu, 30 Apr 2020 21:11:50 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 30 Apr 2020 21:11:53 GMT
VOLUME [/data]
# Thu, 30 Apr 2020 21:11:56 GMT
WORKDIR /data
# Thu, 30 Apr 2020 21:11:57 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Thu, 30 Apr 2020 21:12:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Apr 2020 21:12:03 GMT
EXPOSE 6379
# Thu, 30 Apr 2020 21:12:06 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:9a8fdc5b698322331ee7eba7dd6f66f3a4e956554db22dd1e834d519415b4f8e`  
		Last Modified: Thu, 23 Apr 2020 20:41:33 GMT  
		Size: 2.8 MB (2821843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dc79e36a18515157312416d029cb35887ee8668b53b6c0e3867a4d0dd8dd231`  
		Last Modified: Fri, 24 Apr 2020 09:06:56 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb83078862453fa1de07d734ccc5b995c92cd74710488c11d066ad752e3402d`  
		Last Modified: Fri, 24 Apr 2020 09:06:57 GMT  
		Size: 409.9 KB (409875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2fb9bf2dcf849e33064f8089b1c5286a3046f24052887a9660a9f888cb2d8cb`  
		Last Modified: Thu, 30 Apr 2020 21:13:32 GMT  
		Size: 7.9 MB (7886244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac7d1b847cfea73afe57e24773738fdd4b156217ceb09bcae6cf3697598f275a`  
		Last Modified: Thu, 30 Apr 2020 21:13:27 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce48e7cd95a41a8db831ab10e8bb9a0e8df91e48e5d05008c193bb7e656a4a6f`  
		Last Modified: Thu, 30 Apr 2020 21:13:27 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-alpine` - linux; s390x

```console
$ docker pull redis@sha256:2360c616f1d19c5447ab57f1de3e22975d0f93c312574f32c54d8c0b8baf418f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.6 MB (10640841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca50b1907b502df8de3fdd3ca915945020749a24fccee55360c203664e8289c7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 17:50:57 GMT
ADD file:a59a30c2fd43c9f3b820751a6f5a54688c14440a1ddace1ab255475f46e6ba2d in / 
# Thu, 23 Apr 2020 17:50:58 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 07:02:35 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Fri, 24 Apr 2020 07:02:36 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Thu, 30 Apr 2020 20:54:48 GMT
ENV REDIS_VERSION=6.0.0
# Thu, 30 Apr 2020 20:54:48 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.0.tar.gz
# Thu, 30 Apr 2020 20:54:49 GMT
ENV REDIS_DOWNLOAD_SHA=16d13ec1c3255206deb4818ed444dca6dda1482b551736f0033253c211b788fc
# Thu, 30 Apr 2020 20:55:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Thu, 30 Apr 2020 20:55:23 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 30 Apr 2020 20:55:23 GMT
VOLUME [/data]
# Thu, 30 Apr 2020 20:55:23 GMT
WORKDIR /data
# Thu, 30 Apr 2020 20:55:23 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Thu, 30 Apr 2020 20:55:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Apr 2020 20:55:24 GMT
EXPOSE 6379
# Thu, 30 Apr 2020 20:55:24 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:7184c046fdf17da4c16ca482e5ede36e1f2d41ac8cea9c036e488fd149d6e8e7`  
		Last Modified: Thu, 23 Apr 2020 17:51:38 GMT  
		Size: 2.6 MB (2582859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2da1b54f68b54cfd646e4cf510a14593b857e3c6e7732985b5a3bc5e213a72a`  
		Last Modified: Fri, 24 Apr 2020 07:04:54 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41f0a46f7a997ac6f05cd804b3a0f56c74348f25fd9e164c66ab7c5c4a6a2c82`  
		Last Modified: Fri, 24 Apr 2020 07:04:54 GMT  
		Size: 407.4 KB (407392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db4d8b698b86ff9a3a3b84ef1d16c6a7c47ee55339d1b39414d705d8bf90688`  
		Last Modified: Thu, 30 Apr 2020 20:56:14 GMT  
		Size: 7.6 MB (7648785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe3843366e5473610c61bcf4a5a4b4b64071c8bc3d89eaa92dea680cafcb423a`  
		Last Modified: Thu, 30 Apr 2020 20:56:10 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f5afebfc4fc6494509c630816a1959890c1b22e3985f5b0c5418af91cf66181`  
		Last Modified: Thu, 30 Apr 2020 20:56:15 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
