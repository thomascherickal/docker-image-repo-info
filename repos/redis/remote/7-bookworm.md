## `redis:7-bookworm`

```console
$ docker pull redis@sha256:d39a86a7406f0b3fe2b2f935cb5797737eba5c2586745553c2cc1cd54c49cd8a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `redis:7-bookworm` - linux; amd64

```console
$ docker pull redis@sha256:178215249742b63308db1a5373a7c627714c582362f3dcd24b2eec849dc16e67
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.1 MB (48125584 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e69fcb59ff4a25f87cf68cf2558df9c56df3c3c8ef709677dc602a458fe9b2d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:42 GMT
ADD file:ba1250b6ecd5dd09d4914189d72741c2817988994e7da514bf62be439a34bdb5 in / 
# Mon, 12 Jun 2023 23:20:42 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 21:53:38 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Wed, 14 Jun 2023 21:53:38 GMT
ENV GOSU_VERSION=1.16
# Wed, 14 Jun 2023 21:53:52 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 14 Jun 2023 21:56:11 GMT
ENV REDIS_VERSION=7.0.11
# Wed, 14 Jun 2023 21:56:11 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.0.11.tar.gz
# Wed, 14 Jun 2023 21:56:11 GMT
ENV REDIS_DOWNLOAD_SHA=ce250d1fba042c613de38a15d40889b78f7cb6d5461a27e35017ba39b07221e3
# Wed, 14 Jun 2023 21:57:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Wed, 14 Jun 2023 21:57:04 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 14 Jun 2023 21:57:04 GMT
VOLUME [/data]
# Wed, 14 Jun 2023 21:57:04 GMT
WORKDIR /data
# Wed, 14 Jun 2023 21:57:04 GMT
COPY file:e873a0e3c13001b5e1c63f9dbe60cc65722af522671787f68b8e8cbcae7d02ac in /usr/local/bin/ 
# Wed, 14 Jun 2023 21:57:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 21:57:04 GMT
EXPOSE 6379
# Wed, 14 Jun 2023 21:57:04 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:5b5fe70539cd6989aa19f25826309f9715a9489cf1c057982d6a84c1ad8975c7`  
		Last Modified: Mon, 12 Jun 2023 23:25:49 GMT  
		Size: 29.1 MB (29124744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1bc4b7ad0f02fe99bf6836ed4f7cb4509d9c7d94627ace9f43133fdbeaf764e`  
		Last Modified: Wed, 14 Jun 2023 22:01:30 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a33d2f01ead9ae4e9f5bf12af82045ef150407cc8098dd0decaaee54ac36f4f0`  
		Last Modified: Wed, 14 Jun 2023 22:01:30 GMT  
		Size: 1.4 MB (1436811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94b33095e71ca50a19c4e55bf6e70638c6391dece2b7281720c2b284c61218a0`  
		Last Modified: Wed, 14 Jun 2023 22:02:01 GMT  
		Size: 17.6 MB (17562202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3c2b649b97ccdfb269abba0191215f9d5a3c6ee4aa72210c74a25220c9143d1`  
		Last Modified: Wed, 14 Jun 2023 22:01:58 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a5bf7f0acd78ea73ec7fd047448cac874569cf69b57568668553c3f7bf35f83`  
		Last Modified: Wed, 14 Jun 2023 22:01:58 GMT  
		Size: 574.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:7-bookworm` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:02f48bad3678cba7ef08f68f83b266d26a20c0fe042725bcd8a684365ea6e225
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.0 MB (47045023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6f5d0b64daf7f45bb302346a9cb8a5a86f1d29bb45de6384540bbe51f4cf788`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:13 GMT
ADD file:f75c3fe22fec548b35a86a9a5802fdc97497f5d253cf630d65f13282169d3f3f in / 
# Mon, 12 Jun 2023 23:40:14 GMT
CMD ["bash"]
# Wed, 14 Jun 2023 21:50:14 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Wed, 14 Jun 2023 21:50:14 GMT
ENV GOSU_VERSION=1.16
# Wed, 14 Jun 2023 21:50:25 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 14 Jun 2023 21:52:03 GMT
ENV REDIS_VERSION=7.0.11
# Wed, 14 Jun 2023 21:52:03 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-7.0.11.tar.gz
# Wed, 14 Jun 2023 21:52:03 GMT
ENV REDIS_DOWNLOAD_SHA=ce250d1fba042c613de38a15d40889b78f7cb6d5461a27e35017ba39b07221e3
# Wed, 14 Jun 2023 21:52:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Wed, 14 Jun 2023 21:52:42 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 14 Jun 2023 21:52:42 GMT
VOLUME [/data]
# Wed, 14 Jun 2023 21:52:42 GMT
WORKDIR /data
# Wed, 14 Jun 2023 21:52:43 GMT
COPY file:e873a0e3c13001b5e1c63f9dbe60cc65722af522671787f68b8e8cbcae7d02ac in /usr/local/bin/ 
# Wed, 14 Jun 2023 21:52:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Jun 2023 21:52:43 GMT
EXPOSE 6379
# Wed, 14 Jun 2023 21:52:43 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:95039a22a7cc3ae41d71f075e6e09e91e8da850fb5f80aba2f4a09f254520539`  
		Last Modified: Mon, 12 Jun 2023 23:44:08 GMT  
		Size: 29.2 MB (29152534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1759dbde33aa972cbcf138cba603f858cf627f00c4007f4a49183c1de2c85f34`  
		Last Modified: Wed, 14 Jun 2023 21:56:22 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c302c4311d2e0ea61eedbcc3e2b4f8743076e32323d0076166e84f2721aa0c7`  
		Last Modified: Wed, 14 Jun 2023 21:56:23 GMT  
		Size: 1.4 MB (1368131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d78a60c5fcd285ac9d54cb03c351f1d7690ef3bf37ef853ee3e29ce047ba62`  
		Last Modified: Wed, 14 Jun 2023 21:56:53 GMT  
		Size: 16.5 MB (16522531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad510f4863eed3df42896129bb948149e0f77a3352ccfc5858c6c85653085d0b`  
		Last Modified: Wed, 14 Jun 2023 21:56:50 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0fd2612b38ae8a22c9bb115fa1662307513f04e0b5c069156911552d93cc0c`  
		Last Modified: Wed, 14 Jun 2023 21:56:50 GMT  
		Size: 572.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
