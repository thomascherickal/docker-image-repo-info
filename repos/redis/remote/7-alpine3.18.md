## `redis:7-alpine3.18`

```console
$ docker pull redis@sha256:2d44eb73209e5af4118de67e89b01709bfec7cc5a4c1cec29665f6d011c70783
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 13
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `redis:7-alpine3.18` - linux; amd64

```console
$ docker pull redis@sha256:6a6e00d7e9c27c3ac28444054773d4921dccf4d6f3eacde11a73af915b6db70f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (16022704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cd3929a2ac462b7f8a754b3e2a2611a4027377ef0704300a1d3b74a83777ad7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Wed, 18 Oct 2023 09:03:13 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
ENV REDIS_VERSION=7.2.2
# Wed, 18 Oct 2023 09:03:13 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.2.2.tar.gz
# Wed, 18 Oct 2023 09:03:13 GMT
ENV REDIS_DOWNLOAD_SHA=ca999be08800edc6d265379c4c7aafad92f0ee400692e4e2d69829ab4b4c3d08
# Wed, 18 Oct 2023 09:03:13 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
RUN mkdir /data && chown redis:redis /data # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
VOLUME [/data]
# Wed, 18 Oct 2023 09:03:13 GMT
WORKDIR /data
# Wed, 18 Oct 2023 09:03:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Oct 2023 09:03:13 GMT
EXPOSE map[6379/tcp:{}]
# Wed, 18 Oct 2023 09:03:13 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b11f9c76abbd533c9e64f773ad6c35e136d335ceca5dc6db94affcf25a5cd158`  
		Last Modified: Thu, 19 Oct 2023 01:03:05 GMT  
		Size: 1.2 KB (1246 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6617b52cbeba581a20b39289b538d8deff27ebe370ef6ede6d33446158fe345e`  
		Last Modified: Thu, 19 Oct 2023 01:03:05 GMT  
		Size: 347.4 KB (347375 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d690774d7e1aa27f9b38262e1778cf54be83d11f63afa312e31bbfd1eb5b3647`  
		Last Modified: Thu, 19 Oct 2023 01:03:06 GMT  
		Size: 12.3 MB (12271409 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7c08c8068f7a8d9d730507b512611fa07c7197378d070f52d28070881bb451f3`  
		Last Modified: Thu, 19 Oct 2023 01:03:05 GMT  
		Size: 100.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ea389a5fca7b3649136fc4a7300956c9efa61b88d8ac045c9cfe456e7d0ec8f6`  
		Last Modified: Thu, 19 Oct 2023 01:03:06 GMT  
		Size: 575.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redis:7-alpine3.18` - unknown; unknown

```console
$ docker pull redis@sha256:6ed1c191fbdf0780980c20299f226cfdc45810afdac235e0abe739bbf456e13f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **752.7 KB (752688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c2342ce075067bca3d9dd4a7ed8fb489a664068361a4a8d8c6dc409173fb56f`

```dockerfile
```

-	Layers:
	-	`sha256:f841782589b090e99a533abfc25b6725e42abf484c879b3a60f5ea718d944ffb`  
		Last Modified: Thu, 19 Oct 2023 01:03:05 GMT  
		Size: 726.4 KB (726434 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:e4ec30e7202de3393c14345d4aa0f464970f59e0a060cfb98ba71e7f23359a10`  
		Last Modified: Thu, 19 Oct 2023 01:03:05 GMT  
		Size: 26.3 KB (26254 bytes)  
		MIME: application/vnd.in-toto+json

### `redis:7-alpine3.18` - linux; arm variant v6

```console
$ docker pull redis@sha256:711643a0b6ad3512a55b12b721949aac04a3e90bd9a7a5bd52c8a74e268330c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.9 MB (15920227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd0a79bc18a89f810f0d5609c1ac5d1e02b34400a73a12e15eafe42ead81231e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Wed, 18 Oct 2023 09:03:13 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
ENV REDIS_VERSION=7.2.2
# Wed, 18 Oct 2023 09:03:13 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.2.2.tar.gz
# Wed, 18 Oct 2023 09:03:13 GMT
ENV REDIS_DOWNLOAD_SHA=ca999be08800edc6d265379c4c7aafad92f0ee400692e4e2d69829ab4b4c3d08
# Wed, 18 Oct 2023 09:03:13 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
RUN mkdir /data && chown redis:redis /data # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
VOLUME [/data]
# Wed, 18 Oct 2023 09:03:13 GMT
WORKDIR /data
# Wed, 18 Oct 2023 09:03:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Oct 2023 09:03:13 GMT
EXPOSE map[6379/tcp:{}]
# Wed, 18 Oct 2023 09:03:13 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a61b7be475a718c982548ef463e0c9e4a89c8e4295022c7ff8dd1ca8f9b9bf`  
		Last Modified: Tue, 03 Oct 2023 22:59:50 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c175be1a443b134a9e8b9971f24266cb06f3e831d2d20258a597465cab769c5d`  
		Last Modified: Tue, 03 Oct 2023 22:59:50 GMT  
		Size: 347.1 KB (347147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:163be5424bd585d5ef2836820d9bc56e81031705dbd0e095d1986eeeb5d9fd0f`  
		Last Modified: Thu, 19 Oct 2023 04:11:10 GMT  
		Size: 12.4 MB (12425841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da59fd8f8556d7bad67a1f40ab325775547c53df15dab074de3d0a3fa8bc3f3b`  
		Last Modified: Thu, 19 Oct 2023 04:11:07 GMT  
		Size: 100.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:539caf9f4c8df7c381b36f58036197c37edf4ac48888153e5e012df56285aef6`  
		Last Modified: Thu, 19 Oct 2023 04:11:07 GMT  
		Size: 573.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:7-alpine3.18` - linux; arm variant v7

```console
$ docker pull redis@sha256:53671702b535b03e058f84a4898024bb3bc5a2eb13b77c39235476119d89228d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.5 MB (15519711 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48484546b4f921e0d80cfe4d3d8ae5dae39556b32290cbc5f9c78b5dcdc11bd0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Wed, 18 Oct 2023 09:03:13 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
ENV REDIS_VERSION=7.2.2
# Wed, 18 Oct 2023 09:03:13 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.2.2.tar.gz
# Wed, 18 Oct 2023 09:03:13 GMT
ENV REDIS_DOWNLOAD_SHA=ca999be08800edc6d265379c4c7aafad92f0ee400692e4e2d69829ab4b4c3d08
# Wed, 18 Oct 2023 09:03:13 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
RUN mkdir /data && chown redis:redis /data # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
VOLUME [/data]
# Wed, 18 Oct 2023 09:03:13 GMT
WORKDIR /data
# Wed, 18 Oct 2023 09:03:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Oct 2023 09:03:13 GMT
EXPOSE map[6379/tcp:{}]
# Wed, 18 Oct 2023 09:03:13 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:da8bcc30219a3b5ad7547cb998dbc925d87391c679fec1abae88483d4839fa51`  
		Last Modified: Tue, 03 Oct 2023 23:23:43 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1a1e96038724920ff29465fba0c7aca16d709e1f1d94b903204ed8b6af9e8387`  
		Last Modified: Tue, 03 Oct 2023 23:23:43 GMT  
		Size: 347.0 KB (346994 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d83440224bfd8ba77cba21927d4f10b4ce416e61d3c7c4117c5966c752580d2b`  
		Last Modified: Thu, 19 Oct 2023 06:09:26 GMT  
		Size: 12.3 MB (12270860 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:af87460eea2892fc2eafdd8ca40b4d8c95b6e0f93bba1106f1590a5a5684d60b`  
		Last Modified: Thu, 19 Oct 2023 06:09:25 GMT  
		Size: 100.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:947664452a73a67a7ba789aa7fbfdde18cd9923d3e6bba1ed0d80625aa9be086`  
		Last Modified: Thu, 19 Oct 2023 06:09:26 GMT  
		Size: 575.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redis:7-alpine3.18` - unknown; unknown

```console
$ docker pull redis@sha256:06298301f782dc6f2a44aacc699fde484406c49197f82b29b6aeea1048159502
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **755.2 KB (755204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ad4339300ba515f52970b6032472d1057fe03c8cd71955a11b112b365e948be`

```dockerfile
```

-	Layers:
	-	`sha256:5ee8d836a1eb66f3ebeef767c07a18f81267dd2d209514ded781e1c85858b8e7`  
		Last Modified: Thu, 19 Oct 2023 06:09:26 GMT  
		Size: 729.0 KB (728975 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:b17a89a28ecd9b8db286be06b0b5dee47a9b152e92197e512d015c40d5100cb0`  
		Last Modified: Thu, 19 Oct 2023 06:09:25 GMT  
		Size: 26.2 KB (26229 bytes)  
		MIME: application/vnd.in-toto+json

### `redis:7-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:16f7271a1a04dff5e2592ce8808a4411a85f8165479364ce25799eb3c90168e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16134598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d4c89bd4fa6947ea1ec699a1cd675b36f944cb6f661427cc1c7f9ebbb833fba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Wed, 18 Oct 2023 09:03:13 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
ENV REDIS_VERSION=7.2.2
# Wed, 18 Oct 2023 09:03:13 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.2.2.tar.gz
# Wed, 18 Oct 2023 09:03:13 GMT
ENV REDIS_DOWNLOAD_SHA=ca999be08800edc6d265379c4c7aafad92f0ee400692e4e2d69829ab4b4c3d08
# Wed, 18 Oct 2023 09:03:13 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
RUN mkdir /data && chown redis:redis /data # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
VOLUME [/data]
# Wed, 18 Oct 2023 09:03:13 GMT
WORKDIR /data
# Wed, 18 Oct 2023 09:03:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Oct 2023 09:03:13 GMT
EXPOSE map[6379/tcp:{}]
# Wed, 18 Oct 2023 09:03:13 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2e0feb8fddc533ebe8fa3e28ab60443a2b6a5a7e46ff3560b1e79f4ff945a70f`  
		Last Modified: Tue, 03 Oct 2023 23:02:00 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a743b36a722987becef2b73971d75377bee67a2a6577cbdfddc1da3634eb4a73`  
		Last Modified: Tue, 03 Oct 2023 23:02:01 GMT  
		Size: 347.6 KB (347581 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8a4454015f0a1fafa6f99ec67cbbdd248c826b222118a7adb7754953ba02670b`  
		Last Modified: Thu, 19 Oct 2023 08:33:42 GMT  
		Size: 12.5 MB (12453238 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3459080ba272e7ff461d3a38189a5b310e79ad2440b12145832e6c1d14b8834a`  
		Last Modified: Thu, 19 Oct 2023 08:33:41 GMT  
		Size: 100.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:987c3a7be955efe4151431e4fa7611ac8d9e7dfa17199f6e64bf1452fcb0d3db`  
		Last Modified: Thu, 19 Oct 2023 08:33:41 GMT  
		Size: 573.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redis:7-alpine3.18` - unknown; unknown

```console
$ docker pull redis@sha256:2aced6443738ed5ad44105596bdb6deb2ae47547672fa4b9858c7b9b9be8d8f0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **752.6 KB (752561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f365323684770f8e7723aafd8abde19fee38d195b9628f3b08e223b32899975`

```dockerfile
```

-	Layers:
	-	`sha256:34502cff934d776dcd1528fa6879c6eb2197472fba5e6c81b46f9096d25b9d8d`  
		Last Modified: Thu, 19 Oct 2023 08:33:41 GMT  
		Size: 726.5 KB (726455 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:20b7bcb88a4df89c3a93910159148a0bc5e844a80a4dc31d1b7f203f563fd0a2`  
		Last Modified: Thu, 19 Oct 2023 08:33:41 GMT  
		Size: 26.1 KB (26106 bytes)  
		MIME: application/vnd.in-toto+json

### `redis:7-alpine3.18` - linux; 386

```console
$ docker pull redis@sha256:31e4edc3fd1c570f3b7cf008354ed8640a20c40c07c7ef95236581dca145c4b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.5 MB (15482834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21af0f9fa0f8ea421fdc20b983e5d43256e46c3ac9a4df9b1c799809d98392b3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 28 Sep 2023 20:38:19 GMT
ADD file:8402753f294e403e92353bd65c86a6428c960be5116c0a15484b663a84f66fcd in / 
# Thu, 28 Sep 2023 20:38:20 GMT
CMD ["/bin/sh"]
# Wed, 18 Oct 2023 09:03:13 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
ENV REDIS_VERSION=7.2.2
# Wed, 18 Oct 2023 09:03:13 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.2.2.tar.gz
# Wed, 18 Oct 2023 09:03:13 GMT
ENV REDIS_DOWNLOAD_SHA=ca999be08800edc6d265379c4c7aafad92f0ee400692e4e2d69829ab4b4c3d08
# Wed, 18 Oct 2023 09:03:13 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
RUN mkdir /data && chown redis:redis /data # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
VOLUME [/data]
# Wed, 18 Oct 2023 09:03:13 GMT
WORKDIR /data
# Wed, 18 Oct 2023 09:03:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Oct 2023 09:03:13 GMT
EXPOSE map[6379/tcp:{}]
# Wed, 18 Oct 2023 09:03:13 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:dc95107ad2a031a015320bb397f73ec151d738127175b31ad643120697dc7e90`  
		Last Modified: Thu, 28 Sep 2023 20:39:32 GMT  
		Size: 3.2 MB (3235757 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a3ed283d16ea7da6df0e955f810835fa6fc1f25e0aaff52196ec14553c9c2f8a`  
		Last Modified: Thu, 19 Oct 2023 01:03:56 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:09eaaa97ec7da3470c167f110fb7cb0e5ba0a28730f6c991b68a923f890d5970`  
		Last Modified: Thu, 19 Oct 2023 01:03:56 GMT  
		Size: 347.4 KB (347378 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:32b61e8abaa11d1df5f019323f4c85bd3aac924eab6655b4417c8c678643bea5`  
		Last Modified: Thu, 19 Oct 2023 01:03:57 GMT  
		Size: 11.9 MB (11897745 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7d61f873c75c64e4767322ecb20a8539dfe1b4b93f3e53605da13511bd625982`  
		Last Modified: Thu, 19 Oct 2023 01:03:56 GMT  
		Size: 99.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:260c44bcdf74f5fd1f7c3731ed2e092767fecbf61d02dd409693c1becc4d5fca`  
		Last Modified: Thu, 19 Oct 2023 01:03:57 GMT  
		Size: 578.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redis:7-alpine3.18` - unknown; unknown

```console
$ docker pull redis@sha256:e191a0a65754c3b4c59c39f13558b50611ff8cb470153f569d14feaaec661624
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 KB (25981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebe07b6a7b6d7847b30e2351eca635fa0e184ccba27806825b38f701c7ad7029`

```dockerfile
```

-	Layers:
	-	`sha256:3a8b872642224e2743af51f8fd9e9ff87dc2f394edbcc89e583c4e64189a91c8`  
		Last Modified: Thu, 19 Oct 2023 01:03:56 GMT  
		Size: 26.0 KB (25981 bytes)  
		MIME: application/vnd.in-toto+json

### `redis:7-alpine3.18` - linux; ppc64le

```console
$ docker pull redis@sha256:e428e036b0ef95c7a2464bfe1bb04a6d0c7578f448e759fab2fc94357f2bc389
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16845157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f8b9a9327e092c21330b8674e406e6cf6d3b127d0244f1ccff8cd4e4211f201`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Wed, 18 Oct 2023 09:03:13 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
ENV REDIS_VERSION=7.2.2
# Wed, 18 Oct 2023 09:03:13 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.2.2.tar.gz
# Wed, 18 Oct 2023 09:03:13 GMT
ENV REDIS_DOWNLOAD_SHA=ca999be08800edc6d265379c4c7aafad92f0ee400692e4e2d69829ab4b4c3d08
# Wed, 18 Oct 2023 09:03:13 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
RUN mkdir /data && chown redis:redis /data # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
VOLUME [/data]
# Wed, 18 Oct 2023 09:03:13 GMT
WORKDIR /data
# Wed, 18 Oct 2023 09:03:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Oct 2023 09:03:13 GMT
EXPOSE map[6379/tcp:{}]
# Wed, 18 Oct 2023 09:03:13 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e963944e7d7c85e7e5202f0596efabc5d145dfc37f6e0a9b481b7e185470e576`  
		Last Modified: Tue, 03 Oct 2023 23:04:16 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d5c07f1f59e5142c61f551a02105a3fe01c28e7ae009ba3c9ef69dc54d2c90a8`  
		Last Modified: Tue, 03 Oct 2023 23:04:16 GMT  
		Size: 347.6 KB (347649 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ab04e2ae1208c061ac9d662585939ba670137d75236b33b743c6255fa3c2a70d`  
		Last Modified: Thu, 19 Oct 2023 02:25:09 GMT  
		Size: 13.1 MB (13149048 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:80a7e1b6bd14f5aac67c8f7ba90e1b7eaa391c85cec0ffc64b035ce9afb166b2`  
		Last Modified: Thu, 19 Oct 2023 02:25:07 GMT  
		Size: 101.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fc6af823d3db5d682de4e4cae4adf355197867f80342df36e3ce35bbfe9a7666`  
		Last Modified: Thu, 19 Oct 2023 02:25:08 GMT  
		Size: 574.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redis:7-alpine3.18` - unknown; unknown

```console
$ docker pull redis@sha256:cb400dd59df184c16fe3fe4622563c352704806126f0999571fd3e926b803b99
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **750.7 KB (750727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c48dabe305576593cc1624b2206509d85f6246d7808429631ea74c760b557d63`

```dockerfile
```

-	Layers:
	-	`sha256:7deaa752c184846f25bb499a64366812f0cb8c03d74832d8d0a74e8a14a5c0e9`  
		Last Modified: Thu, 19 Oct 2023 02:25:08 GMT  
		Size: 724.6 KB (724572 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:0a4a8f4b1cbfcabc0deb33cb25a0e0877914b80703caa7ad266fa4a3e64a019e`  
		Last Modified: Thu, 19 Oct 2023 02:25:07 GMT  
		Size: 26.2 KB (26155 bytes)  
		MIME: application/vnd.in-toto+json

### `redis:7-alpine3.18` - linux; s390x

```console
$ docker pull redis@sha256:e671056e126080382e7fdd12ee2bfa6f352f23f2aef217a7828f1d955d323a68
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.2 MB (16211517 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6da9b36807244accdcd2f9a976023f99fd5922c861bcaa26542da38626089d94`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Wed, 18 Oct 2023 09:03:13 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
ENV REDIS_VERSION=7.2.2
# Wed, 18 Oct 2023 09:03:13 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.2.2.tar.gz
# Wed, 18 Oct 2023 09:03:13 GMT
ENV REDIS_DOWNLOAD_SHA=ca999be08800edc6d265379c4c7aafad92f0ee400692e4e2d69829ab4b4c3d08
# Wed, 18 Oct 2023 09:03:13 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
RUN mkdir /data && chown redis:redis /data # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
VOLUME [/data]
# Wed, 18 Oct 2023 09:03:13 GMT
WORKDIR /data
# Wed, 18 Oct 2023 09:03:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 18 Oct 2023 09:03:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Oct 2023 09:03:13 GMT
EXPOSE map[6379/tcp:{}]
# Wed, 18 Oct 2023 09:03:13 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2f8fb319e3e2b6d090a150207805753dae05abe1df53b9dae9b211d46986bb8e`  
		Last Modified: Tue, 03 Oct 2023 23:15:31 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8b8fdacac4cf0c35819b1f0be78d8bed53f4dfdce11d17b3918d554a29299129`  
		Last Modified: Tue, 03 Oct 2023 23:15:31 GMT  
		Size: 347.4 KB (347360 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:efb972e3a4f29c2cb43c7194d56da0535ce1d380d51355b7dcbed219b63fbc52`  
		Last Modified: Thu, 19 Oct 2023 02:53:57 GMT  
		Size: 12.6 MB (12647104 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:eb8c6bc1b25e10e7d187e7177a2d13bba22ec2975c5534d42a67a2ebbb416a3d`  
		Last Modified: Thu, 19 Oct 2023 02:53:57 GMT  
		Size: 100.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:20e1d300e53543f38ae4a314255649f4844c5f25bbeb0b0b7fb0631aa3a6f315`  
		Last Modified: Thu, 19 Oct 2023 02:53:57 GMT  
		Size: 575.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redis:7-alpine3.18` - unknown; unknown

```console
$ docker pull redis@sha256:7577f4551dca1991a6a42d47303e58a18c9eff35ed3ffc69b7f07eafd17e5e86
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **750.6 KB (750590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c090913a6cc74cf7a4730672dd984c0f8391e8cd3462819566dd185c9749174`

```dockerfile
```

-	Layers:
	-	`sha256:b2947b09b725fb11cdbcf7c02d14fd0df0a783edd10570d64d5b388885ce8aeb`  
		Last Modified: Thu, 19 Oct 2023 02:53:57 GMT  
		Size: 724.5 KB (724502 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:318aada70c03ceab5b30afbad58ca06a7a10ceec7a4173a5e87d8759db8ad35c`  
		Last Modified: Thu, 19 Oct 2023 02:53:56 GMT  
		Size: 26.1 KB (26088 bytes)  
		MIME: application/vnd.in-toto+json
