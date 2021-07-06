## `redis:5-alpine3.14`

```console
$ docker pull redis@sha256:c720d5c0f8fd75ddb82bd527da141199b98d4dcbe875cf2cf3cdb26dde134708
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; 386

### `redis:5-alpine3.14` - linux; amd64

```console
$ docker pull redis@sha256:afe2d89d3167f766189ce0afde55be2f1cab459423368b985552b9be1e01122f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.8 MB (9840968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51bbd55867dd975a18bf5bc650fd96ef641952f9662459607ed3bf0d006a380c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Tue, 06 Jul 2021 17:54:35 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Tue, 06 Jul 2021 17:54:36 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Tue, 06 Jul 2021 17:57:20 GMT
ENV REDIS_VERSION=5.0.12
# Tue, 06 Jul 2021 17:57:20 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.12.tar.gz
# Tue, 06 Jul 2021 17:57:21 GMT
ENV REDIS_DOWNLOAD_SHA=7040eba5910f7c3d38f05ea5a1d88b480488215bdbd2e10ec70d18380108e31e
# Tue, 06 Jul 2021 17:58:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Tue, 06 Jul 2021 17:58:17 GMT
RUN mkdir /data && chown redis:redis /data
# Tue, 06 Jul 2021 17:58:17 GMT
VOLUME [/data]
# Tue, 06 Jul 2021 17:58:17 GMT
WORKDIR /data
# Tue, 06 Jul 2021 17:58:17 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Tue, 06 Jul 2021 17:58:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Jul 2021 17:58:18 GMT
EXPOSE 6379
# Tue, 06 Jul 2021 17:58:18 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db2305878ef924f3ebdc23c7f93c84e1406eca01618c945f859736bccd4692d`  
		Last Modified: Tue, 06 Jul 2021 17:59:24 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3558750a1d54c99f919b839c9dde5afd8f769bd3afee3f0f6ec1b9b451fde5e7`  
		Last Modified: Tue, 06 Jul 2021 17:59:24 GMT  
		Size: 384.4 KB (384421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8afb5c59cd2c853808d96058c45127adce02509dc5aa271813885fb6009e2cb`  
		Last Modified: Tue, 06 Jul 2021 18:00:25 GMT  
		Size: 6.6 MB (6643254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc5f4327098aab27e926123244c050e0d795f61352b3b90bbe73318692961dc`  
		Last Modified: Tue, 06 Jul 2021 18:00:23 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f27610209d4b92c6630aa25576f2b357587ff5496310423fbde4333faee59d6`  
		Last Modified: Tue, 06 Jul 2021 18:00:23 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-alpine3.14` - linux; arm variant v6

```console
$ docker pull redis@sha256:5135998e111b71791595e761d9780e8313e07e2383837570e0fb55dfe6f9063e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9582631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f018096d13ed98777c3a4b2198747e7d0160d9d96fbda6d7e960398f374ddc50`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:26 GMT
ADD file:c80bc2b093cbc0fc466582ef21cbed377de9fa874aedbf320079525ddacd1200 in / 
# Tue, 15 Jun 2021 22:57:26 GMT
CMD ["/bin/sh"]
# Tue, 06 Jul 2021 17:03:28 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Tue, 06 Jul 2021 17:03:31 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Tue, 06 Jul 2021 17:06:37 GMT
ENV REDIS_VERSION=5.0.12
# Tue, 06 Jul 2021 17:06:38 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.12.tar.gz
# Tue, 06 Jul 2021 17:06:38 GMT
ENV REDIS_DOWNLOAD_SHA=7040eba5910f7c3d38f05ea5a1d88b480488215bdbd2e10ec70d18380108e31e
# Tue, 06 Jul 2021 17:07:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Tue, 06 Jul 2021 17:07:45 GMT
RUN mkdir /data && chown redis:redis /data
# Tue, 06 Jul 2021 17:07:45 GMT
VOLUME [/data]
# Tue, 06 Jul 2021 17:07:46 GMT
WORKDIR /data
# Tue, 06 Jul 2021 17:07:46 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Tue, 06 Jul 2021 17:07:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Jul 2021 17:07:47 GMT
EXPOSE 6379
# Tue, 06 Jul 2021 17:07:47 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:b4c9a0924271af3466de27804af26420eb58da1466e7eaaba127d178b380fea3`  
		Last Modified: Tue, 15 Jun 2021 22:58:47 GMT  
		Size: 2.6 MB (2624382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597047ceadae07829fd8b80127f94d3d69704d627c57bb16d7e83c9def767301`  
		Last Modified: Tue, 06 Jul 2021 17:09:20 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570997ff334916737428e81b30711552ca4fab99d9025f566edcf44c3e13ca1e`  
		Last Modified: Tue, 06 Jul 2021 17:09:21 GMT  
		Size: 388.4 KB (388435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afb959d22171e488eabdc06392dd9eeef580c563909c71fa03dd45b45d130fb2`  
		Last Modified: Tue, 06 Jul 2021 17:10:32 GMT  
		Size: 6.6 MB (6567998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98e07799beaadc6c3a3c625c8a2fabd186530a79201582705877b5326c45e264`  
		Last Modified: Tue, 06 Jul 2021 17:10:28 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26620602ff6992381c520e49611a06ef4e1131851ba9232da77f7f950f72c7e2`  
		Last Modified: Tue, 06 Jul 2021 17:10:28 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-alpine3.14` - linux; arm variant v7

```console
$ docker pull redis@sha256:2e58ce79352da9c0570169adee5dc8f226eca98e62a1140551e5368ca55bc4d8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9277993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3719cfbc845aae2a1dd0f3c68f712a9b7c944650d6d34fbf928cc59bad8fe3bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:05 GMT
ADD file:416a8b507abdc6bdcb22997a4be0a4170796c3f9f77e315b2dbff2b0a212bc68 in / 
# Tue, 15 Jun 2021 23:15:06 GMT
CMD ["/bin/sh"]
# Tue, 06 Jul 2021 18:09:03 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Tue, 06 Jul 2021 18:09:08 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Tue, 06 Jul 2021 18:13:36 GMT
ENV REDIS_VERSION=5.0.12
# Tue, 06 Jul 2021 18:13:37 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.12.tar.gz
# Tue, 06 Jul 2021 18:13:38 GMT
ENV REDIS_DOWNLOAD_SHA=7040eba5910f7c3d38f05ea5a1d88b480488215bdbd2e10ec70d18380108e31e
# Tue, 06 Jul 2021 18:14:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Tue, 06 Jul 2021 18:14:52 GMT
RUN mkdir /data && chown redis:redis /data
# Tue, 06 Jul 2021 18:14:53 GMT
VOLUME [/data]
# Tue, 06 Jul 2021 18:14:54 GMT
WORKDIR /data
# Tue, 06 Jul 2021 18:14:56 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Tue, 06 Jul 2021 18:14:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Jul 2021 18:14:58 GMT
EXPOSE 6379
# Tue, 06 Jul 2021 18:14:59 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:136482bf81d1fa351b424ebb8c7e34d15f2c5ed3fc0b66b544b8312bda3d52d9`  
		Last Modified: Tue, 15 Jun 2021 23:16:40 GMT  
		Size: 2.4 MB (2427917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e6ae5782522d489b98cc4cf0217b5ebdc53a69e00fb48e9f17256e53036e0c`  
		Last Modified: Tue, 06 Jul 2021 18:18:30 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66778e3445c034f863fc933b171106e21d3fcca76fe28d94af1b1f17aa19e5fd`  
		Last Modified: Tue, 06 Jul 2021 18:18:30 GMT  
		Size: 383.2 KB (383231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a300ee30c795d0cc6534fe79bfb079b924c045ec5457717dbfd01bea3835e4`  
		Last Modified: Tue, 06 Jul 2021 18:19:52 GMT  
		Size: 6.5 MB (6465026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733c1e783b2bfcf183a98a67bfd368e2bb45344f01871df3e233bc73df3841b9`  
		Last Modified: Tue, 06 Jul 2021 18:19:48 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a21c6c648dc4e81ea43e8359541476176f52ecb3d5602e7651eb9368b0f07ab`  
		Last Modified: Tue, 06 Jul 2021 18:19:48 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-alpine3.14` - linux; 386

```console
$ docker pull redis@sha256:352bedbd87cf68edf4a75fa1b12ecf462e767a2e802b2b73e093624edb503790
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9572676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:179062366aa5b37e41f2e9a78f22d25ed78b590fedb8a9aa3b88d68c3af61e1a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Tue, 15 Jun 2021 21:38:30 GMT
ADD file:3b0fe1454491bb05e218b090fd461f2fd39546aa4a53eb3f953ee8eae149ac57 in / 
# Tue, 15 Jun 2021 21:38:30 GMT
CMD ["/bin/sh"]
# Tue, 06 Jul 2021 17:58:37 GMT
RUN addgroup -S -g 1000 redis && adduser -S -G redis -u 999 redis
# Tue, 06 Jul 2021 17:58:39 GMT
RUN apk add --no-cache 		'su-exec>=0.2' 		tzdata
# Tue, 06 Jul 2021 18:01:42 GMT
ENV REDIS_VERSION=5.0.12
# Tue, 06 Jul 2021 18:01:42 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.12.tar.gz
# Tue, 06 Jul 2021 18:01:42 GMT
ENV REDIS_DOWNLOAD_SHA=7040eba5910f7c3d38f05ea5a1d88b480488215bdbd2e10ec70d18380108e31e
# Tue, 06 Jul 2021 18:02:50 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		dpkg-dev dpkg 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 		wget 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Tue, 06 Jul 2021 18:02:52 GMT
RUN mkdir /data && chown redis:redis /data
# Tue, 06 Jul 2021 18:02:52 GMT
VOLUME [/data]
# Tue, 06 Jul 2021 18:02:52 GMT
WORKDIR /data
# Tue, 06 Jul 2021 18:02:52 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Tue, 06 Jul 2021 18:02:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Jul 2021 18:02:53 GMT
EXPOSE 6379
# Tue, 06 Jul 2021 18:02:53 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:be21df321efb39c5daf3151073ebff7688e15ea6cd5158878bc9559a5db76ac6`  
		Last Modified: Tue, 15 Jun 2021 21:39:16 GMT  
		Size: 2.8 MB (2820718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2551de8396d4fcd47753ef4d9beb999c0b7ea922e5a92009681b6f94f5c0506b`  
		Last Modified: Tue, 06 Jul 2021 18:04:37 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec7f9665c61bd95041cf22f6ce770b5e8bbbbbad420a7eb1f7566217c27198d8`  
		Last Modified: Tue, 06 Jul 2021 18:04:37 GMT  
		Size: 390.8 KB (390807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0a1f6d5139539ef032bae16dc836795fb323bb5c2814e762a57f2d863b65b12`  
		Last Modified: Tue, 06 Jul 2021 18:05:44 GMT  
		Size: 6.4 MB (6359336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c06fed275b9bbadc7399b8cb2b25c566f46b46e4e6c3518c41fe11cc6a51d4`  
		Last Modified: Tue, 06 Jul 2021 18:05:42 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ea3dea4df2776fb0421b527b213e0cae227833b4f72ef51655d289d122e9c9e`  
		Last Modified: Tue, 06 Jul 2021 18:05:42 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
