## `redis:rc-alpine3.11`

```console
$ docker pull redis@sha256:f4b9f9819caedb455a797f5e2b4e3c647461294221109ce9ea73e10e5ae517d8
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
$ docker pull redis@sha256:675dc41b94a4616271790b25a1568671fd63565f74b48322168e7ef31949e62c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.5 MB (10545857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1d3dc64bdd7b527a2a8e4a800dff82151c5d03b6b5b8392a37b2a11fc22b8f0`
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
# Tue, 24 Mar 2020 00:50:00 GMT
ENV REDIS_VERSION=6.0-rc2
# Tue, 24 Mar 2020 00:50:00 GMT
ENV REDIS_DOWNLOAD_URL=https://github.com/antirez/redis/archive/6.0-rc2.tar.gz
# Tue, 24 Mar 2020 00:50:00 GMT
ENV REDIS_DOWNLOAD_SHA=ac8ac8aae2c143ba972c386f9852ae40b418dbcecab3841bf7f6d4b71fccd7cb
# Tue, 24 Mar 2020 00:51:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Tue, 24 Mar 2020 00:51:16 GMT
RUN mkdir /data && chown redis:redis /data
# Tue, 24 Mar 2020 00:51:16 GMT
VOLUME [/data]
# Tue, 24 Mar 2020 00:51:17 GMT
WORKDIR /data
# Tue, 24 Mar 2020 00:51:17 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Tue, 24 Mar 2020 00:51:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Mar 2020 00:51:17 GMT
EXPOSE 6379
# Tue, 24 Mar 2020 00:51:17 GMT
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
	-	`sha256:550915052f7548c6b5d35044cf866383fbc77b28c346b171e924e9dfb000c30f`  
		Last Modified: Tue, 24 Mar 2020 00:54:03 GMT  
		Size: 7.3 MB (7338290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c2c4d1c332e0a07b3401948934fc1edef866a9229baf4bafe10c0c035de3d7`  
		Last Modified: Tue, 24 Mar 2020 00:54:01 GMT  
		Size: 100.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d96855a2c92d07733efd828a73ab06943225670cdffcafda68c68dfec2e16d`  
		Last Modified: Tue, 24 Mar 2020 00:54:01 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:rc-alpine3.11` - linux; arm variant v6

```console
$ docker pull redis@sha256:524fe1bd205d4d9ac49da07c879c0784fbfbad2b6610d7eef957f1e844110053
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.3 MB (10267148 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b23adcf5459b09bd34338139085637edb878d37bf8000a90796681beff80c2f0`
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
# Wed, 01 Apr 2020 02:34:02 GMT
ENV REDIS_VERSION=6.0-rc3
# Wed, 01 Apr 2020 02:34:03 GMT
ENV REDIS_DOWNLOAD_URL=https://github.com/antirez/redis/archive/6.0-rc3.tar.gz
# Wed, 01 Apr 2020 02:34:03 GMT
ENV REDIS_DOWNLOAD_SHA=a81f92ed0aeb2ecab1488ce916725da1283fa86c3ff43828430e77ce8e612534
# Wed, 01 Apr 2020 02:34:54 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Wed, 01 Apr 2020 02:34:58 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 01 Apr 2020 02:35:00 GMT
VOLUME [/data]
# Wed, 01 Apr 2020 02:35:02 GMT
WORKDIR /data
# Wed, 01 Apr 2020 02:35:04 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Wed, 01 Apr 2020 02:35:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Apr 2020 02:35:07 GMT
EXPOSE 6379
# Wed, 01 Apr 2020 02:35:09 GMT
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
	-	`sha256:22c2d53317c515732967388c4e07433387260c4a153c03c471be83f78b1512cc`  
		Last Modified: Wed, 01 Apr 2020 02:35:42 GMT  
		Size: 7.2 MB (7240964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee567b8242051b48a0c36086ff8dcada4c9a28ca13a0afc86eda1d8971846612`  
		Last Modified: Wed, 01 Apr 2020 02:35:41 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce7a36d7d0aef79fc89c0dc7ac8acdaf1618dfcfb205985d3aec78486a32e42`  
		Last Modified: Wed, 01 Apr 2020 02:35:41 GMT  
		Size: 415.0 B  
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
$ docker pull redis@sha256:e340523b57bcfaf3c472c734117a8adcc6b3eb00c38b869d3196ac71c5cad59c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.5 MB (10462187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cbc31f1c5f703dc98529f902eacff91aac0549ee22f2ad00efff6253415326a`
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
# Tue, 24 Mar 2020 05:27:26 GMT
ENV REDIS_VERSION=6.0-rc2
# Tue, 24 Mar 2020 05:27:26 GMT
ENV REDIS_DOWNLOAD_URL=https://github.com/antirez/redis/archive/6.0-rc2.tar.gz
# Tue, 24 Mar 2020 05:27:27 GMT
ENV REDIS_DOWNLOAD_SHA=ac8ac8aae2c143ba972c386f9852ae40b418dbcecab3841bf7f6d4b71fccd7cb
# Tue, 24 Mar 2020 05:28:14 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Tue, 24 Mar 2020 05:28:16 GMT
RUN mkdir /data && chown redis:redis /data
# Tue, 24 Mar 2020 05:28:17 GMT
VOLUME [/data]
# Tue, 24 Mar 2020 05:28:18 GMT
WORKDIR /data
# Tue, 24 Mar 2020 05:28:19 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Tue, 24 Mar 2020 05:28:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Mar 2020 05:28:20 GMT
EXPOSE 6379
# Tue, 24 Mar 2020 05:28:21 GMT
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
	-	`sha256:4577a37ec07866b4fba98f8b974df0194a8928db040af1fa64c3862db72d182c`  
		Last Modified: Tue, 24 Mar 2020 05:31:02 GMT  
		Size: 7.3 MB (7332583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4640eb6d8ced93f97bdb520f72844fd8bb59fac10c71d3ff19ef5758979c98b`  
		Last Modified: Tue, 24 Mar 2020 05:30:59 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb244c91da8e2d160e03e3d46444d076ad8413365a793116558165525997d05`  
		Last Modified: Tue, 24 Mar 2020 05:30:59 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:rc-alpine3.11` - linux; 386

```console
$ docker pull redis@sha256:7900c298c5598747cd37dea28d0fc5cede4ca03d005759694420a2dc2423b134
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.2 MB (10243364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:787f6e9c53bb6d478db8c238bbf86666218d4c1ee7fdf4f9f644d03e2e7bc7f2`
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
# Wed, 01 Apr 2020 02:07:45 GMT
ENV REDIS_VERSION=6.0-rc3
# Wed, 01 Apr 2020 02:07:46 GMT
ENV REDIS_DOWNLOAD_URL=https://github.com/antirez/redis/archive/6.0-rc3.tar.gz
# Wed, 01 Apr 2020 02:07:46 GMT
ENV REDIS_DOWNLOAD_SHA=a81f92ed0aeb2ecab1488ce916725da1283fa86c3ff43828430e77ce8e612534
# Wed, 01 Apr 2020 02:09:14 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Wed, 01 Apr 2020 02:09:15 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 01 Apr 2020 02:09:15 GMT
VOLUME [/data]
# Wed, 01 Apr 2020 02:09:16 GMT
WORKDIR /data
# Wed, 01 Apr 2020 02:09:16 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Wed, 01 Apr 2020 02:09:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Apr 2020 02:09:16 GMT
EXPOSE 6379
# Wed, 01 Apr 2020 02:09:16 GMT
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
	-	`sha256:5a3a8b7e64929abc56c9fa5f3bb9b500aa3c8850ab8bcf1523a18b062b1212af`  
		Last Modified: Wed, 01 Apr 2020 02:10:27 GMT  
		Size: 7.0 MB (7027608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dbd068810fabeeef9d9069adcbd33a8575333350fd3c7874ef70053c113b38e`  
		Last Modified: Wed, 01 Apr 2020 02:10:25 GMT  
		Size: 99.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ad7791868a2d3b0516c3df938c72fcdaf2d1c3597518ffbcc339cc1f64f7cb9`  
		Last Modified: Wed, 01 Apr 2020 02:10:25 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:rc-alpine3.11` - linux; ppc64le

```console
$ docker pull redis@sha256:91b4dc17b3db383441e9df9a5db16bdb626129184344be1a4e7b5ca1aaa7e185
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.1 MB (11063531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c8954372f3af76a5467dcf7c9f643c60495b8f297557b25710b603a9538701a`
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
# Tue, 24 Mar 2020 00:19:58 GMT
ENV REDIS_VERSION=6.0-rc2
# Tue, 24 Mar 2020 00:20:02 GMT
ENV REDIS_DOWNLOAD_URL=https://github.com/antirez/redis/archive/6.0-rc2.tar.gz
# Tue, 24 Mar 2020 00:20:04 GMT
ENV REDIS_DOWNLOAD_SHA=ac8ac8aae2c143ba972c386f9852ae40b418dbcecab3841bf7f6d4b71fccd7cb
# Tue, 24 Mar 2020 00:20:57 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Tue, 24 Mar 2020 00:21:05 GMT
RUN mkdir /data && chown redis:redis /data
# Tue, 24 Mar 2020 00:21:07 GMT
VOLUME [/data]
# Tue, 24 Mar 2020 00:21:09 GMT
WORKDIR /data
# Tue, 24 Mar 2020 00:21:10 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Tue, 24 Mar 2020 00:21:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Mar 2020 00:21:15 GMT
EXPOSE 6379
# Tue, 24 Mar 2020 00:21:19 GMT
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
	-	`sha256:c5b679a66cebde6dca10a03004b9650faf91cd8c4049d50b567aea71555f2fc8`  
		Last Modified: Tue, 24 Mar 2020 00:25:03 GMT  
		Size: 7.8 MB (7831808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2555fcf00093162a904da17cf21a23b47e40e908fffcbbe3859a11c8ca5a911c`  
		Last Modified: Tue, 24 Mar 2020 00:25:01 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f1997181b83458f47c5e5b4b6de4dc7050fe1f8b835433a2b958547b919437`  
		Last Modified: Tue, 24 Mar 2020 00:25:01 GMT  
		Size: 413.0 B  
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
