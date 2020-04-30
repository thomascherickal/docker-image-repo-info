<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `redis`

-	[`redis:5`](#redis5)
-	[`redis:5.0`](#redis50)
-	[`redis:5.0-32bit`](#redis50-32bit)
-	[`redis:5.0-32bit-buster`](#redis50-32bit-buster)
-	[`redis:5.0.9`](#redis509)
-	[`redis:5.0.9-32bit`](#redis509-32bit)
-	[`redis:5.0.9-32bit-buster`](#redis509-32bit-buster)
-	[`redis:5.0.9-alpine`](#redis509-alpine)
-	[`redis:5.0.9-alpine3.11`](#redis509-alpine311)
-	[`redis:5.0.9-buster`](#redis509-buster)
-	[`redis:5.0-alpine`](#redis50-alpine)
-	[`redis:5.0-alpine3.11`](#redis50-alpine311)
-	[`redis:5.0-buster`](#redis50-buster)
-	[`redis:5-32bit`](#redis5-32bit)
-	[`redis:5-32bit-buster`](#redis5-32bit-buster)
-	[`redis:5-alpine`](#redis5-alpine)
-	[`redis:5-alpine3.11`](#redis5-alpine311)
-	[`redis:5-buster`](#redis5-buster)
-	[`redis:6`](#redis6)
-	[`redis:6.0`](#redis60)
-	[`redis:6.0.0`](#redis600)
-	[`redis:6.0.0-alpine`](#redis600-alpine)
-	[`redis:6.0.0-alpine3.11`](#redis600-alpine311)
-	[`redis:6.0.0-buster`](#redis600-buster)
-	[`redis:6.0-alpine`](#redis60-alpine)
-	[`redis:6.0-alpine3.11`](#redis60-alpine311)
-	[`redis:6.0-buster`](#redis60-buster)
-	[`redis:6-alpine`](#redis6-alpine)
-	[`redis:6-alpine3.11`](#redis6-alpine311)
-	[`redis:6-buster`](#redis6-buster)
-	[`redis:alpine`](#redisalpine)
-	[`redis:alpine3.11`](#redisalpine311)
-	[`redis:buster`](#redisbuster)
-	[`redis:latest`](#redislatest)

## `redis:5`

```console
$ docker pull redis@sha256:157a95b41b0dca8c308a33489dfdb28019e033110320414b4b16fad7d28c0f9f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `redis:5` - linux; amd64

```console
$ docker pull redis@sha256:43dbbe6f633572d66e84e7162245d8d70a18f00b819d6c0bf98ca02109f4788c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35863297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4d3716dbb72408a7843e12d7d9f6a5addf7ab28ac21e9e9da4a6a51f1b32da9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:20:32 GMT
ADD file:9b8be2b52ee0fa31da1b6256099030b73546253a57e94cccb24605cd888bb74d in / 
# Thu, 23 Apr 2020 00:20:32 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 19:48:34 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 19:48:34 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 19:48:46 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 19:50:08 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 19:50:08 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 19:50:08 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 19:51:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 19:51:26 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 19:51:26 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 19:51:27 GMT
WORKDIR /data
# Thu, 23 Apr 2020 19:51:27 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 19:51:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 19:51:28 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 19:51:28 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:54fec2fa59d0a0de9cd2dec9850b36c43de451f1fd1c0a5bf8f1cf26a61a5da4`  
		Last Modified: Thu, 23 Apr 2020 00:25:10 GMT  
		Size: 27.1 MB (27098254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c94e11103d92f2a83b82e5d4287445cba073af0002cecee98d85d68ccec0f89`  
		Last Modified: Thu, 23 Apr 2020 19:55:42 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ab1bfc453f19989c401c2f0622df3363b5182bdea1af9e59ee2ceea3a9931c`  
		Last Modified: Thu, 23 Apr 2020 19:55:43 GMT  
		Size: 1.4 MB (1417711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f71e6b94d83f5a0df5d032ce4998b4834287bd4ed307ff7c9a31ad0a60caa98`  
		Last Modified: Thu, 23 Apr 2020 19:55:55 GMT  
		Size: 7.3 MB (7345094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2729a8234dd5e724571528d78d5f581702abc77be39db93fc0ae741340eb1c18`  
		Last Modified: Thu, 23 Apr 2020 19:55:53 GMT  
		Size: 97.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2683d7f177455cf86b4cf424cc757f1d177d5772df77bdaeeace411006eb88a5`  
		Last Modified: Thu, 23 Apr 2020 19:55:53 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5` - linux; arm variant v5

```console
$ docker pull redis@sha256:5a474d0e7c55a7e45ddaf530f4f2ab4bc8dcaba6d85b0829f1121f7fe53414fd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.4 MB (33394023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b83a1e222e2b9be5acf1ae9a03cd2e6d2c7a4efcd3b73a275481c652552de80`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:52:22 GMT
ADD file:62a9732be4e3237ccc896f724a34606e01f351c4877e52c9a9cd85029c06b956 in / 
# Thu, 23 Apr 2020 00:52:23 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 09:33:20 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 09:33:21 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 09:33:56 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 09:35:38 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 09:35:39 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 09:35:39 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 09:36:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 09:36:48 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 09:36:48 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 09:36:49 GMT
WORKDIR /data
# Thu, 23 Apr 2020 09:36:50 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 09:36:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 09:36:51 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 09:36:52 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:a8c46e5952878f9f324df86c5a2b45b2e0020f6721e820981e74461d77a100dd`  
		Last Modified: Thu, 23 Apr 2020 00:59:50 GMT  
		Size: 24.8 MB (24836319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471287e557b84038803c3a26dee3987da48cbcae6529a77a28f486e4527757f7`  
		Last Modified: Thu, 23 Apr 2020 09:39:42 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:016e8ff197695f0c8e2c3ae127ac9459df9c71e52ae54500970e692d2799c944`  
		Last Modified: Thu, 23 Apr 2020 09:39:42 GMT  
		Size: 1.4 MB (1376131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd64ec452edc906dc611493aae3c90529a0d5787d8dc3b8c1088b41b53379d2d`  
		Last Modified: Thu, 23 Apr 2020 09:40:07 GMT  
		Size: 7.2 MB (7179305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ca72abe00cf1354dc501a32ed89705fdacd4905631c42186458d9d3202cc90`  
		Last Modified: Thu, 23 Apr 2020 09:40:05 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e7807337a06858bed0eac541f5935b123a4abb0d973dacb1973753c6dcb2469`  
		Last Modified: Thu, 23 Apr 2020 09:40:04 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5` - linux; arm variant v7

```console
$ docker pull redis@sha256:afc097fd6784e016756816ecc4ae33dc9ef22f5715db3593b90b7ec17e906edf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.1 MB (31109340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:632cd87ac6e4d8bda115f5e32e2b45cb8e28c59bd4c6e24b87985cf6b1f93354`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 01:03:26 GMT
ADD file:db6122b36f3e70c5f490b50afba99d49fa345f11d0f5c77bb3c6749f8e2a4f81 in / 
# Thu, 23 Apr 2020 01:03:28 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 13:54:58 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 13:54:59 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 13:55:22 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 13:57:35 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 13:57:35 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 13:57:36 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 13:58:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 13:58:37 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 13:58:38 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 13:58:39 GMT
WORKDIR /data
# Thu, 23 Apr 2020 13:58:39 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 13:58:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 13:58:41 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 13:58:41 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:50fb0052086928803f00724ca465c89c45dde5b082b1e59dadb8101286dd5ab6`  
		Last Modified: Thu, 23 Apr 2020 01:11:08 GMT  
		Size: 22.7 MB (22705377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98fc1f5e139d98aa45f74dfddb32ca22bec51ecf2fcab9bb372d91c14cc971d2`  
		Last Modified: Thu, 23 Apr 2020 14:00:18 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa98edd0b4c481052caeb348af3e906ef75764353840cfe2518af73963fcf2d`  
		Last Modified: Thu, 23 Apr 2020 14:00:18 GMT  
		Size: 1.4 MB (1368177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1ae9f68f12644f241fb270f9baf2e62d5b1380083acada1fdae86374998430`  
		Last Modified: Thu, 23 Apr 2020 14:00:21 GMT  
		Size: 7.0 MB (7033517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a23909059832233f41bcba599ec5bb698e278c652cf313dc6e8724fae8aa40cf`  
		Last Modified: Thu, 23 Apr 2020 14:00:19 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f5f6de32828cf1cb128a0cba17dc0396dead74aa6cc963394ac4f8b05540179`  
		Last Modified: Thu, 23 Apr 2020 14:00:18 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:be463e278dc2125ea4c8984cd6a990353dfaa7f94570856734f86b900debc008
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 MB (34548547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0da52d2315939d969b12f3db6ae0aa5716074833f1ef06a42a544aec452d0ab2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:54:55 GMT
ADD file:581ee9c3c19f0d971aeda008fd399f59171cae75e8936b967dbf3888db4fc0d0 in / 
# Thu, 23 Apr 2020 00:54:58 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 16:01:56 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 16:01:57 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 16:02:29 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 16:04:19 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 16:04:20 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 16:04:20 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 16:05:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 16:05:20 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 16:05:20 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 16:05:21 GMT
WORKDIR /data
# Thu, 23 Apr 2020 16:05:21 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 16:05:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 16:05:22 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 16:05:24 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:bdc84a41f2513e28e99efeff9fcbb196b7df9883fb30532184bd67ca415b4673`  
		Last Modified: Thu, 23 Apr 2020 01:03:27 GMT  
		Size: 25.9 MB (25857800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698d3e76f19fb83cee90fe071552d86509322f0b8316774550c1ea7398327369`  
		Last Modified: Thu, 23 Apr 2020 16:07:31 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac4bbea6248caf60d5eca4d3e15d73d9cc18a5154a795c5ca3937eb040c9daae`  
		Last Modified: Thu, 23 Apr 2020 16:07:31 GMT  
		Size: 1.4 MB (1352987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1590123d45656fbb5cabd427b87908fd7347ef2fc6b0fba354f2b83771ec8882`  
		Last Modified: Thu, 23 Apr 2020 16:07:57 GMT  
		Size: 7.3 MB (7335481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e21891406b8ecd80c9cc4be90337cdd8d8935229002e8162d9afc9b68d2a4c30`  
		Last Modified: Thu, 23 Apr 2020 16:07:55 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d793eb07a5bc754267edbd54feb6cb25e4c28e7056a87e27960de4901d1dcc3`  
		Last Modified: Thu, 23 Apr 2020 16:07:55 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5` - linux; 386

```console
$ docker pull redis@sha256:0ac1dbfd6ca80b45aa587ecaa0632457ca254eea674a50e8574e8677f7a193a0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.2 MB (36151602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34c763545c4e57aabcdc00c9448e439a81bdaf47ae32d7711bc8e1252fb7ef59`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:39:36 GMT
ADD file:ca6a74f6b738c738c033152fab2a9aacf22bec5f19a994e6a02b5f919ee33ee9 in / 
# Thu, 23 Apr 2020 00:39:36 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 11:23:53 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 11:23:53 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 11:24:11 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 11:26:28 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 11:26:28 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 11:26:28 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 11:27:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 11:27:59 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 11:28:00 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 11:28:00 GMT
WORKDIR /data
# Thu, 23 Apr 2020 11:28:00 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 11:28:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 11:28:01 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 11:28:01 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:5d3da8f33b97fc107a05b3255a55836b76df9f817de632b1fb63c6e9c024f0df`  
		Last Modified: Thu, 23 Apr 2020 00:44:35 GMT  
		Size: 27.8 MB (27753972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f572d913eaf53def72d8eeff5384464ae75f0da9041d63ef0cd2fb2a43e21e`  
		Last Modified: Thu, 23 Apr 2020 11:30:12 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36c13a7e7929be4f05fbeddd74c94dfe85b704c504f7d13aa45bdb84bae79ccb`  
		Last Modified: Thu, 23 Apr 2020 11:30:12 GMT  
		Size: 1.4 MB (1387411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680a9b72444c93256224c2c5394c18343047b8b7dc305a4301401e7a6b494d03`  
		Last Modified: Thu, 23 Apr 2020 11:30:25 GMT  
		Size: 7.0 MB (7007988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e6148f8fb3eb037aaf97a9736b49d92d77541c5bbb6219db62f8af4f8d5e54`  
		Last Modified: Thu, 23 Apr 2020 11:30:23 GMT  
		Size: 97.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fae33d9962de4399f135693d495b300515e9d363f74683c3c366cd6e32290e1`  
		Last Modified: Thu, 23 Apr 2020 11:30:23 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5` - linux; mips64le

```console
$ docker pull redis@sha256:8860ea6be85bfa12a7a62f37e07716f197be8e76f498d1e62d3c4319582a3b60
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34731728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eab8ac536ee15de9306c977271c71a293db05c67e582fe002279ba86c8fff0a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:09:47 GMT
ADD file:7509945bd8a224048260e88b466aa3b156615e16b64e0a6702da277052fcb98b in / 
# Thu, 23 Apr 2020 00:09:48 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 09:24:32 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 09:24:33 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 09:25:02 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 09:28:42 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 09:28:42 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 09:28:43 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 09:31:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 09:32:01 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 09:32:01 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 09:32:01 GMT
WORKDIR /data
# Thu, 23 Apr 2020 09:32:02 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 09:32:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 09:32:02 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 09:32:03 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:ae8f0fa6cb0d971b4b8fedf7fc9b00f61f780b383fe7d64e6c2e4be8d20c3987`  
		Last Modified: Thu, 23 Apr 2020 00:17:46 GMT  
		Size: 25.8 MB (25762125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faf65c067540cd52d99f7f6df4511fb45d6a0485e47338d0239a052fcd64c8e3`  
		Last Modified: Thu, 23 Apr 2020 09:34:32 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef207bf80aefb18eba12c119d07499e37b5ea7bec06bc1e0c2dd749ddde45a1`  
		Last Modified: Thu, 23 Apr 2020 09:34:34 GMT  
		Size: 1.3 MB (1305489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae62dd92cc34f4856c15b7614910c5578f2d91d96d96469c21f8ca741c1061f5`  
		Last Modified: Thu, 23 Apr 2020 09:35:08 GMT  
		Size: 7.7 MB (7661872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693fe2f4d6e93636c838f7fb3a49c859d72138e5a25fd1687e590fcf3bb74dfb`  
		Last Modified: Thu, 23 Apr 2020 09:35:00 GMT  
		Size: 99.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:153c8eb8631e42a4705a53461aeb1c1edea4a60ad71a759b5eafeccbf3f5c142`  
		Last Modified: Thu, 23 Apr 2020 09:35:00 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5` - linux; ppc64le

```console
$ docker pull redis@sha256:e1c410783ee0d501a9804b3050db559054e95e91bb3cd8f3e81324baef92f730
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.7 MB (39696544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34098209a59e39ee25eeb2b0bf53ba98f873314c75110d6841a0793d5e1bc182`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:36:00 GMT
ADD file:5b3c3d2945800e1743dc02a4f68bd830fe2f67ca437223692eb460147c158c2b in / 
# Thu, 23 Apr 2020 00:36:04 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 17:29:48 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 17:29:51 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 17:31:38 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 17:35:14 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 17:35:18 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 17:35:23 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 17:38:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 17:38:25 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 17:38:28 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 17:38:32 GMT
WORKDIR /data
# Thu, 23 Apr 2020 17:38:34 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 17:38:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 17:38:42 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 17:38:45 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:012c6cdbd1af202bbfbea5945fafbb9aca9097f1fa3cb493a29155fdc02cc43c`  
		Last Modified: Thu, 23 Apr 2020 00:50:14 GMT  
		Size: 30.5 MB (30524638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee5a34bf53dadebb7466557f439affba6f1c11ddbdd7d2c1376f9540c294a7a`  
		Last Modified: Thu, 23 Apr 2020 17:42:03 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dedf97e3c0bcb476732135fc70dee2ba4766ff50ec51f93b1929ebaa6c4863f`  
		Last Modified: Thu, 23 Apr 2020 17:42:03 GMT  
		Size: 1.3 MB (1335327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2a1294a7da3aa34af8f45c22665913b8780fcf4dec6b52b108541e496dd0cc`  
		Last Modified: Thu, 23 Apr 2020 17:42:27 GMT  
		Size: 7.8 MB (7834296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51726f5fc1a7b6d031cad4d822aaf6c1801262570fb662454f1f2dc93cd4e551`  
		Last Modified: Thu, 23 Apr 2020 17:42:25 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e62728fce47996c1059a9f4f18e5e1efea4ebc55e17f82aa362f8985e7f019e`  
		Last Modified: Thu, 23 Apr 2020 17:42:25 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5` - linux; s390x

```console
$ docker pull redis@sha256:80a22e71a515d761d2c50a5873fc228fe165a627f9f91641391ce1548bc23f03
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34709447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5556ba73cac9fdc7f38ea53f8961a08497e52b1fa62f83611a9228a5d495e8fb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:51:48 GMT
ADD file:f6c2560f9185c1bcaff95e576e57449f606d51b85fad02646c1b0962bc9353c9 in / 
# Thu, 23 Apr 2020 00:51:50 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 06:58:44 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 06:58:44 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 06:58:58 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 06:59:46 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 06:59:47 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 06:59:47 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 07:00:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 07:00:24 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 07:00:24 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 07:00:24 GMT
WORKDIR /data
# Thu, 23 Apr 2020 07:00:24 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 07:00:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 07:00:25 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 07:00:25 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:d89dc3741ad42b79c3d8545495c429f3100d3f22234ff993bd04017b0675e868`  
		Last Modified: Thu, 23 Apr 2020 00:56:00 GMT  
		Size: 25.7 MB (25712105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c9894c70b29dc7cbad7e69c5f898b0a5d6f82aac9aff00e2645a6f8a9eff88`  
		Last Modified: Thu, 23 Apr 2020 07:01:34 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fba24ca231c607425b0e92a8a39c3174a8b9cb56ddeee71fc43f2f9dd9b1d2c`  
		Last Modified: Thu, 23 Apr 2020 07:01:35 GMT  
		Size: 1.4 MB (1403679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22d299e81a09eaaf9da803a2b3775444f312a34b2b7dd8e0c1c10d0171225ba`  
		Last Modified: Thu, 23 Apr 2020 07:01:52 GMT  
		Size: 7.6 MB (7591385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46db2cefe8baf230709535dd5f96c93520ca156d9821649ce8e8a2410e49d54`  
		Last Modified: Thu, 23 Apr 2020 07:01:56 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ec0a42c81dfec4356c31366a6ddf246ebac63394fafd37549a4483fd537513`  
		Last Modified: Thu, 23 Apr 2020 07:01:50 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redis:5.0`

```console
$ docker pull redis@sha256:157a95b41b0dca8c308a33489dfdb28019e033110320414b4b16fad7d28c0f9f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `redis:5.0` - linux; amd64

```console
$ docker pull redis@sha256:43dbbe6f633572d66e84e7162245d8d70a18f00b819d6c0bf98ca02109f4788c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35863297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4d3716dbb72408a7843e12d7d9f6a5addf7ab28ac21e9e9da4a6a51f1b32da9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:20:32 GMT
ADD file:9b8be2b52ee0fa31da1b6256099030b73546253a57e94cccb24605cd888bb74d in / 
# Thu, 23 Apr 2020 00:20:32 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 19:48:34 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 19:48:34 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 19:48:46 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 19:50:08 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 19:50:08 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 19:50:08 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 19:51:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 19:51:26 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 19:51:26 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 19:51:27 GMT
WORKDIR /data
# Thu, 23 Apr 2020 19:51:27 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 19:51:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 19:51:28 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 19:51:28 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:54fec2fa59d0a0de9cd2dec9850b36c43de451f1fd1c0a5bf8f1cf26a61a5da4`  
		Last Modified: Thu, 23 Apr 2020 00:25:10 GMT  
		Size: 27.1 MB (27098254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c94e11103d92f2a83b82e5d4287445cba073af0002cecee98d85d68ccec0f89`  
		Last Modified: Thu, 23 Apr 2020 19:55:42 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ab1bfc453f19989c401c2f0622df3363b5182bdea1af9e59ee2ceea3a9931c`  
		Last Modified: Thu, 23 Apr 2020 19:55:43 GMT  
		Size: 1.4 MB (1417711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f71e6b94d83f5a0df5d032ce4998b4834287bd4ed307ff7c9a31ad0a60caa98`  
		Last Modified: Thu, 23 Apr 2020 19:55:55 GMT  
		Size: 7.3 MB (7345094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2729a8234dd5e724571528d78d5f581702abc77be39db93fc0ae741340eb1c18`  
		Last Modified: Thu, 23 Apr 2020 19:55:53 GMT  
		Size: 97.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2683d7f177455cf86b4cf424cc757f1d177d5772df77bdaeeace411006eb88a5`  
		Last Modified: Thu, 23 Apr 2020 19:55:53 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5.0` - linux; arm variant v5

```console
$ docker pull redis@sha256:5a474d0e7c55a7e45ddaf530f4f2ab4bc8dcaba6d85b0829f1121f7fe53414fd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.4 MB (33394023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b83a1e222e2b9be5acf1ae9a03cd2e6d2c7a4efcd3b73a275481c652552de80`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:52:22 GMT
ADD file:62a9732be4e3237ccc896f724a34606e01f351c4877e52c9a9cd85029c06b956 in / 
# Thu, 23 Apr 2020 00:52:23 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 09:33:20 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 09:33:21 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 09:33:56 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 09:35:38 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 09:35:39 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 09:35:39 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 09:36:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 09:36:48 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 09:36:48 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 09:36:49 GMT
WORKDIR /data
# Thu, 23 Apr 2020 09:36:50 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 09:36:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 09:36:51 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 09:36:52 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:a8c46e5952878f9f324df86c5a2b45b2e0020f6721e820981e74461d77a100dd`  
		Last Modified: Thu, 23 Apr 2020 00:59:50 GMT  
		Size: 24.8 MB (24836319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471287e557b84038803c3a26dee3987da48cbcae6529a77a28f486e4527757f7`  
		Last Modified: Thu, 23 Apr 2020 09:39:42 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:016e8ff197695f0c8e2c3ae127ac9459df9c71e52ae54500970e692d2799c944`  
		Last Modified: Thu, 23 Apr 2020 09:39:42 GMT  
		Size: 1.4 MB (1376131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd64ec452edc906dc611493aae3c90529a0d5787d8dc3b8c1088b41b53379d2d`  
		Last Modified: Thu, 23 Apr 2020 09:40:07 GMT  
		Size: 7.2 MB (7179305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ca72abe00cf1354dc501a32ed89705fdacd4905631c42186458d9d3202cc90`  
		Last Modified: Thu, 23 Apr 2020 09:40:05 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e7807337a06858bed0eac541f5935b123a4abb0d973dacb1973753c6dcb2469`  
		Last Modified: Thu, 23 Apr 2020 09:40:04 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5.0` - linux; arm variant v7

```console
$ docker pull redis@sha256:afc097fd6784e016756816ecc4ae33dc9ef22f5715db3593b90b7ec17e906edf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.1 MB (31109340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:632cd87ac6e4d8bda115f5e32e2b45cb8e28c59bd4c6e24b87985cf6b1f93354`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 01:03:26 GMT
ADD file:db6122b36f3e70c5f490b50afba99d49fa345f11d0f5c77bb3c6749f8e2a4f81 in / 
# Thu, 23 Apr 2020 01:03:28 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 13:54:58 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 13:54:59 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 13:55:22 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 13:57:35 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 13:57:35 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 13:57:36 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 13:58:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 13:58:37 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 13:58:38 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 13:58:39 GMT
WORKDIR /data
# Thu, 23 Apr 2020 13:58:39 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 13:58:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 13:58:41 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 13:58:41 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:50fb0052086928803f00724ca465c89c45dde5b082b1e59dadb8101286dd5ab6`  
		Last Modified: Thu, 23 Apr 2020 01:11:08 GMT  
		Size: 22.7 MB (22705377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98fc1f5e139d98aa45f74dfddb32ca22bec51ecf2fcab9bb372d91c14cc971d2`  
		Last Modified: Thu, 23 Apr 2020 14:00:18 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa98edd0b4c481052caeb348af3e906ef75764353840cfe2518af73963fcf2d`  
		Last Modified: Thu, 23 Apr 2020 14:00:18 GMT  
		Size: 1.4 MB (1368177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1ae9f68f12644f241fb270f9baf2e62d5b1380083acada1fdae86374998430`  
		Last Modified: Thu, 23 Apr 2020 14:00:21 GMT  
		Size: 7.0 MB (7033517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a23909059832233f41bcba599ec5bb698e278c652cf313dc6e8724fae8aa40cf`  
		Last Modified: Thu, 23 Apr 2020 14:00:19 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f5f6de32828cf1cb128a0cba17dc0396dead74aa6cc963394ac4f8b05540179`  
		Last Modified: Thu, 23 Apr 2020 14:00:18 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5.0` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:be463e278dc2125ea4c8984cd6a990353dfaa7f94570856734f86b900debc008
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 MB (34548547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0da52d2315939d969b12f3db6ae0aa5716074833f1ef06a42a544aec452d0ab2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:54:55 GMT
ADD file:581ee9c3c19f0d971aeda008fd399f59171cae75e8936b967dbf3888db4fc0d0 in / 
# Thu, 23 Apr 2020 00:54:58 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 16:01:56 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 16:01:57 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 16:02:29 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 16:04:19 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 16:04:20 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 16:04:20 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 16:05:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 16:05:20 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 16:05:20 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 16:05:21 GMT
WORKDIR /data
# Thu, 23 Apr 2020 16:05:21 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 16:05:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 16:05:22 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 16:05:24 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:bdc84a41f2513e28e99efeff9fcbb196b7df9883fb30532184bd67ca415b4673`  
		Last Modified: Thu, 23 Apr 2020 01:03:27 GMT  
		Size: 25.9 MB (25857800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698d3e76f19fb83cee90fe071552d86509322f0b8316774550c1ea7398327369`  
		Last Modified: Thu, 23 Apr 2020 16:07:31 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac4bbea6248caf60d5eca4d3e15d73d9cc18a5154a795c5ca3937eb040c9daae`  
		Last Modified: Thu, 23 Apr 2020 16:07:31 GMT  
		Size: 1.4 MB (1352987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1590123d45656fbb5cabd427b87908fd7347ef2fc6b0fba354f2b83771ec8882`  
		Last Modified: Thu, 23 Apr 2020 16:07:57 GMT  
		Size: 7.3 MB (7335481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e21891406b8ecd80c9cc4be90337cdd8d8935229002e8162d9afc9b68d2a4c30`  
		Last Modified: Thu, 23 Apr 2020 16:07:55 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d793eb07a5bc754267edbd54feb6cb25e4c28e7056a87e27960de4901d1dcc3`  
		Last Modified: Thu, 23 Apr 2020 16:07:55 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5.0` - linux; 386

```console
$ docker pull redis@sha256:0ac1dbfd6ca80b45aa587ecaa0632457ca254eea674a50e8574e8677f7a193a0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.2 MB (36151602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34c763545c4e57aabcdc00c9448e439a81bdaf47ae32d7711bc8e1252fb7ef59`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:39:36 GMT
ADD file:ca6a74f6b738c738c033152fab2a9aacf22bec5f19a994e6a02b5f919ee33ee9 in / 
# Thu, 23 Apr 2020 00:39:36 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 11:23:53 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 11:23:53 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 11:24:11 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 11:26:28 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 11:26:28 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 11:26:28 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 11:27:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 11:27:59 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 11:28:00 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 11:28:00 GMT
WORKDIR /data
# Thu, 23 Apr 2020 11:28:00 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 11:28:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 11:28:01 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 11:28:01 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:5d3da8f33b97fc107a05b3255a55836b76df9f817de632b1fb63c6e9c024f0df`  
		Last Modified: Thu, 23 Apr 2020 00:44:35 GMT  
		Size: 27.8 MB (27753972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f572d913eaf53def72d8eeff5384464ae75f0da9041d63ef0cd2fb2a43e21e`  
		Last Modified: Thu, 23 Apr 2020 11:30:12 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36c13a7e7929be4f05fbeddd74c94dfe85b704c504f7d13aa45bdb84bae79ccb`  
		Last Modified: Thu, 23 Apr 2020 11:30:12 GMT  
		Size: 1.4 MB (1387411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680a9b72444c93256224c2c5394c18343047b8b7dc305a4301401e7a6b494d03`  
		Last Modified: Thu, 23 Apr 2020 11:30:25 GMT  
		Size: 7.0 MB (7007988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e6148f8fb3eb037aaf97a9736b49d92d77541c5bbb6219db62f8af4f8d5e54`  
		Last Modified: Thu, 23 Apr 2020 11:30:23 GMT  
		Size: 97.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fae33d9962de4399f135693d495b300515e9d363f74683c3c366cd6e32290e1`  
		Last Modified: Thu, 23 Apr 2020 11:30:23 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5.0` - linux; mips64le

```console
$ docker pull redis@sha256:8860ea6be85bfa12a7a62f37e07716f197be8e76f498d1e62d3c4319582a3b60
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34731728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eab8ac536ee15de9306c977271c71a293db05c67e582fe002279ba86c8fff0a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:09:47 GMT
ADD file:7509945bd8a224048260e88b466aa3b156615e16b64e0a6702da277052fcb98b in / 
# Thu, 23 Apr 2020 00:09:48 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 09:24:32 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 09:24:33 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 09:25:02 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 09:28:42 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 09:28:42 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 09:28:43 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 09:31:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 09:32:01 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 09:32:01 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 09:32:01 GMT
WORKDIR /data
# Thu, 23 Apr 2020 09:32:02 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 09:32:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 09:32:02 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 09:32:03 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:ae8f0fa6cb0d971b4b8fedf7fc9b00f61f780b383fe7d64e6c2e4be8d20c3987`  
		Last Modified: Thu, 23 Apr 2020 00:17:46 GMT  
		Size: 25.8 MB (25762125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faf65c067540cd52d99f7f6df4511fb45d6a0485e47338d0239a052fcd64c8e3`  
		Last Modified: Thu, 23 Apr 2020 09:34:32 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef207bf80aefb18eba12c119d07499e37b5ea7bec06bc1e0c2dd749ddde45a1`  
		Last Modified: Thu, 23 Apr 2020 09:34:34 GMT  
		Size: 1.3 MB (1305489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae62dd92cc34f4856c15b7614910c5578f2d91d96d96469c21f8ca741c1061f5`  
		Last Modified: Thu, 23 Apr 2020 09:35:08 GMT  
		Size: 7.7 MB (7661872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693fe2f4d6e93636c838f7fb3a49c859d72138e5a25fd1687e590fcf3bb74dfb`  
		Last Modified: Thu, 23 Apr 2020 09:35:00 GMT  
		Size: 99.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:153c8eb8631e42a4705a53461aeb1c1edea4a60ad71a759b5eafeccbf3f5c142`  
		Last Modified: Thu, 23 Apr 2020 09:35:00 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5.0` - linux; ppc64le

```console
$ docker pull redis@sha256:e1c410783ee0d501a9804b3050db559054e95e91bb3cd8f3e81324baef92f730
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.7 MB (39696544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34098209a59e39ee25eeb2b0bf53ba98f873314c75110d6841a0793d5e1bc182`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:36:00 GMT
ADD file:5b3c3d2945800e1743dc02a4f68bd830fe2f67ca437223692eb460147c158c2b in / 
# Thu, 23 Apr 2020 00:36:04 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 17:29:48 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 17:29:51 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 17:31:38 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 17:35:14 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 17:35:18 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 17:35:23 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 17:38:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 17:38:25 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 17:38:28 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 17:38:32 GMT
WORKDIR /data
# Thu, 23 Apr 2020 17:38:34 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 17:38:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 17:38:42 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 17:38:45 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:012c6cdbd1af202bbfbea5945fafbb9aca9097f1fa3cb493a29155fdc02cc43c`  
		Last Modified: Thu, 23 Apr 2020 00:50:14 GMT  
		Size: 30.5 MB (30524638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee5a34bf53dadebb7466557f439affba6f1c11ddbdd7d2c1376f9540c294a7a`  
		Last Modified: Thu, 23 Apr 2020 17:42:03 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dedf97e3c0bcb476732135fc70dee2ba4766ff50ec51f93b1929ebaa6c4863f`  
		Last Modified: Thu, 23 Apr 2020 17:42:03 GMT  
		Size: 1.3 MB (1335327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2a1294a7da3aa34af8f45c22665913b8780fcf4dec6b52b108541e496dd0cc`  
		Last Modified: Thu, 23 Apr 2020 17:42:27 GMT  
		Size: 7.8 MB (7834296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51726f5fc1a7b6d031cad4d822aaf6c1801262570fb662454f1f2dc93cd4e551`  
		Last Modified: Thu, 23 Apr 2020 17:42:25 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e62728fce47996c1059a9f4f18e5e1efea4ebc55e17f82aa362f8985e7f019e`  
		Last Modified: Thu, 23 Apr 2020 17:42:25 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5.0` - linux; s390x

```console
$ docker pull redis@sha256:80a22e71a515d761d2c50a5873fc228fe165a627f9f91641391ce1548bc23f03
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34709447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5556ba73cac9fdc7f38ea53f8961a08497e52b1fa62f83611a9228a5d495e8fb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:51:48 GMT
ADD file:f6c2560f9185c1bcaff95e576e57449f606d51b85fad02646c1b0962bc9353c9 in / 
# Thu, 23 Apr 2020 00:51:50 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 06:58:44 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 06:58:44 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 06:58:58 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 06:59:46 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 06:59:47 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 06:59:47 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 07:00:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 07:00:24 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 07:00:24 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 07:00:24 GMT
WORKDIR /data
# Thu, 23 Apr 2020 07:00:24 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 07:00:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 07:00:25 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 07:00:25 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:d89dc3741ad42b79c3d8545495c429f3100d3f22234ff993bd04017b0675e868`  
		Last Modified: Thu, 23 Apr 2020 00:56:00 GMT  
		Size: 25.7 MB (25712105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c9894c70b29dc7cbad7e69c5f898b0a5d6f82aac9aff00e2645a6f8a9eff88`  
		Last Modified: Thu, 23 Apr 2020 07:01:34 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fba24ca231c607425b0e92a8a39c3174a8b9cb56ddeee71fc43f2f9dd9b1d2c`  
		Last Modified: Thu, 23 Apr 2020 07:01:35 GMT  
		Size: 1.4 MB (1403679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22d299e81a09eaaf9da803a2b3775444f312a34b2b7dd8e0c1c10d0171225ba`  
		Last Modified: Thu, 23 Apr 2020 07:01:52 GMT  
		Size: 7.6 MB (7591385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46db2cefe8baf230709535dd5f96c93520ca156d9821649ce8e8a2410e49d54`  
		Last Modified: Thu, 23 Apr 2020 07:01:56 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ec0a42c81dfec4356c31366a6ddf246ebac63394fafd37549a4483fd537513`  
		Last Modified: Thu, 23 Apr 2020 07:01:50 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redis:5.0-32bit`

```console
$ docker pull redis@sha256:021a0c5614223ddc6a302017241389a0d06d559eca7868ac964be52b1c695328
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redis:5.0-32bit` - linux; amd64

```console
$ docker pull redis@sha256:734e0a8d1994e025f766201cd7ed0ee736053c88599e048aa3fe7044444751c8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40576869 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffbc0eed192b290957b3d6f2568222df0745389d5c8c6d6a2e434395b7540589`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:20:32 GMT
ADD file:9b8be2b52ee0fa31da1b6256099030b73546253a57e94cccb24605cd888bb74d in / 
# Thu, 23 Apr 2020 00:20:32 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 19:48:34 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 19:48:34 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 19:48:46 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 19:50:08 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 19:50:08 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 19:50:08 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 19:52:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev-i386 gcc-multilib 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" 32bit; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 19:52:54 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 19:52:54 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 19:52:55 GMT
WORKDIR /data
# Thu, 23 Apr 2020 19:52:55 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 19:52:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 19:52:55 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 19:52:55 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:54fec2fa59d0a0de9cd2dec9850b36c43de451f1fd1c0a5bf8f1cf26a61a5da4`  
		Last Modified: Thu, 23 Apr 2020 00:25:10 GMT  
		Size: 27.1 MB (27098254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c94e11103d92f2a83b82e5d4287445cba073af0002cecee98d85d68ccec0f89`  
		Last Modified: Thu, 23 Apr 2020 19:55:42 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ab1bfc453f19989c401c2f0622df3363b5182bdea1af9e59ee2ceea3a9931c`  
		Last Modified: Thu, 23 Apr 2020 19:55:43 GMT  
		Size: 1.4 MB (1417711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fedad42a33a3821f6b477a48ad2c5cb4d05dd795fc6af2fbba817ce1a2365dd0`  
		Last Modified: Thu, 23 Apr 2020 19:56:14 GMT  
		Size: 12.1 MB (12058659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b58703ecd075fd32ee51dd28840b9622cc5aaac3bb2d77c841515846571805e`  
		Last Modified: Thu, 23 Apr 2020 19:56:03 GMT  
		Size: 99.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bece53145f7f86a1877242e552825b494f227a3f4facff30334248943c4ad49`  
		Last Modified: Thu, 23 Apr 2020 19:56:04 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redis:5.0-32bit-buster`

```console
$ docker pull redis@sha256:021a0c5614223ddc6a302017241389a0d06d559eca7868ac964be52b1c695328
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redis:5.0-32bit-buster` - linux; amd64

```console
$ docker pull redis@sha256:734e0a8d1994e025f766201cd7ed0ee736053c88599e048aa3fe7044444751c8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40576869 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffbc0eed192b290957b3d6f2568222df0745389d5c8c6d6a2e434395b7540589`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:20:32 GMT
ADD file:9b8be2b52ee0fa31da1b6256099030b73546253a57e94cccb24605cd888bb74d in / 
# Thu, 23 Apr 2020 00:20:32 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 19:48:34 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 19:48:34 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 19:48:46 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 19:50:08 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 19:50:08 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 19:50:08 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 19:52:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev-i386 gcc-multilib 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" 32bit; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 19:52:54 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 19:52:54 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 19:52:55 GMT
WORKDIR /data
# Thu, 23 Apr 2020 19:52:55 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 19:52:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 19:52:55 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 19:52:55 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:54fec2fa59d0a0de9cd2dec9850b36c43de451f1fd1c0a5bf8f1cf26a61a5da4`  
		Last Modified: Thu, 23 Apr 2020 00:25:10 GMT  
		Size: 27.1 MB (27098254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c94e11103d92f2a83b82e5d4287445cba073af0002cecee98d85d68ccec0f89`  
		Last Modified: Thu, 23 Apr 2020 19:55:42 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ab1bfc453f19989c401c2f0622df3363b5182bdea1af9e59ee2ceea3a9931c`  
		Last Modified: Thu, 23 Apr 2020 19:55:43 GMT  
		Size: 1.4 MB (1417711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fedad42a33a3821f6b477a48ad2c5cb4d05dd795fc6af2fbba817ce1a2365dd0`  
		Last Modified: Thu, 23 Apr 2020 19:56:14 GMT  
		Size: 12.1 MB (12058659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b58703ecd075fd32ee51dd28840b9622cc5aaac3bb2d77c841515846571805e`  
		Last Modified: Thu, 23 Apr 2020 19:56:03 GMT  
		Size: 99.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bece53145f7f86a1877242e552825b494f227a3f4facff30334248943c4ad49`  
		Last Modified: Thu, 23 Apr 2020 19:56:04 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redis:5.0.9`

```console
$ docker pull redis@sha256:157a95b41b0dca8c308a33489dfdb28019e033110320414b4b16fad7d28c0f9f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `redis:5.0.9` - linux; amd64

```console
$ docker pull redis@sha256:43dbbe6f633572d66e84e7162245d8d70a18f00b819d6c0bf98ca02109f4788c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35863297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4d3716dbb72408a7843e12d7d9f6a5addf7ab28ac21e9e9da4a6a51f1b32da9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:20:32 GMT
ADD file:9b8be2b52ee0fa31da1b6256099030b73546253a57e94cccb24605cd888bb74d in / 
# Thu, 23 Apr 2020 00:20:32 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 19:48:34 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 19:48:34 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 19:48:46 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 19:50:08 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 19:50:08 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 19:50:08 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 19:51:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 19:51:26 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 19:51:26 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 19:51:27 GMT
WORKDIR /data
# Thu, 23 Apr 2020 19:51:27 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 19:51:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 19:51:28 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 19:51:28 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:54fec2fa59d0a0de9cd2dec9850b36c43de451f1fd1c0a5bf8f1cf26a61a5da4`  
		Last Modified: Thu, 23 Apr 2020 00:25:10 GMT  
		Size: 27.1 MB (27098254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c94e11103d92f2a83b82e5d4287445cba073af0002cecee98d85d68ccec0f89`  
		Last Modified: Thu, 23 Apr 2020 19:55:42 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ab1bfc453f19989c401c2f0622df3363b5182bdea1af9e59ee2ceea3a9931c`  
		Last Modified: Thu, 23 Apr 2020 19:55:43 GMT  
		Size: 1.4 MB (1417711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f71e6b94d83f5a0df5d032ce4998b4834287bd4ed307ff7c9a31ad0a60caa98`  
		Last Modified: Thu, 23 Apr 2020 19:55:55 GMT  
		Size: 7.3 MB (7345094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2729a8234dd5e724571528d78d5f581702abc77be39db93fc0ae741340eb1c18`  
		Last Modified: Thu, 23 Apr 2020 19:55:53 GMT  
		Size: 97.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2683d7f177455cf86b4cf424cc757f1d177d5772df77bdaeeace411006eb88a5`  
		Last Modified: Thu, 23 Apr 2020 19:55:53 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5.0.9` - linux; arm variant v5

```console
$ docker pull redis@sha256:5a474d0e7c55a7e45ddaf530f4f2ab4bc8dcaba6d85b0829f1121f7fe53414fd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.4 MB (33394023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b83a1e222e2b9be5acf1ae9a03cd2e6d2c7a4efcd3b73a275481c652552de80`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:52:22 GMT
ADD file:62a9732be4e3237ccc896f724a34606e01f351c4877e52c9a9cd85029c06b956 in / 
# Thu, 23 Apr 2020 00:52:23 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 09:33:20 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 09:33:21 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 09:33:56 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 09:35:38 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 09:35:39 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 09:35:39 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 09:36:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 09:36:48 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 09:36:48 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 09:36:49 GMT
WORKDIR /data
# Thu, 23 Apr 2020 09:36:50 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 09:36:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 09:36:51 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 09:36:52 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:a8c46e5952878f9f324df86c5a2b45b2e0020f6721e820981e74461d77a100dd`  
		Last Modified: Thu, 23 Apr 2020 00:59:50 GMT  
		Size: 24.8 MB (24836319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471287e557b84038803c3a26dee3987da48cbcae6529a77a28f486e4527757f7`  
		Last Modified: Thu, 23 Apr 2020 09:39:42 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:016e8ff197695f0c8e2c3ae127ac9459df9c71e52ae54500970e692d2799c944`  
		Last Modified: Thu, 23 Apr 2020 09:39:42 GMT  
		Size: 1.4 MB (1376131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd64ec452edc906dc611493aae3c90529a0d5787d8dc3b8c1088b41b53379d2d`  
		Last Modified: Thu, 23 Apr 2020 09:40:07 GMT  
		Size: 7.2 MB (7179305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ca72abe00cf1354dc501a32ed89705fdacd4905631c42186458d9d3202cc90`  
		Last Modified: Thu, 23 Apr 2020 09:40:05 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e7807337a06858bed0eac541f5935b123a4abb0d973dacb1973753c6dcb2469`  
		Last Modified: Thu, 23 Apr 2020 09:40:04 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5.0.9` - linux; arm variant v7

```console
$ docker pull redis@sha256:afc097fd6784e016756816ecc4ae33dc9ef22f5715db3593b90b7ec17e906edf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.1 MB (31109340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:632cd87ac6e4d8bda115f5e32e2b45cb8e28c59bd4c6e24b87985cf6b1f93354`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 01:03:26 GMT
ADD file:db6122b36f3e70c5f490b50afba99d49fa345f11d0f5c77bb3c6749f8e2a4f81 in / 
# Thu, 23 Apr 2020 01:03:28 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 13:54:58 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 13:54:59 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 13:55:22 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 13:57:35 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 13:57:35 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 13:57:36 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 13:58:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 13:58:37 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 13:58:38 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 13:58:39 GMT
WORKDIR /data
# Thu, 23 Apr 2020 13:58:39 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 13:58:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 13:58:41 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 13:58:41 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:50fb0052086928803f00724ca465c89c45dde5b082b1e59dadb8101286dd5ab6`  
		Last Modified: Thu, 23 Apr 2020 01:11:08 GMT  
		Size: 22.7 MB (22705377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98fc1f5e139d98aa45f74dfddb32ca22bec51ecf2fcab9bb372d91c14cc971d2`  
		Last Modified: Thu, 23 Apr 2020 14:00:18 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa98edd0b4c481052caeb348af3e906ef75764353840cfe2518af73963fcf2d`  
		Last Modified: Thu, 23 Apr 2020 14:00:18 GMT  
		Size: 1.4 MB (1368177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1ae9f68f12644f241fb270f9baf2e62d5b1380083acada1fdae86374998430`  
		Last Modified: Thu, 23 Apr 2020 14:00:21 GMT  
		Size: 7.0 MB (7033517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a23909059832233f41bcba599ec5bb698e278c652cf313dc6e8724fae8aa40cf`  
		Last Modified: Thu, 23 Apr 2020 14:00:19 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f5f6de32828cf1cb128a0cba17dc0396dead74aa6cc963394ac4f8b05540179`  
		Last Modified: Thu, 23 Apr 2020 14:00:18 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5.0.9` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:be463e278dc2125ea4c8984cd6a990353dfaa7f94570856734f86b900debc008
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 MB (34548547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0da52d2315939d969b12f3db6ae0aa5716074833f1ef06a42a544aec452d0ab2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:54:55 GMT
ADD file:581ee9c3c19f0d971aeda008fd399f59171cae75e8936b967dbf3888db4fc0d0 in / 
# Thu, 23 Apr 2020 00:54:58 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 16:01:56 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 16:01:57 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 16:02:29 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 16:04:19 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 16:04:20 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 16:04:20 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 16:05:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 16:05:20 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 16:05:20 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 16:05:21 GMT
WORKDIR /data
# Thu, 23 Apr 2020 16:05:21 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 16:05:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 16:05:22 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 16:05:24 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:bdc84a41f2513e28e99efeff9fcbb196b7df9883fb30532184bd67ca415b4673`  
		Last Modified: Thu, 23 Apr 2020 01:03:27 GMT  
		Size: 25.9 MB (25857800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698d3e76f19fb83cee90fe071552d86509322f0b8316774550c1ea7398327369`  
		Last Modified: Thu, 23 Apr 2020 16:07:31 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac4bbea6248caf60d5eca4d3e15d73d9cc18a5154a795c5ca3937eb040c9daae`  
		Last Modified: Thu, 23 Apr 2020 16:07:31 GMT  
		Size: 1.4 MB (1352987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1590123d45656fbb5cabd427b87908fd7347ef2fc6b0fba354f2b83771ec8882`  
		Last Modified: Thu, 23 Apr 2020 16:07:57 GMT  
		Size: 7.3 MB (7335481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e21891406b8ecd80c9cc4be90337cdd8d8935229002e8162d9afc9b68d2a4c30`  
		Last Modified: Thu, 23 Apr 2020 16:07:55 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d793eb07a5bc754267edbd54feb6cb25e4c28e7056a87e27960de4901d1dcc3`  
		Last Modified: Thu, 23 Apr 2020 16:07:55 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5.0.9` - linux; 386

```console
$ docker pull redis@sha256:0ac1dbfd6ca80b45aa587ecaa0632457ca254eea674a50e8574e8677f7a193a0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.2 MB (36151602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34c763545c4e57aabcdc00c9448e439a81bdaf47ae32d7711bc8e1252fb7ef59`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:39:36 GMT
ADD file:ca6a74f6b738c738c033152fab2a9aacf22bec5f19a994e6a02b5f919ee33ee9 in / 
# Thu, 23 Apr 2020 00:39:36 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 11:23:53 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 11:23:53 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 11:24:11 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 11:26:28 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 11:26:28 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 11:26:28 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 11:27:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 11:27:59 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 11:28:00 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 11:28:00 GMT
WORKDIR /data
# Thu, 23 Apr 2020 11:28:00 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 11:28:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 11:28:01 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 11:28:01 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:5d3da8f33b97fc107a05b3255a55836b76df9f817de632b1fb63c6e9c024f0df`  
		Last Modified: Thu, 23 Apr 2020 00:44:35 GMT  
		Size: 27.8 MB (27753972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f572d913eaf53def72d8eeff5384464ae75f0da9041d63ef0cd2fb2a43e21e`  
		Last Modified: Thu, 23 Apr 2020 11:30:12 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36c13a7e7929be4f05fbeddd74c94dfe85b704c504f7d13aa45bdb84bae79ccb`  
		Last Modified: Thu, 23 Apr 2020 11:30:12 GMT  
		Size: 1.4 MB (1387411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680a9b72444c93256224c2c5394c18343047b8b7dc305a4301401e7a6b494d03`  
		Last Modified: Thu, 23 Apr 2020 11:30:25 GMT  
		Size: 7.0 MB (7007988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e6148f8fb3eb037aaf97a9736b49d92d77541c5bbb6219db62f8af4f8d5e54`  
		Last Modified: Thu, 23 Apr 2020 11:30:23 GMT  
		Size: 97.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fae33d9962de4399f135693d495b300515e9d363f74683c3c366cd6e32290e1`  
		Last Modified: Thu, 23 Apr 2020 11:30:23 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5.0.9` - linux; mips64le

```console
$ docker pull redis@sha256:8860ea6be85bfa12a7a62f37e07716f197be8e76f498d1e62d3c4319582a3b60
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34731728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eab8ac536ee15de9306c977271c71a293db05c67e582fe002279ba86c8fff0a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:09:47 GMT
ADD file:7509945bd8a224048260e88b466aa3b156615e16b64e0a6702da277052fcb98b in / 
# Thu, 23 Apr 2020 00:09:48 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 09:24:32 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 09:24:33 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 09:25:02 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 09:28:42 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 09:28:42 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 09:28:43 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 09:31:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 09:32:01 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 09:32:01 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 09:32:01 GMT
WORKDIR /data
# Thu, 23 Apr 2020 09:32:02 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 09:32:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 09:32:02 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 09:32:03 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:ae8f0fa6cb0d971b4b8fedf7fc9b00f61f780b383fe7d64e6c2e4be8d20c3987`  
		Last Modified: Thu, 23 Apr 2020 00:17:46 GMT  
		Size: 25.8 MB (25762125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faf65c067540cd52d99f7f6df4511fb45d6a0485e47338d0239a052fcd64c8e3`  
		Last Modified: Thu, 23 Apr 2020 09:34:32 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef207bf80aefb18eba12c119d07499e37b5ea7bec06bc1e0c2dd749ddde45a1`  
		Last Modified: Thu, 23 Apr 2020 09:34:34 GMT  
		Size: 1.3 MB (1305489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae62dd92cc34f4856c15b7614910c5578f2d91d96d96469c21f8ca741c1061f5`  
		Last Modified: Thu, 23 Apr 2020 09:35:08 GMT  
		Size: 7.7 MB (7661872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693fe2f4d6e93636c838f7fb3a49c859d72138e5a25fd1687e590fcf3bb74dfb`  
		Last Modified: Thu, 23 Apr 2020 09:35:00 GMT  
		Size: 99.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:153c8eb8631e42a4705a53461aeb1c1edea4a60ad71a759b5eafeccbf3f5c142`  
		Last Modified: Thu, 23 Apr 2020 09:35:00 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5.0.9` - linux; ppc64le

```console
$ docker pull redis@sha256:e1c410783ee0d501a9804b3050db559054e95e91bb3cd8f3e81324baef92f730
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.7 MB (39696544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34098209a59e39ee25eeb2b0bf53ba98f873314c75110d6841a0793d5e1bc182`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:36:00 GMT
ADD file:5b3c3d2945800e1743dc02a4f68bd830fe2f67ca437223692eb460147c158c2b in / 
# Thu, 23 Apr 2020 00:36:04 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 17:29:48 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 17:29:51 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 17:31:38 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 17:35:14 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 17:35:18 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 17:35:23 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 17:38:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 17:38:25 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 17:38:28 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 17:38:32 GMT
WORKDIR /data
# Thu, 23 Apr 2020 17:38:34 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 17:38:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 17:38:42 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 17:38:45 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:012c6cdbd1af202bbfbea5945fafbb9aca9097f1fa3cb493a29155fdc02cc43c`  
		Last Modified: Thu, 23 Apr 2020 00:50:14 GMT  
		Size: 30.5 MB (30524638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee5a34bf53dadebb7466557f439affba6f1c11ddbdd7d2c1376f9540c294a7a`  
		Last Modified: Thu, 23 Apr 2020 17:42:03 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dedf97e3c0bcb476732135fc70dee2ba4766ff50ec51f93b1929ebaa6c4863f`  
		Last Modified: Thu, 23 Apr 2020 17:42:03 GMT  
		Size: 1.3 MB (1335327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2a1294a7da3aa34af8f45c22665913b8780fcf4dec6b52b108541e496dd0cc`  
		Last Modified: Thu, 23 Apr 2020 17:42:27 GMT  
		Size: 7.8 MB (7834296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51726f5fc1a7b6d031cad4d822aaf6c1801262570fb662454f1f2dc93cd4e551`  
		Last Modified: Thu, 23 Apr 2020 17:42:25 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e62728fce47996c1059a9f4f18e5e1efea4ebc55e17f82aa362f8985e7f019e`  
		Last Modified: Thu, 23 Apr 2020 17:42:25 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5.0.9` - linux; s390x

```console
$ docker pull redis@sha256:80a22e71a515d761d2c50a5873fc228fe165a627f9f91641391ce1548bc23f03
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34709447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5556ba73cac9fdc7f38ea53f8961a08497e52b1fa62f83611a9228a5d495e8fb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:51:48 GMT
ADD file:f6c2560f9185c1bcaff95e576e57449f606d51b85fad02646c1b0962bc9353c9 in / 
# Thu, 23 Apr 2020 00:51:50 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 06:58:44 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 06:58:44 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 06:58:58 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 06:59:46 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 06:59:47 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 06:59:47 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 07:00:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 07:00:24 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 07:00:24 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 07:00:24 GMT
WORKDIR /data
# Thu, 23 Apr 2020 07:00:24 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 07:00:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 07:00:25 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 07:00:25 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:d89dc3741ad42b79c3d8545495c429f3100d3f22234ff993bd04017b0675e868`  
		Last Modified: Thu, 23 Apr 2020 00:56:00 GMT  
		Size: 25.7 MB (25712105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c9894c70b29dc7cbad7e69c5f898b0a5d6f82aac9aff00e2645a6f8a9eff88`  
		Last Modified: Thu, 23 Apr 2020 07:01:34 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fba24ca231c607425b0e92a8a39c3174a8b9cb56ddeee71fc43f2f9dd9b1d2c`  
		Last Modified: Thu, 23 Apr 2020 07:01:35 GMT  
		Size: 1.4 MB (1403679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22d299e81a09eaaf9da803a2b3775444f312a34b2b7dd8e0c1c10d0171225ba`  
		Last Modified: Thu, 23 Apr 2020 07:01:52 GMT  
		Size: 7.6 MB (7591385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46db2cefe8baf230709535dd5f96c93520ca156d9821649ce8e8a2410e49d54`  
		Last Modified: Thu, 23 Apr 2020 07:01:56 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ec0a42c81dfec4356c31366a6ddf246ebac63394fafd37549a4483fd537513`  
		Last Modified: Thu, 23 Apr 2020 07:01:50 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redis:5.0.9-32bit`

```console
$ docker pull redis@sha256:021a0c5614223ddc6a302017241389a0d06d559eca7868ac964be52b1c695328
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redis:5.0.9-32bit` - linux; amd64

```console
$ docker pull redis@sha256:734e0a8d1994e025f766201cd7ed0ee736053c88599e048aa3fe7044444751c8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40576869 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffbc0eed192b290957b3d6f2568222df0745389d5c8c6d6a2e434395b7540589`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:20:32 GMT
ADD file:9b8be2b52ee0fa31da1b6256099030b73546253a57e94cccb24605cd888bb74d in / 
# Thu, 23 Apr 2020 00:20:32 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 19:48:34 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 19:48:34 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 19:48:46 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 19:50:08 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 19:50:08 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 19:50:08 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 19:52:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev-i386 gcc-multilib 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" 32bit; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 19:52:54 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 19:52:54 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 19:52:55 GMT
WORKDIR /data
# Thu, 23 Apr 2020 19:52:55 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 19:52:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 19:52:55 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 19:52:55 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:54fec2fa59d0a0de9cd2dec9850b36c43de451f1fd1c0a5bf8f1cf26a61a5da4`  
		Last Modified: Thu, 23 Apr 2020 00:25:10 GMT  
		Size: 27.1 MB (27098254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c94e11103d92f2a83b82e5d4287445cba073af0002cecee98d85d68ccec0f89`  
		Last Modified: Thu, 23 Apr 2020 19:55:42 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ab1bfc453f19989c401c2f0622df3363b5182bdea1af9e59ee2ceea3a9931c`  
		Last Modified: Thu, 23 Apr 2020 19:55:43 GMT  
		Size: 1.4 MB (1417711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fedad42a33a3821f6b477a48ad2c5cb4d05dd795fc6af2fbba817ce1a2365dd0`  
		Last Modified: Thu, 23 Apr 2020 19:56:14 GMT  
		Size: 12.1 MB (12058659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b58703ecd075fd32ee51dd28840b9622cc5aaac3bb2d77c841515846571805e`  
		Last Modified: Thu, 23 Apr 2020 19:56:03 GMT  
		Size: 99.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bece53145f7f86a1877242e552825b494f227a3f4facff30334248943c4ad49`  
		Last Modified: Thu, 23 Apr 2020 19:56:04 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redis:5.0.9-32bit-buster`

```console
$ docker pull redis@sha256:021a0c5614223ddc6a302017241389a0d06d559eca7868ac964be52b1c695328
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redis:5.0.9-32bit-buster` - linux; amd64

```console
$ docker pull redis@sha256:734e0a8d1994e025f766201cd7ed0ee736053c88599e048aa3fe7044444751c8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40576869 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffbc0eed192b290957b3d6f2568222df0745389d5c8c6d6a2e434395b7540589`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:20:32 GMT
ADD file:9b8be2b52ee0fa31da1b6256099030b73546253a57e94cccb24605cd888bb74d in / 
# Thu, 23 Apr 2020 00:20:32 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 19:48:34 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 19:48:34 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 19:48:46 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 19:50:08 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 19:50:08 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 19:50:08 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 19:52:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev-i386 gcc-multilib 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" 32bit; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 19:52:54 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 19:52:54 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 19:52:55 GMT
WORKDIR /data
# Thu, 23 Apr 2020 19:52:55 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 19:52:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 19:52:55 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 19:52:55 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:54fec2fa59d0a0de9cd2dec9850b36c43de451f1fd1c0a5bf8f1cf26a61a5da4`  
		Last Modified: Thu, 23 Apr 2020 00:25:10 GMT  
		Size: 27.1 MB (27098254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c94e11103d92f2a83b82e5d4287445cba073af0002cecee98d85d68ccec0f89`  
		Last Modified: Thu, 23 Apr 2020 19:55:42 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ab1bfc453f19989c401c2f0622df3363b5182bdea1af9e59ee2ceea3a9931c`  
		Last Modified: Thu, 23 Apr 2020 19:55:43 GMT  
		Size: 1.4 MB (1417711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fedad42a33a3821f6b477a48ad2c5cb4d05dd795fc6af2fbba817ce1a2365dd0`  
		Last Modified: Thu, 23 Apr 2020 19:56:14 GMT  
		Size: 12.1 MB (12058659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b58703ecd075fd32ee51dd28840b9622cc5aaac3bb2d77c841515846571805e`  
		Last Modified: Thu, 23 Apr 2020 19:56:03 GMT  
		Size: 99.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bece53145f7f86a1877242e552825b494f227a3f4facff30334248943c4ad49`  
		Last Modified: Thu, 23 Apr 2020 19:56:04 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redis:5.0.9-alpine`

```console
$ docker pull redis@sha256:83a3af36d5e57f2901b4783c313720e5fa3ecf0424ba86ad9775e06a9a5e35d0
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

### `redis:5.0.9-alpine` - linux; amd64

```console
$ docker pull redis@sha256:d4ada5d910403607b3f579d7171f36108c2e1cf67da966a712812230171fc153
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (9998790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3661c84ee9d0f6312a076b69eb2bd112674cadb70ef7e1594c4f00193f8df08e`
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
# Fri, 24 Apr 2020 19:20:54 GMT
ENV REDIS_VERSION=5.0.9
# Fri, 24 Apr 2020 19:20:54 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Fri, 24 Apr 2020 19:20:55 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Fri, 24 Apr 2020 19:21:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 24 Apr 2020 19:21:49 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 24 Apr 2020 19:21:49 GMT
VOLUME [/data]
# Fri, 24 Apr 2020 19:21:50 GMT
WORKDIR /data
# Fri, 24 Apr 2020 19:21:50 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 24 Apr 2020 19:21:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 19:21:50 GMT
EXPOSE 6379
# Fri, 24 Apr 2020 19:21:50 GMT
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
	-	`sha256:3e45770272d96deeb96c4bfa3cffde811f318823b4422bdbbf909148dc5669bb`  
		Last Modified: Fri, 24 Apr 2020 19:23:14 GMT  
		Size: 6.8 MB (6781166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:558de8ea3153bdccfaf67fadf7bbbdc60bf357f33ff0070df617d6e22ad46a13`  
		Last Modified: Fri, 24 Apr 2020 19:23:13 GMT  
		Size: 99.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2c65255161264f51556db666aa812834b3f51c8403b09799a46e4d0909e4aa4`  
		Last Modified: Fri, 24 Apr 2020 19:23:12 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5.0.9-alpine` - linux; arm variant v6

```console
$ docker pull redis@sha256:867b50998330ae4743e95c8be69dee7ad37cbba8057659bef4dc142838d7f3e0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9725047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:333723767b2b5747763b5483d4742558e9abe6d70b98ee05d527643b5eb088d5`
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
# Thu, 23 Apr 2020 22:31:34 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 22:31:35 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 22:31:36 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 22:32:24 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 22:32:27 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 22:32:29 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 22:32:30 GMT
WORKDIR /data
# Thu, 23 Apr 2020 22:32:31 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Thu, 23 Apr 2020 22:32:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 22:32:33 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 22:32:34 GMT
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
	-	`sha256:75a2919ec032b1198ca13b052499b7c193e45d93756a3b0d7bb10c8db4f3db65`  
		Last Modified: Thu, 23 Apr 2020 22:34:01 GMT  
		Size: 6.7 MB (6697511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b2e77e4c2604e8e74b4c471b4a04d1a768eb84eadcfcd3621f135f7d4d90ca`  
		Last Modified: Thu, 23 Apr 2020 22:33:57 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18df89faaf97292802f6bca82a98892b7b0a168230ca31ae16e3cf307614a7a8`  
		Last Modified: Thu, 23 Apr 2020 22:33:57 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5.0.9-alpine` - linux; arm variant v7

```console
$ docker pull redis@sha256:1c10570f57cb14b4fbd3446c61303aeb7db18b45abffc49974d5bde7e4a89de4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9394623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56a7ba195be67da9c68c67aa8d6eefa737236f15d3a9b490504ce943465c3a9f`
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
# Fri, 24 Apr 2020 08:52:43 GMT
ENV REDIS_VERSION=5.0.9
# Fri, 24 Apr 2020 08:52:43 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Fri, 24 Apr 2020 08:52:44 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Fri, 24 Apr 2020 08:53:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 24 Apr 2020 08:53:30 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 24 Apr 2020 08:53:31 GMT
VOLUME [/data]
# Fri, 24 Apr 2020 08:53:32 GMT
WORKDIR /data
# Fri, 24 Apr 2020 08:53:32 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 24 Apr 2020 08:53:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 08:53:34 GMT
EXPOSE 6379
# Fri, 24 Apr 2020 08:53:34 GMT
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
	-	`sha256:531954b17ac2db3cd86f3ced48c7c4f9fe053fad0792b7038321a667c911953a`  
		Last Modified: Fri, 24 Apr 2020 08:55:41 GMT  
		Size: 6.6 MB (6570977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d550a31e99202186ed01f1a5a4c96bab49dc143ad2a113696ecb48947836c0`  
		Last Modified: Fri, 24 Apr 2020 08:55:38 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a842b77b23971198e093c671bcf1e2cf6df771a6138ffb4132bfb37af22f17`  
		Last Modified: Fri, 24 Apr 2020 08:55:38 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5.0.9-alpine` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:2ebdecb52315772800ba4549b9dc83910d9ae7de5364c3092b0390d7266e94a9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9918976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b6acb4ad7ccdd962d8579a0929ab5920a1f58ff996cd4812188219c1eb74e91`
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
# Fri, 24 Apr 2020 12:46:32 GMT
ENV REDIS_VERSION=5.0.9
# Fri, 24 Apr 2020 12:46:33 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Fri, 24 Apr 2020 12:46:34 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Fri, 24 Apr 2020 12:47:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 24 Apr 2020 12:47:24 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 24 Apr 2020 12:47:24 GMT
VOLUME [/data]
# Fri, 24 Apr 2020 12:47:25 GMT
WORKDIR /data
# Fri, 24 Apr 2020 12:47:26 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 24 Apr 2020 12:47:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 12:47:28 GMT
EXPOSE 6379
# Fri, 24 Apr 2020 12:47:29 GMT
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
	-	`sha256:f5ca1db598d2278e5526b65dcad0d96f0f0264060f879f1b437f58a467e27382`  
		Last Modified: Fri, 24 Apr 2020 12:49:17 GMT  
		Size: 6.8 MB (6788089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87542dce16ad38aeb18ffe2e2266f3bd9b8cbc70f6f4450be0e9f621022fabb5`  
		Last Modified: Fri, 24 Apr 2020 12:49:15 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a20d19811afde1a300515cade1279f18fb3ca0ef1800b52dcb45127731bd5f4`  
		Last Modified: Fri, 24 Apr 2020 12:49:15 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5.0.9-alpine` - linux; 386

```console
$ docker pull redis@sha256:3ab6896b5efe215c5cc110a835fecb73d5f55672ad4443f4baf51822db1854c6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9710040 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bba820d7067104939d7ec907ee1fa581e9c7d40b0a204a14caf709f4dce84732`
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
# Fri, 24 Apr 2020 05:51:10 GMT
ENV REDIS_VERSION=5.0.9
# Fri, 24 Apr 2020 05:51:10 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Fri, 24 Apr 2020 05:51:10 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Fri, 24 Apr 2020 05:52:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 24 Apr 2020 05:52:17 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 24 Apr 2020 05:52:17 GMT
VOLUME [/data]
# Fri, 24 Apr 2020 05:52:17 GMT
WORKDIR /data
# Fri, 24 Apr 2020 05:52:17 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 24 Apr 2020 05:52:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 05:52:18 GMT
EXPOSE 6379
# Fri, 24 Apr 2020 05:52:18 GMT
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
	-	`sha256:7ed6bb387586efb069405e1b2fea60bf1718da22582dade16723a6ce6beb111c`  
		Last Modified: Fri, 24 Apr 2020 05:53:49 GMT  
		Size: 6.5 MB (6491980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ee2bc48c46cc40ec8951486a93e65583168f55239b5e10e350ceda82120fa3`  
		Last Modified: Fri, 24 Apr 2020 05:53:48 GMT  
		Size: 98.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae5b0c59c675cf868993ca6ec424636476caea5bc4e43525a866864d0b8bbd1`  
		Last Modified: Fri, 24 Apr 2020 05:53:48 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5.0.9-alpine` - linux; ppc64le

```console
$ docker pull redis@sha256:14dfcd56148c897338a1306bf23b392e6ffce4ee486ddfcd77fb515e8f0f1557
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.5 MB (10494033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a0a1b6eb6701cd8c4349958777c681d81e0520d3e82317e2419b56b4d4ce4bf`
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
# Fri, 24 Apr 2020 09:03:45 GMT
ENV REDIS_VERSION=5.0.9
# Fri, 24 Apr 2020 09:03:48 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Fri, 24 Apr 2020 09:03:50 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Fri, 24 Apr 2020 09:04:40 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 24 Apr 2020 09:04:46 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 24 Apr 2020 09:04:50 GMT
VOLUME [/data]
# Fri, 24 Apr 2020 09:04:53 GMT
WORKDIR /data
# Fri, 24 Apr 2020 09:04:56 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 24 Apr 2020 09:04:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 09:05:01 GMT
EXPOSE 6379
# Fri, 24 Apr 2020 09:05:07 GMT
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
	-	`sha256:1ad3f9cade0fa9bda2c0f45df3a77c780ebc4adea7badb3b8387fed928c60ed7`  
		Last Modified: Fri, 24 Apr 2020 09:07:21 GMT  
		Size: 7.3 MB (7260512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ad499a196593cd717672adacc0550293f8b2c00a5907255640b27d266bc05a`  
		Last Modified: Fri, 24 Apr 2020 09:07:21 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5831b0ffd2731f416315c93a640459b17492812a21b7a6fba00919faaeb1d5`  
		Last Modified: Fri, 24 Apr 2020 09:07:19 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5.0.9-alpine` - linux; s390x

```console
$ docker pull redis@sha256:5ad55b9f660c1e3b315e26e3497b9e4d270a5dd7ff431b14d9a17cf78fcac287
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (10008638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78dd64fd99b54ef1c40f2cd3351efcaf43b4d026dfcfe78315787e7a8220ffee`
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
# Fri, 24 Apr 2020 07:03:22 GMT
ENV REDIS_VERSION=5.0.9
# Fri, 24 Apr 2020 07:03:22 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Fri, 24 Apr 2020 07:03:22 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Fri, 24 Apr 2020 07:03:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 24 Apr 2020 07:03:53 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 24 Apr 2020 07:03:53 GMT
VOLUME [/data]
# Fri, 24 Apr 2020 07:03:54 GMT
WORKDIR /data
# Fri, 24 Apr 2020 07:03:54 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 24 Apr 2020 07:03:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 07:03:54 GMT
EXPOSE 6379
# Fri, 24 Apr 2020 07:03:54 GMT
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
	-	`sha256:4b3c809e9bcb4892e2da01d3bae84664c06e6bb0929c6813ef47a1aaaa3d675f`  
		Last Modified: Fri, 24 Apr 2020 07:05:07 GMT  
		Size: 7.0 MB (7016584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd1cb7e35314fbaf45935cb538fb36cc01e53dff4d37131a3497fd376720294e`  
		Last Modified: Fri, 24 Apr 2020 07:05:11 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529922dc84cb9fec77a0630b9ad535a7c843db2cd4518c25442c47fbc986d8b7`  
		Last Modified: Fri, 24 Apr 2020 07:05:06 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redis:5.0.9-alpine3.11`

```console
$ docker pull redis@sha256:83a3af36d5e57f2901b4783c313720e5fa3ecf0424ba86ad9775e06a9a5e35d0
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

### `redis:5.0.9-alpine3.11` - linux; amd64

```console
$ docker pull redis@sha256:d4ada5d910403607b3f579d7171f36108c2e1cf67da966a712812230171fc153
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (9998790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3661c84ee9d0f6312a076b69eb2bd112674cadb70ef7e1594c4f00193f8df08e`
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
# Fri, 24 Apr 2020 19:20:54 GMT
ENV REDIS_VERSION=5.0.9
# Fri, 24 Apr 2020 19:20:54 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Fri, 24 Apr 2020 19:20:55 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Fri, 24 Apr 2020 19:21:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 24 Apr 2020 19:21:49 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 24 Apr 2020 19:21:49 GMT
VOLUME [/data]
# Fri, 24 Apr 2020 19:21:50 GMT
WORKDIR /data
# Fri, 24 Apr 2020 19:21:50 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 24 Apr 2020 19:21:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 19:21:50 GMT
EXPOSE 6379
# Fri, 24 Apr 2020 19:21:50 GMT
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
	-	`sha256:3e45770272d96deeb96c4bfa3cffde811f318823b4422bdbbf909148dc5669bb`  
		Last Modified: Fri, 24 Apr 2020 19:23:14 GMT  
		Size: 6.8 MB (6781166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:558de8ea3153bdccfaf67fadf7bbbdc60bf357f33ff0070df617d6e22ad46a13`  
		Last Modified: Fri, 24 Apr 2020 19:23:13 GMT  
		Size: 99.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2c65255161264f51556db666aa812834b3f51c8403b09799a46e4d0909e4aa4`  
		Last Modified: Fri, 24 Apr 2020 19:23:12 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5.0.9-alpine3.11` - linux; arm variant v6

```console
$ docker pull redis@sha256:867b50998330ae4743e95c8be69dee7ad37cbba8057659bef4dc142838d7f3e0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9725047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:333723767b2b5747763b5483d4742558e9abe6d70b98ee05d527643b5eb088d5`
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
# Thu, 23 Apr 2020 22:31:34 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 22:31:35 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 22:31:36 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 22:32:24 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 22:32:27 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 22:32:29 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 22:32:30 GMT
WORKDIR /data
# Thu, 23 Apr 2020 22:32:31 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Thu, 23 Apr 2020 22:32:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 22:32:33 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 22:32:34 GMT
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
	-	`sha256:75a2919ec032b1198ca13b052499b7c193e45d93756a3b0d7bb10c8db4f3db65`  
		Last Modified: Thu, 23 Apr 2020 22:34:01 GMT  
		Size: 6.7 MB (6697511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b2e77e4c2604e8e74b4c471b4a04d1a768eb84eadcfcd3621f135f7d4d90ca`  
		Last Modified: Thu, 23 Apr 2020 22:33:57 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18df89faaf97292802f6bca82a98892b7b0a168230ca31ae16e3cf307614a7a8`  
		Last Modified: Thu, 23 Apr 2020 22:33:57 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5.0.9-alpine3.11` - linux; arm variant v7

```console
$ docker pull redis@sha256:1c10570f57cb14b4fbd3446c61303aeb7db18b45abffc49974d5bde7e4a89de4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9394623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56a7ba195be67da9c68c67aa8d6eefa737236f15d3a9b490504ce943465c3a9f`
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
# Fri, 24 Apr 2020 08:52:43 GMT
ENV REDIS_VERSION=5.0.9
# Fri, 24 Apr 2020 08:52:43 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Fri, 24 Apr 2020 08:52:44 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Fri, 24 Apr 2020 08:53:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 24 Apr 2020 08:53:30 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 24 Apr 2020 08:53:31 GMT
VOLUME [/data]
# Fri, 24 Apr 2020 08:53:32 GMT
WORKDIR /data
# Fri, 24 Apr 2020 08:53:32 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 24 Apr 2020 08:53:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 08:53:34 GMT
EXPOSE 6379
# Fri, 24 Apr 2020 08:53:34 GMT
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
	-	`sha256:531954b17ac2db3cd86f3ced48c7c4f9fe053fad0792b7038321a667c911953a`  
		Last Modified: Fri, 24 Apr 2020 08:55:41 GMT  
		Size: 6.6 MB (6570977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d550a31e99202186ed01f1a5a4c96bab49dc143ad2a113696ecb48947836c0`  
		Last Modified: Fri, 24 Apr 2020 08:55:38 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a842b77b23971198e093c671bcf1e2cf6df771a6138ffb4132bfb37af22f17`  
		Last Modified: Fri, 24 Apr 2020 08:55:38 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5.0.9-alpine3.11` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:2ebdecb52315772800ba4549b9dc83910d9ae7de5364c3092b0390d7266e94a9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9918976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b6acb4ad7ccdd962d8579a0929ab5920a1f58ff996cd4812188219c1eb74e91`
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
# Fri, 24 Apr 2020 12:46:32 GMT
ENV REDIS_VERSION=5.0.9
# Fri, 24 Apr 2020 12:46:33 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Fri, 24 Apr 2020 12:46:34 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Fri, 24 Apr 2020 12:47:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 24 Apr 2020 12:47:24 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 24 Apr 2020 12:47:24 GMT
VOLUME [/data]
# Fri, 24 Apr 2020 12:47:25 GMT
WORKDIR /data
# Fri, 24 Apr 2020 12:47:26 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 24 Apr 2020 12:47:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 12:47:28 GMT
EXPOSE 6379
# Fri, 24 Apr 2020 12:47:29 GMT
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
	-	`sha256:f5ca1db598d2278e5526b65dcad0d96f0f0264060f879f1b437f58a467e27382`  
		Last Modified: Fri, 24 Apr 2020 12:49:17 GMT  
		Size: 6.8 MB (6788089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87542dce16ad38aeb18ffe2e2266f3bd9b8cbc70f6f4450be0e9f621022fabb5`  
		Last Modified: Fri, 24 Apr 2020 12:49:15 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a20d19811afde1a300515cade1279f18fb3ca0ef1800b52dcb45127731bd5f4`  
		Last Modified: Fri, 24 Apr 2020 12:49:15 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5.0.9-alpine3.11` - linux; 386

```console
$ docker pull redis@sha256:3ab6896b5efe215c5cc110a835fecb73d5f55672ad4443f4baf51822db1854c6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9710040 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bba820d7067104939d7ec907ee1fa581e9c7d40b0a204a14caf709f4dce84732`
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
# Fri, 24 Apr 2020 05:51:10 GMT
ENV REDIS_VERSION=5.0.9
# Fri, 24 Apr 2020 05:51:10 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Fri, 24 Apr 2020 05:51:10 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Fri, 24 Apr 2020 05:52:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 24 Apr 2020 05:52:17 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 24 Apr 2020 05:52:17 GMT
VOLUME [/data]
# Fri, 24 Apr 2020 05:52:17 GMT
WORKDIR /data
# Fri, 24 Apr 2020 05:52:17 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 24 Apr 2020 05:52:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 05:52:18 GMT
EXPOSE 6379
# Fri, 24 Apr 2020 05:52:18 GMT
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
	-	`sha256:7ed6bb387586efb069405e1b2fea60bf1718da22582dade16723a6ce6beb111c`  
		Last Modified: Fri, 24 Apr 2020 05:53:49 GMT  
		Size: 6.5 MB (6491980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ee2bc48c46cc40ec8951486a93e65583168f55239b5e10e350ceda82120fa3`  
		Last Modified: Fri, 24 Apr 2020 05:53:48 GMT  
		Size: 98.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae5b0c59c675cf868993ca6ec424636476caea5bc4e43525a866864d0b8bbd1`  
		Last Modified: Fri, 24 Apr 2020 05:53:48 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5.0.9-alpine3.11` - linux; ppc64le

```console
$ docker pull redis@sha256:14dfcd56148c897338a1306bf23b392e6ffce4ee486ddfcd77fb515e8f0f1557
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.5 MB (10494033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a0a1b6eb6701cd8c4349958777c681d81e0520d3e82317e2419b56b4d4ce4bf`
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
# Fri, 24 Apr 2020 09:03:45 GMT
ENV REDIS_VERSION=5.0.9
# Fri, 24 Apr 2020 09:03:48 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Fri, 24 Apr 2020 09:03:50 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Fri, 24 Apr 2020 09:04:40 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 24 Apr 2020 09:04:46 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 24 Apr 2020 09:04:50 GMT
VOLUME [/data]
# Fri, 24 Apr 2020 09:04:53 GMT
WORKDIR /data
# Fri, 24 Apr 2020 09:04:56 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 24 Apr 2020 09:04:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 09:05:01 GMT
EXPOSE 6379
# Fri, 24 Apr 2020 09:05:07 GMT
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
	-	`sha256:1ad3f9cade0fa9bda2c0f45df3a77c780ebc4adea7badb3b8387fed928c60ed7`  
		Last Modified: Fri, 24 Apr 2020 09:07:21 GMT  
		Size: 7.3 MB (7260512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ad499a196593cd717672adacc0550293f8b2c00a5907255640b27d266bc05a`  
		Last Modified: Fri, 24 Apr 2020 09:07:21 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5831b0ffd2731f416315c93a640459b17492812a21b7a6fba00919faaeb1d5`  
		Last Modified: Fri, 24 Apr 2020 09:07:19 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5.0.9-alpine3.11` - linux; s390x

```console
$ docker pull redis@sha256:5ad55b9f660c1e3b315e26e3497b9e4d270a5dd7ff431b14d9a17cf78fcac287
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (10008638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78dd64fd99b54ef1c40f2cd3351efcaf43b4d026dfcfe78315787e7a8220ffee`
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
# Fri, 24 Apr 2020 07:03:22 GMT
ENV REDIS_VERSION=5.0.9
# Fri, 24 Apr 2020 07:03:22 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Fri, 24 Apr 2020 07:03:22 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Fri, 24 Apr 2020 07:03:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 24 Apr 2020 07:03:53 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 24 Apr 2020 07:03:53 GMT
VOLUME [/data]
# Fri, 24 Apr 2020 07:03:54 GMT
WORKDIR /data
# Fri, 24 Apr 2020 07:03:54 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 24 Apr 2020 07:03:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 07:03:54 GMT
EXPOSE 6379
# Fri, 24 Apr 2020 07:03:54 GMT
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
	-	`sha256:4b3c809e9bcb4892e2da01d3bae84664c06e6bb0929c6813ef47a1aaaa3d675f`  
		Last Modified: Fri, 24 Apr 2020 07:05:07 GMT  
		Size: 7.0 MB (7016584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd1cb7e35314fbaf45935cb538fb36cc01e53dff4d37131a3497fd376720294e`  
		Last Modified: Fri, 24 Apr 2020 07:05:11 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529922dc84cb9fec77a0630b9ad535a7c843db2cd4518c25442c47fbc986d8b7`  
		Last Modified: Fri, 24 Apr 2020 07:05:06 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redis:5.0.9-buster`

```console
$ docker pull redis@sha256:157a95b41b0dca8c308a33489dfdb28019e033110320414b4b16fad7d28c0f9f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `redis:5.0.9-buster` - linux; amd64

```console
$ docker pull redis@sha256:43dbbe6f633572d66e84e7162245d8d70a18f00b819d6c0bf98ca02109f4788c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35863297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4d3716dbb72408a7843e12d7d9f6a5addf7ab28ac21e9e9da4a6a51f1b32da9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:20:32 GMT
ADD file:9b8be2b52ee0fa31da1b6256099030b73546253a57e94cccb24605cd888bb74d in / 
# Thu, 23 Apr 2020 00:20:32 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 19:48:34 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 19:48:34 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 19:48:46 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 19:50:08 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 19:50:08 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 19:50:08 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 19:51:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 19:51:26 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 19:51:26 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 19:51:27 GMT
WORKDIR /data
# Thu, 23 Apr 2020 19:51:27 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 19:51:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 19:51:28 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 19:51:28 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:54fec2fa59d0a0de9cd2dec9850b36c43de451f1fd1c0a5bf8f1cf26a61a5da4`  
		Last Modified: Thu, 23 Apr 2020 00:25:10 GMT  
		Size: 27.1 MB (27098254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c94e11103d92f2a83b82e5d4287445cba073af0002cecee98d85d68ccec0f89`  
		Last Modified: Thu, 23 Apr 2020 19:55:42 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ab1bfc453f19989c401c2f0622df3363b5182bdea1af9e59ee2ceea3a9931c`  
		Last Modified: Thu, 23 Apr 2020 19:55:43 GMT  
		Size: 1.4 MB (1417711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f71e6b94d83f5a0df5d032ce4998b4834287bd4ed307ff7c9a31ad0a60caa98`  
		Last Modified: Thu, 23 Apr 2020 19:55:55 GMT  
		Size: 7.3 MB (7345094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2729a8234dd5e724571528d78d5f581702abc77be39db93fc0ae741340eb1c18`  
		Last Modified: Thu, 23 Apr 2020 19:55:53 GMT  
		Size: 97.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2683d7f177455cf86b4cf424cc757f1d177d5772df77bdaeeace411006eb88a5`  
		Last Modified: Thu, 23 Apr 2020 19:55:53 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5.0.9-buster` - linux; arm variant v5

```console
$ docker pull redis@sha256:5a474d0e7c55a7e45ddaf530f4f2ab4bc8dcaba6d85b0829f1121f7fe53414fd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.4 MB (33394023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b83a1e222e2b9be5acf1ae9a03cd2e6d2c7a4efcd3b73a275481c652552de80`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:52:22 GMT
ADD file:62a9732be4e3237ccc896f724a34606e01f351c4877e52c9a9cd85029c06b956 in / 
# Thu, 23 Apr 2020 00:52:23 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 09:33:20 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 09:33:21 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 09:33:56 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 09:35:38 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 09:35:39 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 09:35:39 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 09:36:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 09:36:48 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 09:36:48 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 09:36:49 GMT
WORKDIR /data
# Thu, 23 Apr 2020 09:36:50 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 09:36:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 09:36:51 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 09:36:52 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:a8c46e5952878f9f324df86c5a2b45b2e0020f6721e820981e74461d77a100dd`  
		Last Modified: Thu, 23 Apr 2020 00:59:50 GMT  
		Size: 24.8 MB (24836319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471287e557b84038803c3a26dee3987da48cbcae6529a77a28f486e4527757f7`  
		Last Modified: Thu, 23 Apr 2020 09:39:42 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:016e8ff197695f0c8e2c3ae127ac9459df9c71e52ae54500970e692d2799c944`  
		Last Modified: Thu, 23 Apr 2020 09:39:42 GMT  
		Size: 1.4 MB (1376131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd64ec452edc906dc611493aae3c90529a0d5787d8dc3b8c1088b41b53379d2d`  
		Last Modified: Thu, 23 Apr 2020 09:40:07 GMT  
		Size: 7.2 MB (7179305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ca72abe00cf1354dc501a32ed89705fdacd4905631c42186458d9d3202cc90`  
		Last Modified: Thu, 23 Apr 2020 09:40:05 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e7807337a06858bed0eac541f5935b123a4abb0d973dacb1973753c6dcb2469`  
		Last Modified: Thu, 23 Apr 2020 09:40:04 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5.0.9-buster` - linux; arm variant v7

```console
$ docker pull redis@sha256:afc097fd6784e016756816ecc4ae33dc9ef22f5715db3593b90b7ec17e906edf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.1 MB (31109340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:632cd87ac6e4d8bda115f5e32e2b45cb8e28c59bd4c6e24b87985cf6b1f93354`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 01:03:26 GMT
ADD file:db6122b36f3e70c5f490b50afba99d49fa345f11d0f5c77bb3c6749f8e2a4f81 in / 
# Thu, 23 Apr 2020 01:03:28 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 13:54:58 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 13:54:59 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 13:55:22 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 13:57:35 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 13:57:35 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 13:57:36 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 13:58:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 13:58:37 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 13:58:38 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 13:58:39 GMT
WORKDIR /data
# Thu, 23 Apr 2020 13:58:39 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 13:58:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 13:58:41 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 13:58:41 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:50fb0052086928803f00724ca465c89c45dde5b082b1e59dadb8101286dd5ab6`  
		Last Modified: Thu, 23 Apr 2020 01:11:08 GMT  
		Size: 22.7 MB (22705377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98fc1f5e139d98aa45f74dfddb32ca22bec51ecf2fcab9bb372d91c14cc971d2`  
		Last Modified: Thu, 23 Apr 2020 14:00:18 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa98edd0b4c481052caeb348af3e906ef75764353840cfe2518af73963fcf2d`  
		Last Modified: Thu, 23 Apr 2020 14:00:18 GMT  
		Size: 1.4 MB (1368177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1ae9f68f12644f241fb270f9baf2e62d5b1380083acada1fdae86374998430`  
		Last Modified: Thu, 23 Apr 2020 14:00:21 GMT  
		Size: 7.0 MB (7033517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a23909059832233f41bcba599ec5bb698e278c652cf313dc6e8724fae8aa40cf`  
		Last Modified: Thu, 23 Apr 2020 14:00:19 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f5f6de32828cf1cb128a0cba17dc0396dead74aa6cc963394ac4f8b05540179`  
		Last Modified: Thu, 23 Apr 2020 14:00:18 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5.0.9-buster` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:be463e278dc2125ea4c8984cd6a990353dfaa7f94570856734f86b900debc008
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 MB (34548547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0da52d2315939d969b12f3db6ae0aa5716074833f1ef06a42a544aec452d0ab2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:54:55 GMT
ADD file:581ee9c3c19f0d971aeda008fd399f59171cae75e8936b967dbf3888db4fc0d0 in / 
# Thu, 23 Apr 2020 00:54:58 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 16:01:56 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 16:01:57 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 16:02:29 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 16:04:19 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 16:04:20 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 16:04:20 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 16:05:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 16:05:20 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 16:05:20 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 16:05:21 GMT
WORKDIR /data
# Thu, 23 Apr 2020 16:05:21 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 16:05:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 16:05:22 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 16:05:24 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:bdc84a41f2513e28e99efeff9fcbb196b7df9883fb30532184bd67ca415b4673`  
		Last Modified: Thu, 23 Apr 2020 01:03:27 GMT  
		Size: 25.9 MB (25857800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698d3e76f19fb83cee90fe071552d86509322f0b8316774550c1ea7398327369`  
		Last Modified: Thu, 23 Apr 2020 16:07:31 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac4bbea6248caf60d5eca4d3e15d73d9cc18a5154a795c5ca3937eb040c9daae`  
		Last Modified: Thu, 23 Apr 2020 16:07:31 GMT  
		Size: 1.4 MB (1352987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1590123d45656fbb5cabd427b87908fd7347ef2fc6b0fba354f2b83771ec8882`  
		Last Modified: Thu, 23 Apr 2020 16:07:57 GMT  
		Size: 7.3 MB (7335481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e21891406b8ecd80c9cc4be90337cdd8d8935229002e8162d9afc9b68d2a4c30`  
		Last Modified: Thu, 23 Apr 2020 16:07:55 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d793eb07a5bc754267edbd54feb6cb25e4c28e7056a87e27960de4901d1dcc3`  
		Last Modified: Thu, 23 Apr 2020 16:07:55 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5.0.9-buster` - linux; 386

```console
$ docker pull redis@sha256:0ac1dbfd6ca80b45aa587ecaa0632457ca254eea674a50e8574e8677f7a193a0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.2 MB (36151602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34c763545c4e57aabcdc00c9448e439a81bdaf47ae32d7711bc8e1252fb7ef59`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:39:36 GMT
ADD file:ca6a74f6b738c738c033152fab2a9aacf22bec5f19a994e6a02b5f919ee33ee9 in / 
# Thu, 23 Apr 2020 00:39:36 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 11:23:53 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 11:23:53 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 11:24:11 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 11:26:28 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 11:26:28 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 11:26:28 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 11:27:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 11:27:59 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 11:28:00 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 11:28:00 GMT
WORKDIR /data
# Thu, 23 Apr 2020 11:28:00 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 11:28:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 11:28:01 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 11:28:01 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:5d3da8f33b97fc107a05b3255a55836b76df9f817de632b1fb63c6e9c024f0df`  
		Last Modified: Thu, 23 Apr 2020 00:44:35 GMT  
		Size: 27.8 MB (27753972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f572d913eaf53def72d8eeff5384464ae75f0da9041d63ef0cd2fb2a43e21e`  
		Last Modified: Thu, 23 Apr 2020 11:30:12 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36c13a7e7929be4f05fbeddd74c94dfe85b704c504f7d13aa45bdb84bae79ccb`  
		Last Modified: Thu, 23 Apr 2020 11:30:12 GMT  
		Size: 1.4 MB (1387411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680a9b72444c93256224c2c5394c18343047b8b7dc305a4301401e7a6b494d03`  
		Last Modified: Thu, 23 Apr 2020 11:30:25 GMT  
		Size: 7.0 MB (7007988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e6148f8fb3eb037aaf97a9736b49d92d77541c5bbb6219db62f8af4f8d5e54`  
		Last Modified: Thu, 23 Apr 2020 11:30:23 GMT  
		Size: 97.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fae33d9962de4399f135693d495b300515e9d363f74683c3c366cd6e32290e1`  
		Last Modified: Thu, 23 Apr 2020 11:30:23 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5.0.9-buster` - linux; mips64le

```console
$ docker pull redis@sha256:8860ea6be85bfa12a7a62f37e07716f197be8e76f498d1e62d3c4319582a3b60
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34731728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eab8ac536ee15de9306c977271c71a293db05c67e582fe002279ba86c8fff0a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:09:47 GMT
ADD file:7509945bd8a224048260e88b466aa3b156615e16b64e0a6702da277052fcb98b in / 
# Thu, 23 Apr 2020 00:09:48 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 09:24:32 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 09:24:33 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 09:25:02 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 09:28:42 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 09:28:42 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 09:28:43 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 09:31:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 09:32:01 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 09:32:01 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 09:32:01 GMT
WORKDIR /data
# Thu, 23 Apr 2020 09:32:02 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 09:32:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 09:32:02 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 09:32:03 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:ae8f0fa6cb0d971b4b8fedf7fc9b00f61f780b383fe7d64e6c2e4be8d20c3987`  
		Last Modified: Thu, 23 Apr 2020 00:17:46 GMT  
		Size: 25.8 MB (25762125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faf65c067540cd52d99f7f6df4511fb45d6a0485e47338d0239a052fcd64c8e3`  
		Last Modified: Thu, 23 Apr 2020 09:34:32 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef207bf80aefb18eba12c119d07499e37b5ea7bec06bc1e0c2dd749ddde45a1`  
		Last Modified: Thu, 23 Apr 2020 09:34:34 GMT  
		Size: 1.3 MB (1305489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae62dd92cc34f4856c15b7614910c5578f2d91d96d96469c21f8ca741c1061f5`  
		Last Modified: Thu, 23 Apr 2020 09:35:08 GMT  
		Size: 7.7 MB (7661872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693fe2f4d6e93636c838f7fb3a49c859d72138e5a25fd1687e590fcf3bb74dfb`  
		Last Modified: Thu, 23 Apr 2020 09:35:00 GMT  
		Size: 99.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:153c8eb8631e42a4705a53461aeb1c1edea4a60ad71a759b5eafeccbf3f5c142`  
		Last Modified: Thu, 23 Apr 2020 09:35:00 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5.0.9-buster` - linux; ppc64le

```console
$ docker pull redis@sha256:e1c410783ee0d501a9804b3050db559054e95e91bb3cd8f3e81324baef92f730
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.7 MB (39696544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34098209a59e39ee25eeb2b0bf53ba98f873314c75110d6841a0793d5e1bc182`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:36:00 GMT
ADD file:5b3c3d2945800e1743dc02a4f68bd830fe2f67ca437223692eb460147c158c2b in / 
# Thu, 23 Apr 2020 00:36:04 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 17:29:48 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 17:29:51 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 17:31:38 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 17:35:14 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 17:35:18 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 17:35:23 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 17:38:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 17:38:25 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 17:38:28 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 17:38:32 GMT
WORKDIR /data
# Thu, 23 Apr 2020 17:38:34 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 17:38:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 17:38:42 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 17:38:45 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:012c6cdbd1af202bbfbea5945fafbb9aca9097f1fa3cb493a29155fdc02cc43c`  
		Last Modified: Thu, 23 Apr 2020 00:50:14 GMT  
		Size: 30.5 MB (30524638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee5a34bf53dadebb7466557f439affba6f1c11ddbdd7d2c1376f9540c294a7a`  
		Last Modified: Thu, 23 Apr 2020 17:42:03 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dedf97e3c0bcb476732135fc70dee2ba4766ff50ec51f93b1929ebaa6c4863f`  
		Last Modified: Thu, 23 Apr 2020 17:42:03 GMT  
		Size: 1.3 MB (1335327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2a1294a7da3aa34af8f45c22665913b8780fcf4dec6b52b108541e496dd0cc`  
		Last Modified: Thu, 23 Apr 2020 17:42:27 GMT  
		Size: 7.8 MB (7834296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51726f5fc1a7b6d031cad4d822aaf6c1801262570fb662454f1f2dc93cd4e551`  
		Last Modified: Thu, 23 Apr 2020 17:42:25 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e62728fce47996c1059a9f4f18e5e1efea4ebc55e17f82aa362f8985e7f019e`  
		Last Modified: Thu, 23 Apr 2020 17:42:25 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5.0.9-buster` - linux; s390x

```console
$ docker pull redis@sha256:80a22e71a515d761d2c50a5873fc228fe165a627f9f91641391ce1548bc23f03
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34709447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5556ba73cac9fdc7f38ea53f8961a08497e52b1fa62f83611a9228a5d495e8fb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:51:48 GMT
ADD file:f6c2560f9185c1bcaff95e576e57449f606d51b85fad02646c1b0962bc9353c9 in / 
# Thu, 23 Apr 2020 00:51:50 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 06:58:44 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 06:58:44 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 06:58:58 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 06:59:46 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 06:59:47 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 06:59:47 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 07:00:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 07:00:24 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 07:00:24 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 07:00:24 GMT
WORKDIR /data
# Thu, 23 Apr 2020 07:00:24 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 07:00:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 07:00:25 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 07:00:25 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:d89dc3741ad42b79c3d8545495c429f3100d3f22234ff993bd04017b0675e868`  
		Last Modified: Thu, 23 Apr 2020 00:56:00 GMT  
		Size: 25.7 MB (25712105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c9894c70b29dc7cbad7e69c5f898b0a5d6f82aac9aff00e2645a6f8a9eff88`  
		Last Modified: Thu, 23 Apr 2020 07:01:34 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fba24ca231c607425b0e92a8a39c3174a8b9cb56ddeee71fc43f2f9dd9b1d2c`  
		Last Modified: Thu, 23 Apr 2020 07:01:35 GMT  
		Size: 1.4 MB (1403679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22d299e81a09eaaf9da803a2b3775444f312a34b2b7dd8e0c1c10d0171225ba`  
		Last Modified: Thu, 23 Apr 2020 07:01:52 GMT  
		Size: 7.6 MB (7591385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46db2cefe8baf230709535dd5f96c93520ca156d9821649ce8e8a2410e49d54`  
		Last Modified: Thu, 23 Apr 2020 07:01:56 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ec0a42c81dfec4356c31366a6ddf246ebac63394fafd37549a4483fd537513`  
		Last Modified: Thu, 23 Apr 2020 07:01:50 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redis:5.0-alpine`

```console
$ docker pull redis@sha256:83a3af36d5e57f2901b4783c313720e5fa3ecf0424ba86ad9775e06a9a5e35d0
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

### `redis:5.0-alpine` - linux; amd64

```console
$ docker pull redis@sha256:d4ada5d910403607b3f579d7171f36108c2e1cf67da966a712812230171fc153
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (9998790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3661c84ee9d0f6312a076b69eb2bd112674cadb70ef7e1594c4f00193f8df08e`
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
# Fri, 24 Apr 2020 19:20:54 GMT
ENV REDIS_VERSION=5.0.9
# Fri, 24 Apr 2020 19:20:54 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Fri, 24 Apr 2020 19:20:55 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Fri, 24 Apr 2020 19:21:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 24 Apr 2020 19:21:49 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 24 Apr 2020 19:21:49 GMT
VOLUME [/data]
# Fri, 24 Apr 2020 19:21:50 GMT
WORKDIR /data
# Fri, 24 Apr 2020 19:21:50 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 24 Apr 2020 19:21:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 19:21:50 GMT
EXPOSE 6379
# Fri, 24 Apr 2020 19:21:50 GMT
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
	-	`sha256:3e45770272d96deeb96c4bfa3cffde811f318823b4422bdbbf909148dc5669bb`  
		Last Modified: Fri, 24 Apr 2020 19:23:14 GMT  
		Size: 6.8 MB (6781166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:558de8ea3153bdccfaf67fadf7bbbdc60bf357f33ff0070df617d6e22ad46a13`  
		Last Modified: Fri, 24 Apr 2020 19:23:13 GMT  
		Size: 99.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2c65255161264f51556db666aa812834b3f51c8403b09799a46e4d0909e4aa4`  
		Last Modified: Fri, 24 Apr 2020 19:23:12 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5.0-alpine` - linux; arm variant v6

```console
$ docker pull redis@sha256:867b50998330ae4743e95c8be69dee7ad37cbba8057659bef4dc142838d7f3e0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9725047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:333723767b2b5747763b5483d4742558e9abe6d70b98ee05d527643b5eb088d5`
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
# Thu, 23 Apr 2020 22:31:34 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 22:31:35 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 22:31:36 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 22:32:24 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 22:32:27 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 22:32:29 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 22:32:30 GMT
WORKDIR /data
# Thu, 23 Apr 2020 22:32:31 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Thu, 23 Apr 2020 22:32:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 22:32:33 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 22:32:34 GMT
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
	-	`sha256:75a2919ec032b1198ca13b052499b7c193e45d93756a3b0d7bb10c8db4f3db65`  
		Last Modified: Thu, 23 Apr 2020 22:34:01 GMT  
		Size: 6.7 MB (6697511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b2e77e4c2604e8e74b4c471b4a04d1a768eb84eadcfcd3621f135f7d4d90ca`  
		Last Modified: Thu, 23 Apr 2020 22:33:57 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18df89faaf97292802f6bca82a98892b7b0a168230ca31ae16e3cf307614a7a8`  
		Last Modified: Thu, 23 Apr 2020 22:33:57 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5.0-alpine` - linux; arm variant v7

```console
$ docker pull redis@sha256:1c10570f57cb14b4fbd3446c61303aeb7db18b45abffc49974d5bde7e4a89de4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9394623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56a7ba195be67da9c68c67aa8d6eefa737236f15d3a9b490504ce943465c3a9f`
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
# Fri, 24 Apr 2020 08:52:43 GMT
ENV REDIS_VERSION=5.0.9
# Fri, 24 Apr 2020 08:52:43 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Fri, 24 Apr 2020 08:52:44 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Fri, 24 Apr 2020 08:53:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 24 Apr 2020 08:53:30 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 24 Apr 2020 08:53:31 GMT
VOLUME [/data]
# Fri, 24 Apr 2020 08:53:32 GMT
WORKDIR /data
# Fri, 24 Apr 2020 08:53:32 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 24 Apr 2020 08:53:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 08:53:34 GMT
EXPOSE 6379
# Fri, 24 Apr 2020 08:53:34 GMT
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
	-	`sha256:531954b17ac2db3cd86f3ced48c7c4f9fe053fad0792b7038321a667c911953a`  
		Last Modified: Fri, 24 Apr 2020 08:55:41 GMT  
		Size: 6.6 MB (6570977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d550a31e99202186ed01f1a5a4c96bab49dc143ad2a113696ecb48947836c0`  
		Last Modified: Fri, 24 Apr 2020 08:55:38 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a842b77b23971198e093c671bcf1e2cf6df771a6138ffb4132bfb37af22f17`  
		Last Modified: Fri, 24 Apr 2020 08:55:38 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5.0-alpine` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:2ebdecb52315772800ba4549b9dc83910d9ae7de5364c3092b0390d7266e94a9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9918976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b6acb4ad7ccdd962d8579a0929ab5920a1f58ff996cd4812188219c1eb74e91`
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
# Fri, 24 Apr 2020 12:46:32 GMT
ENV REDIS_VERSION=5.0.9
# Fri, 24 Apr 2020 12:46:33 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Fri, 24 Apr 2020 12:46:34 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Fri, 24 Apr 2020 12:47:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 24 Apr 2020 12:47:24 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 24 Apr 2020 12:47:24 GMT
VOLUME [/data]
# Fri, 24 Apr 2020 12:47:25 GMT
WORKDIR /data
# Fri, 24 Apr 2020 12:47:26 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 24 Apr 2020 12:47:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 12:47:28 GMT
EXPOSE 6379
# Fri, 24 Apr 2020 12:47:29 GMT
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
	-	`sha256:f5ca1db598d2278e5526b65dcad0d96f0f0264060f879f1b437f58a467e27382`  
		Last Modified: Fri, 24 Apr 2020 12:49:17 GMT  
		Size: 6.8 MB (6788089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87542dce16ad38aeb18ffe2e2266f3bd9b8cbc70f6f4450be0e9f621022fabb5`  
		Last Modified: Fri, 24 Apr 2020 12:49:15 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a20d19811afde1a300515cade1279f18fb3ca0ef1800b52dcb45127731bd5f4`  
		Last Modified: Fri, 24 Apr 2020 12:49:15 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5.0-alpine` - linux; 386

```console
$ docker pull redis@sha256:3ab6896b5efe215c5cc110a835fecb73d5f55672ad4443f4baf51822db1854c6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9710040 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bba820d7067104939d7ec907ee1fa581e9c7d40b0a204a14caf709f4dce84732`
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
# Fri, 24 Apr 2020 05:51:10 GMT
ENV REDIS_VERSION=5.0.9
# Fri, 24 Apr 2020 05:51:10 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Fri, 24 Apr 2020 05:51:10 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Fri, 24 Apr 2020 05:52:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 24 Apr 2020 05:52:17 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 24 Apr 2020 05:52:17 GMT
VOLUME [/data]
# Fri, 24 Apr 2020 05:52:17 GMT
WORKDIR /data
# Fri, 24 Apr 2020 05:52:17 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 24 Apr 2020 05:52:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 05:52:18 GMT
EXPOSE 6379
# Fri, 24 Apr 2020 05:52:18 GMT
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
	-	`sha256:7ed6bb387586efb069405e1b2fea60bf1718da22582dade16723a6ce6beb111c`  
		Last Modified: Fri, 24 Apr 2020 05:53:49 GMT  
		Size: 6.5 MB (6491980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ee2bc48c46cc40ec8951486a93e65583168f55239b5e10e350ceda82120fa3`  
		Last Modified: Fri, 24 Apr 2020 05:53:48 GMT  
		Size: 98.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae5b0c59c675cf868993ca6ec424636476caea5bc4e43525a866864d0b8bbd1`  
		Last Modified: Fri, 24 Apr 2020 05:53:48 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5.0-alpine` - linux; ppc64le

```console
$ docker pull redis@sha256:14dfcd56148c897338a1306bf23b392e6ffce4ee486ddfcd77fb515e8f0f1557
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.5 MB (10494033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a0a1b6eb6701cd8c4349958777c681d81e0520d3e82317e2419b56b4d4ce4bf`
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
# Fri, 24 Apr 2020 09:03:45 GMT
ENV REDIS_VERSION=5.0.9
# Fri, 24 Apr 2020 09:03:48 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Fri, 24 Apr 2020 09:03:50 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Fri, 24 Apr 2020 09:04:40 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 24 Apr 2020 09:04:46 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 24 Apr 2020 09:04:50 GMT
VOLUME [/data]
# Fri, 24 Apr 2020 09:04:53 GMT
WORKDIR /data
# Fri, 24 Apr 2020 09:04:56 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 24 Apr 2020 09:04:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 09:05:01 GMT
EXPOSE 6379
# Fri, 24 Apr 2020 09:05:07 GMT
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
	-	`sha256:1ad3f9cade0fa9bda2c0f45df3a77c780ebc4adea7badb3b8387fed928c60ed7`  
		Last Modified: Fri, 24 Apr 2020 09:07:21 GMT  
		Size: 7.3 MB (7260512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ad499a196593cd717672adacc0550293f8b2c00a5907255640b27d266bc05a`  
		Last Modified: Fri, 24 Apr 2020 09:07:21 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5831b0ffd2731f416315c93a640459b17492812a21b7a6fba00919faaeb1d5`  
		Last Modified: Fri, 24 Apr 2020 09:07:19 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5.0-alpine` - linux; s390x

```console
$ docker pull redis@sha256:5ad55b9f660c1e3b315e26e3497b9e4d270a5dd7ff431b14d9a17cf78fcac287
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (10008638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78dd64fd99b54ef1c40f2cd3351efcaf43b4d026dfcfe78315787e7a8220ffee`
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
# Fri, 24 Apr 2020 07:03:22 GMT
ENV REDIS_VERSION=5.0.9
# Fri, 24 Apr 2020 07:03:22 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Fri, 24 Apr 2020 07:03:22 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Fri, 24 Apr 2020 07:03:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 24 Apr 2020 07:03:53 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 24 Apr 2020 07:03:53 GMT
VOLUME [/data]
# Fri, 24 Apr 2020 07:03:54 GMT
WORKDIR /data
# Fri, 24 Apr 2020 07:03:54 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 24 Apr 2020 07:03:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 07:03:54 GMT
EXPOSE 6379
# Fri, 24 Apr 2020 07:03:54 GMT
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
	-	`sha256:4b3c809e9bcb4892e2da01d3bae84664c06e6bb0929c6813ef47a1aaaa3d675f`  
		Last Modified: Fri, 24 Apr 2020 07:05:07 GMT  
		Size: 7.0 MB (7016584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd1cb7e35314fbaf45935cb538fb36cc01e53dff4d37131a3497fd376720294e`  
		Last Modified: Fri, 24 Apr 2020 07:05:11 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529922dc84cb9fec77a0630b9ad535a7c843db2cd4518c25442c47fbc986d8b7`  
		Last Modified: Fri, 24 Apr 2020 07:05:06 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redis:5.0-alpine3.11`

```console
$ docker pull redis@sha256:83a3af36d5e57f2901b4783c313720e5fa3ecf0424ba86ad9775e06a9a5e35d0
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

### `redis:5.0-alpine3.11` - linux; amd64

```console
$ docker pull redis@sha256:d4ada5d910403607b3f579d7171f36108c2e1cf67da966a712812230171fc153
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (9998790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3661c84ee9d0f6312a076b69eb2bd112674cadb70ef7e1594c4f00193f8df08e`
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
# Fri, 24 Apr 2020 19:20:54 GMT
ENV REDIS_VERSION=5.0.9
# Fri, 24 Apr 2020 19:20:54 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Fri, 24 Apr 2020 19:20:55 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Fri, 24 Apr 2020 19:21:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 24 Apr 2020 19:21:49 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 24 Apr 2020 19:21:49 GMT
VOLUME [/data]
# Fri, 24 Apr 2020 19:21:50 GMT
WORKDIR /data
# Fri, 24 Apr 2020 19:21:50 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 24 Apr 2020 19:21:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 19:21:50 GMT
EXPOSE 6379
# Fri, 24 Apr 2020 19:21:50 GMT
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
	-	`sha256:3e45770272d96deeb96c4bfa3cffde811f318823b4422bdbbf909148dc5669bb`  
		Last Modified: Fri, 24 Apr 2020 19:23:14 GMT  
		Size: 6.8 MB (6781166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:558de8ea3153bdccfaf67fadf7bbbdc60bf357f33ff0070df617d6e22ad46a13`  
		Last Modified: Fri, 24 Apr 2020 19:23:13 GMT  
		Size: 99.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2c65255161264f51556db666aa812834b3f51c8403b09799a46e4d0909e4aa4`  
		Last Modified: Fri, 24 Apr 2020 19:23:12 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5.0-alpine3.11` - linux; arm variant v6

```console
$ docker pull redis@sha256:867b50998330ae4743e95c8be69dee7ad37cbba8057659bef4dc142838d7f3e0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9725047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:333723767b2b5747763b5483d4742558e9abe6d70b98ee05d527643b5eb088d5`
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
# Thu, 23 Apr 2020 22:31:34 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 22:31:35 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 22:31:36 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 22:32:24 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 22:32:27 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 22:32:29 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 22:32:30 GMT
WORKDIR /data
# Thu, 23 Apr 2020 22:32:31 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Thu, 23 Apr 2020 22:32:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 22:32:33 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 22:32:34 GMT
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
	-	`sha256:75a2919ec032b1198ca13b052499b7c193e45d93756a3b0d7bb10c8db4f3db65`  
		Last Modified: Thu, 23 Apr 2020 22:34:01 GMT  
		Size: 6.7 MB (6697511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b2e77e4c2604e8e74b4c471b4a04d1a768eb84eadcfcd3621f135f7d4d90ca`  
		Last Modified: Thu, 23 Apr 2020 22:33:57 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18df89faaf97292802f6bca82a98892b7b0a168230ca31ae16e3cf307614a7a8`  
		Last Modified: Thu, 23 Apr 2020 22:33:57 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5.0-alpine3.11` - linux; arm variant v7

```console
$ docker pull redis@sha256:1c10570f57cb14b4fbd3446c61303aeb7db18b45abffc49974d5bde7e4a89de4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9394623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56a7ba195be67da9c68c67aa8d6eefa737236f15d3a9b490504ce943465c3a9f`
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
# Fri, 24 Apr 2020 08:52:43 GMT
ENV REDIS_VERSION=5.0.9
# Fri, 24 Apr 2020 08:52:43 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Fri, 24 Apr 2020 08:52:44 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Fri, 24 Apr 2020 08:53:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 24 Apr 2020 08:53:30 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 24 Apr 2020 08:53:31 GMT
VOLUME [/data]
# Fri, 24 Apr 2020 08:53:32 GMT
WORKDIR /data
# Fri, 24 Apr 2020 08:53:32 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 24 Apr 2020 08:53:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 08:53:34 GMT
EXPOSE 6379
# Fri, 24 Apr 2020 08:53:34 GMT
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
	-	`sha256:531954b17ac2db3cd86f3ced48c7c4f9fe053fad0792b7038321a667c911953a`  
		Last Modified: Fri, 24 Apr 2020 08:55:41 GMT  
		Size: 6.6 MB (6570977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d550a31e99202186ed01f1a5a4c96bab49dc143ad2a113696ecb48947836c0`  
		Last Modified: Fri, 24 Apr 2020 08:55:38 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a842b77b23971198e093c671bcf1e2cf6df771a6138ffb4132bfb37af22f17`  
		Last Modified: Fri, 24 Apr 2020 08:55:38 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5.0-alpine3.11` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:2ebdecb52315772800ba4549b9dc83910d9ae7de5364c3092b0390d7266e94a9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9918976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b6acb4ad7ccdd962d8579a0929ab5920a1f58ff996cd4812188219c1eb74e91`
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
# Fri, 24 Apr 2020 12:46:32 GMT
ENV REDIS_VERSION=5.0.9
# Fri, 24 Apr 2020 12:46:33 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Fri, 24 Apr 2020 12:46:34 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Fri, 24 Apr 2020 12:47:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 24 Apr 2020 12:47:24 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 24 Apr 2020 12:47:24 GMT
VOLUME [/data]
# Fri, 24 Apr 2020 12:47:25 GMT
WORKDIR /data
# Fri, 24 Apr 2020 12:47:26 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 24 Apr 2020 12:47:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 12:47:28 GMT
EXPOSE 6379
# Fri, 24 Apr 2020 12:47:29 GMT
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
	-	`sha256:f5ca1db598d2278e5526b65dcad0d96f0f0264060f879f1b437f58a467e27382`  
		Last Modified: Fri, 24 Apr 2020 12:49:17 GMT  
		Size: 6.8 MB (6788089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87542dce16ad38aeb18ffe2e2266f3bd9b8cbc70f6f4450be0e9f621022fabb5`  
		Last Modified: Fri, 24 Apr 2020 12:49:15 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a20d19811afde1a300515cade1279f18fb3ca0ef1800b52dcb45127731bd5f4`  
		Last Modified: Fri, 24 Apr 2020 12:49:15 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5.0-alpine3.11` - linux; 386

```console
$ docker pull redis@sha256:3ab6896b5efe215c5cc110a835fecb73d5f55672ad4443f4baf51822db1854c6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9710040 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bba820d7067104939d7ec907ee1fa581e9c7d40b0a204a14caf709f4dce84732`
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
# Fri, 24 Apr 2020 05:51:10 GMT
ENV REDIS_VERSION=5.0.9
# Fri, 24 Apr 2020 05:51:10 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Fri, 24 Apr 2020 05:51:10 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Fri, 24 Apr 2020 05:52:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 24 Apr 2020 05:52:17 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 24 Apr 2020 05:52:17 GMT
VOLUME [/data]
# Fri, 24 Apr 2020 05:52:17 GMT
WORKDIR /data
# Fri, 24 Apr 2020 05:52:17 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 24 Apr 2020 05:52:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 05:52:18 GMT
EXPOSE 6379
# Fri, 24 Apr 2020 05:52:18 GMT
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
	-	`sha256:7ed6bb387586efb069405e1b2fea60bf1718da22582dade16723a6ce6beb111c`  
		Last Modified: Fri, 24 Apr 2020 05:53:49 GMT  
		Size: 6.5 MB (6491980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ee2bc48c46cc40ec8951486a93e65583168f55239b5e10e350ceda82120fa3`  
		Last Modified: Fri, 24 Apr 2020 05:53:48 GMT  
		Size: 98.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae5b0c59c675cf868993ca6ec424636476caea5bc4e43525a866864d0b8bbd1`  
		Last Modified: Fri, 24 Apr 2020 05:53:48 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5.0-alpine3.11` - linux; ppc64le

```console
$ docker pull redis@sha256:14dfcd56148c897338a1306bf23b392e6ffce4ee486ddfcd77fb515e8f0f1557
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.5 MB (10494033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a0a1b6eb6701cd8c4349958777c681d81e0520d3e82317e2419b56b4d4ce4bf`
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
# Fri, 24 Apr 2020 09:03:45 GMT
ENV REDIS_VERSION=5.0.9
# Fri, 24 Apr 2020 09:03:48 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Fri, 24 Apr 2020 09:03:50 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Fri, 24 Apr 2020 09:04:40 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 24 Apr 2020 09:04:46 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 24 Apr 2020 09:04:50 GMT
VOLUME [/data]
# Fri, 24 Apr 2020 09:04:53 GMT
WORKDIR /data
# Fri, 24 Apr 2020 09:04:56 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 24 Apr 2020 09:04:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 09:05:01 GMT
EXPOSE 6379
# Fri, 24 Apr 2020 09:05:07 GMT
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
	-	`sha256:1ad3f9cade0fa9bda2c0f45df3a77c780ebc4adea7badb3b8387fed928c60ed7`  
		Last Modified: Fri, 24 Apr 2020 09:07:21 GMT  
		Size: 7.3 MB (7260512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ad499a196593cd717672adacc0550293f8b2c00a5907255640b27d266bc05a`  
		Last Modified: Fri, 24 Apr 2020 09:07:21 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5831b0ffd2731f416315c93a640459b17492812a21b7a6fba00919faaeb1d5`  
		Last Modified: Fri, 24 Apr 2020 09:07:19 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5.0-alpine3.11` - linux; s390x

```console
$ docker pull redis@sha256:5ad55b9f660c1e3b315e26e3497b9e4d270a5dd7ff431b14d9a17cf78fcac287
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (10008638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78dd64fd99b54ef1c40f2cd3351efcaf43b4d026dfcfe78315787e7a8220ffee`
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
# Fri, 24 Apr 2020 07:03:22 GMT
ENV REDIS_VERSION=5.0.9
# Fri, 24 Apr 2020 07:03:22 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Fri, 24 Apr 2020 07:03:22 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Fri, 24 Apr 2020 07:03:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 24 Apr 2020 07:03:53 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 24 Apr 2020 07:03:53 GMT
VOLUME [/data]
# Fri, 24 Apr 2020 07:03:54 GMT
WORKDIR /data
# Fri, 24 Apr 2020 07:03:54 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 24 Apr 2020 07:03:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 07:03:54 GMT
EXPOSE 6379
# Fri, 24 Apr 2020 07:03:54 GMT
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
	-	`sha256:4b3c809e9bcb4892e2da01d3bae84664c06e6bb0929c6813ef47a1aaaa3d675f`  
		Last Modified: Fri, 24 Apr 2020 07:05:07 GMT  
		Size: 7.0 MB (7016584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd1cb7e35314fbaf45935cb538fb36cc01e53dff4d37131a3497fd376720294e`  
		Last Modified: Fri, 24 Apr 2020 07:05:11 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529922dc84cb9fec77a0630b9ad535a7c843db2cd4518c25442c47fbc986d8b7`  
		Last Modified: Fri, 24 Apr 2020 07:05:06 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redis:5.0-buster`

```console
$ docker pull redis@sha256:157a95b41b0dca8c308a33489dfdb28019e033110320414b4b16fad7d28c0f9f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `redis:5.0-buster` - linux; amd64

```console
$ docker pull redis@sha256:43dbbe6f633572d66e84e7162245d8d70a18f00b819d6c0bf98ca02109f4788c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35863297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4d3716dbb72408a7843e12d7d9f6a5addf7ab28ac21e9e9da4a6a51f1b32da9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:20:32 GMT
ADD file:9b8be2b52ee0fa31da1b6256099030b73546253a57e94cccb24605cd888bb74d in / 
# Thu, 23 Apr 2020 00:20:32 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 19:48:34 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 19:48:34 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 19:48:46 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 19:50:08 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 19:50:08 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 19:50:08 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 19:51:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 19:51:26 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 19:51:26 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 19:51:27 GMT
WORKDIR /data
# Thu, 23 Apr 2020 19:51:27 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 19:51:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 19:51:28 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 19:51:28 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:54fec2fa59d0a0de9cd2dec9850b36c43de451f1fd1c0a5bf8f1cf26a61a5da4`  
		Last Modified: Thu, 23 Apr 2020 00:25:10 GMT  
		Size: 27.1 MB (27098254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c94e11103d92f2a83b82e5d4287445cba073af0002cecee98d85d68ccec0f89`  
		Last Modified: Thu, 23 Apr 2020 19:55:42 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ab1bfc453f19989c401c2f0622df3363b5182bdea1af9e59ee2ceea3a9931c`  
		Last Modified: Thu, 23 Apr 2020 19:55:43 GMT  
		Size: 1.4 MB (1417711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f71e6b94d83f5a0df5d032ce4998b4834287bd4ed307ff7c9a31ad0a60caa98`  
		Last Modified: Thu, 23 Apr 2020 19:55:55 GMT  
		Size: 7.3 MB (7345094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2729a8234dd5e724571528d78d5f581702abc77be39db93fc0ae741340eb1c18`  
		Last Modified: Thu, 23 Apr 2020 19:55:53 GMT  
		Size: 97.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2683d7f177455cf86b4cf424cc757f1d177d5772df77bdaeeace411006eb88a5`  
		Last Modified: Thu, 23 Apr 2020 19:55:53 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5.0-buster` - linux; arm variant v5

```console
$ docker pull redis@sha256:5a474d0e7c55a7e45ddaf530f4f2ab4bc8dcaba6d85b0829f1121f7fe53414fd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.4 MB (33394023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b83a1e222e2b9be5acf1ae9a03cd2e6d2c7a4efcd3b73a275481c652552de80`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:52:22 GMT
ADD file:62a9732be4e3237ccc896f724a34606e01f351c4877e52c9a9cd85029c06b956 in / 
# Thu, 23 Apr 2020 00:52:23 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 09:33:20 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 09:33:21 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 09:33:56 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 09:35:38 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 09:35:39 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 09:35:39 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 09:36:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 09:36:48 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 09:36:48 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 09:36:49 GMT
WORKDIR /data
# Thu, 23 Apr 2020 09:36:50 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 09:36:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 09:36:51 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 09:36:52 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:a8c46e5952878f9f324df86c5a2b45b2e0020f6721e820981e74461d77a100dd`  
		Last Modified: Thu, 23 Apr 2020 00:59:50 GMT  
		Size: 24.8 MB (24836319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471287e557b84038803c3a26dee3987da48cbcae6529a77a28f486e4527757f7`  
		Last Modified: Thu, 23 Apr 2020 09:39:42 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:016e8ff197695f0c8e2c3ae127ac9459df9c71e52ae54500970e692d2799c944`  
		Last Modified: Thu, 23 Apr 2020 09:39:42 GMT  
		Size: 1.4 MB (1376131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd64ec452edc906dc611493aae3c90529a0d5787d8dc3b8c1088b41b53379d2d`  
		Last Modified: Thu, 23 Apr 2020 09:40:07 GMT  
		Size: 7.2 MB (7179305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ca72abe00cf1354dc501a32ed89705fdacd4905631c42186458d9d3202cc90`  
		Last Modified: Thu, 23 Apr 2020 09:40:05 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e7807337a06858bed0eac541f5935b123a4abb0d973dacb1973753c6dcb2469`  
		Last Modified: Thu, 23 Apr 2020 09:40:04 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5.0-buster` - linux; arm variant v7

```console
$ docker pull redis@sha256:afc097fd6784e016756816ecc4ae33dc9ef22f5715db3593b90b7ec17e906edf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.1 MB (31109340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:632cd87ac6e4d8bda115f5e32e2b45cb8e28c59bd4c6e24b87985cf6b1f93354`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 01:03:26 GMT
ADD file:db6122b36f3e70c5f490b50afba99d49fa345f11d0f5c77bb3c6749f8e2a4f81 in / 
# Thu, 23 Apr 2020 01:03:28 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 13:54:58 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 13:54:59 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 13:55:22 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 13:57:35 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 13:57:35 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 13:57:36 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 13:58:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 13:58:37 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 13:58:38 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 13:58:39 GMT
WORKDIR /data
# Thu, 23 Apr 2020 13:58:39 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 13:58:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 13:58:41 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 13:58:41 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:50fb0052086928803f00724ca465c89c45dde5b082b1e59dadb8101286dd5ab6`  
		Last Modified: Thu, 23 Apr 2020 01:11:08 GMT  
		Size: 22.7 MB (22705377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98fc1f5e139d98aa45f74dfddb32ca22bec51ecf2fcab9bb372d91c14cc971d2`  
		Last Modified: Thu, 23 Apr 2020 14:00:18 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa98edd0b4c481052caeb348af3e906ef75764353840cfe2518af73963fcf2d`  
		Last Modified: Thu, 23 Apr 2020 14:00:18 GMT  
		Size: 1.4 MB (1368177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1ae9f68f12644f241fb270f9baf2e62d5b1380083acada1fdae86374998430`  
		Last Modified: Thu, 23 Apr 2020 14:00:21 GMT  
		Size: 7.0 MB (7033517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a23909059832233f41bcba599ec5bb698e278c652cf313dc6e8724fae8aa40cf`  
		Last Modified: Thu, 23 Apr 2020 14:00:19 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f5f6de32828cf1cb128a0cba17dc0396dead74aa6cc963394ac4f8b05540179`  
		Last Modified: Thu, 23 Apr 2020 14:00:18 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5.0-buster` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:be463e278dc2125ea4c8984cd6a990353dfaa7f94570856734f86b900debc008
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 MB (34548547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0da52d2315939d969b12f3db6ae0aa5716074833f1ef06a42a544aec452d0ab2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:54:55 GMT
ADD file:581ee9c3c19f0d971aeda008fd399f59171cae75e8936b967dbf3888db4fc0d0 in / 
# Thu, 23 Apr 2020 00:54:58 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 16:01:56 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 16:01:57 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 16:02:29 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 16:04:19 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 16:04:20 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 16:04:20 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 16:05:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 16:05:20 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 16:05:20 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 16:05:21 GMT
WORKDIR /data
# Thu, 23 Apr 2020 16:05:21 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 16:05:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 16:05:22 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 16:05:24 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:bdc84a41f2513e28e99efeff9fcbb196b7df9883fb30532184bd67ca415b4673`  
		Last Modified: Thu, 23 Apr 2020 01:03:27 GMT  
		Size: 25.9 MB (25857800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698d3e76f19fb83cee90fe071552d86509322f0b8316774550c1ea7398327369`  
		Last Modified: Thu, 23 Apr 2020 16:07:31 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac4bbea6248caf60d5eca4d3e15d73d9cc18a5154a795c5ca3937eb040c9daae`  
		Last Modified: Thu, 23 Apr 2020 16:07:31 GMT  
		Size: 1.4 MB (1352987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1590123d45656fbb5cabd427b87908fd7347ef2fc6b0fba354f2b83771ec8882`  
		Last Modified: Thu, 23 Apr 2020 16:07:57 GMT  
		Size: 7.3 MB (7335481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e21891406b8ecd80c9cc4be90337cdd8d8935229002e8162d9afc9b68d2a4c30`  
		Last Modified: Thu, 23 Apr 2020 16:07:55 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d793eb07a5bc754267edbd54feb6cb25e4c28e7056a87e27960de4901d1dcc3`  
		Last Modified: Thu, 23 Apr 2020 16:07:55 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5.0-buster` - linux; 386

```console
$ docker pull redis@sha256:0ac1dbfd6ca80b45aa587ecaa0632457ca254eea674a50e8574e8677f7a193a0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.2 MB (36151602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34c763545c4e57aabcdc00c9448e439a81bdaf47ae32d7711bc8e1252fb7ef59`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:39:36 GMT
ADD file:ca6a74f6b738c738c033152fab2a9aacf22bec5f19a994e6a02b5f919ee33ee9 in / 
# Thu, 23 Apr 2020 00:39:36 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 11:23:53 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 11:23:53 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 11:24:11 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 11:26:28 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 11:26:28 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 11:26:28 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 11:27:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 11:27:59 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 11:28:00 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 11:28:00 GMT
WORKDIR /data
# Thu, 23 Apr 2020 11:28:00 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 11:28:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 11:28:01 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 11:28:01 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:5d3da8f33b97fc107a05b3255a55836b76df9f817de632b1fb63c6e9c024f0df`  
		Last Modified: Thu, 23 Apr 2020 00:44:35 GMT  
		Size: 27.8 MB (27753972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f572d913eaf53def72d8eeff5384464ae75f0da9041d63ef0cd2fb2a43e21e`  
		Last Modified: Thu, 23 Apr 2020 11:30:12 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36c13a7e7929be4f05fbeddd74c94dfe85b704c504f7d13aa45bdb84bae79ccb`  
		Last Modified: Thu, 23 Apr 2020 11:30:12 GMT  
		Size: 1.4 MB (1387411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680a9b72444c93256224c2c5394c18343047b8b7dc305a4301401e7a6b494d03`  
		Last Modified: Thu, 23 Apr 2020 11:30:25 GMT  
		Size: 7.0 MB (7007988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e6148f8fb3eb037aaf97a9736b49d92d77541c5bbb6219db62f8af4f8d5e54`  
		Last Modified: Thu, 23 Apr 2020 11:30:23 GMT  
		Size: 97.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fae33d9962de4399f135693d495b300515e9d363f74683c3c366cd6e32290e1`  
		Last Modified: Thu, 23 Apr 2020 11:30:23 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5.0-buster` - linux; mips64le

```console
$ docker pull redis@sha256:8860ea6be85bfa12a7a62f37e07716f197be8e76f498d1e62d3c4319582a3b60
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34731728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eab8ac536ee15de9306c977271c71a293db05c67e582fe002279ba86c8fff0a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:09:47 GMT
ADD file:7509945bd8a224048260e88b466aa3b156615e16b64e0a6702da277052fcb98b in / 
# Thu, 23 Apr 2020 00:09:48 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 09:24:32 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 09:24:33 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 09:25:02 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 09:28:42 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 09:28:42 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 09:28:43 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 09:31:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 09:32:01 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 09:32:01 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 09:32:01 GMT
WORKDIR /data
# Thu, 23 Apr 2020 09:32:02 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 09:32:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 09:32:02 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 09:32:03 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:ae8f0fa6cb0d971b4b8fedf7fc9b00f61f780b383fe7d64e6c2e4be8d20c3987`  
		Last Modified: Thu, 23 Apr 2020 00:17:46 GMT  
		Size: 25.8 MB (25762125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faf65c067540cd52d99f7f6df4511fb45d6a0485e47338d0239a052fcd64c8e3`  
		Last Modified: Thu, 23 Apr 2020 09:34:32 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef207bf80aefb18eba12c119d07499e37b5ea7bec06bc1e0c2dd749ddde45a1`  
		Last Modified: Thu, 23 Apr 2020 09:34:34 GMT  
		Size: 1.3 MB (1305489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae62dd92cc34f4856c15b7614910c5578f2d91d96d96469c21f8ca741c1061f5`  
		Last Modified: Thu, 23 Apr 2020 09:35:08 GMT  
		Size: 7.7 MB (7661872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693fe2f4d6e93636c838f7fb3a49c859d72138e5a25fd1687e590fcf3bb74dfb`  
		Last Modified: Thu, 23 Apr 2020 09:35:00 GMT  
		Size: 99.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:153c8eb8631e42a4705a53461aeb1c1edea4a60ad71a759b5eafeccbf3f5c142`  
		Last Modified: Thu, 23 Apr 2020 09:35:00 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5.0-buster` - linux; ppc64le

```console
$ docker pull redis@sha256:e1c410783ee0d501a9804b3050db559054e95e91bb3cd8f3e81324baef92f730
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.7 MB (39696544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34098209a59e39ee25eeb2b0bf53ba98f873314c75110d6841a0793d5e1bc182`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:36:00 GMT
ADD file:5b3c3d2945800e1743dc02a4f68bd830fe2f67ca437223692eb460147c158c2b in / 
# Thu, 23 Apr 2020 00:36:04 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 17:29:48 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 17:29:51 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 17:31:38 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 17:35:14 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 17:35:18 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 17:35:23 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 17:38:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 17:38:25 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 17:38:28 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 17:38:32 GMT
WORKDIR /data
# Thu, 23 Apr 2020 17:38:34 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 17:38:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 17:38:42 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 17:38:45 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:012c6cdbd1af202bbfbea5945fafbb9aca9097f1fa3cb493a29155fdc02cc43c`  
		Last Modified: Thu, 23 Apr 2020 00:50:14 GMT  
		Size: 30.5 MB (30524638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee5a34bf53dadebb7466557f439affba6f1c11ddbdd7d2c1376f9540c294a7a`  
		Last Modified: Thu, 23 Apr 2020 17:42:03 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dedf97e3c0bcb476732135fc70dee2ba4766ff50ec51f93b1929ebaa6c4863f`  
		Last Modified: Thu, 23 Apr 2020 17:42:03 GMT  
		Size: 1.3 MB (1335327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2a1294a7da3aa34af8f45c22665913b8780fcf4dec6b52b108541e496dd0cc`  
		Last Modified: Thu, 23 Apr 2020 17:42:27 GMT  
		Size: 7.8 MB (7834296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51726f5fc1a7b6d031cad4d822aaf6c1801262570fb662454f1f2dc93cd4e551`  
		Last Modified: Thu, 23 Apr 2020 17:42:25 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e62728fce47996c1059a9f4f18e5e1efea4ebc55e17f82aa362f8985e7f019e`  
		Last Modified: Thu, 23 Apr 2020 17:42:25 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5.0-buster` - linux; s390x

```console
$ docker pull redis@sha256:80a22e71a515d761d2c50a5873fc228fe165a627f9f91641391ce1548bc23f03
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34709447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5556ba73cac9fdc7f38ea53f8961a08497e52b1fa62f83611a9228a5d495e8fb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:51:48 GMT
ADD file:f6c2560f9185c1bcaff95e576e57449f606d51b85fad02646c1b0962bc9353c9 in / 
# Thu, 23 Apr 2020 00:51:50 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 06:58:44 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 06:58:44 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 06:58:58 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 06:59:46 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 06:59:47 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 06:59:47 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 07:00:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 07:00:24 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 07:00:24 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 07:00:24 GMT
WORKDIR /data
# Thu, 23 Apr 2020 07:00:24 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 07:00:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 07:00:25 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 07:00:25 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:d89dc3741ad42b79c3d8545495c429f3100d3f22234ff993bd04017b0675e868`  
		Last Modified: Thu, 23 Apr 2020 00:56:00 GMT  
		Size: 25.7 MB (25712105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c9894c70b29dc7cbad7e69c5f898b0a5d6f82aac9aff00e2645a6f8a9eff88`  
		Last Modified: Thu, 23 Apr 2020 07:01:34 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fba24ca231c607425b0e92a8a39c3174a8b9cb56ddeee71fc43f2f9dd9b1d2c`  
		Last Modified: Thu, 23 Apr 2020 07:01:35 GMT  
		Size: 1.4 MB (1403679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22d299e81a09eaaf9da803a2b3775444f312a34b2b7dd8e0c1c10d0171225ba`  
		Last Modified: Thu, 23 Apr 2020 07:01:52 GMT  
		Size: 7.6 MB (7591385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46db2cefe8baf230709535dd5f96c93520ca156d9821649ce8e8a2410e49d54`  
		Last Modified: Thu, 23 Apr 2020 07:01:56 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ec0a42c81dfec4356c31366a6ddf246ebac63394fafd37549a4483fd537513`  
		Last Modified: Thu, 23 Apr 2020 07:01:50 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redis:5-32bit`

```console
$ docker pull redis@sha256:021a0c5614223ddc6a302017241389a0d06d559eca7868ac964be52b1c695328
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redis:5-32bit` - linux; amd64

```console
$ docker pull redis@sha256:734e0a8d1994e025f766201cd7ed0ee736053c88599e048aa3fe7044444751c8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40576869 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffbc0eed192b290957b3d6f2568222df0745389d5c8c6d6a2e434395b7540589`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:20:32 GMT
ADD file:9b8be2b52ee0fa31da1b6256099030b73546253a57e94cccb24605cd888bb74d in / 
# Thu, 23 Apr 2020 00:20:32 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 19:48:34 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 19:48:34 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 19:48:46 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 19:50:08 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 19:50:08 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 19:50:08 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 19:52:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev-i386 gcc-multilib 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" 32bit; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 19:52:54 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 19:52:54 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 19:52:55 GMT
WORKDIR /data
# Thu, 23 Apr 2020 19:52:55 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 19:52:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 19:52:55 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 19:52:55 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:54fec2fa59d0a0de9cd2dec9850b36c43de451f1fd1c0a5bf8f1cf26a61a5da4`  
		Last Modified: Thu, 23 Apr 2020 00:25:10 GMT  
		Size: 27.1 MB (27098254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c94e11103d92f2a83b82e5d4287445cba073af0002cecee98d85d68ccec0f89`  
		Last Modified: Thu, 23 Apr 2020 19:55:42 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ab1bfc453f19989c401c2f0622df3363b5182bdea1af9e59ee2ceea3a9931c`  
		Last Modified: Thu, 23 Apr 2020 19:55:43 GMT  
		Size: 1.4 MB (1417711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fedad42a33a3821f6b477a48ad2c5cb4d05dd795fc6af2fbba817ce1a2365dd0`  
		Last Modified: Thu, 23 Apr 2020 19:56:14 GMT  
		Size: 12.1 MB (12058659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b58703ecd075fd32ee51dd28840b9622cc5aaac3bb2d77c841515846571805e`  
		Last Modified: Thu, 23 Apr 2020 19:56:03 GMT  
		Size: 99.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bece53145f7f86a1877242e552825b494f227a3f4facff30334248943c4ad49`  
		Last Modified: Thu, 23 Apr 2020 19:56:04 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redis:5-32bit-buster`

```console
$ docker pull redis@sha256:021a0c5614223ddc6a302017241389a0d06d559eca7868ac964be52b1c695328
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redis:5-32bit-buster` - linux; amd64

```console
$ docker pull redis@sha256:734e0a8d1994e025f766201cd7ed0ee736053c88599e048aa3fe7044444751c8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40576869 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffbc0eed192b290957b3d6f2568222df0745389d5c8c6d6a2e434395b7540589`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:20:32 GMT
ADD file:9b8be2b52ee0fa31da1b6256099030b73546253a57e94cccb24605cd888bb74d in / 
# Thu, 23 Apr 2020 00:20:32 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 19:48:34 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 19:48:34 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 19:48:46 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 19:50:08 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 19:50:08 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 19:50:08 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 19:52:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev-i386 gcc-multilib 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" 32bit; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 19:52:54 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 19:52:54 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 19:52:55 GMT
WORKDIR /data
# Thu, 23 Apr 2020 19:52:55 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 19:52:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 19:52:55 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 19:52:55 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:54fec2fa59d0a0de9cd2dec9850b36c43de451f1fd1c0a5bf8f1cf26a61a5da4`  
		Last Modified: Thu, 23 Apr 2020 00:25:10 GMT  
		Size: 27.1 MB (27098254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c94e11103d92f2a83b82e5d4287445cba073af0002cecee98d85d68ccec0f89`  
		Last Modified: Thu, 23 Apr 2020 19:55:42 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ab1bfc453f19989c401c2f0622df3363b5182bdea1af9e59ee2ceea3a9931c`  
		Last Modified: Thu, 23 Apr 2020 19:55:43 GMT  
		Size: 1.4 MB (1417711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fedad42a33a3821f6b477a48ad2c5cb4d05dd795fc6af2fbba817ce1a2365dd0`  
		Last Modified: Thu, 23 Apr 2020 19:56:14 GMT  
		Size: 12.1 MB (12058659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b58703ecd075fd32ee51dd28840b9622cc5aaac3bb2d77c841515846571805e`  
		Last Modified: Thu, 23 Apr 2020 19:56:03 GMT  
		Size: 99.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bece53145f7f86a1877242e552825b494f227a3f4facff30334248943c4ad49`  
		Last Modified: Thu, 23 Apr 2020 19:56:04 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redis:5-alpine`

```console
$ docker pull redis@sha256:83a3af36d5e57f2901b4783c313720e5fa3ecf0424ba86ad9775e06a9a5e35d0
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

### `redis:5-alpine` - linux; amd64

```console
$ docker pull redis@sha256:d4ada5d910403607b3f579d7171f36108c2e1cf67da966a712812230171fc153
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (9998790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3661c84ee9d0f6312a076b69eb2bd112674cadb70ef7e1594c4f00193f8df08e`
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
# Fri, 24 Apr 2020 19:20:54 GMT
ENV REDIS_VERSION=5.0.9
# Fri, 24 Apr 2020 19:20:54 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Fri, 24 Apr 2020 19:20:55 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Fri, 24 Apr 2020 19:21:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 24 Apr 2020 19:21:49 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 24 Apr 2020 19:21:49 GMT
VOLUME [/data]
# Fri, 24 Apr 2020 19:21:50 GMT
WORKDIR /data
# Fri, 24 Apr 2020 19:21:50 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 24 Apr 2020 19:21:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 19:21:50 GMT
EXPOSE 6379
# Fri, 24 Apr 2020 19:21:50 GMT
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
	-	`sha256:3e45770272d96deeb96c4bfa3cffde811f318823b4422bdbbf909148dc5669bb`  
		Last Modified: Fri, 24 Apr 2020 19:23:14 GMT  
		Size: 6.8 MB (6781166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:558de8ea3153bdccfaf67fadf7bbbdc60bf357f33ff0070df617d6e22ad46a13`  
		Last Modified: Fri, 24 Apr 2020 19:23:13 GMT  
		Size: 99.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2c65255161264f51556db666aa812834b3f51c8403b09799a46e4d0909e4aa4`  
		Last Modified: Fri, 24 Apr 2020 19:23:12 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-alpine` - linux; arm variant v6

```console
$ docker pull redis@sha256:867b50998330ae4743e95c8be69dee7ad37cbba8057659bef4dc142838d7f3e0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9725047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:333723767b2b5747763b5483d4742558e9abe6d70b98ee05d527643b5eb088d5`
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
# Thu, 23 Apr 2020 22:31:34 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 22:31:35 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 22:31:36 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 22:32:24 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 22:32:27 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 22:32:29 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 22:32:30 GMT
WORKDIR /data
# Thu, 23 Apr 2020 22:32:31 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Thu, 23 Apr 2020 22:32:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 22:32:33 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 22:32:34 GMT
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
	-	`sha256:75a2919ec032b1198ca13b052499b7c193e45d93756a3b0d7bb10c8db4f3db65`  
		Last Modified: Thu, 23 Apr 2020 22:34:01 GMT  
		Size: 6.7 MB (6697511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b2e77e4c2604e8e74b4c471b4a04d1a768eb84eadcfcd3621f135f7d4d90ca`  
		Last Modified: Thu, 23 Apr 2020 22:33:57 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18df89faaf97292802f6bca82a98892b7b0a168230ca31ae16e3cf307614a7a8`  
		Last Modified: Thu, 23 Apr 2020 22:33:57 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-alpine` - linux; arm variant v7

```console
$ docker pull redis@sha256:1c10570f57cb14b4fbd3446c61303aeb7db18b45abffc49974d5bde7e4a89de4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9394623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56a7ba195be67da9c68c67aa8d6eefa737236f15d3a9b490504ce943465c3a9f`
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
# Fri, 24 Apr 2020 08:52:43 GMT
ENV REDIS_VERSION=5.0.9
# Fri, 24 Apr 2020 08:52:43 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Fri, 24 Apr 2020 08:52:44 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Fri, 24 Apr 2020 08:53:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 24 Apr 2020 08:53:30 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 24 Apr 2020 08:53:31 GMT
VOLUME [/data]
# Fri, 24 Apr 2020 08:53:32 GMT
WORKDIR /data
# Fri, 24 Apr 2020 08:53:32 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 24 Apr 2020 08:53:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 08:53:34 GMT
EXPOSE 6379
# Fri, 24 Apr 2020 08:53:34 GMT
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
	-	`sha256:531954b17ac2db3cd86f3ced48c7c4f9fe053fad0792b7038321a667c911953a`  
		Last Modified: Fri, 24 Apr 2020 08:55:41 GMT  
		Size: 6.6 MB (6570977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d550a31e99202186ed01f1a5a4c96bab49dc143ad2a113696ecb48947836c0`  
		Last Modified: Fri, 24 Apr 2020 08:55:38 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a842b77b23971198e093c671bcf1e2cf6df771a6138ffb4132bfb37af22f17`  
		Last Modified: Fri, 24 Apr 2020 08:55:38 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-alpine` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:2ebdecb52315772800ba4549b9dc83910d9ae7de5364c3092b0390d7266e94a9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9918976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b6acb4ad7ccdd962d8579a0929ab5920a1f58ff996cd4812188219c1eb74e91`
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
# Fri, 24 Apr 2020 12:46:32 GMT
ENV REDIS_VERSION=5.0.9
# Fri, 24 Apr 2020 12:46:33 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Fri, 24 Apr 2020 12:46:34 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Fri, 24 Apr 2020 12:47:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 24 Apr 2020 12:47:24 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 24 Apr 2020 12:47:24 GMT
VOLUME [/data]
# Fri, 24 Apr 2020 12:47:25 GMT
WORKDIR /data
# Fri, 24 Apr 2020 12:47:26 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 24 Apr 2020 12:47:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 12:47:28 GMT
EXPOSE 6379
# Fri, 24 Apr 2020 12:47:29 GMT
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
	-	`sha256:f5ca1db598d2278e5526b65dcad0d96f0f0264060f879f1b437f58a467e27382`  
		Last Modified: Fri, 24 Apr 2020 12:49:17 GMT  
		Size: 6.8 MB (6788089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87542dce16ad38aeb18ffe2e2266f3bd9b8cbc70f6f4450be0e9f621022fabb5`  
		Last Modified: Fri, 24 Apr 2020 12:49:15 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a20d19811afde1a300515cade1279f18fb3ca0ef1800b52dcb45127731bd5f4`  
		Last Modified: Fri, 24 Apr 2020 12:49:15 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-alpine` - linux; 386

```console
$ docker pull redis@sha256:3ab6896b5efe215c5cc110a835fecb73d5f55672ad4443f4baf51822db1854c6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9710040 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bba820d7067104939d7ec907ee1fa581e9c7d40b0a204a14caf709f4dce84732`
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
# Fri, 24 Apr 2020 05:51:10 GMT
ENV REDIS_VERSION=5.0.9
# Fri, 24 Apr 2020 05:51:10 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Fri, 24 Apr 2020 05:51:10 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Fri, 24 Apr 2020 05:52:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 24 Apr 2020 05:52:17 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 24 Apr 2020 05:52:17 GMT
VOLUME [/data]
# Fri, 24 Apr 2020 05:52:17 GMT
WORKDIR /data
# Fri, 24 Apr 2020 05:52:17 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 24 Apr 2020 05:52:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 05:52:18 GMT
EXPOSE 6379
# Fri, 24 Apr 2020 05:52:18 GMT
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
	-	`sha256:7ed6bb387586efb069405e1b2fea60bf1718da22582dade16723a6ce6beb111c`  
		Last Modified: Fri, 24 Apr 2020 05:53:49 GMT  
		Size: 6.5 MB (6491980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ee2bc48c46cc40ec8951486a93e65583168f55239b5e10e350ceda82120fa3`  
		Last Modified: Fri, 24 Apr 2020 05:53:48 GMT  
		Size: 98.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae5b0c59c675cf868993ca6ec424636476caea5bc4e43525a866864d0b8bbd1`  
		Last Modified: Fri, 24 Apr 2020 05:53:48 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-alpine` - linux; ppc64le

```console
$ docker pull redis@sha256:14dfcd56148c897338a1306bf23b392e6ffce4ee486ddfcd77fb515e8f0f1557
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.5 MB (10494033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a0a1b6eb6701cd8c4349958777c681d81e0520d3e82317e2419b56b4d4ce4bf`
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
# Fri, 24 Apr 2020 09:03:45 GMT
ENV REDIS_VERSION=5.0.9
# Fri, 24 Apr 2020 09:03:48 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Fri, 24 Apr 2020 09:03:50 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Fri, 24 Apr 2020 09:04:40 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 24 Apr 2020 09:04:46 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 24 Apr 2020 09:04:50 GMT
VOLUME [/data]
# Fri, 24 Apr 2020 09:04:53 GMT
WORKDIR /data
# Fri, 24 Apr 2020 09:04:56 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 24 Apr 2020 09:04:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 09:05:01 GMT
EXPOSE 6379
# Fri, 24 Apr 2020 09:05:07 GMT
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
	-	`sha256:1ad3f9cade0fa9bda2c0f45df3a77c780ebc4adea7badb3b8387fed928c60ed7`  
		Last Modified: Fri, 24 Apr 2020 09:07:21 GMT  
		Size: 7.3 MB (7260512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ad499a196593cd717672adacc0550293f8b2c00a5907255640b27d266bc05a`  
		Last Modified: Fri, 24 Apr 2020 09:07:21 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5831b0ffd2731f416315c93a640459b17492812a21b7a6fba00919faaeb1d5`  
		Last Modified: Fri, 24 Apr 2020 09:07:19 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-alpine` - linux; s390x

```console
$ docker pull redis@sha256:5ad55b9f660c1e3b315e26e3497b9e4d270a5dd7ff431b14d9a17cf78fcac287
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (10008638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78dd64fd99b54ef1c40f2cd3351efcaf43b4d026dfcfe78315787e7a8220ffee`
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
# Fri, 24 Apr 2020 07:03:22 GMT
ENV REDIS_VERSION=5.0.9
# Fri, 24 Apr 2020 07:03:22 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Fri, 24 Apr 2020 07:03:22 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Fri, 24 Apr 2020 07:03:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 24 Apr 2020 07:03:53 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 24 Apr 2020 07:03:53 GMT
VOLUME [/data]
# Fri, 24 Apr 2020 07:03:54 GMT
WORKDIR /data
# Fri, 24 Apr 2020 07:03:54 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 24 Apr 2020 07:03:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 07:03:54 GMT
EXPOSE 6379
# Fri, 24 Apr 2020 07:03:54 GMT
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
	-	`sha256:4b3c809e9bcb4892e2da01d3bae84664c06e6bb0929c6813ef47a1aaaa3d675f`  
		Last Modified: Fri, 24 Apr 2020 07:05:07 GMT  
		Size: 7.0 MB (7016584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd1cb7e35314fbaf45935cb538fb36cc01e53dff4d37131a3497fd376720294e`  
		Last Modified: Fri, 24 Apr 2020 07:05:11 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529922dc84cb9fec77a0630b9ad535a7c843db2cd4518c25442c47fbc986d8b7`  
		Last Modified: Fri, 24 Apr 2020 07:05:06 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redis:5-alpine3.11`

```console
$ docker pull redis@sha256:83a3af36d5e57f2901b4783c313720e5fa3ecf0424ba86ad9775e06a9a5e35d0
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
$ docker pull redis@sha256:d4ada5d910403607b3f579d7171f36108c2e1cf67da966a712812230171fc153
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (9998790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3661c84ee9d0f6312a076b69eb2bd112674cadb70ef7e1594c4f00193f8df08e`
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
# Fri, 24 Apr 2020 19:20:54 GMT
ENV REDIS_VERSION=5.0.9
# Fri, 24 Apr 2020 19:20:54 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Fri, 24 Apr 2020 19:20:55 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Fri, 24 Apr 2020 19:21:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 24 Apr 2020 19:21:49 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 24 Apr 2020 19:21:49 GMT
VOLUME [/data]
# Fri, 24 Apr 2020 19:21:50 GMT
WORKDIR /data
# Fri, 24 Apr 2020 19:21:50 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 24 Apr 2020 19:21:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 19:21:50 GMT
EXPOSE 6379
# Fri, 24 Apr 2020 19:21:50 GMT
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
	-	`sha256:3e45770272d96deeb96c4bfa3cffde811f318823b4422bdbbf909148dc5669bb`  
		Last Modified: Fri, 24 Apr 2020 19:23:14 GMT  
		Size: 6.8 MB (6781166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:558de8ea3153bdccfaf67fadf7bbbdc60bf357f33ff0070df617d6e22ad46a13`  
		Last Modified: Fri, 24 Apr 2020 19:23:13 GMT  
		Size: 99.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2c65255161264f51556db666aa812834b3f51c8403b09799a46e4d0909e4aa4`  
		Last Modified: Fri, 24 Apr 2020 19:23:12 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-alpine3.11` - linux; arm variant v6

```console
$ docker pull redis@sha256:867b50998330ae4743e95c8be69dee7ad37cbba8057659bef4dc142838d7f3e0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9725047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:333723767b2b5747763b5483d4742558e9abe6d70b98ee05d527643b5eb088d5`
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
# Thu, 23 Apr 2020 22:31:34 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 22:31:35 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 22:31:36 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 22:32:24 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 22:32:27 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 22:32:29 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 22:32:30 GMT
WORKDIR /data
# Thu, 23 Apr 2020 22:32:31 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Thu, 23 Apr 2020 22:32:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 22:32:33 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 22:32:34 GMT
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
	-	`sha256:75a2919ec032b1198ca13b052499b7c193e45d93756a3b0d7bb10c8db4f3db65`  
		Last Modified: Thu, 23 Apr 2020 22:34:01 GMT  
		Size: 6.7 MB (6697511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b2e77e4c2604e8e74b4c471b4a04d1a768eb84eadcfcd3621f135f7d4d90ca`  
		Last Modified: Thu, 23 Apr 2020 22:33:57 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18df89faaf97292802f6bca82a98892b7b0a168230ca31ae16e3cf307614a7a8`  
		Last Modified: Thu, 23 Apr 2020 22:33:57 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-alpine3.11` - linux; arm variant v7

```console
$ docker pull redis@sha256:1c10570f57cb14b4fbd3446c61303aeb7db18b45abffc49974d5bde7e4a89de4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9394623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56a7ba195be67da9c68c67aa8d6eefa737236f15d3a9b490504ce943465c3a9f`
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
# Fri, 24 Apr 2020 08:52:43 GMT
ENV REDIS_VERSION=5.0.9
# Fri, 24 Apr 2020 08:52:43 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Fri, 24 Apr 2020 08:52:44 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Fri, 24 Apr 2020 08:53:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 24 Apr 2020 08:53:30 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 24 Apr 2020 08:53:31 GMT
VOLUME [/data]
# Fri, 24 Apr 2020 08:53:32 GMT
WORKDIR /data
# Fri, 24 Apr 2020 08:53:32 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 24 Apr 2020 08:53:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 08:53:34 GMT
EXPOSE 6379
# Fri, 24 Apr 2020 08:53:34 GMT
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
	-	`sha256:531954b17ac2db3cd86f3ced48c7c4f9fe053fad0792b7038321a667c911953a`  
		Last Modified: Fri, 24 Apr 2020 08:55:41 GMT  
		Size: 6.6 MB (6570977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d550a31e99202186ed01f1a5a4c96bab49dc143ad2a113696ecb48947836c0`  
		Last Modified: Fri, 24 Apr 2020 08:55:38 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a842b77b23971198e093c671bcf1e2cf6df771a6138ffb4132bfb37af22f17`  
		Last Modified: Fri, 24 Apr 2020 08:55:38 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-alpine3.11` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:2ebdecb52315772800ba4549b9dc83910d9ae7de5364c3092b0390d7266e94a9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9918976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b6acb4ad7ccdd962d8579a0929ab5920a1f58ff996cd4812188219c1eb74e91`
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
# Fri, 24 Apr 2020 12:46:32 GMT
ENV REDIS_VERSION=5.0.9
# Fri, 24 Apr 2020 12:46:33 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Fri, 24 Apr 2020 12:46:34 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Fri, 24 Apr 2020 12:47:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 24 Apr 2020 12:47:24 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 24 Apr 2020 12:47:24 GMT
VOLUME [/data]
# Fri, 24 Apr 2020 12:47:25 GMT
WORKDIR /data
# Fri, 24 Apr 2020 12:47:26 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 24 Apr 2020 12:47:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 12:47:28 GMT
EXPOSE 6379
# Fri, 24 Apr 2020 12:47:29 GMT
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
	-	`sha256:f5ca1db598d2278e5526b65dcad0d96f0f0264060f879f1b437f58a467e27382`  
		Last Modified: Fri, 24 Apr 2020 12:49:17 GMT  
		Size: 6.8 MB (6788089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87542dce16ad38aeb18ffe2e2266f3bd9b8cbc70f6f4450be0e9f621022fabb5`  
		Last Modified: Fri, 24 Apr 2020 12:49:15 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a20d19811afde1a300515cade1279f18fb3ca0ef1800b52dcb45127731bd5f4`  
		Last Modified: Fri, 24 Apr 2020 12:49:15 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-alpine3.11` - linux; 386

```console
$ docker pull redis@sha256:3ab6896b5efe215c5cc110a835fecb73d5f55672ad4443f4baf51822db1854c6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9710040 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bba820d7067104939d7ec907ee1fa581e9c7d40b0a204a14caf709f4dce84732`
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
# Fri, 24 Apr 2020 05:51:10 GMT
ENV REDIS_VERSION=5.0.9
# Fri, 24 Apr 2020 05:51:10 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Fri, 24 Apr 2020 05:51:10 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Fri, 24 Apr 2020 05:52:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 24 Apr 2020 05:52:17 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 24 Apr 2020 05:52:17 GMT
VOLUME [/data]
# Fri, 24 Apr 2020 05:52:17 GMT
WORKDIR /data
# Fri, 24 Apr 2020 05:52:17 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 24 Apr 2020 05:52:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 05:52:18 GMT
EXPOSE 6379
# Fri, 24 Apr 2020 05:52:18 GMT
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
	-	`sha256:7ed6bb387586efb069405e1b2fea60bf1718da22582dade16723a6ce6beb111c`  
		Last Modified: Fri, 24 Apr 2020 05:53:49 GMT  
		Size: 6.5 MB (6491980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ee2bc48c46cc40ec8951486a93e65583168f55239b5e10e350ceda82120fa3`  
		Last Modified: Fri, 24 Apr 2020 05:53:48 GMT  
		Size: 98.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae5b0c59c675cf868993ca6ec424636476caea5bc4e43525a866864d0b8bbd1`  
		Last Modified: Fri, 24 Apr 2020 05:53:48 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-alpine3.11` - linux; ppc64le

```console
$ docker pull redis@sha256:14dfcd56148c897338a1306bf23b392e6ffce4ee486ddfcd77fb515e8f0f1557
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.5 MB (10494033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a0a1b6eb6701cd8c4349958777c681d81e0520d3e82317e2419b56b4d4ce4bf`
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
# Fri, 24 Apr 2020 09:03:45 GMT
ENV REDIS_VERSION=5.0.9
# Fri, 24 Apr 2020 09:03:48 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Fri, 24 Apr 2020 09:03:50 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Fri, 24 Apr 2020 09:04:40 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 24 Apr 2020 09:04:46 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 24 Apr 2020 09:04:50 GMT
VOLUME [/data]
# Fri, 24 Apr 2020 09:04:53 GMT
WORKDIR /data
# Fri, 24 Apr 2020 09:04:56 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 24 Apr 2020 09:04:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 09:05:01 GMT
EXPOSE 6379
# Fri, 24 Apr 2020 09:05:07 GMT
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
	-	`sha256:1ad3f9cade0fa9bda2c0f45df3a77c780ebc4adea7badb3b8387fed928c60ed7`  
		Last Modified: Fri, 24 Apr 2020 09:07:21 GMT  
		Size: 7.3 MB (7260512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ad499a196593cd717672adacc0550293f8b2c00a5907255640b27d266bc05a`  
		Last Modified: Fri, 24 Apr 2020 09:07:21 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5831b0ffd2731f416315c93a640459b17492812a21b7a6fba00919faaeb1d5`  
		Last Modified: Fri, 24 Apr 2020 09:07:19 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-alpine3.11` - linux; s390x

```console
$ docker pull redis@sha256:5ad55b9f660c1e3b315e26e3497b9e4d270a5dd7ff431b14d9a17cf78fcac287
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (10008638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78dd64fd99b54ef1c40f2cd3351efcaf43b4d026dfcfe78315787e7a8220ffee`
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
# Fri, 24 Apr 2020 07:03:22 GMT
ENV REDIS_VERSION=5.0.9
# Fri, 24 Apr 2020 07:03:22 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Fri, 24 Apr 2020 07:03:22 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Fri, 24 Apr 2020 07:03:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 24 Apr 2020 07:03:53 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 24 Apr 2020 07:03:53 GMT
VOLUME [/data]
# Fri, 24 Apr 2020 07:03:54 GMT
WORKDIR /data
# Fri, 24 Apr 2020 07:03:54 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 24 Apr 2020 07:03:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 07:03:54 GMT
EXPOSE 6379
# Fri, 24 Apr 2020 07:03:54 GMT
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
	-	`sha256:4b3c809e9bcb4892e2da01d3bae84664c06e6bb0929c6813ef47a1aaaa3d675f`  
		Last Modified: Fri, 24 Apr 2020 07:05:07 GMT  
		Size: 7.0 MB (7016584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd1cb7e35314fbaf45935cb538fb36cc01e53dff4d37131a3497fd376720294e`  
		Last Modified: Fri, 24 Apr 2020 07:05:11 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529922dc84cb9fec77a0630b9ad535a7c843db2cd4518c25442c47fbc986d8b7`  
		Last Modified: Fri, 24 Apr 2020 07:05:06 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redis:5-buster`

```console
$ docker pull redis@sha256:157a95b41b0dca8c308a33489dfdb28019e033110320414b4b16fad7d28c0f9f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `redis:5-buster` - linux; amd64

```console
$ docker pull redis@sha256:43dbbe6f633572d66e84e7162245d8d70a18f00b819d6c0bf98ca02109f4788c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35863297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4d3716dbb72408a7843e12d7d9f6a5addf7ab28ac21e9e9da4a6a51f1b32da9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:20:32 GMT
ADD file:9b8be2b52ee0fa31da1b6256099030b73546253a57e94cccb24605cd888bb74d in / 
# Thu, 23 Apr 2020 00:20:32 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 19:48:34 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 19:48:34 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 19:48:46 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 19:50:08 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 19:50:08 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 19:50:08 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 19:51:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 19:51:26 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 19:51:26 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 19:51:27 GMT
WORKDIR /data
# Thu, 23 Apr 2020 19:51:27 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 19:51:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 19:51:28 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 19:51:28 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:54fec2fa59d0a0de9cd2dec9850b36c43de451f1fd1c0a5bf8f1cf26a61a5da4`  
		Last Modified: Thu, 23 Apr 2020 00:25:10 GMT  
		Size: 27.1 MB (27098254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c94e11103d92f2a83b82e5d4287445cba073af0002cecee98d85d68ccec0f89`  
		Last Modified: Thu, 23 Apr 2020 19:55:42 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ab1bfc453f19989c401c2f0622df3363b5182bdea1af9e59ee2ceea3a9931c`  
		Last Modified: Thu, 23 Apr 2020 19:55:43 GMT  
		Size: 1.4 MB (1417711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f71e6b94d83f5a0df5d032ce4998b4834287bd4ed307ff7c9a31ad0a60caa98`  
		Last Modified: Thu, 23 Apr 2020 19:55:55 GMT  
		Size: 7.3 MB (7345094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2729a8234dd5e724571528d78d5f581702abc77be39db93fc0ae741340eb1c18`  
		Last Modified: Thu, 23 Apr 2020 19:55:53 GMT  
		Size: 97.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2683d7f177455cf86b4cf424cc757f1d177d5772df77bdaeeace411006eb88a5`  
		Last Modified: Thu, 23 Apr 2020 19:55:53 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-buster` - linux; arm variant v5

```console
$ docker pull redis@sha256:5a474d0e7c55a7e45ddaf530f4f2ab4bc8dcaba6d85b0829f1121f7fe53414fd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.4 MB (33394023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b83a1e222e2b9be5acf1ae9a03cd2e6d2c7a4efcd3b73a275481c652552de80`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:52:22 GMT
ADD file:62a9732be4e3237ccc896f724a34606e01f351c4877e52c9a9cd85029c06b956 in / 
# Thu, 23 Apr 2020 00:52:23 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 09:33:20 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 09:33:21 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 09:33:56 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 09:35:38 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 09:35:39 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 09:35:39 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 09:36:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 09:36:48 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 09:36:48 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 09:36:49 GMT
WORKDIR /data
# Thu, 23 Apr 2020 09:36:50 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 09:36:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 09:36:51 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 09:36:52 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:a8c46e5952878f9f324df86c5a2b45b2e0020f6721e820981e74461d77a100dd`  
		Last Modified: Thu, 23 Apr 2020 00:59:50 GMT  
		Size: 24.8 MB (24836319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471287e557b84038803c3a26dee3987da48cbcae6529a77a28f486e4527757f7`  
		Last Modified: Thu, 23 Apr 2020 09:39:42 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:016e8ff197695f0c8e2c3ae127ac9459df9c71e52ae54500970e692d2799c944`  
		Last Modified: Thu, 23 Apr 2020 09:39:42 GMT  
		Size: 1.4 MB (1376131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd64ec452edc906dc611493aae3c90529a0d5787d8dc3b8c1088b41b53379d2d`  
		Last Modified: Thu, 23 Apr 2020 09:40:07 GMT  
		Size: 7.2 MB (7179305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ca72abe00cf1354dc501a32ed89705fdacd4905631c42186458d9d3202cc90`  
		Last Modified: Thu, 23 Apr 2020 09:40:05 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e7807337a06858bed0eac541f5935b123a4abb0d973dacb1973753c6dcb2469`  
		Last Modified: Thu, 23 Apr 2020 09:40:04 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-buster` - linux; arm variant v7

```console
$ docker pull redis@sha256:afc097fd6784e016756816ecc4ae33dc9ef22f5715db3593b90b7ec17e906edf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.1 MB (31109340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:632cd87ac6e4d8bda115f5e32e2b45cb8e28c59bd4c6e24b87985cf6b1f93354`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 01:03:26 GMT
ADD file:db6122b36f3e70c5f490b50afba99d49fa345f11d0f5c77bb3c6749f8e2a4f81 in / 
# Thu, 23 Apr 2020 01:03:28 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 13:54:58 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 13:54:59 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 13:55:22 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 13:57:35 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 13:57:35 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 13:57:36 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 13:58:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 13:58:37 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 13:58:38 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 13:58:39 GMT
WORKDIR /data
# Thu, 23 Apr 2020 13:58:39 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 13:58:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 13:58:41 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 13:58:41 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:50fb0052086928803f00724ca465c89c45dde5b082b1e59dadb8101286dd5ab6`  
		Last Modified: Thu, 23 Apr 2020 01:11:08 GMT  
		Size: 22.7 MB (22705377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98fc1f5e139d98aa45f74dfddb32ca22bec51ecf2fcab9bb372d91c14cc971d2`  
		Last Modified: Thu, 23 Apr 2020 14:00:18 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa98edd0b4c481052caeb348af3e906ef75764353840cfe2518af73963fcf2d`  
		Last Modified: Thu, 23 Apr 2020 14:00:18 GMT  
		Size: 1.4 MB (1368177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1ae9f68f12644f241fb270f9baf2e62d5b1380083acada1fdae86374998430`  
		Last Modified: Thu, 23 Apr 2020 14:00:21 GMT  
		Size: 7.0 MB (7033517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a23909059832233f41bcba599ec5bb698e278c652cf313dc6e8724fae8aa40cf`  
		Last Modified: Thu, 23 Apr 2020 14:00:19 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f5f6de32828cf1cb128a0cba17dc0396dead74aa6cc963394ac4f8b05540179`  
		Last Modified: Thu, 23 Apr 2020 14:00:18 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-buster` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:be463e278dc2125ea4c8984cd6a990353dfaa7f94570856734f86b900debc008
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 MB (34548547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0da52d2315939d969b12f3db6ae0aa5716074833f1ef06a42a544aec452d0ab2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:54:55 GMT
ADD file:581ee9c3c19f0d971aeda008fd399f59171cae75e8936b967dbf3888db4fc0d0 in / 
# Thu, 23 Apr 2020 00:54:58 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 16:01:56 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 16:01:57 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 16:02:29 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 16:04:19 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 16:04:20 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 16:04:20 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 16:05:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 16:05:20 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 16:05:20 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 16:05:21 GMT
WORKDIR /data
# Thu, 23 Apr 2020 16:05:21 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 16:05:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 16:05:22 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 16:05:24 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:bdc84a41f2513e28e99efeff9fcbb196b7df9883fb30532184bd67ca415b4673`  
		Last Modified: Thu, 23 Apr 2020 01:03:27 GMT  
		Size: 25.9 MB (25857800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698d3e76f19fb83cee90fe071552d86509322f0b8316774550c1ea7398327369`  
		Last Modified: Thu, 23 Apr 2020 16:07:31 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac4bbea6248caf60d5eca4d3e15d73d9cc18a5154a795c5ca3937eb040c9daae`  
		Last Modified: Thu, 23 Apr 2020 16:07:31 GMT  
		Size: 1.4 MB (1352987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1590123d45656fbb5cabd427b87908fd7347ef2fc6b0fba354f2b83771ec8882`  
		Last Modified: Thu, 23 Apr 2020 16:07:57 GMT  
		Size: 7.3 MB (7335481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e21891406b8ecd80c9cc4be90337cdd8d8935229002e8162d9afc9b68d2a4c30`  
		Last Modified: Thu, 23 Apr 2020 16:07:55 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d793eb07a5bc754267edbd54feb6cb25e4c28e7056a87e27960de4901d1dcc3`  
		Last Modified: Thu, 23 Apr 2020 16:07:55 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-buster` - linux; 386

```console
$ docker pull redis@sha256:0ac1dbfd6ca80b45aa587ecaa0632457ca254eea674a50e8574e8677f7a193a0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.2 MB (36151602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34c763545c4e57aabcdc00c9448e439a81bdaf47ae32d7711bc8e1252fb7ef59`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:39:36 GMT
ADD file:ca6a74f6b738c738c033152fab2a9aacf22bec5f19a994e6a02b5f919ee33ee9 in / 
# Thu, 23 Apr 2020 00:39:36 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 11:23:53 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 11:23:53 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 11:24:11 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 11:26:28 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 11:26:28 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 11:26:28 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 11:27:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 11:27:59 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 11:28:00 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 11:28:00 GMT
WORKDIR /data
# Thu, 23 Apr 2020 11:28:00 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 11:28:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 11:28:01 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 11:28:01 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:5d3da8f33b97fc107a05b3255a55836b76df9f817de632b1fb63c6e9c024f0df`  
		Last Modified: Thu, 23 Apr 2020 00:44:35 GMT  
		Size: 27.8 MB (27753972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f572d913eaf53def72d8eeff5384464ae75f0da9041d63ef0cd2fb2a43e21e`  
		Last Modified: Thu, 23 Apr 2020 11:30:12 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36c13a7e7929be4f05fbeddd74c94dfe85b704c504f7d13aa45bdb84bae79ccb`  
		Last Modified: Thu, 23 Apr 2020 11:30:12 GMT  
		Size: 1.4 MB (1387411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680a9b72444c93256224c2c5394c18343047b8b7dc305a4301401e7a6b494d03`  
		Last Modified: Thu, 23 Apr 2020 11:30:25 GMT  
		Size: 7.0 MB (7007988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e6148f8fb3eb037aaf97a9736b49d92d77541c5bbb6219db62f8af4f8d5e54`  
		Last Modified: Thu, 23 Apr 2020 11:30:23 GMT  
		Size: 97.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fae33d9962de4399f135693d495b300515e9d363f74683c3c366cd6e32290e1`  
		Last Modified: Thu, 23 Apr 2020 11:30:23 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-buster` - linux; mips64le

```console
$ docker pull redis@sha256:8860ea6be85bfa12a7a62f37e07716f197be8e76f498d1e62d3c4319582a3b60
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34731728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eab8ac536ee15de9306c977271c71a293db05c67e582fe002279ba86c8fff0a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:09:47 GMT
ADD file:7509945bd8a224048260e88b466aa3b156615e16b64e0a6702da277052fcb98b in / 
# Thu, 23 Apr 2020 00:09:48 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 09:24:32 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 09:24:33 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 09:25:02 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 09:28:42 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 09:28:42 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 09:28:43 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 09:31:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 09:32:01 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 09:32:01 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 09:32:01 GMT
WORKDIR /data
# Thu, 23 Apr 2020 09:32:02 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 09:32:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 09:32:02 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 09:32:03 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:ae8f0fa6cb0d971b4b8fedf7fc9b00f61f780b383fe7d64e6c2e4be8d20c3987`  
		Last Modified: Thu, 23 Apr 2020 00:17:46 GMT  
		Size: 25.8 MB (25762125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faf65c067540cd52d99f7f6df4511fb45d6a0485e47338d0239a052fcd64c8e3`  
		Last Modified: Thu, 23 Apr 2020 09:34:32 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef207bf80aefb18eba12c119d07499e37b5ea7bec06bc1e0c2dd749ddde45a1`  
		Last Modified: Thu, 23 Apr 2020 09:34:34 GMT  
		Size: 1.3 MB (1305489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae62dd92cc34f4856c15b7614910c5578f2d91d96d96469c21f8ca741c1061f5`  
		Last Modified: Thu, 23 Apr 2020 09:35:08 GMT  
		Size: 7.7 MB (7661872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693fe2f4d6e93636c838f7fb3a49c859d72138e5a25fd1687e590fcf3bb74dfb`  
		Last Modified: Thu, 23 Apr 2020 09:35:00 GMT  
		Size: 99.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:153c8eb8631e42a4705a53461aeb1c1edea4a60ad71a759b5eafeccbf3f5c142`  
		Last Modified: Thu, 23 Apr 2020 09:35:00 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-buster` - linux; ppc64le

```console
$ docker pull redis@sha256:e1c410783ee0d501a9804b3050db559054e95e91bb3cd8f3e81324baef92f730
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.7 MB (39696544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34098209a59e39ee25eeb2b0bf53ba98f873314c75110d6841a0793d5e1bc182`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:36:00 GMT
ADD file:5b3c3d2945800e1743dc02a4f68bd830fe2f67ca437223692eb460147c158c2b in / 
# Thu, 23 Apr 2020 00:36:04 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 17:29:48 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 17:29:51 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 17:31:38 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 17:35:14 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 17:35:18 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 17:35:23 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 17:38:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 17:38:25 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 17:38:28 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 17:38:32 GMT
WORKDIR /data
# Thu, 23 Apr 2020 17:38:34 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 17:38:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 17:38:42 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 17:38:45 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:012c6cdbd1af202bbfbea5945fafbb9aca9097f1fa3cb493a29155fdc02cc43c`  
		Last Modified: Thu, 23 Apr 2020 00:50:14 GMT  
		Size: 30.5 MB (30524638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee5a34bf53dadebb7466557f439affba6f1c11ddbdd7d2c1376f9540c294a7a`  
		Last Modified: Thu, 23 Apr 2020 17:42:03 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dedf97e3c0bcb476732135fc70dee2ba4766ff50ec51f93b1929ebaa6c4863f`  
		Last Modified: Thu, 23 Apr 2020 17:42:03 GMT  
		Size: 1.3 MB (1335327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2a1294a7da3aa34af8f45c22665913b8780fcf4dec6b52b108541e496dd0cc`  
		Last Modified: Thu, 23 Apr 2020 17:42:27 GMT  
		Size: 7.8 MB (7834296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51726f5fc1a7b6d031cad4d822aaf6c1801262570fb662454f1f2dc93cd4e551`  
		Last Modified: Thu, 23 Apr 2020 17:42:25 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e62728fce47996c1059a9f4f18e5e1efea4ebc55e17f82aa362f8985e7f019e`  
		Last Modified: Thu, 23 Apr 2020 17:42:25 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-buster` - linux; s390x

```console
$ docker pull redis@sha256:80a22e71a515d761d2c50a5873fc228fe165a627f9f91641391ce1548bc23f03
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34709447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5556ba73cac9fdc7f38ea53f8961a08497e52b1fa62f83611a9228a5d495e8fb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:51:48 GMT
ADD file:f6c2560f9185c1bcaff95e576e57449f606d51b85fad02646c1b0962bc9353c9 in / 
# Thu, 23 Apr 2020 00:51:50 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 06:58:44 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 06:58:44 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 06:58:58 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 06:59:46 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 06:59:47 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 06:59:47 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 07:00:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 07:00:24 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 07:00:24 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 07:00:24 GMT
WORKDIR /data
# Thu, 23 Apr 2020 07:00:24 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 07:00:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 07:00:25 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 07:00:25 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:d89dc3741ad42b79c3d8545495c429f3100d3f22234ff993bd04017b0675e868`  
		Last Modified: Thu, 23 Apr 2020 00:56:00 GMT  
		Size: 25.7 MB (25712105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c9894c70b29dc7cbad7e69c5f898b0a5d6f82aac9aff00e2645a6f8a9eff88`  
		Last Modified: Thu, 23 Apr 2020 07:01:34 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fba24ca231c607425b0e92a8a39c3174a8b9cb56ddeee71fc43f2f9dd9b1d2c`  
		Last Modified: Thu, 23 Apr 2020 07:01:35 GMT  
		Size: 1.4 MB (1403679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22d299e81a09eaaf9da803a2b3775444f312a34b2b7dd8e0c1c10d0171225ba`  
		Last Modified: Thu, 23 Apr 2020 07:01:52 GMT  
		Size: 7.6 MB (7591385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46db2cefe8baf230709535dd5f96c93520ca156d9821649ce8e8a2410e49d54`  
		Last Modified: Thu, 23 Apr 2020 07:01:56 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ec0a42c81dfec4356c31366a6ddf246ebac63394fafd37549a4483fd537513`  
		Last Modified: Thu, 23 Apr 2020 07:01:50 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redis:6`

```console
$ docker pull redis@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `redis:6.0`

```console
$ docker pull redis@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `redis:6.0.0`

```console
$ docker pull redis@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `redis:6.0.0-alpine`

```console
$ docker pull redis@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `redis:6.0.0-alpine3.11`

```console
$ docker pull redis@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `redis:6.0.0-buster`

```console
$ docker pull redis@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `redis:6.0-alpine`

```console
$ docker pull redis@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `redis:6.0-alpine3.11`

```console
$ docker pull redis@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `redis:6.0-buster`

```console
$ docker pull redis@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `redis:6-alpine`

```console
$ docker pull redis@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `redis:6-alpine3.11`

```console
$ docker pull redis@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `redis:6-buster`

```console
$ docker pull redis@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `redis:alpine`

```console
$ docker pull redis@sha256:83a3af36d5e57f2901b4783c313720e5fa3ecf0424ba86ad9775e06a9a5e35d0
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

### `redis:alpine` - linux; amd64

```console
$ docker pull redis@sha256:d4ada5d910403607b3f579d7171f36108c2e1cf67da966a712812230171fc153
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (9998790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3661c84ee9d0f6312a076b69eb2bd112674cadb70ef7e1594c4f00193f8df08e`
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
# Fri, 24 Apr 2020 19:20:54 GMT
ENV REDIS_VERSION=5.0.9
# Fri, 24 Apr 2020 19:20:54 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Fri, 24 Apr 2020 19:20:55 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Fri, 24 Apr 2020 19:21:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 24 Apr 2020 19:21:49 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 24 Apr 2020 19:21:49 GMT
VOLUME [/data]
# Fri, 24 Apr 2020 19:21:50 GMT
WORKDIR /data
# Fri, 24 Apr 2020 19:21:50 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 24 Apr 2020 19:21:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 19:21:50 GMT
EXPOSE 6379
# Fri, 24 Apr 2020 19:21:50 GMT
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
	-	`sha256:3e45770272d96deeb96c4bfa3cffde811f318823b4422bdbbf909148dc5669bb`  
		Last Modified: Fri, 24 Apr 2020 19:23:14 GMT  
		Size: 6.8 MB (6781166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:558de8ea3153bdccfaf67fadf7bbbdc60bf357f33ff0070df617d6e22ad46a13`  
		Last Modified: Fri, 24 Apr 2020 19:23:13 GMT  
		Size: 99.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2c65255161264f51556db666aa812834b3f51c8403b09799a46e4d0909e4aa4`  
		Last Modified: Fri, 24 Apr 2020 19:23:12 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:alpine` - linux; arm variant v6

```console
$ docker pull redis@sha256:867b50998330ae4743e95c8be69dee7ad37cbba8057659bef4dc142838d7f3e0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9725047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:333723767b2b5747763b5483d4742558e9abe6d70b98ee05d527643b5eb088d5`
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
# Thu, 23 Apr 2020 22:31:34 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 22:31:35 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 22:31:36 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 22:32:24 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 22:32:27 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 22:32:29 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 22:32:30 GMT
WORKDIR /data
# Thu, 23 Apr 2020 22:32:31 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Thu, 23 Apr 2020 22:32:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 22:32:33 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 22:32:34 GMT
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
	-	`sha256:75a2919ec032b1198ca13b052499b7c193e45d93756a3b0d7bb10c8db4f3db65`  
		Last Modified: Thu, 23 Apr 2020 22:34:01 GMT  
		Size: 6.7 MB (6697511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b2e77e4c2604e8e74b4c471b4a04d1a768eb84eadcfcd3621f135f7d4d90ca`  
		Last Modified: Thu, 23 Apr 2020 22:33:57 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18df89faaf97292802f6bca82a98892b7b0a168230ca31ae16e3cf307614a7a8`  
		Last Modified: Thu, 23 Apr 2020 22:33:57 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:alpine` - linux; arm variant v7

```console
$ docker pull redis@sha256:1c10570f57cb14b4fbd3446c61303aeb7db18b45abffc49974d5bde7e4a89de4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9394623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56a7ba195be67da9c68c67aa8d6eefa737236f15d3a9b490504ce943465c3a9f`
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
# Fri, 24 Apr 2020 08:52:43 GMT
ENV REDIS_VERSION=5.0.9
# Fri, 24 Apr 2020 08:52:43 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Fri, 24 Apr 2020 08:52:44 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Fri, 24 Apr 2020 08:53:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 24 Apr 2020 08:53:30 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 24 Apr 2020 08:53:31 GMT
VOLUME [/data]
# Fri, 24 Apr 2020 08:53:32 GMT
WORKDIR /data
# Fri, 24 Apr 2020 08:53:32 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 24 Apr 2020 08:53:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 08:53:34 GMT
EXPOSE 6379
# Fri, 24 Apr 2020 08:53:34 GMT
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
	-	`sha256:531954b17ac2db3cd86f3ced48c7c4f9fe053fad0792b7038321a667c911953a`  
		Last Modified: Fri, 24 Apr 2020 08:55:41 GMT  
		Size: 6.6 MB (6570977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d550a31e99202186ed01f1a5a4c96bab49dc143ad2a113696ecb48947836c0`  
		Last Modified: Fri, 24 Apr 2020 08:55:38 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a842b77b23971198e093c671bcf1e2cf6df771a6138ffb4132bfb37af22f17`  
		Last Modified: Fri, 24 Apr 2020 08:55:38 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:alpine` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:2ebdecb52315772800ba4549b9dc83910d9ae7de5364c3092b0390d7266e94a9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9918976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b6acb4ad7ccdd962d8579a0929ab5920a1f58ff996cd4812188219c1eb74e91`
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
# Fri, 24 Apr 2020 12:46:32 GMT
ENV REDIS_VERSION=5.0.9
# Fri, 24 Apr 2020 12:46:33 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Fri, 24 Apr 2020 12:46:34 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Fri, 24 Apr 2020 12:47:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 24 Apr 2020 12:47:24 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 24 Apr 2020 12:47:24 GMT
VOLUME [/data]
# Fri, 24 Apr 2020 12:47:25 GMT
WORKDIR /data
# Fri, 24 Apr 2020 12:47:26 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 24 Apr 2020 12:47:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 12:47:28 GMT
EXPOSE 6379
# Fri, 24 Apr 2020 12:47:29 GMT
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
	-	`sha256:f5ca1db598d2278e5526b65dcad0d96f0f0264060f879f1b437f58a467e27382`  
		Last Modified: Fri, 24 Apr 2020 12:49:17 GMT  
		Size: 6.8 MB (6788089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87542dce16ad38aeb18ffe2e2266f3bd9b8cbc70f6f4450be0e9f621022fabb5`  
		Last Modified: Fri, 24 Apr 2020 12:49:15 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a20d19811afde1a300515cade1279f18fb3ca0ef1800b52dcb45127731bd5f4`  
		Last Modified: Fri, 24 Apr 2020 12:49:15 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:alpine` - linux; 386

```console
$ docker pull redis@sha256:3ab6896b5efe215c5cc110a835fecb73d5f55672ad4443f4baf51822db1854c6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9710040 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bba820d7067104939d7ec907ee1fa581e9c7d40b0a204a14caf709f4dce84732`
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
# Fri, 24 Apr 2020 05:51:10 GMT
ENV REDIS_VERSION=5.0.9
# Fri, 24 Apr 2020 05:51:10 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Fri, 24 Apr 2020 05:51:10 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Fri, 24 Apr 2020 05:52:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 24 Apr 2020 05:52:17 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 24 Apr 2020 05:52:17 GMT
VOLUME [/data]
# Fri, 24 Apr 2020 05:52:17 GMT
WORKDIR /data
# Fri, 24 Apr 2020 05:52:17 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 24 Apr 2020 05:52:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 05:52:18 GMT
EXPOSE 6379
# Fri, 24 Apr 2020 05:52:18 GMT
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
	-	`sha256:7ed6bb387586efb069405e1b2fea60bf1718da22582dade16723a6ce6beb111c`  
		Last Modified: Fri, 24 Apr 2020 05:53:49 GMT  
		Size: 6.5 MB (6491980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ee2bc48c46cc40ec8951486a93e65583168f55239b5e10e350ceda82120fa3`  
		Last Modified: Fri, 24 Apr 2020 05:53:48 GMT  
		Size: 98.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae5b0c59c675cf868993ca6ec424636476caea5bc4e43525a866864d0b8bbd1`  
		Last Modified: Fri, 24 Apr 2020 05:53:48 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:alpine` - linux; ppc64le

```console
$ docker pull redis@sha256:14dfcd56148c897338a1306bf23b392e6ffce4ee486ddfcd77fb515e8f0f1557
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.5 MB (10494033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a0a1b6eb6701cd8c4349958777c681d81e0520d3e82317e2419b56b4d4ce4bf`
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
# Fri, 24 Apr 2020 09:03:45 GMT
ENV REDIS_VERSION=5.0.9
# Fri, 24 Apr 2020 09:03:48 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Fri, 24 Apr 2020 09:03:50 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Fri, 24 Apr 2020 09:04:40 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 24 Apr 2020 09:04:46 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 24 Apr 2020 09:04:50 GMT
VOLUME [/data]
# Fri, 24 Apr 2020 09:04:53 GMT
WORKDIR /data
# Fri, 24 Apr 2020 09:04:56 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 24 Apr 2020 09:04:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 09:05:01 GMT
EXPOSE 6379
# Fri, 24 Apr 2020 09:05:07 GMT
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
	-	`sha256:1ad3f9cade0fa9bda2c0f45df3a77c780ebc4adea7badb3b8387fed928c60ed7`  
		Last Modified: Fri, 24 Apr 2020 09:07:21 GMT  
		Size: 7.3 MB (7260512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ad499a196593cd717672adacc0550293f8b2c00a5907255640b27d266bc05a`  
		Last Modified: Fri, 24 Apr 2020 09:07:21 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5831b0ffd2731f416315c93a640459b17492812a21b7a6fba00919faaeb1d5`  
		Last Modified: Fri, 24 Apr 2020 09:07:19 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:alpine` - linux; s390x

```console
$ docker pull redis@sha256:5ad55b9f660c1e3b315e26e3497b9e4d270a5dd7ff431b14d9a17cf78fcac287
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (10008638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78dd64fd99b54ef1c40f2cd3351efcaf43b4d026dfcfe78315787e7a8220ffee`
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
# Fri, 24 Apr 2020 07:03:22 GMT
ENV REDIS_VERSION=5.0.9
# Fri, 24 Apr 2020 07:03:22 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Fri, 24 Apr 2020 07:03:22 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Fri, 24 Apr 2020 07:03:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 24 Apr 2020 07:03:53 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 24 Apr 2020 07:03:53 GMT
VOLUME [/data]
# Fri, 24 Apr 2020 07:03:54 GMT
WORKDIR /data
# Fri, 24 Apr 2020 07:03:54 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 24 Apr 2020 07:03:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 07:03:54 GMT
EXPOSE 6379
# Fri, 24 Apr 2020 07:03:54 GMT
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
	-	`sha256:4b3c809e9bcb4892e2da01d3bae84664c06e6bb0929c6813ef47a1aaaa3d675f`  
		Last Modified: Fri, 24 Apr 2020 07:05:07 GMT  
		Size: 7.0 MB (7016584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd1cb7e35314fbaf45935cb538fb36cc01e53dff4d37131a3497fd376720294e`  
		Last Modified: Fri, 24 Apr 2020 07:05:11 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529922dc84cb9fec77a0630b9ad535a7c843db2cd4518c25442c47fbc986d8b7`  
		Last Modified: Fri, 24 Apr 2020 07:05:06 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redis:alpine3.11`

```console
$ docker pull redis@sha256:83a3af36d5e57f2901b4783c313720e5fa3ecf0424ba86ad9775e06a9a5e35d0
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

### `redis:alpine3.11` - linux; amd64

```console
$ docker pull redis@sha256:d4ada5d910403607b3f579d7171f36108c2e1cf67da966a712812230171fc153
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (9998790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3661c84ee9d0f6312a076b69eb2bd112674cadb70ef7e1594c4f00193f8df08e`
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
# Fri, 24 Apr 2020 19:20:54 GMT
ENV REDIS_VERSION=5.0.9
# Fri, 24 Apr 2020 19:20:54 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Fri, 24 Apr 2020 19:20:55 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Fri, 24 Apr 2020 19:21:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 24 Apr 2020 19:21:49 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 24 Apr 2020 19:21:49 GMT
VOLUME [/data]
# Fri, 24 Apr 2020 19:21:50 GMT
WORKDIR /data
# Fri, 24 Apr 2020 19:21:50 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 24 Apr 2020 19:21:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 19:21:50 GMT
EXPOSE 6379
# Fri, 24 Apr 2020 19:21:50 GMT
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
	-	`sha256:3e45770272d96deeb96c4bfa3cffde811f318823b4422bdbbf909148dc5669bb`  
		Last Modified: Fri, 24 Apr 2020 19:23:14 GMT  
		Size: 6.8 MB (6781166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:558de8ea3153bdccfaf67fadf7bbbdc60bf357f33ff0070df617d6e22ad46a13`  
		Last Modified: Fri, 24 Apr 2020 19:23:13 GMT  
		Size: 99.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2c65255161264f51556db666aa812834b3f51c8403b09799a46e4d0909e4aa4`  
		Last Modified: Fri, 24 Apr 2020 19:23:12 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:alpine3.11` - linux; arm variant v6

```console
$ docker pull redis@sha256:867b50998330ae4743e95c8be69dee7ad37cbba8057659bef4dc142838d7f3e0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9725047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:333723767b2b5747763b5483d4742558e9abe6d70b98ee05d527643b5eb088d5`
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
# Thu, 23 Apr 2020 22:31:34 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 22:31:35 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 22:31:36 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 22:32:24 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 22:32:27 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 22:32:29 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 22:32:30 GMT
WORKDIR /data
# Thu, 23 Apr 2020 22:32:31 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Thu, 23 Apr 2020 22:32:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 22:32:33 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 22:32:34 GMT
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
	-	`sha256:75a2919ec032b1198ca13b052499b7c193e45d93756a3b0d7bb10c8db4f3db65`  
		Last Modified: Thu, 23 Apr 2020 22:34:01 GMT  
		Size: 6.7 MB (6697511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b2e77e4c2604e8e74b4c471b4a04d1a768eb84eadcfcd3621f135f7d4d90ca`  
		Last Modified: Thu, 23 Apr 2020 22:33:57 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18df89faaf97292802f6bca82a98892b7b0a168230ca31ae16e3cf307614a7a8`  
		Last Modified: Thu, 23 Apr 2020 22:33:57 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:alpine3.11` - linux; arm variant v7

```console
$ docker pull redis@sha256:1c10570f57cb14b4fbd3446c61303aeb7db18b45abffc49974d5bde7e4a89de4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9394623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56a7ba195be67da9c68c67aa8d6eefa737236f15d3a9b490504ce943465c3a9f`
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
# Fri, 24 Apr 2020 08:52:43 GMT
ENV REDIS_VERSION=5.0.9
# Fri, 24 Apr 2020 08:52:43 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Fri, 24 Apr 2020 08:52:44 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Fri, 24 Apr 2020 08:53:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 24 Apr 2020 08:53:30 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 24 Apr 2020 08:53:31 GMT
VOLUME [/data]
# Fri, 24 Apr 2020 08:53:32 GMT
WORKDIR /data
# Fri, 24 Apr 2020 08:53:32 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 24 Apr 2020 08:53:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 08:53:34 GMT
EXPOSE 6379
# Fri, 24 Apr 2020 08:53:34 GMT
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
	-	`sha256:531954b17ac2db3cd86f3ced48c7c4f9fe053fad0792b7038321a667c911953a`  
		Last Modified: Fri, 24 Apr 2020 08:55:41 GMT  
		Size: 6.6 MB (6570977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d550a31e99202186ed01f1a5a4c96bab49dc143ad2a113696ecb48947836c0`  
		Last Modified: Fri, 24 Apr 2020 08:55:38 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a842b77b23971198e093c671bcf1e2cf6df771a6138ffb4132bfb37af22f17`  
		Last Modified: Fri, 24 Apr 2020 08:55:38 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:alpine3.11` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:2ebdecb52315772800ba4549b9dc83910d9ae7de5364c3092b0390d7266e94a9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9918976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b6acb4ad7ccdd962d8579a0929ab5920a1f58ff996cd4812188219c1eb74e91`
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
# Fri, 24 Apr 2020 12:46:32 GMT
ENV REDIS_VERSION=5.0.9
# Fri, 24 Apr 2020 12:46:33 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Fri, 24 Apr 2020 12:46:34 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Fri, 24 Apr 2020 12:47:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 24 Apr 2020 12:47:24 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 24 Apr 2020 12:47:24 GMT
VOLUME [/data]
# Fri, 24 Apr 2020 12:47:25 GMT
WORKDIR /data
# Fri, 24 Apr 2020 12:47:26 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 24 Apr 2020 12:47:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 12:47:28 GMT
EXPOSE 6379
# Fri, 24 Apr 2020 12:47:29 GMT
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
	-	`sha256:f5ca1db598d2278e5526b65dcad0d96f0f0264060f879f1b437f58a467e27382`  
		Last Modified: Fri, 24 Apr 2020 12:49:17 GMT  
		Size: 6.8 MB (6788089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87542dce16ad38aeb18ffe2e2266f3bd9b8cbc70f6f4450be0e9f621022fabb5`  
		Last Modified: Fri, 24 Apr 2020 12:49:15 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a20d19811afde1a300515cade1279f18fb3ca0ef1800b52dcb45127731bd5f4`  
		Last Modified: Fri, 24 Apr 2020 12:49:15 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:alpine3.11` - linux; 386

```console
$ docker pull redis@sha256:3ab6896b5efe215c5cc110a835fecb73d5f55672ad4443f4baf51822db1854c6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9710040 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bba820d7067104939d7ec907ee1fa581e9c7d40b0a204a14caf709f4dce84732`
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
# Fri, 24 Apr 2020 05:51:10 GMT
ENV REDIS_VERSION=5.0.9
# Fri, 24 Apr 2020 05:51:10 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Fri, 24 Apr 2020 05:51:10 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Fri, 24 Apr 2020 05:52:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 24 Apr 2020 05:52:17 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 24 Apr 2020 05:52:17 GMT
VOLUME [/data]
# Fri, 24 Apr 2020 05:52:17 GMT
WORKDIR /data
# Fri, 24 Apr 2020 05:52:17 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 24 Apr 2020 05:52:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 05:52:18 GMT
EXPOSE 6379
# Fri, 24 Apr 2020 05:52:18 GMT
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
	-	`sha256:7ed6bb387586efb069405e1b2fea60bf1718da22582dade16723a6ce6beb111c`  
		Last Modified: Fri, 24 Apr 2020 05:53:49 GMT  
		Size: 6.5 MB (6491980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ee2bc48c46cc40ec8951486a93e65583168f55239b5e10e350ceda82120fa3`  
		Last Modified: Fri, 24 Apr 2020 05:53:48 GMT  
		Size: 98.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae5b0c59c675cf868993ca6ec424636476caea5bc4e43525a866864d0b8bbd1`  
		Last Modified: Fri, 24 Apr 2020 05:53:48 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:alpine3.11` - linux; ppc64le

```console
$ docker pull redis@sha256:14dfcd56148c897338a1306bf23b392e6ffce4ee486ddfcd77fb515e8f0f1557
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.5 MB (10494033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a0a1b6eb6701cd8c4349958777c681d81e0520d3e82317e2419b56b4d4ce4bf`
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
# Fri, 24 Apr 2020 09:03:45 GMT
ENV REDIS_VERSION=5.0.9
# Fri, 24 Apr 2020 09:03:48 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Fri, 24 Apr 2020 09:03:50 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Fri, 24 Apr 2020 09:04:40 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 24 Apr 2020 09:04:46 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 24 Apr 2020 09:04:50 GMT
VOLUME [/data]
# Fri, 24 Apr 2020 09:04:53 GMT
WORKDIR /data
# Fri, 24 Apr 2020 09:04:56 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 24 Apr 2020 09:04:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 09:05:01 GMT
EXPOSE 6379
# Fri, 24 Apr 2020 09:05:07 GMT
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
	-	`sha256:1ad3f9cade0fa9bda2c0f45df3a77c780ebc4adea7badb3b8387fed928c60ed7`  
		Last Modified: Fri, 24 Apr 2020 09:07:21 GMT  
		Size: 7.3 MB (7260512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0ad499a196593cd717672adacc0550293f8b2c00a5907255640b27d266bc05a`  
		Last Modified: Fri, 24 Apr 2020 09:07:21 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5831b0ffd2731f416315c93a640459b17492812a21b7a6fba00919faaeb1d5`  
		Last Modified: Fri, 24 Apr 2020 09:07:19 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:alpine3.11` - linux; s390x

```console
$ docker pull redis@sha256:5ad55b9f660c1e3b315e26e3497b9e4d270a5dd7ff431b14d9a17cf78fcac287
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (10008638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78dd64fd99b54ef1c40f2cd3351efcaf43b4d026dfcfe78315787e7a8220ffee`
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
# Fri, 24 Apr 2020 07:03:22 GMT
ENV REDIS_VERSION=5.0.9
# Fri, 24 Apr 2020 07:03:22 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Fri, 24 Apr 2020 07:03:22 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Fri, 24 Apr 2020 07:03:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		gcc 		linux-headers 		make 		musl-dev 		openssl-dev 	; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redis-rundeps $runDeps; 	apk del --no-network .build-deps; 		redis-cli --version; 	redis-server --version
# Fri, 24 Apr 2020 07:03:53 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 24 Apr 2020 07:03:53 GMT
VOLUME [/data]
# Fri, 24 Apr 2020 07:03:54 GMT
WORKDIR /data
# Fri, 24 Apr 2020 07:03:54 GMT
COPY file:c48b97ea65422782310396358f838c38c0747767dd606a88d4c3d0b034a60762 in /usr/local/bin/ 
# Fri, 24 Apr 2020 07:03:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 07:03:54 GMT
EXPOSE 6379
# Fri, 24 Apr 2020 07:03:54 GMT
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
	-	`sha256:4b3c809e9bcb4892e2da01d3bae84664c06e6bb0929c6813ef47a1aaaa3d675f`  
		Last Modified: Fri, 24 Apr 2020 07:05:07 GMT  
		Size: 7.0 MB (7016584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd1cb7e35314fbaf45935cb538fb36cc01e53dff4d37131a3497fd376720294e`  
		Last Modified: Fri, 24 Apr 2020 07:05:11 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529922dc84cb9fec77a0630b9ad535a7c843db2cd4518c25442c47fbc986d8b7`  
		Last Modified: Fri, 24 Apr 2020 07:05:06 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redis:buster`

```console
$ docker pull redis@sha256:157a95b41b0dca8c308a33489dfdb28019e033110320414b4b16fad7d28c0f9f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `redis:buster` - linux; amd64

```console
$ docker pull redis@sha256:43dbbe6f633572d66e84e7162245d8d70a18f00b819d6c0bf98ca02109f4788c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35863297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4d3716dbb72408a7843e12d7d9f6a5addf7ab28ac21e9e9da4a6a51f1b32da9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:20:32 GMT
ADD file:9b8be2b52ee0fa31da1b6256099030b73546253a57e94cccb24605cd888bb74d in / 
# Thu, 23 Apr 2020 00:20:32 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 19:48:34 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 19:48:34 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 19:48:46 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 19:50:08 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 19:50:08 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 19:50:08 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 19:51:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 19:51:26 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 19:51:26 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 19:51:27 GMT
WORKDIR /data
# Thu, 23 Apr 2020 19:51:27 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 19:51:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 19:51:28 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 19:51:28 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:54fec2fa59d0a0de9cd2dec9850b36c43de451f1fd1c0a5bf8f1cf26a61a5da4`  
		Last Modified: Thu, 23 Apr 2020 00:25:10 GMT  
		Size: 27.1 MB (27098254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c94e11103d92f2a83b82e5d4287445cba073af0002cecee98d85d68ccec0f89`  
		Last Modified: Thu, 23 Apr 2020 19:55:42 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ab1bfc453f19989c401c2f0622df3363b5182bdea1af9e59ee2ceea3a9931c`  
		Last Modified: Thu, 23 Apr 2020 19:55:43 GMT  
		Size: 1.4 MB (1417711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f71e6b94d83f5a0df5d032ce4998b4834287bd4ed307ff7c9a31ad0a60caa98`  
		Last Modified: Thu, 23 Apr 2020 19:55:55 GMT  
		Size: 7.3 MB (7345094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2729a8234dd5e724571528d78d5f581702abc77be39db93fc0ae741340eb1c18`  
		Last Modified: Thu, 23 Apr 2020 19:55:53 GMT  
		Size: 97.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2683d7f177455cf86b4cf424cc757f1d177d5772df77bdaeeace411006eb88a5`  
		Last Modified: Thu, 23 Apr 2020 19:55:53 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:buster` - linux; arm variant v5

```console
$ docker pull redis@sha256:5a474d0e7c55a7e45ddaf530f4f2ab4bc8dcaba6d85b0829f1121f7fe53414fd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.4 MB (33394023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b83a1e222e2b9be5acf1ae9a03cd2e6d2c7a4efcd3b73a275481c652552de80`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:52:22 GMT
ADD file:62a9732be4e3237ccc896f724a34606e01f351c4877e52c9a9cd85029c06b956 in / 
# Thu, 23 Apr 2020 00:52:23 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 09:33:20 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 09:33:21 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 09:33:56 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 09:35:38 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 09:35:39 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 09:35:39 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 09:36:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 09:36:48 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 09:36:48 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 09:36:49 GMT
WORKDIR /data
# Thu, 23 Apr 2020 09:36:50 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 09:36:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 09:36:51 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 09:36:52 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:a8c46e5952878f9f324df86c5a2b45b2e0020f6721e820981e74461d77a100dd`  
		Last Modified: Thu, 23 Apr 2020 00:59:50 GMT  
		Size: 24.8 MB (24836319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471287e557b84038803c3a26dee3987da48cbcae6529a77a28f486e4527757f7`  
		Last Modified: Thu, 23 Apr 2020 09:39:42 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:016e8ff197695f0c8e2c3ae127ac9459df9c71e52ae54500970e692d2799c944`  
		Last Modified: Thu, 23 Apr 2020 09:39:42 GMT  
		Size: 1.4 MB (1376131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd64ec452edc906dc611493aae3c90529a0d5787d8dc3b8c1088b41b53379d2d`  
		Last Modified: Thu, 23 Apr 2020 09:40:07 GMT  
		Size: 7.2 MB (7179305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ca72abe00cf1354dc501a32ed89705fdacd4905631c42186458d9d3202cc90`  
		Last Modified: Thu, 23 Apr 2020 09:40:05 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e7807337a06858bed0eac541f5935b123a4abb0d973dacb1973753c6dcb2469`  
		Last Modified: Thu, 23 Apr 2020 09:40:04 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:buster` - linux; arm variant v7

```console
$ docker pull redis@sha256:afc097fd6784e016756816ecc4ae33dc9ef22f5715db3593b90b7ec17e906edf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.1 MB (31109340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:632cd87ac6e4d8bda115f5e32e2b45cb8e28c59bd4c6e24b87985cf6b1f93354`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 01:03:26 GMT
ADD file:db6122b36f3e70c5f490b50afba99d49fa345f11d0f5c77bb3c6749f8e2a4f81 in / 
# Thu, 23 Apr 2020 01:03:28 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 13:54:58 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 13:54:59 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 13:55:22 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 13:57:35 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 13:57:35 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 13:57:36 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 13:58:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 13:58:37 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 13:58:38 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 13:58:39 GMT
WORKDIR /data
# Thu, 23 Apr 2020 13:58:39 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 13:58:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 13:58:41 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 13:58:41 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:50fb0052086928803f00724ca465c89c45dde5b082b1e59dadb8101286dd5ab6`  
		Last Modified: Thu, 23 Apr 2020 01:11:08 GMT  
		Size: 22.7 MB (22705377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98fc1f5e139d98aa45f74dfddb32ca22bec51ecf2fcab9bb372d91c14cc971d2`  
		Last Modified: Thu, 23 Apr 2020 14:00:18 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa98edd0b4c481052caeb348af3e906ef75764353840cfe2518af73963fcf2d`  
		Last Modified: Thu, 23 Apr 2020 14:00:18 GMT  
		Size: 1.4 MB (1368177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1ae9f68f12644f241fb270f9baf2e62d5b1380083acada1fdae86374998430`  
		Last Modified: Thu, 23 Apr 2020 14:00:21 GMT  
		Size: 7.0 MB (7033517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a23909059832233f41bcba599ec5bb698e278c652cf313dc6e8724fae8aa40cf`  
		Last Modified: Thu, 23 Apr 2020 14:00:19 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f5f6de32828cf1cb128a0cba17dc0396dead74aa6cc963394ac4f8b05540179`  
		Last Modified: Thu, 23 Apr 2020 14:00:18 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:buster` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:be463e278dc2125ea4c8984cd6a990353dfaa7f94570856734f86b900debc008
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 MB (34548547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0da52d2315939d969b12f3db6ae0aa5716074833f1ef06a42a544aec452d0ab2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:54:55 GMT
ADD file:581ee9c3c19f0d971aeda008fd399f59171cae75e8936b967dbf3888db4fc0d0 in / 
# Thu, 23 Apr 2020 00:54:58 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 16:01:56 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 16:01:57 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 16:02:29 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 16:04:19 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 16:04:20 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 16:04:20 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 16:05:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 16:05:20 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 16:05:20 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 16:05:21 GMT
WORKDIR /data
# Thu, 23 Apr 2020 16:05:21 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 16:05:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 16:05:22 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 16:05:24 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:bdc84a41f2513e28e99efeff9fcbb196b7df9883fb30532184bd67ca415b4673`  
		Last Modified: Thu, 23 Apr 2020 01:03:27 GMT  
		Size: 25.9 MB (25857800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698d3e76f19fb83cee90fe071552d86509322f0b8316774550c1ea7398327369`  
		Last Modified: Thu, 23 Apr 2020 16:07:31 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac4bbea6248caf60d5eca4d3e15d73d9cc18a5154a795c5ca3937eb040c9daae`  
		Last Modified: Thu, 23 Apr 2020 16:07:31 GMT  
		Size: 1.4 MB (1352987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1590123d45656fbb5cabd427b87908fd7347ef2fc6b0fba354f2b83771ec8882`  
		Last Modified: Thu, 23 Apr 2020 16:07:57 GMT  
		Size: 7.3 MB (7335481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e21891406b8ecd80c9cc4be90337cdd8d8935229002e8162d9afc9b68d2a4c30`  
		Last Modified: Thu, 23 Apr 2020 16:07:55 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d793eb07a5bc754267edbd54feb6cb25e4c28e7056a87e27960de4901d1dcc3`  
		Last Modified: Thu, 23 Apr 2020 16:07:55 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:buster` - linux; 386

```console
$ docker pull redis@sha256:0ac1dbfd6ca80b45aa587ecaa0632457ca254eea674a50e8574e8677f7a193a0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.2 MB (36151602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34c763545c4e57aabcdc00c9448e439a81bdaf47ae32d7711bc8e1252fb7ef59`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:39:36 GMT
ADD file:ca6a74f6b738c738c033152fab2a9aacf22bec5f19a994e6a02b5f919ee33ee9 in / 
# Thu, 23 Apr 2020 00:39:36 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 11:23:53 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 11:23:53 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 11:24:11 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 11:26:28 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 11:26:28 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 11:26:28 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 11:27:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 11:27:59 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 11:28:00 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 11:28:00 GMT
WORKDIR /data
# Thu, 23 Apr 2020 11:28:00 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 11:28:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 11:28:01 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 11:28:01 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:5d3da8f33b97fc107a05b3255a55836b76df9f817de632b1fb63c6e9c024f0df`  
		Last Modified: Thu, 23 Apr 2020 00:44:35 GMT  
		Size: 27.8 MB (27753972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f572d913eaf53def72d8eeff5384464ae75f0da9041d63ef0cd2fb2a43e21e`  
		Last Modified: Thu, 23 Apr 2020 11:30:12 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36c13a7e7929be4f05fbeddd74c94dfe85b704c504f7d13aa45bdb84bae79ccb`  
		Last Modified: Thu, 23 Apr 2020 11:30:12 GMT  
		Size: 1.4 MB (1387411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680a9b72444c93256224c2c5394c18343047b8b7dc305a4301401e7a6b494d03`  
		Last Modified: Thu, 23 Apr 2020 11:30:25 GMT  
		Size: 7.0 MB (7007988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e6148f8fb3eb037aaf97a9736b49d92d77541c5bbb6219db62f8af4f8d5e54`  
		Last Modified: Thu, 23 Apr 2020 11:30:23 GMT  
		Size: 97.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fae33d9962de4399f135693d495b300515e9d363f74683c3c366cd6e32290e1`  
		Last Modified: Thu, 23 Apr 2020 11:30:23 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:buster` - linux; mips64le

```console
$ docker pull redis@sha256:8860ea6be85bfa12a7a62f37e07716f197be8e76f498d1e62d3c4319582a3b60
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34731728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eab8ac536ee15de9306c977271c71a293db05c67e582fe002279ba86c8fff0a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:09:47 GMT
ADD file:7509945bd8a224048260e88b466aa3b156615e16b64e0a6702da277052fcb98b in / 
# Thu, 23 Apr 2020 00:09:48 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 09:24:32 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 09:24:33 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 09:25:02 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 09:28:42 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 09:28:42 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 09:28:43 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 09:31:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 09:32:01 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 09:32:01 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 09:32:01 GMT
WORKDIR /data
# Thu, 23 Apr 2020 09:32:02 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 09:32:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 09:32:02 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 09:32:03 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:ae8f0fa6cb0d971b4b8fedf7fc9b00f61f780b383fe7d64e6c2e4be8d20c3987`  
		Last Modified: Thu, 23 Apr 2020 00:17:46 GMT  
		Size: 25.8 MB (25762125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faf65c067540cd52d99f7f6df4511fb45d6a0485e47338d0239a052fcd64c8e3`  
		Last Modified: Thu, 23 Apr 2020 09:34:32 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef207bf80aefb18eba12c119d07499e37b5ea7bec06bc1e0c2dd749ddde45a1`  
		Last Modified: Thu, 23 Apr 2020 09:34:34 GMT  
		Size: 1.3 MB (1305489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae62dd92cc34f4856c15b7614910c5578f2d91d96d96469c21f8ca741c1061f5`  
		Last Modified: Thu, 23 Apr 2020 09:35:08 GMT  
		Size: 7.7 MB (7661872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693fe2f4d6e93636c838f7fb3a49c859d72138e5a25fd1687e590fcf3bb74dfb`  
		Last Modified: Thu, 23 Apr 2020 09:35:00 GMT  
		Size: 99.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:153c8eb8631e42a4705a53461aeb1c1edea4a60ad71a759b5eafeccbf3f5c142`  
		Last Modified: Thu, 23 Apr 2020 09:35:00 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:buster` - linux; ppc64le

```console
$ docker pull redis@sha256:e1c410783ee0d501a9804b3050db559054e95e91bb3cd8f3e81324baef92f730
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.7 MB (39696544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34098209a59e39ee25eeb2b0bf53ba98f873314c75110d6841a0793d5e1bc182`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:36:00 GMT
ADD file:5b3c3d2945800e1743dc02a4f68bd830fe2f67ca437223692eb460147c158c2b in / 
# Thu, 23 Apr 2020 00:36:04 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 17:29:48 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 17:29:51 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 17:31:38 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 17:35:14 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 17:35:18 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 17:35:23 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 17:38:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 17:38:25 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 17:38:28 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 17:38:32 GMT
WORKDIR /data
# Thu, 23 Apr 2020 17:38:34 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 17:38:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 17:38:42 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 17:38:45 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:012c6cdbd1af202bbfbea5945fafbb9aca9097f1fa3cb493a29155fdc02cc43c`  
		Last Modified: Thu, 23 Apr 2020 00:50:14 GMT  
		Size: 30.5 MB (30524638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee5a34bf53dadebb7466557f439affba6f1c11ddbdd7d2c1376f9540c294a7a`  
		Last Modified: Thu, 23 Apr 2020 17:42:03 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dedf97e3c0bcb476732135fc70dee2ba4766ff50ec51f93b1929ebaa6c4863f`  
		Last Modified: Thu, 23 Apr 2020 17:42:03 GMT  
		Size: 1.3 MB (1335327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2a1294a7da3aa34af8f45c22665913b8780fcf4dec6b52b108541e496dd0cc`  
		Last Modified: Thu, 23 Apr 2020 17:42:27 GMT  
		Size: 7.8 MB (7834296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51726f5fc1a7b6d031cad4d822aaf6c1801262570fb662454f1f2dc93cd4e551`  
		Last Modified: Thu, 23 Apr 2020 17:42:25 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e62728fce47996c1059a9f4f18e5e1efea4ebc55e17f82aa362f8985e7f019e`  
		Last Modified: Thu, 23 Apr 2020 17:42:25 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:buster` - linux; s390x

```console
$ docker pull redis@sha256:80a22e71a515d761d2c50a5873fc228fe165a627f9f91641391ce1548bc23f03
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34709447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5556ba73cac9fdc7f38ea53f8961a08497e52b1fa62f83611a9228a5d495e8fb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:51:48 GMT
ADD file:f6c2560f9185c1bcaff95e576e57449f606d51b85fad02646c1b0962bc9353c9 in / 
# Thu, 23 Apr 2020 00:51:50 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 06:58:44 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 06:58:44 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 06:58:58 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 06:59:46 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 06:59:47 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 06:59:47 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 07:00:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 07:00:24 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 07:00:24 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 07:00:24 GMT
WORKDIR /data
# Thu, 23 Apr 2020 07:00:24 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 07:00:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 07:00:25 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 07:00:25 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:d89dc3741ad42b79c3d8545495c429f3100d3f22234ff993bd04017b0675e868`  
		Last Modified: Thu, 23 Apr 2020 00:56:00 GMT  
		Size: 25.7 MB (25712105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c9894c70b29dc7cbad7e69c5f898b0a5d6f82aac9aff00e2645a6f8a9eff88`  
		Last Modified: Thu, 23 Apr 2020 07:01:34 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fba24ca231c607425b0e92a8a39c3174a8b9cb56ddeee71fc43f2f9dd9b1d2c`  
		Last Modified: Thu, 23 Apr 2020 07:01:35 GMT  
		Size: 1.4 MB (1403679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22d299e81a09eaaf9da803a2b3775444f312a34b2b7dd8e0c1c10d0171225ba`  
		Last Modified: Thu, 23 Apr 2020 07:01:52 GMT  
		Size: 7.6 MB (7591385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46db2cefe8baf230709535dd5f96c93520ca156d9821649ce8e8a2410e49d54`  
		Last Modified: Thu, 23 Apr 2020 07:01:56 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ec0a42c81dfec4356c31366a6ddf246ebac63394fafd37549a4483fd537513`  
		Last Modified: Thu, 23 Apr 2020 07:01:50 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redis:latest`

```console
$ docker pull redis@sha256:157a95b41b0dca8c308a33489dfdb28019e033110320414b4b16fad7d28c0f9f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `redis:latest` - linux; amd64

```console
$ docker pull redis@sha256:43dbbe6f633572d66e84e7162245d8d70a18f00b819d6c0bf98ca02109f4788c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35863297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4d3716dbb72408a7843e12d7d9f6a5addf7ab28ac21e9e9da4a6a51f1b32da9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:20:32 GMT
ADD file:9b8be2b52ee0fa31da1b6256099030b73546253a57e94cccb24605cd888bb74d in / 
# Thu, 23 Apr 2020 00:20:32 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 19:48:34 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 19:48:34 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 19:48:46 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 19:50:08 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 19:50:08 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 19:50:08 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 19:51:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 19:51:26 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 19:51:26 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 19:51:27 GMT
WORKDIR /data
# Thu, 23 Apr 2020 19:51:27 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 19:51:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 19:51:28 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 19:51:28 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:54fec2fa59d0a0de9cd2dec9850b36c43de451f1fd1c0a5bf8f1cf26a61a5da4`  
		Last Modified: Thu, 23 Apr 2020 00:25:10 GMT  
		Size: 27.1 MB (27098254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c94e11103d92f2a83b82e5d4287445cba073af0002cecee98d85d68ccec0f89`  
		Last Modified: Thu, 23 Apr 2020 19:55:42 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ab1bfc453f19989c401c2f0622df3363b5182bdea1af9e59ee2ceea3a9931c`  
		Last Modified: Thu, 23 Apr 2020 19:55:43 GMT  
		Size: 1.4 MB (1417711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f71e6b94d83f5a0df5d032ce4998b4834287bd4ed307ff7c9a31ad0a60caa98`  
		Last Modified: Thu, 23 Apr 2020 19:55:55 GMT  
		Size: 7.3 MB (7345094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2729a8234dd5e724571528d78d5f581702abc77be39db93fc0ae741340eb1c18`  
		Last Modified: Thu, 23 Apr 2020 19:55:53 GMT  
		Size: 97.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2683d7f177455cf86b4cf424cc757f1d177d5772df77bdaeeace411006eb88a5`  
		Last Modified: Thu, 23 Apr 2020 19:55:53 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:latest` - linux; arm variant v5

```console
$ docker pull redis@sha256:5a474d0e7c55a7e45ddaf530f4f2ab4bc8dcaba6d85b0829f1121f7fe53414fd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.4 MB (33394023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b83a1e222e2b9be5acf1ae9a03cd2e6d2c7a4efcd3b73a275481c652552de80`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:52:22 GMT
ADD file:62a9732be4e3237ccc896f724a34606e01f351c4877e52c9a9cd85029c06b956 in / 
# Thu, 23 Apr 2020 00:52:23 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 09:33:20 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 09:33:21 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 09:33:56 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 09:35:38 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 09:35:39 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 09:35:39 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 09:36:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 09:36:48 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 09:36:48 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 09:36:49 GMT
WORKDIR /data
# Thu, 23 Apr 2020 09:36:50 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 09:36:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 09:36:51 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 09:36:52 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:a8c46e5952878f9f324df86c5a2b45b2e0020f6721e820981e74461d77a100dd`  
		Last Modified: Thu, 23 Apr 2020 00:59:50 GMT  
		Size: 24.8 MB (24836319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471287e557b84038803c3a26dee3987da48cbcae6529a77a28f486e4527757f7`  
		Last Modified: Thu, 23 Apr 2020 09:39:42 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:016e8ff197695f0c8e2c3ae127ac9459df9c71e52ae54500970e692d2799c944`  
		Last Modified: Thu, 23 Apr 2020 09:39:42 GMT  
		Size: 1.4 MB (1376131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd64ec452edc906dc611493aae3c90529a0d5787d8dc3b8c1088b41b53379d2d`  
		Last Modified: Thu, 23 Apr 2020 09:40:07 GMT  
		Size: 7.2 MB (7179305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ca72abe00cf1354dc501a32ed89705fdacd4905631c42186458d9d3202cc90`  
		Last Modified: Thu, 23 Apr 2020 09:40:05 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e7807337a06858bed0eac541f5935b123a4abb0d973dacb1973753c6dcb2469`  
		Last Modified: Thu, 23 Apr 2020 09:40:04 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:latest` - linux; arm variant v7

```console
$ docker pull redis@sha256:afc097fd6784e016756816ecc4ae33dc9ef22f5715db3593b90b7ec17e906edf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.1 MB (31109340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:632cd87ac6e4d8bda115f5e32e2b45cb8e28c59bd4c6e24b87985cf6b1f93354`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 01:03:26 GMT
ADD file:db6122b36f3e70c5f490b50afba99d49fa345f11d0f5c77bb3c6749f8e2a4f81 in / 
# Thu, 23 Apr 2020 01:03:28 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 13:54:58 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 13:54:59 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 13:55:22 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 13:57:35 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 13:57:35 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 13:57:36 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 13:58:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 13:58:37 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 13:58:38 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 13:58:39 GMT
WORKDIR /data
# Thu, 23 Apr 2020 13:58:39 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 13:58:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 13:58:41 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 13:58:41 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:50fb0052086928803f00724ca465c89c45dde5b082b1e59dadb8101286dd5ab6`  
		Last Modified: Thu, 23 Apr 2020 01:11:08 GMT  
		Size: 22.7 MB (22705377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98fc1f5e139d98aa45f74dfddb32ca22bec51ecf2fcab9bb372d91c14cc971d2`  
		Last Modified: Thu, 23 Apr 2020 14:00:18 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa98edd0b4c481052caeb348af3e906ef75764353840cfe2518af73963fcf2d`  
		Last Modified: Thu, 23 Apr 2020 14:00:18 GMT  
		Size: 1.4 MB (1368177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1ae9f68f12644f241fb270f9baf2e62d5b1380083acada1fdae86374998430`  
		Last Modified: Thu, 23 Apr 2020 14:00:21 GMT  
		Size: 7.0 MB (7033517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a23909059832233f41bcba599ec5bb698e278c652cf313dc6e8724fae8aa40cf`  
		Last Modified: Thu, 23 Apr 2020 14:00:19 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f5f6de32828cf1cb128a0cba17dc0396dead74aa6cc963394ac4f8b05540179`  
		Last Modified: Thu, 23 Apr 2020 14:00:18 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:latest` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:be463e278dc2125ea4c8984cd6a990353dfaa7f94570856734f86b900debc008
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 MB (34548547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0da52d2315939d969b12f3db6ae0aa5716074833f1ef06a42a544aec452d0ab2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:54:55 GMT
ADD file:581ee9c3c19f0d971aeda008fd399f59171cae75e8936b967dbf3888db4fc0d0 in / 
# Thu, 23 Apr 2020 00:54:58 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 16:01:56 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 16:01:57 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 16:02:29 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 16:04:19 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 16:04:20 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 16:04:20 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 16:05:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 16:05:20 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 16:05:20 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 16:05:21 GMT
WORKDIR /data
# Thu, 23 Apr 2020 16:05:21 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 16:05:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 16:05:22 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 16:05:24 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:bdc84a41f2513e28e99efeff9fcbb196b7df9883fb30532184bd67ca415b4673`  
		Last Modified: Thu, 23 Apr 2020 01:03:27 GMT  
		Size: 25.9 MB (25857800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698d3e76f19fb83cee90fe071552d86509322f0b8316774550c1ea7398327369`  
		Last Modified: Thu, 23 Apr 2020 16:07:31 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac4bbea6248caf60d5eca4d3e15d73d9cc18a5154a795c5ca3937eb040c9daae`  
		Last Modified: Thu, 23 Apr 2020 16:07:31 GMT  
		Size: 1.4 MB (1352987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1590123d45656fbb5cabd427b87908fd7347ef2fc6b0fba354f2b83771ec8882`  
		Last Modified: Thu, 23 Apr 2020 16:07:57 GMT  
		Size: 7.3 MB (7335481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e21891406b8ecd80c9cc4be90337cdd8d8935229002e8162d9afc9b68d2a4c30`  
		Last Modified: Thu, 23 Apr 2020 16:07:55 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d793eb07a5bc754267edbd54feb6cb25e4c28e7056a87e27960de4901d1dcc3`  
		Last Modified: Thu, 23 Apr 2020 16:07:55 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:latest` - linux; 386

```console
$ docker pull redis@sha256:0ac1dbfd6ca80b45aa587ecaa0632457ca254eea674a50e8574e8677f7a193a0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.2 MB (36151602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34c763545c4e57aabcdc00c9448e439a81bdaf47ae32d7711bc8e1252fb7ef59`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:39:36 GMT
ADD file:ca6a74f6b738c738c033152fab2a9aacf22bec5f19a994e6a02b5f919ee33ee9 in / 
# Thu, 23 Apr 2020 00:39:36 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 11:23:53 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 11:23:53 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 11:24:11 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 11:26:28 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 11:26:28 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 11:26:28 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 11:27:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 11:27:59 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 11:28:00 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 11:28:00 GMT
WORKDIR /data
# Thu, 23 Apr 2020 11:28:00 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 11:28:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 11:28:01 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 11:28:01 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:5d3da8f33b97fc107a05b3255a55836b76df9f817de632b1fb63c6e9c024f0df`  
		Last Modified: Thu, 23 Apr 2020 00:44:35 GMT  
		Size: 27.8 MB (27753972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f572d913eaf53def72d8eeff5384464ae75f0da9041d63ef0cd2fb2a43e21e`  
		Last Modified: Thu, 23 Apr 2020 11:30:12 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36c13a7e7929be4f05fbeddd74c94dfe85b704c504f7d13aa45bdb84bae79ccb`  
		Last Modified: Thu, 23 Apr 2020 11:30:12 GMT  
		Size: 1.4 MB (1387411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680a9b72444c93256224c2c5394c18343047b8b7dc305a4301401e7a6b494d03`  
		Last Modified: Thu, 23 Apr 2020 11:30:25 GMT  
		Size: 7.0 MB (7007988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e6148f8fb3eb037aaf97a9736b49d92d77541c5bbb6219db62f8af4f8d5e54`  
		Last Modified: Thu, 23 Apr 2020 11:30:23 GMT  
		Size: 97.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fae33d9962de4399f135693d495b300515e9d363f74683c3c366cd6e32290e1`  
		Last Modified: Thu, 23 Apr 2020 11:30:23 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:latest` - linux; mips64le

```console
$ docker pull redis@sha256:8860ea6be85bfa12a7a62f37e07716f197be8e76f498d1e62d3c4319582a3b60
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34731728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eab8ac536ee15de9306c977271c71a293db05c67e582fe002279ba86c8fff0a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:09:47 GMT
ADD file:7509945bd8a224048260e88b466aa3b156615e16b64e0a6702da277052fcb98b in / 
# Thu, 23 Apr 2020 00:09:48 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 09:24:32 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 09:24:33 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 09:25:02 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 09:28:42 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 09:28:42 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 09:28:43 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 09:31:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 09:32:01 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 09:32:01 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 09:32:01 GMT
WORKDIR /data
# Thu, 23 Apr 2020 09:32:02 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 09:32:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 09:32:02 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 09:32:03 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:ae8f0fa6cb0d971b4b8fedf7fc9b00f61f780b383fe7d64e6c2e4be8d20c3987`  
		Last Modified: Thu, 23 Apr 2020 00:17:46 GMT  
		Size: 25.8 MB (25762125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faf65c067540cd52d99f7f6df4511fb45d6a0485e47338d0239a052fcd64c8e3`  
		Last Modified: Thu, 23 Apr 2020 09:34:32 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef207bf80aefb18eba12c119d07499e37b5ea7bec06bc1e0c2dd749ddde45a1`  
		Last Modified: Thu, 23 Apr 2020 09:34:34 GMT  
		Size: 1.3 MB (1305489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae62dd92cc34f4856c15b7614910c5578f2d91d96d96469c21f8ca741c1061f5`  
		Last Modified: Thu, 23 Apr 2020 09:35:08 GMT  
		Size: 7.7 MB (7661872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693fe2f4d6e93636c838f7fb3a49c859d72138e5a25fd1687e590fcf3bb74dfb`  
		Last Modified: Thu, 23 Apr 2020 09:35:00 GMT  
		Size: 99.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:153c8eb8631e42a4705a53461aeb1c1edea4a60ad71a759b5eafeccbf3f5c142`  
		Last Modified: Thu, 23 Apr 2020 09:35:00 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:latest` - linux; ppc64le

```console
$ docker pull redis@sha256:e1c410783ee0d501a9804b3050db559054e95e91bb3cd8f3e81324baef92f730
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.7 MB (39696544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34098209a59e39ee25eeb2b0bf53ba98f873314c75110d6841a0793d5e1bc182`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:36:00 GMT
ADD file:5b3c3d2945800e1743dc02a4f68bd830fe2f67ca437223692eb460147c158c2b in / 
# Thu, 23 Apr 2020 00:36:04 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 17:29:48 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 17:29:51 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 17:31:38 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 17:35:14 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 17:35:18 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 17:35:23 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 17:38:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 17:38:25 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 17:38:28 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 17:38:32 GMT
WORKDIR /data
# Thu, 23 Apr 2020 17:38:34 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 17:38:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 17:38:42 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 17:38:45 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:012c6cdbd1af202bbfbea5945fafbb9aca9097f1fa3cb493a29155fdc02cc43c`  
		Last Modified: Thu, 23 Apr 2020 00:50:14 GMT  
		Size: 30.5 MB (30524638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee5a34bf53dadebb7466557f439affba6f1c11ddbdd7d2c1376f9540c294a7a`  
		Last Modified: Thu, 23 Apr 2020 17:42:03 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dedf97e3c0bcb476732135fc70dee2ba4766ff50ec51f93b1929ebaa6c4863f`  
		Last Modified: Thu, 23 Apr 2020 17:42:03 GMT  
		Size: 1.3 MB (1335327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2a1294a7da3aa34af8f45c22665913b8780fcf4dec6b52b108541e496dd0cc`  
		Last Modified: Thu, 23 Apr 2020 17:42:27 GMT  
		Size: 7.8 MB (7834296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51726f5fc1a7b6d031cad4d822aaf6c1801262570fb662454f1f2dc93cd4e551`  
		Last Modified: Thu, 23 Apr 2020 17:42:25 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e62728fce47996c1059a9f4f18e5e1efea4ebc55e17f82aa362f8985e7f019e`  
		Last Modified: Thu, 23 Apr 2020 17:42:25 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:latest` - linux; s390x

```console
$ docker pull redis@sha256:80a22e71a515d761d2c50a5873fc228fe165a627f9f91641391ce1548bc23f03
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34709447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5556ba73cac9fdc7f38ea53f8961a08497e52b1fa62f83611a9228a5d495e8fb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Apr 2020 00:51:48 GMT
ADD file:f6c2560f9185c1bcaff95e576e57449f606d51b85fad02646c1b0962bc9353c9 in / 
# Thu, 23 Apr 2020 00:51:50 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 06:58:44 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Apr 2020 06:58:44 GMT
ENV GOSU_VERSION=1.12
# Thu, 23 Apr 2020 06:58:58 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Apr 2020 06:59:46 GMT
ENV REDIS_VERSION=5.0.9
# Thu, 23 Apr 2020 06:59:47 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.9.tar.gz
# Thu, 23 Apr 2020 06:59:47 GMT
ENV REDIS_DOWNLOAD_SHA=53d0ae164cd33536c3d4b720ae9a128ea6166ebf04ff1add3b85f1242090cb85
# Thu, 23 Apr 2020 07:00:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Apr 2020 07:00:24 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Apr 2020 07:00:24 GMT
VOLUME [/data]
# Thu, 23 Apr 2020 07:00:24 GMT
WORKDIR /data
# Thu, 23 Apr 2020 07:00:24 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 23 Apr 2020 07:00:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 07:00:25 GMT
EXPOSE 6379
# Thu, 23 Apr 2020 07:00:25 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:d89dc3741ad42b79c3d8545495c429f3100d3f22234ff993bd04017b0675e868`  
		Last Modified: Thu, 23 Apr 2020 00:56:00 GMT  
		Size: 25.7 MB (25712105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c9894c70b29dc7cbad7e69c5f898b0a5d6f82aac9aff00e2645a6f8a9eff88`  
		Last Modified: Thu, 23 Apr 2020 07:01:34 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fba24ca231c607425b0e92a8a39c3174a8b9cb56ddeee71fc43f2f9dd9b1d2c`  
		Last Modified: Thu, 23 Apr 2020 07:01:35 GMT  
		Size: 1.4 MB (1403679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22d299e81a09eaaf9da803a2b3775444f312a34b2b7dd8e0c1c10d0171225ba`  
		Last Modified: Thu, 23 Apr 2020 07:01:52 GMT  
		Size: 7.6 MB (7591385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46db2cefe8baf230709535dd5f96c93520ca156d9821649ce8e8a2410e49d54`  
		Last Modified: Thu, 23 Apr 2020 07:01:56 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ec0a42c81dfec4356c31366a6ddf246ebac63394fafd37549a4483fd537513`  
		Last Modified: Thu, 23 Apr 2020 07:01:50 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
