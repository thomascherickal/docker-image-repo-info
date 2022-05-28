## `redis:5-bullseye`

```console
$ docker pull redis@sha256:7fcdf0623b66f849b2b32167497c0a56041ddc4d36d30eeb16fea0c48323833f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `redis:5-bullseye` - linux; amd64

```console
$ docker pull redis@sha256:be0086e1cc355d2cde5f1a841e900cf8d28b2e8ac1ef5541be901e024c8dd5fe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.1 MB (40063257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a2f426e5487587d5a8dbc4bfa36b62ffda7a8cf71dd56452c13efc914d4a048`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Sat, 28 May 2022 01:20:23 GMT
ADD file:134f25aec8adf83cb940ba073a3409ca85dbb5ae592b704f95193e7d2539a3bc in / 
# Sat, 28 May 2022 01:20:23 GMT
CMD ["bash"]
# Sat, 28 May 2022 10:24:16 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Sat, 28 May 2022 10:24:16 GMT
ENV GOSU_VERSION=1.14
# Sat, 28 May 2022 10:24:28 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 28 May 2022 10:27:08 GMT
ENV REDIS_VERSION=5.0.14
# Sat, 28 May 2022 10:27:08 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.14.tar.gz
# Sat, 28 May 2022 10:27:09 GMT
ENV REDIS_DOWNLOAD_SHA=3ea5024766d983249e80d4aa9457c897a9f079957d0fb1f35682df233f997f32
# Sat, 28 May 2022 10:27:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Sat, 28 May 2022 10:27:48 GMT
RUN mkdir /data && chown redis:redis /data
# Sat, 28 May 2022 10:27:48 GMT
VOLUME [/data]
# Sat, 28 May 2022 10:27:48 GMT
WORKDIR /data
# Sat, 28 May 2022 10:27:48 GMT
COPY file:e873a0e3c13001b5e1c63f9dbe60cc65722af522671787f68b8e8cbcae7d02ac in /usr/local/bin/ 
# Sat, 28 May 2022 10:27:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 May 2022 10:27:48 GMT
EXPOSE 6379
# Sat, 28 May 2022 10:27:48 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:42c077c10790d51b6f75c4eb895cbd4da37558f7215b39cbf64c46b288f89bda`  
		Last Modified: Sat, 28 May 2022 01:25:19 GMT  
		Size: 31.4 MB (31379276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a300d83d65f9ddbf212f8637519a3051af28b8a71cb00db39e8302a7364d6c84`  
		Last Modified: Sat, 28 May 2022 10:29:42 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebdc3afaab5c7bf3a715bb82b1d0c377481b5dadc730c0cc8e33d79fa96663d1`  
		Last Modified: Sat, 28 May 2022 10:29:42 GMT  
		Size: 1.4 MB (1410506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d7ea7a1bd58f32ff222d24bbabe219f3eb802909fb1501474497c0ecd3354f9`  
		Last Modified: Sat, 28 May 2022 10:30:54 GMT  
		Size: 7.3 MB (7271035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427d81a8697ded4110e79289cba595cd26d4047cd588f4074843063fc996606c`  
		Last Modified: Sat, 28 May 2022 10:30:52 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aea92facfe439968987e2c6981b5b2dcf4a98f93f4c102dcd692e51384800ba`  
		Last Modified: Sat, 28 May 2022 10:30:52 GMT  
		Size: 573.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-bullseye` - linux; arm variant v5

```console
$ docker pull redis@sha256:7db151329dd336b48ca1db9432a777a636885caacdfec0ea01b074e02f417a7b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37444321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a03e97408250885d9cafe7f38fd923671b760a4ca856d2a743b56e3b1619ade`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 11 May 2022 00:50:34 GMT
ADD file:72357b75d7e4546f06abf4648ab600980e742a3017f36da3c7a6c086f2f5fb56 in / 
# Wed, 11 May 2022 00:50:35 GMT
CMD ["bash"]
# Wed, 11 May 2022 19:46:45 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Wed, 11 May 2022 19:46:46 GMT
ENV GOSU_VERSION=1.14
# Wed, 11 May 2022 19:47:17 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 11 May 2022 19:53:38 GMT
ENV REDIS_VERSION=5.0.14
# Wed, 11 May 2022 19:53:38 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.14.tar.gz
# Wed, 11 May 2022 19:53:39 GMT
ENV REDIS_DOWNLOAD_SHA=3ea5024766d983249e80d4aa9457c897a9f079957d0fb1f35682df233f997f32
# Wed, 11 May 2022 19:55:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Wed, 11 May 2022 19:55:16 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 11 May 2022 19:55:16 GMT
VOLUME [/data]
# Wed, 11 May 2022 19:55:16 GMT
WORKDIR /data
# Wed, 25 May 2022 19:58:17 GMT
COPY file:e873a0e3c13001b5e1c63f9dbe60cc65722af522671787f68b8e8cbcae7d02ac in /usr/local/bin/ 
# Wed, 25 May 2022 19:58:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 25 May 2022 19:58:18 GMT
EXPOSE 6379
# Wed, 25 May 2022 19:58:18 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:f7b69be15db1cb94a249f74b27edd4f5e5923a8701b026179a593f6888e897aa`  
		Last Modified: Wed, 11 May 2022 01:05:51 GMT  
		Size: 28.9 MB (28921122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5466156c2b85e88038d92e399f37a9b91910bfb316d7232245bc762f8edf43`  
		Last Modified: Wed, 11 May 2022 19:57:11 GMT  
		Size: 1.7 KB (1720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96adc949b6bbca33e6fa94eada8a99b625b4cb0cc2f23f373a5cc63e63c4ae4c`  
		Last Modified: Wed, 11 May 2022 19:57:12 GMT  
		Size: 1.4 MB (1374987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a1650f2387e4360c7497664e4241ada9a06322a0d97d2e5a9d97c0727ad3f45`  
		Last Modified: Wed, 11 May 2022 19:58:54 GMT  
		Size: 7.1 MB (7145784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92fb59813fab07fe9cbc6b89bd280107bdc95d8fc351d067696848f9073ebee`  
		Last Modified: Wed, 11 May 2022 19:58:50 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:778692573ea2054ae908eed2a7e18fe14e41147e3bb7c612ce6ccde53b4b431c`  
		Last Modified: Wed, 25 May 2022 20:01:32 GMT  
		Size: 575.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-bullseye` - linux; arm variant v7

```console
$ docker pull redis@sha256:35dbff4e0e1fa1ae16dc3dc82e49288745ebd7e3e912e3a5839b1f7a4342ad43
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.0 MB (34954619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38a8e1e8e1e91f835293a753daf4845986125529198577ef730ee4483f841c3d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 11 May 2022 01:49:07 GMT
ADD file:7c0451fffe8a520c2ab23048948d76bfe0dc0d90298c3d859279ccd8815b84f6 in / 
# Wed, 11 May 2022 01:49:08 GMT
CMD ["bash"]
# Thu, 12 May 2022 07:50:29 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 12 May 2022 07:50:29 GMT
ENV GOSU_VERSION=1.14
# Thu, 12 May 2022 07:50:56 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 12 May 2022 07:57:40 GMT
ENV REDIS_VERSION=5.0.14
# Thu, 12 May 2022 07:57:40 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.14.tar.gz
# Thu, 12 May 2022 07:57:41 GMT
ENV REDIS_DOWNLOAD_SHA=3ea5024766d983249e80d4aa9457c897a9f079957d0fb1f35682df233f997f32
# Thu, 12 May 2022 07:59:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 12 May 2022 07:59:13 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 12 May 2022 07:59:13 GMT
VOLUME [/data]
# Thu, 12 May 2022 07:59:14 GMT
WORKDIR /data
# Thu, 26 May 2022 01:12:03 GMT
COPY file:e873a0e3c13001b5e1c63f9dbe60cc65722af522671787f68b8e8cbcae7d02ac in /usr/local/bin/ 
# Thu, 26 May 2022 01:12:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 May 2022 01:12:04 GMT
EXPOSE 6379
# Thu, 26 May 2022 01:12:05 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:1a9427b75b1c1db800cae7a9199bb4e508702e6761b17cc904d21441df43016c`  
		Last Modified: Wed, 11 May 2022 02:04:35 GMT  
		Size: 26.6 MB (26575672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dac6d008127fc184e86a9d2088922f033f20295e811e971170bbddcc30b30c2`  
		Last Modified: Thu, 12 May 2022 08:03:02 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36c4e49ca7f5bcbea97305eec81ce73f3b4020b092bf4799f26cc9d6cfff67bf`  
		Last Modified: Thu, 12 May 2022 08:03:03 GMT  
		Size: 1.4 MB (1367122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a311f3cf0536003533a1320a3d4169ca3a5761856ee35b314ee826936677640`  
		Last Modified: Thu, 12 May 2022 08:05:04 GMT  
		Size: 7.0 MB (7009395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:642e49cf905ad368191946792903e53600b9180c3a1f02978eeb160b19feb57f`  
		Last Modified: Thu, 12 May 2022 08:04:58 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20cfcd877278b3c4e650b38805132137a4605da166e0312d0a1d21ff8226b417`  
		Last Modified: Thu, 26 May 2022 01:20:05 GMT  
		Size: 574.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-bullseye` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:843546b8e365a22a5f92c3c245a27edb816ca32c9b71788cfe0af3a2bf4aeed3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.7 MB (38716875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:617257625d8cb5c7c2987e78927f3164dd95a338c4e8a91a5eed2862b0261b56`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Sat, 28 May 2022 00:40:39 GMT
ADD file:55b4fe3115c684f545e4e4148c93745f12192976a08c37d090fcac708fb709a7 in / 
# Sat, 28 May 2022 00:40:39 GMT
CMD ["bash"]
# Sat, 28 May 2022 09:20:47 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Sat, 28 May 2022 09:20:48 GMT
ENV GOSU_VERSION=1.14
# Sat, 28 May 2022 09:21:03 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 28 May 2022 09:24:58 GMT
ENV REDIS_VERSION=5.0.14
# Sat, 28 May 2022 09:24:59 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.14.tar.gz
# Sat, 28 May 2022 09:25:00 GMT
ENV REDIS_DOWNLOAD_SHA=3ea5024766d983249e80d4aa9457c897a9f079957d0fb1f35682df233f997f32
# Sat, 28 May 2022 09:25:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Sat, 28 May 2022 09:25:47 GMT
RUN mkdir /data && chown redis:redis /data
# Sat, 28 May 2022 09:25:48 GMT
VOLUME [/data]
# Sat, 28 May 2022 09:25:49 GMT
WORKDIR /data
# Sat, 28 May 2022 09:25:51 GMT
COPY file:e873a0e3c13001b5e1c63f9dbe60cc65722af522671787f68b8e8cbcae7d02ac in /usr/local/bin/ 
# Sat, 28 May 2022 09:25:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 May 2022 09:25:52 GMT
EXPOSE 6379
# Sat, 28 May 2022 09:25:53 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:dc1f00a5d701e86e2cd2568b860c61b393d66be1341e7267d07e6e57448ceeba`  
		Last Modified: Sat, 28 May 2022 00:47:35 GMT  
		Size: 30.1 MB (30065728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:644966968c49d4337c5807689ca7ea34a776a3cfc3a0e5c1f1036239e6025933`  
		Last Modified: Sat, 28 May 2022 09:27:30 GMT  
		Size: 1.6 KB (1615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac7fabd20a4d9012dd67a09907c6c3374ea44996cafab9c2c162f7d21b3396f`  
		Last Modified: Sat, 28 May 2022 09:27:30 GMT  
		Size: 1.3 MB (1337478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370805dcd7a62914d25bc6e4967876e7175fd50d8d909b2783ff455b6a7440b4`  
		Last Modified: Sat, 28 May 2022 09:29:00 GMT  
		Size: 7.3 MB (7311381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef8000a6cbea70e038191bb768b2eb943f93c1cc8cd34c4dbb2b57d2f57f8a1`  
		Last Modified: Sat, 28 May 2022 09:28:58 GMT  
		Size: 98.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28980b04ae6292a9eb3674696ac38f9342dbdaa16f9e1aa1c86f953c0de0822d`  
		Last Modified: Sat, 28 May 2022 09:28:58 GMT  
		Size: 575.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-bullseye` - linux; 386

```console
$ docker pull redis@sha256:f9f224b10b66e9a97aca14ccebe118e48bb479f5cca5d7d82ca88bf86550060a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.8 MB (40759465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04c2499b22fd8acff5672c43acfd5549259e8c72fe9c6e373df9dde1291112a4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Sat, 28 May 2022 00:39:33 GMT
ADD file:8320d7b95b9f68313e086faff974bb38977e0c9da4984afb6382eb0405742bde in / 
# Sat, 28 May 2022 00:39:33 GMT
CMD ["bash"]
# Sat, 28 May 2022 12:45:21 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Sat, 28 May 2022 12:45:22 GMT
ENV GOSU_VERSION=1.14
# Sat, 28 May 2022 12:45:34 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 28 May 2022 12:49:08 GMT
ENV REDIS_VERSION=5.0.14
# Sat, 28 May 2022 12:49:09 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.14.tar.gz
# Sat, 28 May 2022 12:49:10 GMT
ENV REDIS_DOWNLOAD_SHA=3ea5024766d983249e80d4aa9457c897a9f079957d0fb1f35682df233f997f32
# Sat, 28 May 2022 12:49:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Sat, 28 May 2022 12:49:51 GMT
RUN mkdir /data && chown redis:redis /data
# Sat, 28 May 2022 12:49:52 GMT
VOLUME [/data]
# Sat, 28 May 2022 12:49:53 GMT
WORKDIR /data
# Sat, 28 May 2022 12:49:55 GMT
COPY file:e873a0e3c13001b5e1c63f9dbe60cc65722af522671787f68b8e8cbcae7d02ac in /usr/local/bin/ 
# Sat, 28 May 2022 12:49:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 May 2022 12:49:56 GMT
EXPOSE 6379
# Sat, 28 May 2022 12:49:57 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:5e7494d2ee6c81c73ce32f8bde3ea8658c6224c2cc22d7bb01df4bc3d42949aa`  
		Last Modified: Sat, 28 May 2022 00:46:43 GMT  
		Size: 32.4 MB (32390321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1cf01a868a191abbc1b57ad4cc6a523879c1ef27c79618925c27d71ada5e0f7`  
		Last Modified: Sat, 28 May 2022 12:51:46 GMT  
		Size: 1.6 KB (1609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8535046eb1bb55aded7aebc5e3303b59dc978adc8141eeb50968271659a9097f`  
		Last Modified: Sat, 28 May 2022 12:51:47 GMT  
		Size: 1.4 MB (1376861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f19b75b1d0cbf421befc16a825c041de898b94b79857c5a2b90ad9fb8187b61`  
		Last Modified: Sat, 28 May 2022 12:53:17 GMT  
		Size: 7.0 MB (6990003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4c3a24245e63246f61c480130889b871846b64d861335b78c9667a66f3c15e`  
		Last Modified: Sat, 28 May 2022 12:53:16 GMT  
		Size: 98.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b7c140ca66d7bd83fc7ba774ddb19333c1f879601b97772e2ca5d05a4b25200`  
		Last Modified: Sat, 28 May 2022 12:53:16 GMT  
		Size: 573.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-bullseye` - linux; mips64le

```console
$ docker pull redis@sha256:8ef31f18ae1cd431069beabd25333289b1f28eb1990e05b20e36a607e854683a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.6 MB (38572289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f764a2c2d57fae55b6fc67bad4a76839236a5cf77cd5fc064d729546eb11d3d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Sat, 28 May 2022 01:11:13 GMT
ADD file:f685a156b7ddafe7bafc6fad17cc36cc8a5d6d922fc1c425656ca92266d9a98e in / 
# Sat, 28 May 2022 01:11:18 GMT
CMD ["bash"]
# Sat, 28 May 2022 11:05:18 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Sat, 28 May 2022 11:05:21 GMT
ENV GOSU_VERSION=1.14
# Sat, 28 May 2022 11:06:20 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 28 May 2022 11:20:41 GMT
ENV REDIS_VERSION=5.0.14
# Sat, 28 May 2022 11:20:44 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.14.tar.gz
# Sat, 28 May 2022 11:20:46 GMT
ENV REDIS_DOWNLOAD_SHA=3ea5024766d983249e80d4aa9457c897a9f079957d0fb1f35682df233f997f32
# Sat, 28 May 2022 11:24:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Sat, 28 May 2022 11:24:34 GMT
RUN mkdir /data && chown redis:redis /data
# Sat, 28 May 2022 11:24:37 GMT
VOLUME [/data]
# Sat, 28 May 2022 11:24:40 GMT
WORKDIR /data
# Sat, 28 May 2022 11:24:42 GMT
COPY file:e873a0e3c13001b5e1c63f9dbe60cc65722af522671787f68b8e8cbcae7d02ac in /usr/local/bin/ 
# Sat, 28 May 2022 11:24:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 May 2022 11:24:47 GMT
EXPOSE 6379
# Sat, 28 May 2022 11:24:50 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:fdea7139ce36b557a23c4b9c4255387b175f851ed0c51e1e7d78dd301c0e4da8`  
		Last Modified: Sat, 28 May 2022 01:21:35 GMT  
		Size: 29.6 MB (29641237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e112addd87990e7f2b6c80e25c9274f16fb5367a68a4253946b9e87fc0459c1f`  
		Last Modified: Sat, 28 May 2022 11:25:16 GMT  
		Size: 1.6 KB (1615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708ca3cbb4ee0b9c9dce2baf239d2f414a8ddd5bc063a4c0c8729b8d4cd2e0d2`  
		Last Modified: Sat, 28 May 2022 11:25:17 GMT  
		Size: 1.3 MB (1290094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3b5bdadf01705f6c5ab661873bcc04f7bd070aa5abaf83dba0ab56b395ba7c`  
		Last Modified: Sat, 28 May 2022 11:26:42 GMT  
		Size: 7.6 MB (7638671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81a59a0c91d66733bc19c49220e20a30639636996e6bef04492a9d0ea037ffdf`  
		Last Modified: Sat, 28 May 2022 11:26:36 GMT  
		Size: 98.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47c58bece981465bf615d46a3a093e3ea6d70b736cd181d9c0ce3f06ade5236e`  
		Last Modified: Sat, 28 May 2022 11:26:36 GMT  
		Size: 574.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-bullseye` - linux; ppc64le

```console
$ docker pull redis@sha256:bd5d637422db054b97a9a87cd25bda05ddb16db386ea4064955420f1f9fb42a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.4 MB (44399404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:483553ff6d1cd9319d4a488fdcf78c607f95b8c2cec81b65729143ac4b7fbe80`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 11 May 2022 01:32:29 GMT
ADD file:1e94716789ec21981460f74be38a668bc212bd804c1d41cecf90036a5bccac5a in / 
# Wed, 11 May 2022 01:32:34 GMT
CMD ["bash"]
# Thu, 12 May 2022 04:18:43 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 12 May 2022 04:18:47 GMT
ENV GOSU_VERSION=1.14
# Thu, 12 May 2022 04:20:04 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 12 May 2022 04:34:14 GMT
ENV REDIS_VERSION=5.0.14
# Thu, 12 May 2022 04:34:26 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.14.tar.gz
# Thu, 12 May 2022 04:34:36 GMT
ENV REDIS_DOWNLOAD_SHA=3ea5024766d983249e80d4aa9457c897a9f079957d0fb1f35682df233f997f32
# Thu, 12 May 2022 04:39:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 12 May 2022 04:40:28 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 12 May 2022 04:40:35 GMT
VOLUME [/data]
# Thu, 12 May 2022 04:40:41 GMT
WORKDIR /data
# Thu, 26 May 2022 00:29:41 GMT
COPY file:e873a0e3c13001b5e1c63f9dbe60cc65722af522671787f68b8e8cbcae7d02ac in /usr/local/bin/ 
# Thu, 26 May 2022 00:29:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 May 2022 00:30:01 GMT
EXPOSE 6379
# Thu, 26 May 2022 00:30:09 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:2533109ed11eefd6415e0370d6d7a3ea879b582b1887c98b819a598ad18fca24`  
		Last Modified: Wed, 11 May 2022 01:43:03 GMT  
		Size: 35.3 MB (35286467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98667dd2bfcca5e372307098345b6519ac14fe1d2fcd1a7690292f460f361b2`  
		Last Modified: Thu, 12 May 2022 04:43:23 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0818e0351b73df132bc91c7c3336d26a374f359b935d2268892ffba492714f28`  
		Last Modified: Thu, 12 May 2022 04:43:24 GMT  
		Size: 1.3 MB (1309312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8fc5652b76f056f9213d11d689a28a93e74b538d9bb70e2bab174ba86625f41`  
		Last Modified: Thu, 12 May 2022 04:45:16 GMT  
		Size: 7.8 MB (7801181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09af9b45b39b605cd07e19d6cb44e8c7b534c2f35ed5450a7c7d4e151a0fdbae`  
		Last Modified: Thu, 12 May 2022 04:45:15 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c91b9481f6c708bf73417346220661c1d6059a7f56ef012e64c55aa944055c55`  
		Last Modified: Thu, 26 May 2022 00:37:30 GMT  
		Size: 574.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-bullseye` - linux; s390x

```console
$ docker pull redis@sha256:9e8155ed2e8cf2058116eaf328ec6e8e49c47bc696434a9c10088d9cd4a42baa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.6 MB (38638827 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7ce107dd27379623764b3c601fe2b3d02048014d935272b4546c61f71ddf19b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Sat, 28 May 2022 00:43:00 GMT
ADD file:95dc6dcd4ebd15b42beaf935d91adafb0ea44a443bb44597bc1ff236e831ce18 in / 
# Sat, 28 May 2022 00:43:03 GMT
CMD ["bash"]
# Sat, 28 May 2022 14:14:08 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Sat, 28 May 2022 14:14:09 GMT
ENV GOSU_VERSION=1.14
# Sat, 28 May 2022 14:14:31 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Sat, 28 May 2022 14:20:08 GMT
ENV REDIS_VERSION=5.0.14
# Sat, 28 May 2022 14:20:08 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.14.tar.gz
# Sat, 28 May 2022 14:20:09 GMT
ENV REDIS_DOWNLOAD_SHA=3ea5024766d983249e80d4aa9457c897a9f079957d0fb1f35682df233f997f32
# Sat, 28 May 2022 14:21:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Sat, 28 May 2022 14:21:32 GMT
RUN mkdir /data && chown redis:redis /data
# Sat, 28 May 2022 14:21:32 GMT
VOLUME [/data]
# Sat, 28 May 2022 14:21:33 GMT
WORKDIR /data
# Sat, 28 May 2022 14:21:34 GMT
COPY file:e873a0e3c13001b5e1c63f9dbe60cc65722af522671787f68b8e8cbcae7d02ac in /usr/local/bin/ 
# Sat, 28 May 2022 14:21:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 28 May 2022 14:21:35 GMT
EXPOSE 6379
# Sat, 28 May 2022 14:21:35 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:f7bb6d2d11c3060ba2e66ba762e2aa10a0d1d361cfa6a806bcf26a64cc3a79aa`  
		Last Modified: Sat, 28 May 2022 00:49:46 GMT  
		Size: 29.7 MB (29655258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1006c23c1810b6410c9264b1b7e63550deb844d19b08a3254cf85cdec57de17`  
		Last Modified: Sat, 28 May 2022 14:23:43 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963216691f999de14ff9fa93b595482661e321b0bc3a95730b4c1b66367e2dc0`  
		Last Modified: Sat, 28 May 2022 14:23:43 GMT  
		Size: 1.4 MB (1373794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea9562f0b036e4786cb471b73314e77d27ca4bf0c3b3d10c3e8e18c67aa07c2e`  
		Last Modified: Sat, 28 May 2022 14:25:01 GMT  
		Size: 7.6 MB (7607328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96422def04b8776d3a5148527e8bfc8227af21dcb6cd36382301b8c09505ba6b`  
		Last Modified: Sat, 28 May 2022 14:25:00 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0bc938179c63e86cd83502c531a09148b2608ebea917757ff911ae8c7f99404`  
		Last Modified: Sat, 28 May 2022 14:25:00 GMT  
		Size: 574.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
