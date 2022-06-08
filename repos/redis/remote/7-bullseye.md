## `redis:7-bullseye`

```console
$ docker pull redis@sha256:96c5620546f79b323866e7107406d165ec1020f0754b2fe2fc3067938a085841
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

### `redis:7-bullseye` - linux; amd64

```console
$ docker pull redis@sha256:4aa5e272c44555fecb3382234448b84635c069aad8e28e4c76c9d5eeb0078abb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.3 MB (42341257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd8125f93b9452852d35219a6520c73b3b94d75595ffdfe7ddae917dee3f7da7`
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
# Wed, 08 Jun 2022 18:33:53 GMT
ENV REDIS_VERSION=7.0.1
# Wed, 08 Jun 2022 18:33:53 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.0.1.tar.gz
# Wed, 08 Jun 2022 18:33:54 GMT
ENV REDIS_DOWNLOAD_SHA=ca1820d527e4759884620be2917079e61e996fa81da5fbe5c07c4a7b507264dc
# Wed, 08 Jun 2022 18:34:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Wed, 08 Jun 2022 18:34:42 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 08 Jun 2022 18:34:42 GMT
VOLUME [/data]
# Wed, 08 Jun 2022 18:34:42 GMT
WORKDIR /data
# Wed, 08 Jun 2022 18:34:42 GMT
COPY file:e873a0e3c13001b5e1c63f9dbe60cc65722af522671787f68b8e8cbcae7d02ac in /usr/local/bin/ 
# Wed, 08 Jun 2022 18:34:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Jun 2022 18:34:42 GMT
EXPOSE 6379
# Wed, 08 Jun 2022 18:34:43 GMT
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
	-	`sha256:312c02ded1dd38b0a020ec7a3229dea155c74aefb7914ca760be45d95e2dd74a`  
		Last Modified: Wed, 08 Jun 2022 18:36:55 GMT  
		Size: 9.5 MB (9549030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:604377b42ad54f1d75ba31c1a7d503c1a05f4548118d55048a0b1cc3bfeac08b`  
		Last Modified: Wed, 08 Jun 2022 18:36:53 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:994e00ada2d1d136b52f1dd74911002155a587d83910209810d83ae50b1a0b63`  
		Last Modified: Wed, 08 Jun 2022 18:36:53 GMT  
		Size: 577.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:7-bullseye` - linux; arm variant v5

```console
$ docker pull redis@sha256:4c450e0ec34d67c3de3959775e4a112147cda99f45bcbdc76cb6c2603ad3dd5a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.7 MB (39658959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9df507ab6fa91de8996967c09830ef02064c451ed307767c9c57905744dea001`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Sat, 28 May 2022 02:03:06 GMT
ADD file:d9560b279f64bc3973a6aaa0e0ab8f483d60a1c66647899850689eee01a729ec in / 
# Sat, 28 May 2022 02:03:07 GMT
CMD ["bash"]
# Sat, 28 May 2022 18:06:39 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Sat, 28 May 2022 18:06:39 GMT
ENV GOSU_VERSION=1.14
# Sat, 28 May 2022 18:07:11 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 08 Jun 2022 19:06:06 GMT
ENV REDIS_VERSION=7.0.1
# Wed, 08 Jun 2022 19:06:06 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.0.1.tar.gz
# Wed, 08 Jun 2022 19:06:07 GMT
ENV REDIS_DOWNLOAD_SHA=ca1820d527e4759884620be2917079e61e996fa81da5fbe5c07c4a7b507264dc
# Wed, 08 Jun 2022 19:07:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Wed, 08 Jun 2022 19:07:56 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 08 Jun 2022 19:07:56 GMT
VOLUME [/data]
# Wed, 08 Jun 2022 19:07:57 GMT
WORKDIR /data
# Wed, 08 Jun 2022 19:07:57 GMT
COPY file:e873a0e3c13001b5e1c63f9dbe60cc65722af522671787f68b8e8cbcae7d02ac in /usr/local/bin/ 
# Wed, 08 Jun 2022 19:07:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Jun 2022 19:07:58 GMT
EXPOSE 6379
# Wed, 08 Jun 2022 19:07:59 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:b24540c95c3d5b61dba94dfa3665e0cc1231b3602edfb61432041c1f108be50d`  
		Last Modified: Sat, 28 May 2022 02:18:37 GMT  
		Size: 28.9 MB (28921471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8effe7807064ffd874e38d7087b08f6c0a98c2c5816e8b30affddffb3b18eb92`  
		Last Modified: Sat, 28 May 2022 18:17:12 GMT  
		Size: 1.7 KB (1724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07b4533bb794e8bcf3d387a8eab93b53e34d8b4ce2c87c000e3001000c0c5df2`  
		Last Modified: Sat, 28 May 2022 18:17:13 GMT  
		Size: 1.4 MB (1374975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d1f55e0571f9d4e7d54d1b41ab8d15bd440b041f5a8a5cd2efe350b24fa82dd`  
		Last Modified: Wed, 08 Jun 2022 19:10:39 GMT  
		Size: 9.4 MB (9360078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:938f0cdb2b7fa2386cbd0b81ed0bf45255ff4791082dfc8d93b6e6208ac251e3`  
		Last Modified: Wed, 08 Jun 2022 19:10:35 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f6e9af37e2bd3f5e72e51d8da5e080b48fab000543839f7bf9017697f4ba792`  
		Last Modified: Wed, 08 Jun 2022 19:10:35 GMT  
		Size: 577.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:7-bullseye` - linux; arm variant v7

```console
$ docker pull redis@sha256:29b032222cd76d7ec6e500b1f4f64d0097544d2394250a1c3616e9d14ed9a317
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.1 MB (37137029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a9c746a9b9d38e7b4e26a73bea33058279f9a7b47d603a2124b2070808ecfbc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Sat, 28 May 2022 00:59:48 GMT
ADD file:975c801b5b50aa75e07d18e69af11f21e165561abc16246e2c413c2ef96ce4c6 in / 
# Sat, 28 May 2022 00:59:49 GMT
CMD ["bash"]
# Sun, 29 May 2022 04:18:08 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Sun, 29 May 2022 04:18:09 GMT
ENV GOSU_VERSION=1.14
# Sun, 29 May 2022 04:18:37 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 08 Jun 2022 18:32:46 GMT
ENV REDIS_VERSION=7.0.1
# Wed, 08 Jun 2022 18:32:46 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.0.1.tar.gz
# Wed, 08 Jun 2022 18:32:47 GMT
ENV REDIS_DOWNLOAD_SHA=ca1820d527e4759884620be2917079e61e996fa81da5fbe5c07c4a7b507264dc
# Wed, 08 Jun 2022 18:34:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Wed, 08 Jun 2022 18:34:30 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 08 Jun 2022 18:34:31 GMT
VOLUME [/data]
# Wed, 08 Jun 2022 18:34:31 GMT
WORKDIR /data
# Wed, 08 Jun 2022 18:34:32 GMT
COPY file:e873a0e3c13001b5e1c63f9dbe60cc65722af522671787f68b8e8cbcae7d02ac in /usr/local/bin/ 
# Wed, 08 Jun 2022 18:34:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Jun 2022 18:34:33 GMT
EXPOSE 6379
# Wed, 08 Jun 2022 18:34:33 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:eeb117569618df53320eb28d32b7a1d87792bda3362017123fa1025b55db44c3`  
		Last Modified: Sat, 28 May 2022 01:15:35 GMT  
		Size: 26.6 MB (26576237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13630c86b934535ef45b705bdc0433144695ec359b4663bb2308cebf6e484f8b`  
		Last Modified: Sun, 29 May 2022 04:30:28 GMT  
		Size: 1.7 KB (1724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4686d9efeb45af4a3279032e99de4ec7c1978a64e37a9d02f223ba8d4cf7df8f`  
		Last Modified: Sun, 29 May 2022 04:30:29 GMT  
		Size: 1.4 MB (1367077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba8e43e23ec1f1e9910cdeb961ff3be5331f6063451d91b9d534766f42bbeb71`  
		Last Modified: Wed, 08 Jun 2022 18:41:19 GMT  
		Size: 9.2 MB (9191280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e666b25ed56107e7f346a5c91eae22ba30002bccb1d08282f718f9cb82f40cac`  
		Last Modified: Wed, 08 Jun 2022 18:41:13 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e7e7608d4a32daef8d4b9787adba6324b5dcac9654b7112f44f252326016313`  
		Last Modified: Wed, 08 Jun 2022 18:41:13 GMT  
		Size: 577.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:7-bullseye` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:0ea9c1fc8b222ac3d6859c7f81392f166a749e8ddca8937885ba9f23e209a19a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.0 MB (40977038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:329197e7c3d7bc316bd71b768acb2a0bd27d4b4f32971d95803391a79d01d1b2`
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
# Wed, 08 Jun 2022 19:10:47 GMT
ENV REDIS_VERSION=7.0.1
# Wed, 08 Jun 2022 19:10:48 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.0.1.tar.gz
# Wed, 08 Jun 2022 19:10:49 GMT
ENV REDIS_DOWNLOAD_SHA=ca1820d527e4759884620be2917079e61e996fa81da5fbe5c07c4a7b507264dc
# Wed, 08 Jun 2022 19:11:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Wed, 08 Jun 2022 19:11:33 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 08 Jun 2022 19:11:34 GMT
VOLUME [/data]
# Wed, 08 Jun 2022 19:11:35 GMT
WORKDIR /data
# Wed, 08 Jun 2022 19:11:37 GMT
COPY file:e873a0e3c13001b5e1c63f9dbe60cc65722af522671787f68b8e8cbcae7d02ac in /usr/local/bin/ 
# Wed, 08 Jun 2022 19:11:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Jun 2022 19:11:38 GMT
EXPOSE 6379
# Wed, 08 Jun 2022 19:11:39 GMT
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
	-	`sha256:866ac940e89015a487f5fa8df35ea4095016ae47c3d9b722e2420a3df5d5abf7`  
		Last Modified: Wed, 08 Jun 2022 19:14:58 GMT  
		Size: 9.6 MB (9571545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f8ad6286866db0dd678a374a502eddaddf22b69091784c6cc6e024a562729ca`  
		Last Modified: Wed, 08 Jun 2022 19:14:56 GMT  
		Size: 96.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3585dc77605decadfa348e1c9a03eb32ad535ca51940b61d4db6bc1cd3baa79e`  
		Last Modified: Wed, 08 Jun 2022 19:14:56 GMT  
		Size: 576.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:7-bullseye` - linux; 386

```console
$ docker pull redis@sha256:f41244046b043f801f7cc57089b5736c5b229602679f03689b8f5148646dccfe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.9 MB (42894480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a221bb2ea1af903f48ff3d0533f3c9e97832ba146420583fe280e78b38a3ea2d`
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
# Wed, 08 Jun 2022 18:57:54 GMT
ENV REDIS_VERSION=7.0.1
# Wed, 08 Jun 2022 18:57:55 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.0.1.tar.gz
# Wed, 08 Jun 2022 18:57:56 GMT
ENV REDIS_DOWNLOAD_SHA=ca1820d527e4759884620be2917079e61e996fa81da5fbe5c07c4a7b507264dc
# Wed, 08 Jun 2022 18:58:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Wed, 08 Jun 2022 18:58:44 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 08 Jun 2022 18:58:45 GMT
VOLUME [/data]
# Wed, 08 Jun 2022 18:58:46 GMT
WORKDIR /data
# Wed, 08 Jun 2022 18:58:48 GMT
COPY file:e873a0e3c13001b5e1c63f9dbe60cc65722af522671787f68b8e8cbcae7d02ac in /usr/local/bin/ 
# Wed, 08 Jun 2022 18:58:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Jun 2022 18:58:49 GMT
EXPOSE 6379
# Wed, 08 Jun 2022 18:58:50 GMT
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
	-	`sha256:c91e6f1cf20b8d849f18d61d56eb20929238664b9f78a2e996fdc60d3d77de9f`  
		Last Modified: Wed, 08 Jun 2022 19:02:19 GMT  
		Size: 9.1 MB (9125017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e322bce80175142c79fa571b13226bcd9d85474e75db9e4373ea7f8e74af654a`  
		Last Modified: Wed, 08 Jun 2022 19:02:18 GMT  
		Size: 96.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ef06be405c35fc929ab86114f52a676a7d0dbc6b02e9686b80ccc4d91d217a`  
		Last Modified: Wed, 08 Jun 2022 19:02:18 GMT  
		Size: 576.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:7-bullseye` - linux; mips64le

```console
$ docker pull redis@sha256:188587c12c4c7fb1f97008e4ad5f597bdac057c5d0ffade6b9d2340d283c524a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.7 MB (40691811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25175a37d62111632eac05dad73370dd60db7a2410aa3ad0c9f08b5faaf8668a`
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
# Wed, 08 Jun 2022 18:29:18 GMT
ENV REDIS_VERSION=7.0.1
# Wed, 08 Jun 2022 18:29:20 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.0.1.tar.gz
# Wed, 08 Jun 2022 18:29:22 GMT
ENV REDIS_DOWNLOAD_SHA=ca1820d527e4759884620be2917079e61e996fa81da5fbe5c07c4a7b507264dc
# Wed, 08 Jun 2022 18:33:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Wed, 08 Jun 2022 18:33:42 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 08 Jun 2022 18:33:45 GMT
VOLUME [/data]
# Wed, 08 Jun 2022 18:33:47 GMT
WORKDIR /data
# Wed, 08 Jun 2022 18:33:49 GMT
COPY file:e873a0e3c13001b5e1c63f9dbe60cc65722af522671787f68b8e8cbcae7d02ac in /usr/local/bin/ 
# Wed, 08 Jun 2022 18:33:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Jun 2022 18:33:54 GMT
EXPOSE 6379
# Wed, 08 Jun 2022 18:33:56 GMT
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
	-	`sha256:db58c2ba8e38c0f94367ba6a78918a5bc366e6a22b0537965d138806c2f38f2f`  
		Last Modified: Wed, 08 Jun 2022 18:34:38 GMT  
		Size: 9.8 MB (9758189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2f80231c3fdb0aff6d3007fc9b9d9d2c01fbfdba6e1d526f40928ef0435e7a4`  
		Last Modified: Wed, 08 Jun 2022 18:34:31 GMT  
		Size: 99.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a71600df703c79a4fb585f4789875f3ed7ba224821f73afe9fc9aa382c568b7`  
		Last Modified: Wed, 08 Jun 2022 18:34:31 GMT  
		Size: 577.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:7-bullseye` - linux; ppc64le

```console
$ docker pull redis@sha256:4515f813b02020cf73e19de85543154e9c2822ecc5b44c4a2c3bc38fd12595f7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46660489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c70f246941f15a61e2d56aa2eb90a21dbbc245a6add7ba2825a228a6448b9d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Sat, 28 May 2022 01:22:54 GMT
ADD file:64e264b12eed99d87380e38f36bfecd62b9bb1e5460f0242cfbc5dc76c212ead in / 
# Sat, 28 May 2022 01:22:59 GMT
CMD ["bash"]
# Sat, 28 May 2022 18:21:53 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Sat, 28 May 2022 18:21:57 GMT
ENV GOSU_VERSION=1.14
# Sat, 28 May 2022 18:23:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 08 Jun 2022 19:37:21 GMT
ENV REDIS_VERSION=7.0.1
# Wed, 08 Jun 2022 19:37:24 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.0.1.tar.gz
# Wed, 08 Jun 2022 19:37:28 GMT
ENV REDIS_DOWNLOAD_SHA=ca1820d527e4759884620be2917079e61e996fa81da5fbe5c07c4a7b507264dc
# Wed, 08 Jun 2022 19:40:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Wed, 08 Jun 2022 19:40:34 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 08 Jun 2022 19:40:40 GMT
VOLUME [/data]
# Wed, 08 Jun 2022 19:40:46 GMT
WORKDIR /data
# Wed, 08 Jun 2022 19:40:47 GMT
COPY file:e873a0e3c13001b5e1c63f9dbe60cc65722af522671787f68b8e8cbcae7d02ac in /usr/local/bin/ 
# Wed, 08 Jun 2022 19:40:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Jun 2022 19:40:51 GMT
EXPOSE 6379
# Wed, 08 Jun 2022 19:40:53 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:893e245a8f6219935016f2dd4422ec4b7fdab43d98ba29c024ec0d9ce57794ba`  
		Last Modified: Sat, 28 May 2022 01:32:28 GMT  
		Size: 35.3 MB (35286698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a053b3fb2a951f376a4097306076ce25e3970778a79f552821a30cc61fc7f69`  
		Last Modified: Sat, 28 May 2022 18:39:38 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a5ca55625ffcd597ebc58af223fc478486e078aa225f149dbc28c88f4e534a2`  
		Last Modified: Sat, 28 May 2022 18:39:38 GMT  
		Size: 1.3 MB (1309261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b2d6f0f5fe2679885e0b9b9d16bdb236ad0a7d1d9ef222e8dc3b81269f1845`  
		Last Modified: Wed, 08 Jun 2022 19:45:19 GMT  
		Size: 10.1 MB (10062083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9775ce85a2fc7c56a94a93a574dd820416f8e3086b21c1bad78dd2143998909c`  
		Last Modified: Wed, 08 Jun 2022 19:45:17 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edfffc0a32acb89ba17e4d4ccd09c4de890495bc6229d35179dc6aa191c5afea`  
		Last Modified: Wed, 08 Jun 2022 19:45:17 GMT  
		Size: 577.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:7-bullseye` - linux; s390x

```console
$ docker pull redis@sha256:91fc6a5cb2a2aa904227d7e88cb1ee733a3f43a9766a13aa83352e3d910bf9a9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.9 MB (40878595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2d4a14f06714d2179c92fa6a0d701360c266b2549b1b47ce1989fa3a18584a5`
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
# Wed, 08 Jun 2022 19:10:20 GMT
ENV REDIS_VERSION=7.0.1
# Wed, 08 Jun 2022 19:10:21 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.0.1.tar.gz
# Wed, 08 Jun 2022 19:10:22 GMT
ENV REDIS_DOWNLOAD_SHA=ca1820d527e4759884620be2917079e61e996fa81da5fbe5c07c4a7b507264dc
# Wed, 08 Jun 2022 19:12:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Wed, 08 Jun 2022 19:12:05 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 08 Jun 2022 19:12:06 GMT
VOLUME [/data]
# Wed, 08 Jun 2022 19:12:06 GMT
WORKDIR /data
# Wed, 08 Jun 2022 19:12:07 GMT
COPY file:e873a0e3c13001b5e1c63f9dbe60cc65722af522671787f68b8e8cbcae7d02ac in /usr/local/bin/ 
# Wed, 08 Jun 2022 19:12:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Jun 2022 19:12:08 GMT
EXPOSE 6379
# Wed, 08 Jun 2022 19:12:09 GMT
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
	-	`sha256:76c02e3b0bf0f26e5ba7ad03b43dfca0f80beb53a20dbdd7d603255a9a5ccf67`  
		Last Modified: Wed, 08 Jun 2022 19:16:57 GMT  
		Size: 9.8 MB (9847092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feef8c47e0ac24050aaf276f76836b35ea6106fb87b463b67cd092356225123c`  
		Last Modified: Wed, 08 Jun 2022 19:16:56 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef8e5e62faf1e33a60dee929f87c65d79d59dd80b5feec3109061ba1b241b03`  
		Last Modified: Wed, 08 Jun 2022 19:16:56 GMT  
		Size: 577.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
