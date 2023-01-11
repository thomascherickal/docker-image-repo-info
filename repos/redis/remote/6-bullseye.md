## `redis:6-bullseye`

```console
$ docker pull redis@sha256:35ec0940c1092bb51e527db087b8ef5472c3cae4d3dbc19adcae273c1b330a1d
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

### `redis:6-bullseye` - linux; amd64

```console
$ docker pull redis@sha256:cb4f8c0e6410525371b0f91efc36cf05a1efa3c48c90f0ae4184d684957240f5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.2 MB (41156717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c133222c17bae585cf947af17865cb980096b3216498d3239cd1a5df7355c1d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:44 GMT
ADD file:e2398d0bf516084b2b37ba1bb76b86d56e66999831df692461679fbd6a5d8eb6 in / 
# Wed, 11 Jan 2023 02:34:44 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 09:14:56 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Wed, 11 Jan 2023 09:14:56 GMT
ENV GOSU_VERSION=1.14
# Wed, 11 Jan 2023 09:15:09 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 11 Jan 2023 09:16:06 GMT
ENV REDIS_VERSION=6.2.8
# Wed, 11 Jan 2023 09:16:06 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.8.tar.gz
# Wed, 11 Jan 2023 09:16:07 GMT
ENV REDIS_DOWNLOAD_SHA=f91ab24bcb42673cb853292eb5d43c2017d11d659854808ed6a529c97297fdfe
# Wed, 11 Jan 2023 09:16:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Wed, 11 Jan 2023 09:16:50 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 11 Jan 2023 09:16:50 GMT
VOLUME [/data]
# Wed, 11 Jan 2023 09:16:50 GMT
WORKDIR /data
# Wed, 11 Jan 2023 09:16:51 GMT
COPY file:e873a0e3c13001b5e1c63f9dbe60cc65722af522671787f68b8e8cbcae7d02ac in /usr/local/bin/ 
# Wed, 11 Jan 2023 09:16:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Jan 2023 09:16:51 GMT
EXPOSE 6379
# Wed, 11 Jan 2023 09:16:51 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:8740c948ffd4c816ea7ca963f99ca52f4788baa23f228da9581a9ea2edd3fcd7`  
		Last Modified: Wed, 11 Jan 2023 02:39:07 GMT  
		Size: 31.4 MB (31396972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2271c958e57d5a938bdccac2b84c4c37350a3cf60a14dc9367320acc618e2b2`  
		Last Modified: Wed, 11 Jan 2023 09:18:17 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:495af11a3eac5e4752fd09722eb4381c10f80a04c1f4c132f6869e2c65434108`  
		Last Modified: Wed, 11 Jan 2023 09:18:18 GMT  
		Size: 1.4 MB (1410528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a5e13bc1b8694daa19f35d7f0dfc3aa056189ff823a3629cb8dd494609fc0f2`  
		Last Modified: Wed, 11 Jan 2023 09:18:44 GMT  
		Size: 8.3 MB (8346776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff8b9857595022ad0ad3ce339242a05c27a31b5cf9306ff61b48f98c737067e`  
		Last Modified: Wed, 11 Jan 2023 09:18:42 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7393d1d501457e60af3174d85829963d3df7531fcb1cfe3456ba4fbb6d59e0d`  
		Last Modified: Wed, 11 Jan 2023 09:18:42 GMT  
		Size: 576.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-bullseye` - linux; arm variant v5

```console
$ docker pull redis@sha256:558d947bb8987c1f29958935b5aaf61a80f809ab3abdbbf1406c7bde59634af1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.4 MB (38437854 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15b7096f4caa712a259751c343541365943fc08ab359d45b34a065fb251f2e24`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 21 Dec 2022 01:49:08 GMT
ADD file:89f7788ae38bc6c172614b734ff10cba90c89ee09ca0f1acccc185c1bec630a1 in / 
# Wed, 21 Dec 2022 01:49:09 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 08:50:01 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Wed, 21 Dec 2022 08:50:01 GMT
ENV GOSU_VERSION=1.14
# Wed, 21 Dec 2022 08:50:15 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 21 Dec 2022 08:51:13 GMT
ENV REDIS_VERSION=6.2.8
# Wed, 21 Dec 2022 08:51:13 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.8.tar.gz
# Wed, 21 Dec 2022 08:51:14 GMT
ENV REDIS_DOWNLOAD_SHA=f91ab24bcb42673cb853292eb5d43c2017d11d659854808ed6a529c97297fdfe
# Wed, 21 Dec 2022 08:52:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Wed, 21 Dec 2022 08:52:02 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 21 Dec 2022 08:52:02 GMT
VOLUME [/data]
# Wed, 21 Dec 2022 08:52:02 GMT
WORKDIR /data
# Wed, 21 Dec 2022 08:52:03 GMT
COPY file:e873a0e3c13001b5e1c63f9dbe60cc65722af522671787f68b8e8cbcae7d02ac in /usr/local/bin/ 
# Wed, 21 Dec 2022 08:52:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Dec 2022 08:52:03 GMT
EXPOSE 6379
# Wed, 21 Dec 2022 08:52:03 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:6addfee759f2774f92392906ab5b50ba2f4a14314858c502e856f7d7de2a7e07`  
		Last Modified: Wed, 21 Dec 2022 01:54:03 GMT  
		Size: 28.9 MB (28898607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56036fd69d58a083cfc46ee262a4b3bd278e57f71224bf51e1879ee435fd59c1`  
		Last Modified: Wed, 21 Dec 2022 08:54:05 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ddb75516e5990f716a1695b420629c46d066c9a3be671e0f3e2b1ae3c3cbac`  
		Last Modified: Wed, 21 Dec 2022 08:54:05 GMT  
		Size: 1.4 MB (1374795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b08e3c711b422ec8efc5ad542a4c970ebfb387cf2647772c760741ce12634d`  
		Last Modified: Wed, 21 Dec 2022 08:54:39 GMT  
		Size: 8.2 MB (8162058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b00efcc779860ed820d0371312e922048bf437cc3b685e76512898a294438e9`  
		Last Modified: Wed, 21 Dec 2022 08:54:37 GMT  
		Size: 99.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a026b593ffcb692aebf04e0ca9638853ff7726529674d8650f7c543d5b0af2cc`  
		Last Modified: Wed, 21 Dec 2022 08:54:37 GMT  
		Size: 572.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-bullseye` - linux; arm variant v7

```console
$ docker pull redis@sha256:894fa5200742f33f6f47d33f7b605e467deb804d039a13cbe024dbfea94c1f8f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35931662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:344c6075eb77307d044f55a3768cc8abf45365713f86ea14ac146397968b1130`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 21 Dec 2022 01:58:25 GMT
ADD file:d62015d4eb206b606ae0bc76253de55403ede851d6fae0277e76bdaed196a848 in / 
# Wed, 21 Dec 2022 01:58:26 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 15:53:13 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Wed, 21 Dec 2022 15:53:13 GMT
ENV GOSU_VERSION=1.14
# Wed, 21 Dec 2022 15:53:25 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 21 Dec 2022 15:54:31 GMT
ENV REDIS_VERSION=6.2.8
# Wed, 21 Dec 2022 15:54:31 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.8.tar.gz
# Wed, 21 Dec 2022 15:54:31 GMT
ENV REDIS_DOWNLOAD_SHA=f91ab24bcb42673cb853292eb5d43c2017d11d659854808ed6a529c97297fdfe
# Wed, 21 Dec 2022 15:55:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Wed, 21 Dec 2022 15:55:12 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 21 Dec 2022 15:55:12 GMT
VOLUME [/data]
# Wed, 21 Dec 2022 15:55:12 GMT
WORKDIR /data
# Wed, 21 Dec 2022 15:55:12 GMT
COPY file:e873a0e3c13001b5e1c63f9dbe60cc65722af522671787f68b8e8cbcae7d02ac in /usr/local/bin/ 
# Wed, 21 Dec 2022 15:55:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Dec 2022 15:55:13 GMT
EXPOSE 6379
# Wed, 21 Dec 2022 15:55:13 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:f8686edc9eb6f431c8c17a5eddc7bd38917d3b2d7835970d4fdb2ad0db464766`  
		Last Modified: Wed, 21 Dec 2022 02:05:08 GMT  
		Size: 26.6 MB (26559455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7b14376383f78ae0dcb17d4ff89c4ace81e6eed13e201adb8f1b22ad95b5cda`  
		Last Modified: Wed, 21 Dec 2022 15:57:54 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee62174c29c1a4d7e60bec17384190e8d9df8fca7e727f772056c2ebdadaa9ec`  
		Last Modified: Wed, 21 Dec 2022 15:57:54 GMT  
		Size: 1.4 MB (1366972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57249edbc11d51f9f5caf036d6124fbf0929d97cb0658dbbd75b9f58299f8b9b`  
		Last Modified: Wed, 21 Dec 2022 15:58:34 GMT  
		Size: 8.0 MB (8002835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3c304d18450cc91d8891d78f2899dd27a3e65a2cc2dd2ac4367c5073e1df73`  
		Last Modified: Wed, 21 Dec 2022 15:58:32 GMT  
		Size: 98.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf3313b4bb4f5f4c741b75e932b9df797a92e607da857f13beed1caf23d4c8e7`  
		Last Modified: Wed, 21 Dec 2022 15:58:32 GMT  
		Size: 576.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-bullseye` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:c069c2ecce604d72d55ecfcd4967cfeb657081b93c7990cf0901f217c80f268e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.8 MB (39761779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e76ecca71ce604c042de6b2e78ba3773ea32554ef89b325ed82c256db5c8f2b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:48 GMT
ADD file:3ff0cc8d111595978eb50cdba91144382ce083c400d45785d53dbb03615a4890 in / 
# Wed, 21 Dec 2022 01:39:48 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 12:07:14 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Wed, 21 Dec 2022 12:07:14 GMT
ENV GOSU_VERSION=1.14
# Wed, 21 Dec 2022 12:07:24 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 21 Dec 2022 12:08:13 GMT
ENV REDIS_VERSION=6.2.8
# Wed, 21 Dec 2022 12:08:13 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.8.tar.gz
# Wed, 21 Dec 2022 12:08:13 GMT
ENV REDIS_DOWNLOAD_SHA=f91ab24bcb42673cb853292eb5d43c2017d11d659854808ed6a529c97297fdfe
# Wed, 21 Dec 2022 12:08:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Wed, 21 Dec 2022 12:08:46 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 21 Dec 2022 12:08:46 GMT
VOLUME [/data]
# Wed, 21 Dec 2022 12:08:46 GMT
WORKDIR /data
# Wed, 21 Dec 2022 12:08:46 GMT
COPY file:e873a0e3c13001b5e1c63f9dbe60cc65722af522671787f68b8e8cbcae7d02ac in /usr/local/bin/ 
# Wed, 21 Dec 2022 12:08:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Dec 2022 12:08:46 GMT
EXPOSE 6379
# Wed, 21 Dec 2022 12:08:46 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:4b7f5b2a311310809ab89d92f6f71b0462722fe855d3b92c93098a528aa08791`  
		Last Modified: Wed, 21 Dec 2022 01:43:12 GMT  
		Size: 30.0 MB (30044772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:530f161a295b8beace37204cf469b7a6692a4cb9a670b966f9ac441586c4b9b3`  
		Last Modified: Wed, 21 Dec 2022 12:10:12 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efcdb237d353748f12313236b83a415a7ca100b9ff3f922899e421b93838646c`  
		Last Modified: Wed, 21 Dec 2022 12:10:12 GMT  
		Size: 1.3 MB (1337927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fbef75700db16d170f2c77742fb270b10c8262e8da8bb920ee1eefc8b57a254`  
		Last Modified: Wed, 21 Dec 2022 12:10:39 GMT  
		Size: 8.4 MB (8376635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb59f4849505ddd32dc33e760784d7edfa368d1d5f753634d5a8ee408a2171e`  
		Last Modified: Wed, 21 Dec 2022 12:10:38 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3465878271eb04a9259cc4e47fed51ee34ece4907f411babf89fb107cc9c804`  
		Last Modified: Wed, 21 Dec 2022 12:10:38 GMT  
		Size: 576.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-bullseye` - linux; 386

```console
$ docker pull redis@sha256:638a8af03873eaafd84a895eb951fcfb15dfdd85340b044f80aff650e64ccbea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.8 MB (41752838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3d32f3eb7cae2e183b5575c419ea26aca5538e934bb567d76b429f8ab61c3ce`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:22 GMT
ADD file:5f553fdf893bb3198d173c48f4531e9bfdbab61798c1aa8217fd80e9d686d7ae in / 
# Wed, 21 Dec 2022 01:39:22 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 06:36:54 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Wed, 21 Dec 2022 06:36:54 GMT
ENV GOSU_VERSION=1.14
# Wed, 21 Dec 2022 06:37:06 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 21 Dec 2022 06:38:23 GMT
ENV REDIS_VERSION=6.2.8
# Wed, 21 Dec 2022 06:38:24 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.8.tar.gz
# Wed, 21 Dec 2022 06:38:25 GMT
ENV REDIS_DOWNLOAD_SHA=f91ab24bcb42673cb853292eb5d43c2017d11d659854808ed6a529c97297fdfe
# Wed, 21 Dec 2022 06:39:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Wed, 21 Dec 2022 06:39:09 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 21 Dec 2022 06:39:10 GMT
VOLUME [/data]
# Wed, 21 Dec 2022 06:39:11 GMT
WORKDIR /data
# Wed, 21 Dec 2022 06:39:13 GMT
COPY file:e873a0e3c13001b5e1c63f9dbe60cc65722af522671787f68b8e8cbcae7d02ac in /usr/local/bin/ 
# Wed, 21 Dec 2022 06:39:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Dec 2022 06:39:14 GMT
EXPOSE 6379
# Wed, 21 Dec 2022 06:39:15 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:3228cb514e81f042720b7fd118ace0f279d1a4bc422b7e24189514a574dfa546`  
		Last Modified: Wed, 21 Dec 2022 01:44:46 GMT  
		Size: 32.4 MB (32375745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46c32e677ec37c91180b5338fabaf6c24d84f1060014d584d958363444810f1`  
		Last Modified: Wed, 21 Dec 2022 06:41:40 GMT  
		Size: 1.6 KB (1609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ddec3febb5405cb40dc51990176a80d123dcc0f4d87744daf35b2ce122161ee`  
		Last Modified: Wed, 21 Dec 2022 06:41:41 GMT  
		Size: 1.4 MB (1376929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a01eb6ca35b89b419f774aa41e8e830a76f45de7d5766d018319ab425c55293`  
		Last Modified: Wed, 21 Dec 2022 06:42:19 GMT  
		Size: 8.0 MB (7997883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24fc82637220a0cdac7cdabf80ed754ca7db407acf560e11a909ec1eeb053794`  
		Last Modified: Wed, 21 Dec 2022 06:42:18 GMT  
		Size: 97.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61de698cd76504f4d8a0fd557c3ae2168d0a964870b8e0124dfb9137029726a9`  
		Last Modified: Wed, 21 Dec 2022 06:42:18 GMT  
		Size: 575.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-bullseye` - linux; mips64le

```console
$ docker pull redis@sha256:33169049d3405856e9504dcc925086106e16f2da4212a6bb42a6cb524845e9a8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.6 MB (39607604 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0e61c5d37773ee368ceefbc8e5ab18f7cd29eb39dd1005c39169bdef54b8ab2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 21 Dec 2022 01:10:32 GMT
ADD file:45a0ac3f00e914341df42a4d2a56b9081a224ee58e1167fb05ca87662d42f24c in / 
# Wed, 21 Dec 2022 01:10:37 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 23:06:23 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Wed, 21 Dec 2022 23:06:26 GMT
ENV GOSU_VERSION=1.14
# Wed, 21 Dec 2022 23:07:35 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 21 Dec 2022 23:12:34 GMT
ENV REDIS_VERSION=6.2.8
# Wed, 21 Dec 2022 23:12:36 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.8.tar.gz
# Wed, 21 Dec 2022 23:12:39 GMT
ENV REDIS_DOWNLOAD_SHA=f91ab24bcb42673cb853292eb5d43c2017d11d659854808ed6a529c97297fdfe
# Wed, 21 Dec 2022 23:16:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Wed, 21 Dec 2022 23:16:46 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 21 Dec 2022 23:16:49 GMT
VOLUME [/data]
# Wed, 21 Dec 2022 23:16:51 GMT
WORKDIR /data
# Wed, 21 Dec 2022 23:16:53 GMT
COPY file:e873a0e3c13001b5e1c63f9dbe60cc65722af522671787f68b8e8cbcae7d02ac in /usr/local/bin/ 
# Wed, 21 Dec 2022 23:16:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Dec 2022 23:16:58 GMT
EXPOSE 6379
# Wed, 21 Dec 2022 23:17:01 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:5410793baaff16536eff1e5ac655d98039bd44f581c42d6ceb254202d1196477`  
		Last Modified: Wed, 21 Dec 2022 01:18:42 GMT  
		Size: 29.6 MB (29619894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:880790c5077a275b66d0e14394d8b143af21d05535576e27121babda55bed079`  
		Last Modified: Wed, 21 Dec 2022 23:22:00 GMT  
		Size: 1.6 KB (1615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:422be098ad552318d6e81d511b4ca20047465d0c55389f41b2a6e58695c0df35`  
		Last Modified: Wed, 21 Dec 2022 23:22:01 GMT  
		Size: 1.3 MB (1290155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1017c7f6d984fe68e64d15f3c9cbcb1a66cf6cc84e18e0f898c00596db848c8`  
		Last Modified: Wed, 21 Dec 2022 23:22:37 GMT  
		Size: 8.7 MB (8695268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ff2bb32a3f5afdea1aa369c7baf18629b2ca3b018e4bcd681f1ccf5eac00238`  
		Last Modified: Wed, 21 Dec 2022 23:22:30 GMT  
		Size: 96.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ce734616f55718b4077aae6c417290e0d146481ccbba23c69a13af422750498`  
		Last Modified: Wed, 21 Dec 2022 23:22:30 GMT  
		Size: 576.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-bullseye` - linux; ppc64le

```console
$ docker pull redis@sha256:e1fd622d185acc4a81d6f2fa0b788fae4b6f0c2af44d2912275257e232f66b94
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.5 MB (45497696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:912cfd5d159df3645d4c1be51c6428f8789bd82faf92de35bfcab9d552cccb38`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 11 Jan 2023 03:49:30 GMT
ADD file:3c7553fb5eda606d574ff6c08bc2213f9e6a68910043fe3087e4c1a04b65a18e in / 
# Wed, 11 Jan 2023 03:49:32 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 07:01:08 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Wed, 11 Jan 2023 07:01:08 GMT
ENV GOSU_VERSION=1.14
# Wed, 11 Jan 2023 07:01:30 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 11 Jan 2023 07:03:06 GMT
ENV REDIS_VERSION=6.2.8
# Wed, 11 Jan 2023 07:03:07 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.8.tar.gz
# Wed, 11 Jan 2023 07:03:07 GMT
ENV REDIS_DOWNLOAD_SHA=f91ab24bcb42673cb853292eb5d43c2017d11d659854808ed6a529c97297fdfe
# Wed, 11 Jan 2023 07:04:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Wed, 11 Jan 2023 07:04:21 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 11 Jan 2023 07:04:21 GMT
VOLUME [/data]
# Wed, 11 Jan 2023 07:04:22 GMT
WORKDIR /data
# Wed, 11 Jan 2023 07:04:22 GMT
COPY file:e873a0e3c13001b5e1c63f9dbe60cc65722af522671787f68b8e8cbcae7d02ac in /usr/local/bin/ 
# Wed, 11 Jan 2023 07:04:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Jan 2023 07:04:23 GMT
EXPOSE 6379
# Wed, 11 Jan 2023 07:04:24 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:bbf81328aca90b7ddb122fc175443f5323674a9e51bbb00d5b1d683ef0b858f4`  
		Last Modified: Wed, 11 Jan 2023 03:55:33 GMT  
		Size: 35.3 MB (35268773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5968bc5cbc00603ba0a2c684ad729530a1589bd72ee11fb9a64466b3dc26c85a`  
		Last Modified: Wed, 11 Jan 2023 07:07:17 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19142d90bf79ff79158cacbec48551449a10a9c27e12cc0ced168fe42c3cd901`  
		Last Modified: Wed, 11 Jan 2023 07:07:17 GMT  
		Size: 1.3 MB (1309144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16dcb0e50bed0e529026e24b8bcad122ed16105f77fa1b58141123d6063bd96d`  
		Last Modified: Wed, 11 Jan 2023 07:07:57 GMT  
		Size: 8.9 MB (8917336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af22e01d59de23326b2525d744a6e08d63e295dd41bd85cd444243189e79901`  
		Last Modified: Wed, 11 Jan 2023 07:07:55 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34c212aca4cc571d46ade6da00e4cca7a730611b1931df1de5d21bc51b550175`  
		Last Modified: Wed, 11 Jan 2023 07:07:55 GMT  
		Size: 576.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-bullseye` - linux; s390x

```console
$ docker pull redis@sha256:c6172c8764c9e86ba5113478a179b273991aa50745388cf386a03d07bfbf9104
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.7 MB (39713880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13af3e7b79ca721e70a1722e4e19cee454cb94996adfb97978d71425f1ce7d4e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 11 Jan 2023 02:22:23 GMT
ADD file:14f332233d8fa1ca519992e52aaf550bcee52d346c375e94ee73d36864933f8e in / 
# Wed, 11 Jan 2023 02:22:25 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 08:48:36 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Wed, 11 Jan 2023 08:48:37 GMT
ENV GOSU_VERSION=1.14
# Wed, 11 Jan 2023 08:48:52 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 11 Jan 2023 08:50:13 GMT
ENV REDIS_VERSION=6.2.8
# Wed, 11 Jan 2023 08:50:13 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.8.tar.gz
# Wed, 11 Jan 2023 08:50:13 GMT
ENV REDIS_DOWNLOAD_SHA=f91ab24bcb42673cb853292eb5d43c2017d11d659854808ed6a529c97297fdfe
# Wed, 11 Jan 2023 08:51:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Wed, 11 Jan 2023 08:51:03 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 11 Jan 2023 08:51:03 GMT
VOLUME [/data]
# Wed, 11 Jan 2023 08:51:04 GMT
WORKDIR /data
# Wed, 11 Jan 2023 08:51:04 GMT
COPY file:e873a0e3c13001b5e1c63f9dbe60cc65722af522671787f68b8e8cbcae7d02ac in /usr/local/bin/ 
# Wed, 11 Jan 2023 08:51:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Jan 2023 08:51:04 GMT
EXPOSE 6379
# Wed, 11 Jan 2023 08:51:04 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:5895b3b9300287ac4aca79440c1c4979b6d4fad1ceb06fba32443d012c83cc37`  
		Last Modified: Wed, 11 Jan 2023 02:26:52 GMT  
		Size: 29.6 MB (29629731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5c4131d5a47e1739ccd7f49a1b0b3da85d60b013463e6ef0af7dea813349e6`  
		Last Modified: Wed, 11 Jan 2023 08:53:35 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e110857a1da1ad19a3c15b85ac46038d06fdc17629c503e297a3810a875751`  
		Last Modified: Wed, 11 Jan 2023 08:53:36 GMT  
		Size: 1.4 MB (1373761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3267a838fa04c67a1f7f15db1b4d72df57e3f300a74f88f22bd8acbad03b798b`  
		Last Modified: Wed, 11 Jan 2023 08:54:03 GMT  
		Size: 8.7 MB (8707945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:739baf3bcc879a55d78003bffb652887583d84f30c9dcf4e34ae2a12bc7ced51`  
		Last Modified: Wed, 11 Jan 2023 08:54:01 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc260e43b4b3a2df05d44fe9a70949a96795090ad21a8aece475023682939a4`  
		Last Modified: Wed, 11 Jan 2023 08:54:01 GMT  
		Size: 573.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
