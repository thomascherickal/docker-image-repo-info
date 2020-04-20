## `redis:rc-alpine3.11`

```console
$ docker pull redis@sha256:4e52f39096fd65106ebf306fff1c4ce82549ddc60f33b1a494456b9bc3352c1d
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

### `redis:rc-alpine3.11` - linux; amd64

```console
$ docker pull redis@sha256:c58aaf1ca909c11bc94dde62b4e181d7173592a17617bb3f95b61812bb69d93c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.6 MB (10575612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80f9622b43113ca828cacc3533253b06d90e07e34aac2d975563ded8891bc408`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Mon, 23 Mar 2020 21:19:34 GMT
ADD file:0c4555f363c2672e350001f1293e689875a3760afe7b3f9146886afe67121cba in / 
# Mon, 23 Mar 2020 21:19:34 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 00:49:58 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Tue, 24 Mar 2020 00:49:59 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Mon, 20 Apr 2020 18:33:25 GMT
ENV REDIS_VERSION=6.0-rc4
# Mon, 20 Apr 2020 18:33:26 GMT
ENV REDIS_DOWNLOAD_URL=https://github.com/antirez/redis/archive/6.0-rc4.tar.gz
# Mon, 20 Apr 2020 18:33:26 GMT
ENV REDIS_DOWNLOAD_SHA=dac1ad1253337c06adf2af7f6ec7d2f54371e6b37b3c3d1c9d8fb4b7713d12a7
# Mon, 20 Apr 2020 18:34:39 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Mon, 20 Apr 2020 18:34:40 GMT
RUN mkdir /data && chown redis:redis /data
# Mon, 20 Apr 2020 18:34:40 GMT
VOLUME [/data]
# Mon, 20 Apr 2020 18:34:40 GMT
WORKDIR /data
# Mon, 20 Apr 2020 18:34:40 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Mon, 20 Apr 2020 18:34:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 20 Apr 2020 18:34:41 GMT
EXPOSE 6379
# Mon, 20 Apr 2020 18:34:41 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:aad63a9339440e7c3e1fff2b988991b9bfb81280042fa7f39a5e327023056819`  
		Last Modified: Mon, 23 Mar 2020 21:19:53 GMT  
		Size: 2.8 MB (2803255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:541cb024bf66c36eab08a7896d96ba1e929b45e33b9242d912e4c982a8e6d2c8`  
		Last Modified: Tue, 24 Mar 2020 00:54:02 GMT  
		Size: 1.2 KB (1228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270420c343f3239793a3aa2928f17b524d4061b0d21d3f634b9ccaca25eba02d`  
		Last Modified: Tue, 24 Mar 2020 00:54:01 GMT  
		Size: 402.6 KB (402572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8499fbd1fd104306ba44410768de345527183ec34636d97f3ca58ce492015527`  
		Last Modified: Mon, 20 Apr 2020 18:39:53 GMT  
		Size: 7.4 MB (7368041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d045d7ff6310f3a62051ddab24ddc955ee8bdc240b664c6e4554edf8047e9d03`  
		Last Modified: Mon, 20 Apr 2020 18:39:52 GMT  
		Size: 100.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b14c4df341be109278cc06fc628b3d5dc0a90371aefc084d70d8a6e95dee0b1`  
		Last Modified: Mon, 20 Apr 2020 18:39:52 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:rc-alpine3.11` - linux; arm variant v6

```console
$ docker pull redis@sha256:67845de6c6f104a62148a8c13ca5f60cb959bb9fc95dcb180b9e47612f5f0405
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.3 MB (10283847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94674c0b6510b7552339a8380a15dae799ea59185115cca0f1a722a4d0646cc1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Mon, 23 Mar 2020 21:49:26 GMT
ADD file:e2fdfc637b534345942caf4097883508a5ed23be97d85ccc3357b8277aaa5430 in / 
# Mon, 23 Mar 2020 21:49:27 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 00:28:11 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Tue, 24 Mar 2020 00:28:14 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Mon, 20 Apr 2020 18:49:54 GMT
ENV REDIS_VERSION=6.0-rc4
# Mon, 20 Apr 2020 18:49:56 GMT
ENV REDIS_DOWNLOAD_URL=https://github.com/antirez/redis/archive/6.0-rc4.tar.gz
# Mon, 20 Apr 2020 18:49:58 GMT
ENV REDIS_DOWNLOAD_SHA=dac1ad1253337c06adf2af7f6ec7d2f54371e6b37b3c3d1c9d8fb4b7713d12a7
# Mon, 20 Apr 2020 18:51:07 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Mon, 20 Apr 2020 18:51:14 GMT
RUN mkdir /data && chown redis:redis /data
# Mon, 20 Apr 2020 18:51:15 GMT
VOLUME [/data]
# Mon, 20 Apr 2020 18:51:18 GMT
WORKDIR /data
# Mon, 20 Apr 2020 18:51:20 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Mon, 20 Apr 2020 18:51:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 20 Apr 2020 18:51:24 GMT
EXPOSE 6379
# Mon, 20 Apr 2020 18:51:27 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:0776aeec3430c5a5ba3f43937f0ee6a7770a1fe81a318c9d94cc76512e5375e9`  
		Last Modified: Mon, 23 Mar 2020 21:49:50 GMT  
		Size: 2.6 MB (2618579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f44d20f426629582b73a72c19a7f86d8d643b9c2c3659133cbd53c909bac15`  
		Last Modified: Tue, 24 Mar 2020 00:32:06 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b08e9afe8dbb5799ae804339cf62c92a5d33e67526bcdc12f8528fb5ad6c06`  
		Last Modified: Tue, 24 Mar 2020 00:32:06 GMT  
		Size: 405.8 KB (405798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4c15fa78b9e9fb95307fee324f4c7fe95d1e43af62b9b846ba3197a189bea6`  
		Last Modified: Mon, 20 Apr 2020 18:53:59 GMT  
		Size: 7.3 MB (7257664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe134778b605d4026225c19a5225b30051eca1bc730d16d6ed51868319657b3f`  
		Last Modified: Mon, 20 Apr 2020 18:53:57 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e17df0040b0c3d4ab9faf1e7bb4e1214fa903ddc2810fa7d6748fff9821794`  
		Last Modified: Mon, 20 Apr 2020 18:53:57 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:rc-alpine3.11` - linux; arm variant v7

```console
$ docker pull redis@sha256:39f61423a57afab9a5e671d8939a2df4ca8d796eb7ceb87f5f9d9ded832c534f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9928441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfb13e5a72326b717022d13438bc73fcc25f69b2f5127606b0cbb2293389d356`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Mon, 23 Mar 2020 21:57:55 GMT
ADD file:3bde6b6fd06efbf24e66446c6d32f72294fc749ae9ee6191776242e92b2f8ab4 in / 
# Mon, 23 Mar 2020 21:57:56 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 00:20:27 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Tue, 24 Mar 2020 00:20:36 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Wed, 01 Apr 2020 06:09:58 GMT
ENV REDIS_VERSION=6.0-rc3
# Wed, 01 Apr 2020 06:09:59 GMT
ENV REDIS_DOWNLOAD_URL=https://github.com/antirez/redis/archive/6.0-rc3.tar.gz
# Wed, 01 Apr 2020 06:10:00 GMT
ENV REDIS_DOWNLOAD_SHA=a81f92ed0aeb2ecab1488ce916725da1283fa86c3ff43828430e77ce8e612534
# Wed, 01 Apr 2020 06:10:47 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Wed, 01 Apr 2020 06:10:49 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 01 Apr 2020 06:10:50 GMT
VOLUME [/data]
# Wed, 01 Apr 2020 06:10:51 GMT
WORKDIR /data
# Wed, 01 Apr 2020 06:10:51 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Wed, 01 Apr 2020 06:10:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Apr 2020 06:10:53 GMT
EXPOSE 6379
# Wed, 01 Apr 2020 06:10:54 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:d9bf605ce3d4449f4b90035c3e21d691806324781d43a5287b1da25a01779d6b`  
		Last Modified: Mon, 23 Mar 2020 21:58:16 GMT  
		Size: 2.4 MB (2420493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf903acfc5dda9aef697bfecd22603b39ced652df489747e2c0e3ce61ead1cfe`  
		Last Modified: Tue, 24 Mar 2020 00:25:14 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2ab068417ed691cc347820dd7a39958aacf24f5dee26c4399a12056d661d80`  
		Last Modified: Tue, 24 Mar 2020 00:25:13 GMT  
		Size: 399.8 KB (399770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c581153ddb04ca1546a09c7c314cdeb91943904d4b27a9ac569f63e98361d1fc`  
		Last Modified: Wed, 01 Apr 2020 06:12:11 GMT  
		Size: 7.1 MB (7106374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411e3c97287991f91e074ef4e7171f68f7dc0b78100b56a742013ab00ce3205e`  
		Last Modified: Wed, 01 Apr 2020 06:12:09 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdef6778bba665f0240be0876372efbaaded1e26c27b183da87e2b549f811585`  
		Last Modified: Wed, 01 Apr 2020 06:12:09 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:rc-alpine3.11` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:d014c3e97a532ad460873f60df65c6cd4c6a93cf37035e077635bd439382ef2d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.5 MB (10494351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc3e02c01175964fc451d7bccef3962fa00231d49d8da4e5a9ae1149e6e3b27c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Mon, 23 Mar 2020 21:39:52 GMT
ADD file:746a5c3838a898d6acf7877552ff13d1ab40d0036ace7a662e7c747018315ddb in / 
# Mon, 23 Mar 2020 21:39:53 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 05:27:21 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Tue, 24 Mar 2020 05:27:24 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Mon, 20 Apr 2020 18:27:33 GMT
ENV REDIS_VERSION=6.0-rc4
# Mon, 20 Apr 2020 18:27:36 GMT
ENV REDIS_DOWNLOAD_URL=https://github.com/antirez/redis/archive/6.0-rc4.tar.gz
# Mon, 20 Apr 2020 18:27:39 GMT
ENV REDIS_DOWNLOAD_SHA=dac1ad1253337c06adf2af7f6ec7d2f54371e6b37b3c3d1c9d8fb4b7713d12a7
# Mon, 20 Apr 2020 18:28:54 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Mon, 20 Apr 2020 18:28:59 GMT
RUN mkdir /data && chown redis:redis /data
# Mon, 20 Apr 2020 18:29:01 GMT
VOLUME [/data]
# Mon, 20 Apr 2020 18:29:03 GMT
WORKDIR /data
# Mon, 20 Apr 2020 18:29:05 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Mon, 20 Apr 2020 18:29:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 20 Apr 2020 18:29:10 GMT
EXPOSE 6379
# Mon, 20 Apr 2020 18:29:12 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:8a0637ca1ac98db4cf29f7632449c92801adc80cf0da2cd9c9e39882ce466561`  
		Last Modified: Mon, 23 Mar 2020 21:40:19 GMT  
		Size: 2.7 MB (2723139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97ca613f2fd65fd437b278f2407d1f63c4af7d9b38c7d4e5bc4b94712ee3a09d`  
		Last Modified: Tue, 24 Mar 2020 05:30:59 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d356bfcf65a90e43cf9b6820ef126a002d6c834bf54f563c690ef7745a1305`  
		Last Modified: Tue, 24 Mar 2020 05:30:59 GMT  
		Size: 404.7 KB (404661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd11644f79fb13797887b849a8b16556639902c166421eebb4b5526b96189492`  
		Last Modified: Mon, 20 Apr 2020 18:34:53 GMT  
		Size: 7.4 MB (7364745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7521ac73890c0eecefd0af2364c7ef75fb1c2bfc8dd2d0f98e0f0476a8fde61c`  
		Last Modified: Mon, 20 Apr 2020 18:34:51 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb9bef2f8060945878c193bd2e121b233720eaa6b42168558a25497f6eb5cde`  
		Last Modified: Mon, 20 Apr 2020 18:34:52 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:rc-alpine3.11` - linux; 386

```console
$ docker pull redis@sha256:79fd85fcad6d39476b91805666a0464d2b100353384881f53a3fbb7bb3c15d17
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.3 MB (10261379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb420345bdd443784537f5469930fa18ce6da147d803faee3492a685f28e6a18`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Mon, 23 Mar 2020 21:38:28 GMT
ADD file:99c8234abafd4fa915c0b826eb0e3be0e6aaa7c1e33cb1214ef71a99e9c02e06 in / 
# Mon, 23 Mar 2020 21:38:28 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 04:20:21 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Tue, 24 Mar 2020 04:20:22 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Mon, 20 Apr 2020 18:04:57 GMT
ENV REDIS_VERSION=6.0-rc4
# Mon, 20 Apr 2020 18:04:58 GMT
ENV REDIS_DOWNLOAD_URL=https://github.com/antirez/redis/archive/6.0-rc4.tar.gz
# Mon, 20 Apr 2020 18:04:58 GMT
ENV REDIS_DOWNLOAD_SHA=dac1ad1253337c06adf2af7f6ec7d2f54371e6b37b3c3d1c9d8fb4b7713d12a7
# Mon, 20 Apr 2020 18:06:23 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Mon, 20 Apr 2020 18:06:24 GMT
RUN mkdir /data && chown redis:redis /data
# Mon, 20 Apr 2020 18:06:25 GMT
VOLUME [/data]
# Mon, 20 Apr 2020 18:06:25 GMT
WORKDIR /data
# Mon, 20 Apr 2020 18:06:25 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Mon, 20 Apr 2020 18:06:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 20 Apr 2020 18:06:26 GMT
EXPOSE 6379
# Mon, 20 Apr 2020 18:06:26 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:43f6a4398e1c9e860dfb5c93d7049ab9eedf814513bd6d07e06077c560303c7a`  
		Last Modified: Mon, 23 Mar 2020 21:38:48 GMT  
		Size: 2.8 MB (2806122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:183c50f0f4e4ae6d84cee6e524803493225f47e8002f4458935e4385766be10c`  
		Last Modified: Tue, 24 Mar 2020 04:24:46 GMT  
		Size: 1.2 KB (1227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b176be9a8aea58cd5965d94dcbba8827d6cf5ca8854e65c12335d96e13b31a9d`  
		Last Modified: Tue, 24 Mar 2020 04:24:46 GMT  
		Size: 407.9 KB (407896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79cd6d693866c5e9297cf9f6ef3102aee74fc34b4242925370eea8722bcfd78e`  
		Last Modified: Mon, 20 Apr 2020 18:10:33 GMT  
		Size: 7.0 MB (7045622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f84f99de450ecab65df48a29e62c4ebae9cca47efd3ca3e70f56d99ce533e9`  
		Last Modified: Mon, 20 Apr 2020 18:10:32 GMT  
		Size: 99.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb8ead422bc9df2d8ce1abe4281cb1e728ef837f20aa1e63689cc2dff806eed`  
		Last Modified: Mon, 20 Apr 2020 18:10:32 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:rc-alpine3.11` - linux; ppc64le

```console
$ docker pull redis@sha256:67aa221a58d1c4ee4cc57306f149b4f16689aede94afd6268de6587695769bce
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.1 MB (11083106 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99de3ca224bde6beb21e48e07cdf16cc9baa79ca9d72cd2602cd6272878343be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Mon, 23 Mar 2020 21:21:29 GMT
ADD file:4b35131542b9682214e1c2c72fe3cea215a10e2f775e87befecd80fe2228d5a0 in / 
# Mon, 23 Mar 2020 21:21:32 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 00:19:48 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Tue, 24 Mar 2020 00:19:55 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Wed, 01 Apr 2020 11:38:57 GMT
ENV REDIS_VERSION=6.0-rc3
# Wed, 01 Apr 2020 11:39:00 GMT
ENV REDIS_DOWNLOAD_URL=https://github.com/antirez/redis/archive/6.0-rc3.tar.gz
# Wed, 01 Apr 2020 11:39:04 GMT
ENV REDIS_DOWNLOAD_SHA=a81f92ed0aeb2ecab1488ce916725da1283fa86c3ff43828430e77ce8e612534
# Wed, 01 Apr 2020 11:39:57 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Wed, 01 Apr 2020 11:40:06 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 01 Apr 2020 11:40:09 GMT
VOLUME [/data]
# Wed, 01 Apr 2020 11:40:14 GMT
WORKDIR /data
# Wed, 01 Apr 2020 11:40:15 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Wed, 01 Apr 2020 11:40:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Apr 2020 11:40:22 GMT
EXPOSE 6379
# Wed, 01 Apr 2020 11:40:25 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:bc1c99f4ba60de0d3ca52dc6855483e24c91884e33df71f502bbff6eb909d9b9`  
		Last Modified: Mon, 23 Mar 2020 21:22:12 GMT  
		Size: 2.8 MB (2820052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60b39f7944a074f282929c82323180bb32310c880897a9cafb51d5498c3c2035`  
		Last Modified: Tue, 24 Mar 2020 00:25:01 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb6a13a2a37045b6561b6d04fe2b72af88c07fc13f98fd30c60f36e2761f434`  
		Last Modified: Tue, 24 Mar 2020 00:25:01 GMT  
		Size: 409.9 KB (409863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c35d0b94874db03dcd80be3f237b8d9d0859d65e628aa4c0a17b0a4279cfa983`  
		Last Modified: Wed, 01 Apr 2020 11:41:59 GMT  
		Size: 7.9 MB (7851381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:212c979fa8093f589ef99d0300a5b29c9c2eaa12aef9a8789e1b0d9510358348`  
		Last Modified: Wed, 01 Apr 2020 11:41:57 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50595cee07683215ceb9a4ac6dde187b4c2ac15587e2b08ebaf2167aa45eeceb`  
		Last Modified: Wed, 01 Apr 2020 11:41:57 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:rc-alpine3.11` - linux; s390x

```console
$ docker pull redis@sha256:09a4e4c4e8004195f2a38d59f1f5637827f4d3a7c16af5da42e0de73b019100f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.6 MB (10606028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3da184d9f6131ebcf496f110ed46343e5a00492c8e99ad6c4ee42e5e1331064f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Mon, 23 Mar 2020 21:41:34 GMT
ADD file:b6d4ad8fd0ec7f66e6d54b8cd8937ba7821b44096806af78692b4cab6d087a9c in / 
# Mon, 23 Mar 2020 21:41:34 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 00:34:49 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Tue, 24 Mar 2020 00:34:50 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Wed, 01 Apr 2020 01:53:21 GMT
ENV REDIS_VERSION=6.0-rc3
# Wed, 01 Apr 2020 01:53:21 GMT
ENV REDIS_DOWNLOAD_URL=https://github.com/antirez/redis/archive/6.0-rc3.tar.gz
# Wed, 01 Apr 2020 01:53:21 GMT
ENV REDIS_DOWNLOAD_SHA=a81f92ed0aeb2ecab1488ce916725da1283fa86c3ff43828430e77ce8e612534
# Wed, 01 Apr 2020 01:53:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Wed, 01 Apr 2020 01:53:53 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 01 Apr 2020 01:53:53 GMT
VOLUME [/data]
# Wed, 01 Apr 2020 01:53:54 GMT
WORKDIR /data
# Wed, 01 Apr 2020 01:53:54 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Wed, 01 Apr 2020 01:53:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Apr 2020 01:53:54 GMT
EXPOSE 6379
# Wed, 01 Apr 2020 01:53:54 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:ca1c6795bfb97df28a926fd646127ba4944b69beb1cea7b00d62787b8b3c0108`  
		Last Modified: Mon, 23 Mar 2020 21:41:56 GMT  
		Size: 2.6 MB (2582073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0827e77ef3717c455686b0d943f377dca7d7cbc9e5481ce4400a43fcdc74df2`  
		Last Modified: Tue, 24 Mar 2020 00:36:53 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb53fe37b0f8747adeeffa862b073acea5084cdeb000f2f5acfe4d48b041db8`  
		Last Modified: Tue, 24 Mar 2020 00:36:53 GMT  
		Size: 407.4 KB (407392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99ff7570dc338a1a5b82104eeedc6fd94e0b36877821bbeb77af9e815480c80`  
		Last Modified: Wed, 01 Apr 2020 01:54:52 GMT  
		Size: 7.6 MB (7614758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae6f94b184f87138e7dac9990ae48e2279f91bc0b4092ae67e67714a6991a09`  
		Last Modified: Wed, 01 Apr 2020 01:54:55 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8720f9b826889d7503ba1f7e7c3afbebc1956fe66306e507067d4756c7d79569`  
		Last Modified: Wed, 01 Apr 2020 01:54:56 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
