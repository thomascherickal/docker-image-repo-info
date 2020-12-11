## `redis:5-alpine3.12`

```console
$ docker pull redis@sha256:aa75b84326007fce13e1f432bde5f6a9442a0580fd8965ddec4508ba23089db2
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

### `redis:5-alpine3.12` - linux; amd64

```console
$ docker pull redis@sha256:f583a486ccab58a8d20335a182e8aec0abcbab718ae192c15352ff0d59da0408
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (9965204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21419542e5570a0e016922d2e0f53a3aaf2bf9fe00a67e2717645bc40d52c83b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 16:25:16 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Fri, 11 Dec 2020 16:25:18 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Fri, 11 Dec 2020 16:28:54 GMT
ENV REDIS_VERSION=5.0.10
# Fri, 11 Dec 2020 16:28:55 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.10.tar.gz
# Fri, 11 Dec 2020 16:28:55 GMT
ENV REDIS_DOWNLOAD_SHA=e30a5e7d1593a715cdda2a82deb90190816d06c9d1dc1ef5b36874878c683382
# Fri, 11 Dec 2020 16:29:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 11 Dec 2020 16:29:49 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 11 Dec 2020 16:29:50 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 16:29:50 GMT
WORKDIR /data
# Fri, 11 Dec 2020 16:29:50 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 11 Dec 2020 16:29:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 16:29:50 GMT
EXPOSE 6379
# Fri, 11 Dec 2020 16:29:51 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c9d57a1c7f4bb594339d259d1485b48bd5b81e9e6f662b4791b1dadc5d4daf`  
		Last Modified: Fri, 11 Dec 2020 16:30:52 GMT  
		Size: 1.2 KB (1229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccd033d7ec061821df52b64df5078b36d1f755a2f02e4b6b578e3ebd739313dd`  
		Last Modified: Fri, 11 Dec 2020 16:30:53 GMT  
		Size: 381.5 KB (381504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16dd80ff9c02b717a4cb0d00769618dbbdeb3846e3d5370a21ebcce09a8d0f26`  
		Last Modified: Fri, 11 Dec 2020 16:31:34 GMT  
		Size: 6.8 MB (6785015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f3f60f9f927bed4cc68ead1c9f70a23f4327b8cf258d03faef4b9e735437583`  
		Last Modified: Fri, 11 Dec 2020 16:31:33 GMT  
		Size: 99.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e33c7edd1ed01dfc67669c996a124b2ff880687700538bf84bf6057067b7241f`  
		Last Modified: Fri, 11 Dec 2020 16:31:33 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-alpine3.12` - linux; arm variant v6

```console
$ docker pull redis@sha256:e0fd13008ab0bc854559b83b244c5d682eac87301ec081faa412a04d48e4853f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9675319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:652ad2b1903b63d2eb5195bc70909f5596bdd1ee3f377c4e419be403c16213ff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Fri, 11 Dec 2020 02:17:15 GMT
ADD file:1a9c0a67560d338c0c0e7005d8915d998fc9cf3e9f53bfd7e42e8391f0a39bce in / 
# Fri, 11 Dec 2020 02:17:15 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:10:34 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Fri, 11 Dec 2020 05:10:43 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Fri, 11 Dec 2020 05:12:05 GMT
ENV REDIS_VERSION=5.0.10
# Fri, 11 Dec 2020 05:12:05 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.10.tar.gz
# Fri, 11 Dec 2020 05:12:06 GMT
ENV REDIS_DOWNLOAD_SHA=e30a5e7d1593a715cdda2a82deb90190816d06c9d1dc1ef5b36874878c683382
# Fri, 11 Dec 2020 05:12:53 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 11 Dec 2020 05:12:55 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 11 Dec 2020 05:12:56 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 05:12:57 GMT
WORKDIR /data
# Fri, 11 Dec 2020 05:12:58 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 11 Dec 2020 05:12:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:12:59 GMT
EXPOSE 6379
# Fri, 11 Dec 2020 05:13:00 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:f1c16df8fee33d421d08790b17ca2af67a3fe49e77b6b991dd0c30631f5d1baf`  
		Last Modified: Fri, 11 Dec 2020 02:17:57 GMT  
		Size: 2.6 MB (2601992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:447a76a74c6810b07663d685dcd2f99da1fc67cf7824495b6f04910e7723f678`  
		Last Modified: Fri, 11 Dec 2020 05:13:24 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c23f37f74eda655a638a407067de4a279a1536b0fa95d392a642008f7ca9504c`  
		Last Modified: Fri, 11 Dec 2020 05:13:24 GMT  
		Size: 384.9 KB (384903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37f6600dc1d09a1e9a025f44c575e361a62f31ce101f6cafd6af1abd9205bdcc`  
		Last Modified: Fri, 11 Dec 2020 05:13:44 GMT  
		Size: 6.7 MB (6686619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d9fb151cbd4439df1ba1ee763ed2f7cd949d2656e1e8ee8242b94770719066d`  
		Last Modified: Fri, 11 Dec 2020 05:13:41 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3560954ba168a0acacf9f8467995d59eccc7221cadac863559a3812e73fb0ebf`  
		Last Modified: Fri, 11 Dec 2020 05:13:41 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-alpine3.12` - linux; arm variant v7

```console
$ docker pull redis@sha256:1c009b7b59f032a5446aa859f7bc976a4d621f050e90edcaeb655e64ed3bf3a8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9356843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06338ab0cef7ec3b90a9791f5f7c6635966911d93eeacdf02bccf8eaa351d6a1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Fri, 11 Dec 2020 02:20:33 GMT
ADD file:0e85952ec585d17378d9bb15a94ddc10c3ed8f766f275cf50fb36be1126f35d2 in / 
# Fri, 11 Dec 2020 02:20:34 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 15:47:37 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Fri, 11 Dec 2020 15:47:41 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Fri, 11 Dec 2020 15:51:13 GMT
ENV REDIS_VERSION=5.0.10
# Fri, 11 Dec 2020 15:51:15 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.10.tar.gz
# Fri, 11 Dec 2020 15:51:17 GMT
ENV REDIS_DOWNLOAD_SHA=e30a5e7d1593a715cdda2a82deb90190816d06c9d1dc1ef5b36874878c683382
# Fri, 11 Dec 2020 15:52:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 11 Dec 2020 15:52:13 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 11 Dec 2020 15:52:14 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 15:52:16 GMT
WORKDIR /data
# Fri, 11 Dec 2020 15:52:17 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 11 Dec 2020 15:52:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 15:52:21 GMT
EXPOSE 6379
# Fri, 11 Dec 2020 15:52:23 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:f70c74f2e22556cebd0cbbff78c03d4f0560d76979bf799d67730340a639aa57`  
		Last Modified: Fri, 11 Dec 2020 02:21:18 GMT  
		Size: 2.4 MB (2405692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bdac81f68b558d3a5d368f3b955dc55a67a9c6cfb03221be0d3dfaee25d087e`  
		Last Modified: Fri, 11 Dec 2020 15:53:27 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce249ae19ee7cfd52424c42faa2e50309438aebacb9a43947eb1fdec74bf031`  
		Last Modified: Fri, 11 Dec 2020 15:53:26 GMT  
		Size: 378.5 KB (378477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f0614730ed2ae2bcaaeed7ab7d0b07b9cef8d00ce1c671faff5d183dbe07056`  
		Last Modified: Fri, 11 Dec 2020 15:54:09 GMT  
		Size: 6.6 MB (6570872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d5bd415c6b9d9b98a835bd42791fcb34e8b0c8e9b30a8a48b8091d95fe7f54d`  
		Last Modified: Fri, 11 Dec 2020 15:54:06 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2572f3ce2cadb498eca6976695ff69397db2ccc1bf89997f98643571f281db9`  
		Last Modified: Fri, 11 Dec 2020 15:54:06 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-alpine3.12` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:c05c4bc6ed6ed775aac2b28c59b6a580f3de29579273af785f6f789135eaa816
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9902377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd15870d3ed46933aadfcaaff3ce5374094fc46624c86bd116347dfbed5a5aeb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 15:02:17 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Fri, 11 Dec 2020 15:02:27 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Fri, 11 Dec 2020 15:05:38 GMT
ENV REDIS_VERSION=5.0.10
# Fri, 11 Dec 2020 15:05:40 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.10.tar.gz
# Fri, 11 Dec 2020 15:05:41 GMT
ENV REDIS_DOWNLOAD_SHA=e30a5e7d1593a715cdda2a82deb90190816d06c9d1dc1ef5b36874878c683382
# Fri, 11 Dec 2020 15:06:39 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 11 Dec 2020 15:06:43 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 11 Dec 2020 15:06:44 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 15:06:45 GMT
WORKDIR /data
# Fri, 11 Dec 2020 15:06:46 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 11 Dec 2020 15:06:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 15:06:49 GMT
EXPOSE 6379
# Fri, 11 Dec 2020 15:06:50 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:644769aa9380d3217180aef39343466a8888ab65d032d49b2e0d076e1ae64439`  
		Last Modified: Fri, 11 Dec 2020 15:08:09 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d71757449c7064c22fec07fcdc49bb7e35eb87d73ea3bf8c27d1a905d48919d`  
		Last Modified: Fri, 11 Dec 2020 15:08:09 GMT  
		Size: 383.9 KB (383919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a9bf9611ab569fc532ba0166cc3d81c8a0f0d06f74c0c661e524376910d60f0`  
		Last Modified: Fri, 11 Dec 2020 15:08:58 GMT  
		Size: 6.8 MB (6810033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fb277908ed3e97d7c74c993a7f08961fd866271637d0d0877e212b525862d61`  
		Last Modified: Fri, 11 Dec 2020 15:08:55 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b2663ef5239fc27e567ffa47a490e14ff99d4f0be734e03fd35613aed287fe`  
		Last Modified: Fri, 11 Dec 2020 15:08:55 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-alpine3.12` - linux; 386

```console
$ docker pull redis@sha256:2983ccf26b6cd8f6c98a40bef4fc1a8aca2b50b2f6f507974b01fecd9d8f134d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9551874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4fa1feff85b73b5a191f9534e6f2b97de5fa8973d6074c05513ac5639d83275`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 05:26:45 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Thu, 22 Oct 2020 05:26:47 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Tue, 27 Oct 2020 18:55:18 GMT
ENV REDIS_VERSION=5.0.10
# Tue, 27 Oct 2020 18:55:18 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.10.tar.gz
# Tue, 27 Oct 2020 18:55:18 GMT
ENV REDIS_DOWNLOAD_SHA=e30a5e7d1593a715cdda2a82deb90190816d06c9d1dc1ef5b36874878c683382
# Tue, 27 Oct 2020 18:56:25 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Tue, 27 Oct 2020 18:56:25 GMT
RUN mkdir /data && chown redis:redis /data
# Tue, 27 Oct 2020 18:56:26 GMT
VOLUME [/data]
# Tue, 27 Oct 2020 18:56:26 GMT
WORKDIR /data
# Tue, 27 Oct 2020 18:56:26 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Tue, 27 Oct 2020 18:56:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 27 Oct 2020 18:56:26 GMT
EXPOSE 6379
# Tue, 27 Oct 2020 18:56:27 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e56191a325dfbb700a740ca5d50b18b47cada55e2a160eba04f310d426371cf9`  
		Last Modified: Thu, 22 Oct 2020 05:31:05 GMT  
		Size: 1.2 KB (1228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c130f6497e095cd8ed8ffb5c25fe3fa3a9f1d2dd2e4bf1f8a08b419c7b775a3f`  
		Last Modified: Thu, 22 Oct 2020 05:31:06 GMT  
		Size: 261.4 KB (261385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d92d9bc919d5ea4033a0132b7b2d1ba7d9e21d9bc85129ae1d2d31dc7bf6c31`  
		Last Modified: Tue, 27 Oct 2020 18:57:27 GMT  
		Size: 6.5 MB (6497342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5f50df69c3b675763a6a4f24df723fc47e36654542b3452d0d4230cb1490de1`  
		Last Modified: Tue, 27 Oct 2020 18:57:26 GMT  
		Size: 100.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53c5d7d4878ce3d5610a5bed48d35c538e796c3f5bf74c8063eca1efe01fd613`  
		Last Modified: Tue, 27 Oct 2020 18:57:26 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-alpine3.12` - linux; ppc64le

```console
$ docker pull redis@sha256:c0a9f68b6e72c3bef8a78ae5dce9bd2eed664f7ccc36d25eb37d30888ec384f0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.3 MB (10333098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0657e37de5a42a44826bb2e030c4b936c5f9c4e25718bcebdd77d40f3287c6bf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 22 Oct 2020 11:00:06 GMT
ADD file:176e047fab2c1828575bffa6b14773efa297b7ecf312d86103c5dd4f78ec8027 in / 
# Thu, 22 Oct 2020 11:00:17 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 22:35:47 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Thu, 22 Oct 2020 22:35:57 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Tue, 27 Oct 2020 18:29:07 GMT
ENV REDIS_VERSION=5.0.10
# Tue, 27 Oct 2020 18:29:09 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.10.tar.gz
# Tue, 27 Oct 2020 18:29:13 GMT
ENV REDIS_DOWNLOAD_SHA=e30a5e7d1593a715cdda2a82deb90190816d06c9d1dc1ef5b36874878c683382
# Tue, 27 Oct 2020 18:30:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Tue, 27 Oct 2020 18:30:26 GMT
RUN mkdir /data && chown redis:redis /data
# Tue, 27 Oct 2020 18:30:30 GMT
VOLUME [/data]
# Tue, 27 Oct 2020 18:30:32 GMT
WORKDIR /data
# Tue, 27 Oct 2020 18:30:34 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Tue, 27 Oct 2020 18:30:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 27 Oct 2020 18:30:43 GMT
EXPOSE 6379
# Tue, 27 Oct 2020 18:30:46 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:692a9d763e196c85d79fc3e45b316b1bb557c93ba88a3c8ebf679a585d1efe73`  
		Last Modified: Thu, 22 Oct 2020 11:02:06 GMT  
		Size: 2.8 MB (2803218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e48583f52640e5f838d8293b8b84eb715c9495d35e0d2b59baa879a3032d2434`  
		Last Modified: Thu, 22 Oct 2020 22:40:43 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11a4e4c49b0451515cfa0d5ae9c61c767794ff7b4c305a3b44dd4cb912d7f9e4`  
		Last Modified: Thu, 22 Oct 2020 22:40:43 GMT  
		Size: 263.3 KB (263288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87426b99b35b41fd2c9dd6461910d646f9ff64e56b750bb4ebf70d3a2f5364b3`  
		Last Modified: Tue, 27 Oct 2020 18:32:58 GMT  
		Size: 7.3 MB (7264777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2e167879bca69e1dd10df99f1ee674e3013c1703ca9aedc205cc5445ece4ede`  
		Last Modified: Tue, 27 Oct 2020 18:32:56 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b41a64f28e766e5c1608348c416153e5457e3d6bf6e22e07a62e307c487476c2`  
		Last Modified: Tue, 27 Oct 2020 18:32:56 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-alpine3.12` - linux; s390x

```console
$ docker pull redis@sha256:72819a2bca74d527b3ed22f3ed97e5778a62113fc2ee377ae2746c8621dacc95
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (10003479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4efa806ad5ba31994ddf9471d9f1fb068b670e510e4c7cf5e52611cda737a235`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Fri, 11 Dec 2020 02:09:52 GMT
ADD file:c9395a36a4e03768aabd282eb1f31705cc00181d3147222d9c940eaa5a8fd511 in / 
# Fri, 11 Dec 2020 02:09:53 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 13:58:32 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Fri, 11 Dec 2020 13:58:35 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Fri, 11 Dec 2020 14:02:10 GMT
ENV REDIS_VERSION=5.0.10
# Fri, 11 Dec 2020 14:02:10 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.10.tar.gz
# Fri, 11 Dec 2020 14:02:11 GMT
ENV REDIS_DOWNLOAD_SHA=e30a5e7d1593a715cdda2a82deb90190816d06c9d1dc1ef5b36874878c683382
# Fri, 11 Dec 2020 14:03:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 11 Dec 2020 14:03:12 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 11 Dec 2020 14:03:12 GMT
VOLUME [/data]
# Fri, 11 Dec 2020 14:03:13 GMT
WORKDIR /data
# Fri, 11 Dec 2020 14:03:13 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 11 Dec 2020 14:03:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 14:03:15 GMT
EXPOSE 6379
# Fri, 11 Dec 2020 14:03:15 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:7c2470fe3d16cb70fca0826168095a96838b1322a8cd1502b28284ee8561b491`  
		Last Modified: Fri, 11 Dec 2020 02:10:27 GMT  
		Size: 2.6 MB (2565988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f9fd6145aff29902d4fd018025ad260fe864cbe9f06627b6964ba58e33a2aa7`  
		Last Modified: Fri, 11 Dec 2020 14:04:21 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7732b2116381efd347a216d9f6b13848bbe0ece877b2e04b99db18bb895ef06b`  
		Last Modified: Fri, 11 Dec 2020 14:04:21 GMT  
		Size: 386.4 KB (386378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e7e5ab3356a03b52daa0830ed7f2cb362c81f5891c87e7cead9cd0eb26eaa4`  
		Last Modified: Fri, 11 Dec 2020 14:04:57 GMT  
		Size: 7.0 MB (7049308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26fd93ae3f40cb3a6934e8f2bb2cd18be5469eccf543be77421337dd93a2ba11`  
		Last Modified: Fri, 11 Dec 2020 14:04:55 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:418997c616a8639a188070032a7e166af47e0e4252d4cd92049be591de4b7be2`  
		Last Modified: Fri, 11 Dec 2020 14:04:54 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
