## `redis:latest`

```console
$ docker pull redis@sha256:33a3ee82f1195880b41045d5dab65ebdd61c32d5c0e482392eaa88399eb7a4f2
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

### `redis:latest` - linux; amd64

```console
$ docker pull redis@sha256:31120dcdd310e9a65cbcadd504f4fe60a185bd634ab7c6a35e3e44a941904d97
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.3 MB (42341215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e50d70ba706ed644d475612b998641687dfb2415016b803ca3eb811c7096714`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Jun 2022 00:20:27 GMT
ADD file:8adbbab04d6f84cd83b5f4205b89b0acb7ecbf27a1bb2dc181d0a629479039fe in / 
# Thu, 23 Jun 2022 00:20:27 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 12:29:37 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Jun 2022 12:29:37 GMT
ENV GOSU_VERSION=1.14
# Thu, 23 Jun 2022 12:29:49 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Jun 2022 12:29:49 GMT
ENV REDIS_VERSION=7.0.2
# Thu, 23 Jun 2022 12:29:49 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.0.2.tar.gz
# Thu, 23 Jun 2022 12:29:49 GMT
ENV REDIS_DOWNLOAD_SHA=5e57eafe7d4ac5ecb6a7d64d6b61db775616dbf903293b3fcc660716dbda5eeb
# Thu, 23 Jun 2022 12:30:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Jun 2022 12:30:35 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Jun 2022 12:30:35 GMT
VOLUME [/data]
# Thu, 23 Jun 2022 12:30:35 GMT
WORKDIR /data
# Thu, 23 Jun 2022 12:30:35 GMT
COPY file:e873a0e3c13001b5e1c63f9dbe60cc65722af522671787f68b8e8cbcae7d02ac in /usr/local/bin/ 
# Thu, 23 Jun 2022 12:30:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 12:30:35 GMT
EXPOSE 6379
# Thu, 23 Jun 2022 12:30:35 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:b85a868b505ffd0342a37e6a3b1c49f7c71878afe569a807e6238ef08252fcb7`  
		Last Modified: Thu, 23 Jun 2022 00:25:18 GMT  
		Size: 31.4 MB (31379408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b09642bd3b882657a3d239f48a3f44f0c07e7776a243a575b93504f1f9b49a43`  
		Last Modified: Thu, 23 Jun 2022 12:35:04 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0678a951c8d72b1b826c6d76742580957d64c02081823e69b104971e8c65dcf`  
		Last Modified: Thu, 23 Jun 2022 12:35:04 GMT  
		Size: 1.4 MB (1410505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d7c0a1681bceddc89c27f660ace9c824dd5591fff81cf3bfd1603d7bb50d15`  
		Last Modified: Thu, 23 Jun 2022 12:35:06 GMT  
		Size: 9.5 MB (9548860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:954286b64dd1be62e03bc13e93fb8d477476e40a0b076bf4c1f9712caf20b9e8`  
		Last Modified: Thu, 23 Jun 2022 12:35:04 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58024fcab1ef56e1c0d86a80b3abeab24bf1c6042573eab7645eb11e16ccdca8`  
		Last Modified: Thu, 23 Jun 2022 12:35:04 GMT  
		Size: 576.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:latest` - linux; arm variant v5

```console
$ docker pull redis@sha256:0effbd8beeb5c2cde2ab089f14054afeb97fa84e3c83d2c1b43ec1360bcedeb8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.7 MB (39658804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b79e1ae4f6808223337f9990439da8ac7e3e456bbaf7b941e03220caffbec9ad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Jun 2022 00:50:38 GMT
ADD file:839c0e211e2260f5d54f2633e53c817c1f59e2394ba4b12f60e01e46cee61011 in / 
# Thu, 23 Jun 2022 00:50:39 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 21:44:44 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Jun 2022 21:44:44 GMT
ENV GOSU_VERSION=1.14
# Thu, 23 Jun 2022 21:45:17 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Jun 2022 21:45:17 GMT
ENV REDIS_VERSION=7.0.2
# Thu, 23 Jun 2022 21:45:18 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.0.2.tar.gz
# Thu, 23 Jun 2022 21:45:18 GMT
ENV REDIS_DOWNLOAD_SHA=5e57eafe7d4ac5ecb6a7d64d6b61db775616dbf903293b3fcc660716dbda5eeb
# Thu, 23 Jun 2022 21:47:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Jun 2022 21:47:08 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Jun 2022 21:47:09 GMT
VOLUME [/data]
# Thu, 23 Jun 2022 21:47:09 GMT
WORKDIR /data
# Thu, 23 Jun 2022 21:47:10 GMT
COPY file:e873a0e3c13001b5e1c63f9dbe60cc65722af522671787f68b8e8cbcae7d02ac in /usr/local/bin/ 
# Thu, 23 Jun 2022 21:47:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 21:47:11 GMT
EXPOSE 6379
# Thu, 23 Jun 2022 21:47:11 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:bd2d3b4056bd1b0310082fc5d17c6d03348601456c4b9306d1a333f1cec561f9`  
		Last Modified: Thu, 23 Jun 2022 01:05:39 GMT  
		Size: 28.9 MB (28921550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:744ed6e4eefd8d14a725eca47a69be16c0bb981c11485d8b427a47b4e0bea174`  
		Last Modified: Thu, 23 Jun 2022 21:55:16 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72536b3724733ce3035a9f3143293ad30d9cd95dc66ee3878825bcb7087e735d`  
		Last Modified: Thu, 23 Jun 2022 21:55:17 GMT  
		Size: 1.4 MB (1374977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec82a311804ae2e3cbff2a0dc04e8c76b76cb30b46718afc838fba610c5847e6`  
		Last Modified: Thu, 23 Jun 2022 21:55:22 GMT  
		Size: 9.4 MB (9359842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfaab956b276c0fb24dddb96792eb0d7cc40354cab2e67adc29751dec6f6483c`  
		Last Modified: Thu, 23 Jun 2022 21:55:16 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df2cdc34c0e2674433a692dd53c3081b8fb6e3fbde2f42833faaaa448ebd39d0`  
		Last Modified: Thu, 23 Jun 2022 21:55:16 GMT  
		Size: 576.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:latest` - linux; arm variant v7

```console
$ docker pull redis@sha256:910ec5a26bbeb54969d899aadc375ab57375f40447e918d284f0f6d2f08bd9e5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.1 MB (37136624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d614431061819f793770e9c4cec51750a46ab1de36fe867fb66dbbb04883ceda`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Jun 2022 00:59:45 GMT
ADD file:925abfb9fc0e4a7cc0c979b12c9bd2607f5c493d37b05535ca010f81beb060a9 in / 
# Thu, 23 Jun 2022 00:59:46 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 20:58:26 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Jun 2022 20:58:27 GMT
ENV GOSU_VERSION=1.14
# Thu, 23 Jun 2022 20:58:55 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Jun 2022 20:58:56 GMT
ENV REDIS_VERSION=7.0.2
# Thu, 23 Jun 2022 20:58:56 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.0.2.tar.gz
# Thu, 23 Jun 2022 20:58:57 GMT
ENV REDIS_DOWNLOAD_SHA=5e57eafe7d4ac5ecb6a7d64d6b61db775616dbf903293b3fcc660716dbda5eeb
# Thu, 23 Jun 2022 21:00:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Jun 2022 21:00:41 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Jun 2022 21:00:41 GMT
VOLUME [/data]
# Thu, 23 Jun 2022 21:00:42 GMT
WORKDIR /data
# Thu, 23 Jun 2022 21:00:42 GMT
COPY file:e873a0e3c13001b5e1c63f9dbe60cc65722af522671787f68b8e8cbcae7d02ac in /usr/local/bin/ 
# Thu, 23 Jun 2022 21:00:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 21:00:43 GMT
EXPOSE 6379
# Thu, 23 Jun 2022 21:00:44 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:d2fd562560d8062a78064adfbfa204521167c301f00f5ab3c65b9c2a54083dba`  
		Last Modified: Thu, 23 Jun 2022 01:15:22 GMT  
		Size: 26.6 MB (26576105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f40d6df1afe346571ebb704f64d8e6b5b1b72c906d2b985898af7a6233006d`  
		Last Modified: Thu, 23 Jun 2022 21:10:50 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:555e67427156c528457bf93998c1d0aa3f51c9943a873499be87b247550ceab8`  
		Last Modified: Thu, 23 Jun 2022 21:10:51 GMT  
		Size: 1.4 MB (1367145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3659849ac691b6dcf4635a141ebd40a137e611065e0c1089184a02774b5a93ce`  
		Last Modified: Thu, 23 Jun 2022 21:10:56 GMT  
		Size: 9.2 MB (9190942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a468b05f1334b6f8df0bbdf4015ae5ba5e83abef3e26e24059a263fbafa9110`  
		Last Modified: Thu, 23 Jun 2022 21:10:50 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a17b8836d44a9aeaa383d5a89e5b7bb0701cfc20d3bc74345a75f611a37d403`  
		Last Modified: Thu, 23 Jun 2022 21:10:50 GMT  
		Size: 575.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:latest` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:4b379f9db17105ee6eb8518b2597a65f581bc8f304d657ac321379d643ff42bd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.0 MB (40977325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24f9f41dd1142539fa642e8f8c7da10fe00e15b0c023b45ede31b8d0a51d3c05`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Jun 2022 00:40:43 GMT
ADD file:134be48af13f80f3474bf1b080ca781feb7b972148d482849862e55eb2acd61c in / 
# Thu, 23 Jun 2022 00:40:44 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 09:58:16 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Jun 2022 09:58:16 GMT
ENV GOSU_VERSION=1.14
# Thu, 23 Jun 2022 09:58:28 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Jun 2022 09:58:29 GMT
ENV REDIS_VERSION=7.0.2
# Thu, 23 Jun 2022 09:58:30 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.0.2.tar.gz
# Thu, 23 Jun 2022 09:58:31 GMT
ENV REDIS_DOWNLOAD_SHA=5e57eafe7d4ac5ecb6a7d64d6b61db775616dbf903293b3fcc660716dbda5eeb
# Thu, 23 Jun 2022 09:59:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Jun 2022 09:59:15 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Jun 2022 09:59:16 GMT
VOLUME [/data]
# Thu, 23 Jun 2022 09:59:17 GMT
WORKDIR /data
# Thu, 23 Jun 2022 09:59:19 GMT
COPY file:e873a0e3c13001b5e1c63f9dbe60cc65722af522671787f68b8e8cbcae7d02ac in /usr/local/bin/ 
# Thu, 23 Jun 2022 09:59:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 09:59:20 GMT
EXPOSE 6379
# Thu, 23 Jun 2022 09:59:21 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:3b157c852f2736e12f09046f214fe5f6a0b1652bd860269b3988c92a197026e8`  
		Last Modified: Thu, 23 Jun 2022 00:47:22 GMT  
		Size: 30.1 MB (30065720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b174fe997fdc05b0bc075257797b8f619062206a3e7d3ddc86814d802a42fd89`  
		Last Modified: Thu, 23 Jun 2022 10:04:11 GMT  
		Size: 1.6 KB (1617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f2666c5e5d1a63a82f5f4df7aeb914931cde2e1040d762ee034f1ae1e2f6a7`  
		Last Modified: Thu, 23 Jun 2022 10:04:11 GMT  
		Size: 1.3 MB (1337503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7922f823f8d9e15736a1db18a0fb7564e1485e6e1dc6979b355b3be14529b1bf`  
		Last Modified: Thu, 23 Jun 2022 10:04:13 GMT  
		Size: 9.6 MB (9571811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c5962db7df03e40e834fbcb76627bdced6c9d98cd5e315c3c1ef26d5be4fe6d`  
		Last Modified: Thu, 23 Jun 2022 10:04:11 GMT  
		Size: 99.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b746636ce2c5442e918e57785e7d89e89089963272b18916322864e78869d5b2`  
		Last Modified: Thu, 23 Jun 2022 10:04:11 GMT  
		Size: 575.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:latest` - linux; 386

```console
$ docker pull redis@sha256:9ea0b240729876042adf0d1c3f27c49f0398fdd277a5b20661012c6d1e757d63
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.9 MB (42893782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:268754631e050bf3674e64bf0247c7fa6c928b632a7e1470d254c0909a1dfe0a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Jun 2022 00:39:33 GMT
ADD file:9d46d3f8fb63833a6dbd8dd796ad541d556046a48342d22e1fd3bffa3fb8e504 in / 
# Thu, 23 Jun 2022 00:39:33 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 11:27:14 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Jun 2022 11:27:14 GMT
ENV GOSU_VERSION=1.14
# Thu, 23 Jun 2022 11:27:26 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Jun 2022 11:27:27 GMT
ENV REDIS_VERSION=7.0.2
# Thu, 23 Jun 2022 11:27:28 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.0.2.tar.gz
# Thu, 23 Jun 2022 11:27:29 GMT
ENV REDIS_DOWNLOAD_SHA=5e57eafe7d4ac5ecb6a7d64d6b61db775616dbf903293b3fcc660716dbda5eeb
# Thu, 23 Jun 2022 11:28:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Jun 2022 11:28:16 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Jun 2022 11:28:17 GMT
VOLUME [/data]
# Thu, 23 Jun 2022 11:28:18 GMT
WORKDIR /data
# Thu, 23 Jun 2022 11:28:20 GMT
COPY file:e873a0e3c13001b5e1c63f9dbe60cc65722af522671787f68b8e8cbcae7d02ac in /usr/local/bin/ 
# Thu, 23 Jun 2022 11:28:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 11:28:21 GMT
EXPOSE 6379
# Thu, 23 Jun 2022 11:28:22 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:4870b12e407743816673c11cfb39974d80c1569d876287bef61f8c585954822f`  
		Last Modified: Thu, 23 Jun 2022 00:46:40 GMT  
		Size: 32.4 MB (32390198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e015caf203969918975618f5f17efbaa7378bc9d1b7b0c858a945c3671ad75`  
		Last Modified: Thu, 23 Jun 2022 11:33:36 GMT  
		Size: 1.6 KB (1610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:846e3dc59f910c7ce3d2f1e11c2f93fa8a482b72fdf81180937f411df77dd188`  
		Last Modified: Thu, 23 Jun 2022 11:33:36 GMT  
		Size: 1.4 MB (1376847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22930a0b86fd3a7479def737c7df7d258d003a06e6dd82cd9260c78d3eb89bed`  
		Last Modified: Thu, 23 Jun 2022 11:33:38 GMT  
		Size: 9.1 MB (9124454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb6756d388f7ae7e131b7b29927bc4044c089d982298dc44aabeb4806d48101a`  
		Last Modified: Thu, 23 Jun 2022 11:33:36 GMT  
		Size: 97.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5507f01a9bafb05c23a2138851cf3bf1260ea3b8f0e7ad6a950119e565d5139a`  
		Last Modified: Thu, 23 Jun 2022 11:33:36 GMT  
		Size: 576.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:latest` - linux; mips64le

```console
$ docker pull redis@sha256:4d4dc7bc025d33491b60724790831a71d98552a6bcad4fa395cc33797a435a93
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.7 MB (40691328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44371d034cbdb106d15607c7c2461dbb67d82decdd37b6b5e3051ebd9534fc52`
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
# Mon, 13 Jun 2022 20:39:02 GMT
ENV REDIS_VERSION=7.0.2
# Mon, 13 Jun 2022 20:39:04 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.0.2.tar.gz
# Mon, 13 Jun 2022 20:39:07 GMT
ENV REDIS_DOWNLOAD_SHA=5e57eafe7d4ac5ecb6a7d64d6b61db775616dbf903293b3fcc660716dbda5eeb
# Mon, 13 Jun 2022 20:43:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Mon, 13 Jun 2022 20:43:26 GMT
RUN mkdir /data && chown redis:redis /data
# Mon, 13 Jun 2022 20:43:28 GMT
VOLUME [/data]
# Mon, 13 Jun 2022 20:43:30 GMT
WORKDIR /data
# Mon, 13 Jun 2022 20:43:32 GMT
COPY file:e873a0e3c13001b5e1c63f9dbe60cc65722af522671787f68b8e8cbcae7d02ac in /usr/local/bin/ 
# Mon, 13 Jun 2022 20:43:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 13 Jun 2022 20:43:37 GMT
EXPOSE 6379
# Mon, 13 Jun 2022 20:43:39 GMT
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
	-	`sha256:199140834595679647a45075b5acd4bc0f754a49552a3356fdb3df1ebe2d14ef`  
		Last Modified: Mon, 13 Jun 2022 20:44:20 GMT  
		Size: 9.8 MB (9757709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd0a5b6478b2992eb2b62a01ec2339db067d1e822df31755792a9f9891ca2409`  
		Last Modified: Mon, 13 Jun 2022 20:44:12 GMT  
		Size: 98.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76715553851a3506a38d93741cf59b7c264a32c9f9261abf325d763fad93e881`  
		Last Modified: Mon, 13 Jun 2022 20:44:13 GMT  
		Size: 575.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:latest` - linux; ppc64le

```console
$ docker pull redis@sha256:ffc03159218472e6a667c9a160128953c1493025060de87c16a9846b9c13d15a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46660177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d61a4830bb9d54a286ace137a2e252bb856226773bfe9d8533765e42abaf6b20`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Jun 2022 02:02:32 GMT
ADD file:e18c13649ea1f145047652c8e171c4824f9b6b0dbc92127a914c7fca910acf96 in / 
# Thu, 23 Jun 2022 02:02:34 GMT
CMD ["bash"]
# Fri, 24 Jun 2022 04:00:36 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Fri, 24 Jun 2022 04:00:41 GMT
ENV GOSU_VERSION=1.14
# Fri, 24 Jun 2022 04:02:01 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 24 Jun 2022 04:02:11 GMT
ENV REDIS_VERSION=7.0.2
# Fri, 24 Jun 2022 04:02:17 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.0.2.tar.gz
# Fri, 24 Jun 2022 04:02:19 GMT
ENV REDIS_DOWNLOAD_SHA=5e57eafe7d4ac5ecb6a7d64d6b61db775616dbf903293b3fcc660716dbda5eeb
# Fri, 24 Jun 2022 04:04:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Fri, 24 Jun 2022 04:04:49 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 24 Jun 2022 04:04:51 GMT
VOLUME [/data]
# Fri, 24 Jun 2022 04:04:54 GMT
WORKDIR /data
# Fri, 24 Jun 2022 04:04:57 GMT
COPY file:e873a0e3c13001b5e1c63f9dbe60cc65722af522671787f68b8e8cbcae7d02ac in /usr/local/bin/ 
# Fri, 24 Jun 2022 04:05:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Jun 2022 04:05:03 GMT
EXPOSE 6379
# Fri, 24 Jun 2022 04:05:05 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:7716f0df7ba06b6f1937cd664805984e25e386a4165f2c6acc65356686e35221`  
		Last Modified: Thu, 23 Jun 2022 02:15:20 GMT  
		Size: 35.3 MB (35286823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199dbedb9d84ddec4e3eb1418293a2cf3d961ea08a222c7396633485c11e8d27`  
		Last Modified: Fri, 24 Jun 2022 04:15:56 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2c0ddc41c542322d459d3728d90f76d88fc2911eb076a02cae75430a5ad475`  
		Last Modified: Fri, 24 Jun 2022 04:15:57 GMT  
		Size: 1.3 MB (1309288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56c61bbc7b06ed785f93d1412c53335fcde90dfcb5ab92c316ecc60fbee9e6d5`  
		Last Modified: Fri, 24 Jun 2022 04:15:59 GMT  
		Size: 10.1 MB (10061622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d2d8fb3c2b10cc2562469a241fbdc08950912563c8e0543aec7a69e7e9adb28`  
		Last Modified: Fri, 24 Jun 2022 04:15:56 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30fe015ae059eff01e14915d64bfd1a895d4a6f7b2d667a1be6dcabf0e3a87e3`  
		Last Modified: Fri, 24 Jun 2022 04:15:56 GMT  
		Size: 576.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:latest` - linux; s390x

```console
$ docker pull redis@sha256:7f432c93bf195c80bd938ac16ae15a18b16fb7a4f8bea484d99a54f3c35ed62c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.9 MB (40877652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f5261466d582f4d9e861e626a69f1002ad187045177068346968106cd00284c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 23 Jun 2022 00:43:10 GMT
ADD file:0b511e3efd87267fb27161eae56c4d08f0fed733697da6ffe6ea96a4cb68e938 in / 
# Thu, 23 Jun 2022 00:43:15 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 12:53:36 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 23 Jun 2022 12:53:36 GMT
ENV GOSU_VERSION=1.14
# Thu, 23 Jun 2022 12:53:44 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 23 Jun 2022 12:53:44 GMT
ENV REDIS_VERSION=7.0.2
# Thu, 23 Jun 2022 12:53:44 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.0.2.tar.gz
# Thu, 23 Jun 2022 12:53:44 GMT
ENV REDIS_DOWNLOAD_SHA=5e57eafe7d4ac5ecb6a7d64d6b61db775616dbf903293b3fcc660716dbda5eeb
# Thu, 23 Jun 2022 12:54:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 23 Jun 2022 12:54:25 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 23 Jun 2022 12:54:25 GMT
VOLUME [/data]
# Thu, 23 Jun 2022 12:54:25 GMT
WORKDIR /data
# Thu, 23 Jun 2022 12:54:25 GMT
COPY file:e873a0e3c13001b5e1c63f9dbe60cc65722af522671787f68b8e8cbcae7d02ac in /usr/local/bin/ 
# Thu, 23 Jun 2022 12:54:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jun 2022 12:54:26 GMT
EXPOSE 6379
# Thu, 23 Jun 2022 12:54:26 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:c547f465e0c8708ad0c57cf09caa52f4c2b5b295bf10ab1ce71ca17ff81ea36a`  
		Last Modified: Thu, 23 Jun 2022 00:51:59 GMT  
		Size: 29.7 MB (29655262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c491311d17ad66641274dc510322729b3a3140bebb5258e41d6019e2d75f12`  
		Last Modified: Thu, 23 Jun 2022 12:58:46 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:797c7dee6c60a5e86ca6af23d22527d69ac0a10ecd178d935836f38f2f5344bb`  
		Last Modified: Thu, 23 Jun 2022 12:58:47 GMT  
		Size: 1.4 MB (1373779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa07051ddc9e4fdf137e33d119c4015162c16238af7406faba51ab4b4fc77a9d`  
		Last Modified: Thu, 23 Jun 2022 12:58:48 GMT  
		Size: 9.8 MB (9846168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca8976e01ce73bd9915cf44d97d401509c8a51eff80fd92be7dc79559fea546`  
		Last Modified: Thu, 23 Jun 2022 12:58:46 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42f86cd9f60bd382477477372e66287336d6c075e205025012e9926b7bd1bdd7`  
		Last Modified: Thu, 23 Jun 2022 12:58:46 GMT  
		Size: 576.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
