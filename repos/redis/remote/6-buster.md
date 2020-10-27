## `redis:6-buster`

```console
$ docker pull redis@sha256:91362815a12565b82db6dc137148402063a3935dfb4feff24d36ca93a417d13e
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

### `redis:6-buster` - linux; amd64

```console
$ docker pull redis@sha256:7599352c534698f628f3c8f3d8845317d2bb0b15525ab69c3e04b1a7596db18b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.2 MB (38190240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16ecd277293476392b71021cdd585c40ad68f4a7488752eede95928735e39df4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Tue, 13 Oct 2020 01:39:05 GMT
ADD file:0dc53e7886c35bc21ae6c4f6cedda54d56ae9c9e9cd367678f1a72e68b3c43d4 in / 
# Tue, 13 Oct 2020 01:39:05 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 22:06:03 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Tue, 13 Oct 2020 22:06:03 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 22:06:15 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 22:06:15 GMT
ENV REDIS_VERSION=6.0.8
# Tue, 13 Oct 2020 22:06:15 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.8.tar.gz
# Tue, 13 Oct 2020 22:06:16 GMT
ENV REDIS_DOWNLOAD_SHA=04fa1fddc39bd1aecb6739dd5dd73858a3515b427acd1e2947a66dadce868d68
# Mon, 26 Oct 2020 23:33:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Mon, 26 Oct 2020 23:33:07 GMT
RUN mkdir /data && chown redis:redis /data
# Mon, 26 Oct 2020 23:33:07 GMT
VOLUME [/data]
# Mon, 26 Oct 2020 23:33:07 GMT
WORKDIR /data
# Mon, 26 Oct 2020 23:33:07 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Mon, 26 Oct 2020 23:33:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 26 Oct 2020 23:33:08 GMT
EXPOSE 6379
# Mon, 26 Oct 2020 23:33:08 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:bb79b6b2107fea8e8a47133a660b78e3a546998fcf0427be39ac9a0af4a97e90`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 27.1 MB (27092228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed3521a5dcbd05214eb7f35b952ecf018d5a6610c32ba4e315028c556f45e94`  
		Last Modified: Tue, 13 Oct 2020 22:10:48 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5999b99cee8f2875d391d64df20b6296b63f23951a7d41749f028375e887cd05`  
		Last Modified: Tue, 13 Oct 2020 22:10:49 GMT  
		Size: 1.4 MB (1417672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f806f5245c911de95226a4020a76d80737fdcbffec3a861b271b9b9f04f6580`  
		Last Modified: Mon, 26 Oct 2020 23:38:02 GMT  
		Size: 9.7 MB (9678101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a4497572b28248d5e1178889ddcd6f660d0469de37586a5d1936e4bd35f408`  
		Last Modified: Mon, 26 Oct 2020 23:38:00 GMT  
		Size: 98.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eafe3b6b8d06c477db3a547c13ee9fd4648776cef12f76e1886d164b871c24bc`  
		Last Modified: Mon, 26 Oct 2020 23:38:00 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-buster` - linux; arm variant v5

```console
$ docker pull redis@sha256:6c7e1e64248364a08217d61aa05cdcf038a99835413763791079b6a2450b2e66
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.4 MB (35433770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bde22cbf79a90268b29a54da5f3590d556ab3da84ecd86218a1bbf8d69a3eb4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Tue, 13 Oct 2020 01:52:17 GMT
ADD file:b71c0fa4957d6b65af37231a105f3d17cdbafe5c7d6c37b5843ebf619c608aaa in / 
# Tue, 13 Oct 2020 01:52:27 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 08:39:00 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Tue, 13 Oct 2020 08:39:01 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 08:39:28 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 27 Oct 2020 18:00:17 GMT
ENV REDIS_VERSION=6.0.9
# Tue, 27 Oct 2020 18:00:17 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.9.tar.gz
# Tue, 27 Oct 2020 18:00:18 GMT
ENV REDIS_DOWNLOAD_SHA=dc2bdcf81c620e9f09cfd12e85d3bc631c897b2db7a55218fd8a65eaa37f86dd
# Tue, 27 Oct 2020 18:02:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Tue, 27 Oct 2020 18:02:18 GMT
RUN mkdir /data && chown redis:redis /data
# Tue, 27 Oct 2020 18:02:19 GMT
VOLUME [/data]
# Tue, 27 Oct 2020 18:02:20 GMT
WORKDIR /data
# Tue, 27 Oct 2020 18:02:20 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Tue, 27 Oct 2020 18:02:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 27 Oct 2020 18:02:22 GMT
EXPOSE 6379
# Tue, 27 Oct 2020 18:02:23 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:f991c1e1ee2c48f16625b6b61310bf3c0616c0dbda4762019117e86fd29cf9ce`  
		Last Modified: Tue, 13 Oct 2020 02:01:27 GMT  
		Size: 24.8 MB (24835992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8cf759f7e95eb715991258a6e248d63b70e8c0770266eb48b36f8c936be4eb`  
		Last Modified: Tue, 13 Oct 2020 08:43:16 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b05e13d7cabf4bfada7dd8dc012caab6b0299639f4c9e74cf267dc4da9eefb5`  
		Last Modified: Tue, 13 Oct 2020 08:43:16 GMT  
		Size: 1.4 MB (1376064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88909a533f0874c5c21c81c5a7ec8633dd223450c26ed2cbf8e8fc3ce43a9d31`  
		Last Modified: Tue, 27 Oct 2020 18:04:19 GMT  
		Size: 9.2 MB (9219447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3222b5772ffbe671d3743bf45872d86ee0a373818b5daa0984b11b781c51801`  
		Last Modified: Tue, 27 Oct 2020 18:04:17 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1680390e5b4099a6a538891ea22a713bd3bb846a978d12e011f2caf28776e106`  
		Last Modified: Tue, 27 Oct 2020 18:04:17 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-buster` - linux; arm variant v7

```console
$ docker pull redis@sha256:c7d716c5879df8cb357009d09cc6e1d969f7abe0eb5ba2cf3893da0ace2bf8e5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.1 MB (33054581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6afef9e2c5e4cfbce682869cae09af1059ee5ecf2709859d5cb8947a9c5730a4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Tue, 13 Oct 2020 00:59:29 GMT
ADD file:e423f30ca19eb205a98de21b0545d0a764cfc4f832a9a9631542354d914d98d9 in / 
# Tue, 13 Oct 2020 00:59:31 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 21:24:10 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Tue, 13 Oct 2020 21:24:19 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 21:25:39 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 27 Oct 2020 18:13:34 GMT
ENV REDIS_VERSION=6.0.9
# Tue, 27 Oct 2020 18:13:34 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.9.tar.gz
# Tue, 27 Oct 2020 18:13:35 GMT
ENV REDIS_DOWNLOAD_SHA=dc2bdcf81c620e9f09cfd12e85d3bc631c897b2db7a55218fd8a65eaa37f86dd
# Tue, 27 Oct 2020 18:14:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Tue, 27 Oct 2020 18:14:43 GMT
RUN mkdir /data && chown redis:redis /data
# Tue, 27 Oct 2020 18:14:44 GMT
VOLUME [/data]
# Tue, 27 Oct 2020 18:14:45 GMT
WORKDIR /data
# Tue, 27 Oct 2020 18:14:45 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Tue, 27 Oct 2020 18:14:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 27 Oct 2020 18:14:46 GMT
EXPOSE 6379
# Tue, 27 Oct 2020 18:14:47 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:d6d8411ad43db0022fa0fce094cd2e8b1dd2f8a09d6880ed9beb6b4204867027`  
		Last Modified: Tue, 13 Oct 2020 01:08:28 GMT  
		Size: 22.7 MB (22699849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574e3b674d93eb973c4e7995adb453df6cc957d269af7c586edfcd4579cd3631`  
		Last Modified: Tue, 13 Oct 2020 21:35:41 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0588f32eba23951704a21a3e87340a4e476a34af2f520eea3ca0b8be755d8062`  
		Last Modified: Tue, 13 Oct 2020 21:35:42 GMT  
		Size: 1.4 MB (1368174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b811e3cd5121a480b30560cb0b014ee45a45eb11f83850a057a45177aa9bf96a`  
		Last Modified: Tue, 27 Oct 2020 18:18:36 GMT  
		Size: 9.0 MB (8984286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbb4e68c317b3205aa9d60546b415afc23ffb4694519131afc0f3cbbdbf9b774`  
		Last Modified: Tue, 27 Oct 2020 18:18:33 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00212e6b62741a94c60393c1a48a463ac4cef6b602b2d4f3b56c6789608d2660`  
		Last Modified: Tue, 27 Oct 2020 18:18:34 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-buster` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:2f6d224aec3045a18ba7daa5920fe10bf0ae973e8309d57d922892322a950f04
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.8 MB (36771801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c123aa3694abab0f738cfff0e131d743ee5e9076762b3d1e5deefdebb786601b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Tue, 13 Oct 2020 01:41:09 GMT
ADD file:3488b1423094a75be5bb5956e9187827b8dd35d7a1f2b14081f8e74a1629e7d0 in / 
# Tue, 13 Oct 2020 01:41:11 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 18:33:24 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Tue, 13 Oct 2020 18:33:34 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 18:34:13 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 27 Oct 2020 18:12:48 GMT
ENV REDIS_VERSION=6.0.9
# Tue, 27 Oct 2020 18:12:48 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.9.tar.gz
# Tue, 27 Oct 2020 18:12:49 GMT
ENV REDIS_DOWNLOAD_SHA=dc2bdcf81c620e9f09cfd12e85d3bc631c897b2db7a55218fd8a65eaa37f86dd
# Tue, 27 Oct 2020 18:13:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Tue, 27 Oct 2020 18:13:59 GMT
RUN mkdir /data && chown redis:redis /data
# Tue, 27 Oct 2020 18:14:00 GMT
VOLUME [/data]
# Tue, 27 Oct 2020 18:14:00 GMT
WORKDIR /data
# Tue, 27 Oct 2020 18:14:01 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Tue, 27 Oct 2020 18:14:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 27 Oct 2020 18:14:02 GMT
EXPOSE 6379
# Tue, 27 Oct 2020 18:14:03 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:4e6164a63b7b4cf981546947e191644c122214975d40b51ede0536791ebec3d4`  
		Last Modified: Tue, 13 Oct 2020 01:48:17 GMT  
		Size: 25.8 MB (25849329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a6505e9bfd4801e90be2f8cac431ca10c79d96ada2ffda18b22d4f2b081840`  
		Last Modified: Tue, 13 Oct 2020 18:39:12 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb4766a9fc5330ef8de41a63ceb1c85eeca3a536770e466ade0a018d5c902494`  
		Last Modified: Tue, 13 Oct 2020 18:39:12 GMT  
		Size: 1.4 MB (1352913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56b3977748bf4eb55df6a68ae4dea95a6b3f998cbac37299618f6deebbb0cd5a`  
		Last Modified: Tue, 27 Oct 2020 18:18:28 GMT  
		Size: 9.6 MB (9567278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a858349766d4d246ef9d9cb699e6dd1c0909292f88792d33f06f309c7cd7a61c`  
		Last Modified: Tue, 27 Oct 2020 18:18:25 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5df6354e9527bd5ebc88988ce01e3674c9efd5103affc172aa27cf08c02011c`  
		Last Modified: Tue, 27 Oct 2020 18:18:25 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-buster` - linux; 386

```console
$ docker pull redis@sha256:d60f25da041c0f27b499ab65edac89462b997f16d70a1326de347b0285e62e8d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.5 MB (38453441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b20c81d64b0c714b77a3400605ea1895b60b41a0477c40b27fa1fa60642450fa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Tue, 13 Oct 2020 01:41:03 GMT
ADD file:51108b89c70ce0773c897be520c84454660f38b84ba556da49c7fe77e5d52416 in / 
# Tue, 13 Oct 2020 01:41:03 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 20:15:39 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Tue, 13 Oct 2020 20:15:39 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 20:15:53 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 20:15:53 GMT
ENV REDIS_VERSION=6.0.8
# Tue, 13 Oct 2020 20:15:54 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.8.tar.gz
# Tue, 13 Oct 2020 20:15:54 GMT
ENV REDIS_DOWNLOAD_SHA=04fa1fddc39bd1aecb6739dd5dd73858a3515b427acd1e2947a66dadce868d68
# Mon, 26 Oct 2020 23:46:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Mon, 26 Oct 2020 23:46:49 GMT
RUN mkdir /data && chown redis:redis /data
# Mon, 26 Oct 2020 23:46:49 GMT
VOLUME [/data]
# Mon, 26 Oct 2020 23:46:49 GMT
WORKDIR /data
# Mon, 26 Oct 2020 23:46:50 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Mon, 26 Oct 2020 23:46:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 26 Oct 2020 23:46:50 GMT
EXPOSE 6379
# Mon, 26 Oct 2020 23:46:50 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:97e4efec21eea92209464547d0f52a0f773c505cf4ea9d8090cef667bde145b8`  
		Last Modified: Tue, 13 Oct 2020 01:48:54 GMT  
		Size: 27.8 MB (27750243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b3c3b3d4e931d6652f25eb5e9798ebe6983865347d97b347c7c642aec2b0f3`  
		Last Modified: Tue, 13 Oct 2020 20:19:59 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbd1a88e6706dc9279ab8bb31e8ba3d07df802b563a6a893852154de87c16553`  
		Last Modified: Tue, 13 Oct 2020 20:19:59 GMT  
		Size: 1.4 MB (1387437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:088861f24af5a799e36b3babb94bca7f533258a3c3bc24ecf3b0b17654012ea3`  
		Last Modified: Mon, 26 Oct 2020 23:52:07 GMT  
		Size: 9.3 MB (9313527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29187cf9a67f6270a2efd670329e7a506efa49cc550926542bffeb48568a72fe`  
		Last Modified: Mon, 26 Oct 2020 23:52:05 GMT  
		Size: 98.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62ccf131085e2d3261ee4dece34857d03507b9be126e69f6d7957752bd66582c`  
		Last Modified: Mon, 26 Oct 2020 23:52:05 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-buster` - linux; mips64le

```console
$ docker pull redis@sha256:881dadc43820c9d82809e5ca5f7c1d3d0fc9a0fba79d609ce0aeab57653b9756
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.6 MB (36628870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1444c29fe2fb1f1233991eb5e7d486a036b95448df8865d0273cc8c73742e857`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Tue, 13 Oct 2020 01:09:50 GMT
ADD file:c2ad270f70511601478158cfe3854499c0b4887f049b78b66903412a811a428a in / 
# Tue, 13 Oct 2020 01:09:50 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 14:59:15 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Tue, 13 Oct 2020 14:59:15 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 14:59:42 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 14:59:42 GMT
ENV REDIS_VERSION=6.0.8
# Tue, 13 Oct 2020 14:59:42 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.8.tar.gz
# Tue, 13 Oct 2020 14:59:43 GMT
ENV REDIS_DOWNLOAD_SHA=04fa1fddc39bd1aecb6739dd5dd73858a3515b427acd1e2947a66dadce868d68
# Mon, 26 Oct 2020 23:14:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Mon, 26 Oct 2020 23:14:05 GMT
RUN mkdir /data && chown redis:redis /data
# Mon, 26 Oct 2020 23:14:05 GMT
VOLUME [/data]
# Mon, 26 Oct 2020 23:14:05 GMT
WORKDIR /data
# Mon, 26 Oct 2020 23:14:06 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Mon, 26 Oct 2020 23:14:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 26 Oct 2020 23:14:06 GMT
EXPOSE 6379
# Mon, 26 Oct 2020 23:14:07 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:9bc77d453b2242ec513032b61e23061712b79c3ba0c60114232d743e5ab4e4fa`  
		Last Modified: Tue, 13 Oct 2020 01:16:41 GMT  
		Size: 25.8 MB (25762577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1e078bf8ea454ce2b5aed1c76c6717abef31d5970ae1b88421c727dfe2ce71`  
		Last Modified: Tue, 13 Oct 2020 15:05:48 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c31e6c84861ed98c67f35b0286563f565765aacf384b2a3c2e7235d79407b816`  
		Last Modified: Tue, 13 Oct 2020 15:05:49 GMT  
		Size: 1.3 MB (1305404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fba8a808063b2f937b0a7a3627edd009faa92496afccf804f19f6c3242a3440`  
		Last Modified: Mon, 26 Oct 2020 23:17:41 GMT  
		Size: 9.6 MB (9558649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:212e5e948f3ca5673ad04c92f035f40a54f8c558b00e43e9f7015036991713cc`  
		Last Modified: Mon, 26 Oct 2020 23:17:33 GMT  
		Size: 98.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2bbadfa17c73e3b6eda7808530a3dcd60ab2b1664fc1f0c3fe492c65cc41194`  
		Last Modified: Mon, 26 Oct 2020 23:17:33 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-buster` - linux; ppc64le

```console
$ docker pull redis@sha256:0c2dd3ad8416bc55a6f1fee2eff9b099ad8d1c79c016cdf76579bc15dc3a9a4e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42144013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b54fe27b2f91a18225be2872725794ee70bd28af21c256e3805f20e37ffcb3b3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Tue, 13 Oct 2020 01:38:54 GMT
ADD file:9992867f855c9bed54df6d26f3d8076689aff8a51e808fefba7d3b66dab250e5 in / 
# Tue, 13 Oct 2020 01:38:59 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 15:18:48 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Tue, 13 Oct 2020 15:18:54 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 15:21:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 13 Oct 2020 15:21:16 GMT
ENV REDIS_VERSION=6.0.8
# Tue, 13 Oct 2020 15:21:20 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.8.tar.gz
# Tue, 13 Oct 2020 15:21:26 GMT
ENV REDIS_DOWNLOAD_SHA=04fa1fddc39bd1aecb6739dd5dd73858a3515b427acd1e2947a66dadce868d68
# Mon, 26 Oct 2020 23:39:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Mon, 26 Oct 2020 23:39:16 GMT
RUN mkdir /data && chown redis:redis /data
# Mon, 26 Oct 2020 23:39:18 GMT
VOLUME [/data]
# Mon, 26 Oct 2020 23:39:21 GMT
WORKDIR /data
# Mon, 26 Oct 2020 23:39:23 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Mon, 26 Oct 2020 23:39:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 26 Oct 2020 23:39:28 GMT
EXPOSE 6379
# Mon, 26 Oct 2020 23:39:30 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:523555c6877c72cfcdec912b4d0053c298b1c97835efc7c6b0211585a06bd563`  
		Last Modified: Tue, 13 Oct 2020 01:50:10 GMT  
		Size: 30.5 MB (30517878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c2219729d68aa80b9d2e65733258d633138e027f7771baffb586ee244a6f122`  
		Last Modified: Tue, 13 Oct 2020 15:30:16 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:addc9854ce7a36c25eabc3d95eccda05163da71237c40b0aed41ae9b201375e6`  
		Last Modified: Tue, 13 Oct 2020 15:30:17 GMT  
		Size: 1.3 MB (1335389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cda9c686196a58b2a36a6b7e66ab8dfaf62316d6cb7143362f97f271c554a408`  
		Last Modified: Mon, 26 Oct 2020 23:47:24 GMT  
		Size: 10.3 MB (10288462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ddd169104c0f2f1e825bb02f3e629982ecf684a9578e2376a859a5a59fb117`  
		Last Modified: Mon, 26 Oct 2020 23:47:22 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a886bfee8df23a17ba1d7327df57ce9f3b25b5a117aaf32b72e55a7833a81fed`  
		Last Modified: Mon, 26 Oct 2020 23:47:22 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-buster` - linux; s390x

```console
$ docker pull redis@sha256:aab13b71ae7a5c4e25c9390c970a7f742551e95a2c864b513a39ba109d7cf318
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.8 MB (36817656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:841846e159e8dbc0814f0880c9d5bcee4c67df50d0ce0d7b054e4db268ba767e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Tue, 13 Oct 2020 01:42:26 GMT
ADD file:f932c1176fdc9bf45ced816290f83e6231df3dffa3b7f8de1a3bb0adcff1588b in / 
# Tue, 13 Oct 2020 01:42:27 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 05:48:26 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Tue, 13 Oct 2020 05:48:27 GMT
ENV GOSU_VERSION=1.12
# Tue, 13 Oct 2020 05:48:46 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 27 Oct 2020 18:09:26 GMT
ENV REDIS_VERSION=6.0.9
# Tue, 27 Oct 2020 18:09:26 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.0.9.tar.gz
# Tue, 27 Oct 2020 18:09:26 GMT
ENV REDIS_DOWNLOAD_SHA=dc2bdcf81c620e9f09cfd12e85d3bc631c897b2db7a55218fd8a65eaa37f86dd
# Tue, 27 Oct 2020 18:10:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Tue, 27 Oct 2020 18:10:10 GMT
RUN mkdir /data && chown redis:redis /data
# Tue, 27 Oct 2020 18:10:11 GMT
VOLUME [/data]
# Tue, 27 Oct 2020 18:10:11 GMT
WORKDIR /data
# Tue, 27 Oct 2020 18:10:11 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Tue, 27 Oct 2020 18:10:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 27 Oct 2020 18:10:12 GMT
EXPOSE 6379
# Tue, 27 Oct 2020 18:10:12 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:2a4f9dc00d797c86c4ffce3b50bea9037c2eb4637f045ad3fd68cf151577b639`  
		Last Modified: Tue, 13 Oct 2020 01:45:45 GMT  
		Size: 25.7 MB (25707519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4ae546ec87bc1a8e334b8f0ccd654f12dcb0062b9f4e42bad1a396f51b31fca`  
		Last Modified: Tue, 13 Oct 2020 05:50:56 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75caa05d2c720f15c7b6e7f7b8aadc217725f0c49e4def1b04401d6fb94f48ff`  
		Last Modified: Tue, 13 Oct 2020 05:50:56 GMT  
		Size: 1.4 MB (1403770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47d288b14ca133920cc309f996cefa8f634742a903b8099936633966892e5cc`  
		Last Modified: Tue, 27 Oct 2020 18:13:32 GMT  
		Size: 9.7 MB (9704086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c8b1bfe6099fef9c0be57847b0ce74afc620ed40b69ef7eff6219a0354d347`  
		Last Modified: Tue, 27 Oct 2020 18:13:30 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:683e770c0badcb563323717331bf9aa53fd1859b4ae3edede9fe889a9a876686`  
		Last Modified: Tue, 27 Oct 2020 18:13:29 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
