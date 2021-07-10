## `redis:6-buster`

```console
$ docker pull redis@sha256:2d231464dcde0fc79ddc4631b3b73f82ca5af7557e4de4d034fcc306a188feea
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
$ docker pull redis@sha256:87204a944dc825e2e17019dc438886d4d2b5de2862686c5d69cbc015fd0488d7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.7 MB (38681062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08502081bff61084d64fc76f0f90ea39b89935cd071d9e12c5374ae191ff53c0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 16:35:00 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Wed, 23 Jun 2021 16:35:01 GMT
ENV GOSU_VERSION=1.12
# Wed, 23 Jun 2021 16:35:26 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 23 Jun 2021 16:35:26 GMT
ENV REDIS_VERSION=6.2.4
# Wed, 23 Jun 2021 16:35:26 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.4.tar.gz
# Wed, 23 Jun 2021 16:35:26 GMT
ENV REDIS_DOWNLOAD_SHA=ba32c406a10fc2c09426e2be2787d74ff204eb3a2e496d87cff76a476b6ae16e
# Wed, 23 Jun 2021 16:36:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Wed, 23 Jun 2021 16:36:28 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 23 Jun 2021 16:36:29 GMT
VOLUME [/data]
# Wed, 23 Jun 2021 16:36:29 GMT
WORKDIR /data
# Wed, 23 Jun 2021 16:36:29 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Wed, 23 Jun 2021 16:36:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 16:36:29 GMT
EXPOSE 6379
# Wed, 23 Jun 2021 16:36:30 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86e428f79bcb3c3a51693c7ba2d759530ddd94299606b53032970d0ca3536440`  
		Last Modified: Wed, 23 Jun 2021 16:41:20 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba0d0a0258101b9bdb292dbded947c7ebc3e7179b14de4fee0280e5e6d9b70ce`  
		Last Modified: Wed, 23 Jun 2021 16:41:20 GMT  
		Size: 1.4 MB (1417969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9292c6f77e5ba12b6019af4ab83d5397bcc165550c96abc2eadc1c60d393f0`  
		Last Modified: Wed, 23 Jun 2021 16:41:22 GMT  
		Size: 10.1 MB (10114968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96c0d1da6029a40b57803657fd92385856b618ebb58255b6fd6c6ddf831953e`  
		Last Modified: Wed, 23 Jun 2021 16:41:20 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e4b46455da315e461e249f56fead770361f4c753fa6c993029da4ad5afcf722`  
		Last Modified: Wed, 23 Jun 2021 16:41:20 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-buster` - linux; arm variant v5

```console
$ docker pull redis@sha256:26e0567dca9c576cca449a1bfa1eaf2ade1b03391512b27d7e33a57b00448035
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35878632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0d98f0dd7a8f823e557abfaf435955e9a0c36eee587f46aa7e2c3f2d2c73428`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Tue, 22 Jun 2021 23:50:09 GMT
ADD file:78d4ced31112d85490c684f350aceeebfc72a804262c7ad3e033257e3894f5c4 in / 
# Tue, 22 Jun 2021 23:50:11 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 08:53:19 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Wed, 23 Jun 2021 08:53:20 GMT
ENV GOSU_VERSION=1.12
# Wed, 23 Jun 2021 08:53:50 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 23 Jun 2021 08:53:51 GMT
ENV REDIS_VERSION=6.2.4
# Wed, 23 Jun 2021 08:53:51 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.4.tar.gz
# Wed, 23 Jun 2021 08:53:52 GMT
ENV REDIS_DOWNLOAD_SHA=ba32c406a10fc2c09426e2be2787d74ff204eb3a2e496d87cff76a476b6ae16e
# Wed, 23 Jun 2021 08:55:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Wed, 23 Jun 2021 08:55:29 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 23 Jun 2021 08:55:30 GMT
VOLUME [/data]
# Wed, 23 Jun 2021 08:55:30 GMT
WORKDIR /data
# Wed, 23 Jun 2021 08:55:31 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Wed, 23 Jun 2021 08:55:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 08:55:32 GMT
EXPOSE 6379
# Wed, 23 Jun 2021 08:55:32 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:532d6df30af5174ac6e1b379c32b8f464d44651ac060376a560c4a76a87704a7`  
		Last Modified: Wed, 23 Jun 2021 00:01:46 GMT  
		Size: 24.9 MB (24878945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5962b6323fa14cf23ca9480096cb5c2d12ed4044ba5c6d44677855aabacde85`  
		Last Modified: Wed, 23 Jun 2021 09:00:49 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81bcd1849e7815d429a3279ea092ccb7f2833400ffa8fc9a8f132c63ec92bf28`  
		Last Modified: Wed, 23 Jun 2021 09:00:50 GMT  
		Size: 1.4 MB (1376228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f4617de75cb0ca805d646abceb99d97e497b5c6dc3b6ce53c561a591e4adcc7`  
		Last Modified: Wed, 23 Jun 2021 09:00:56 GMT  
		Size: 9.6 MB (9621193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471a252d7fd20549e2e59aa9453fbc82b9728b9b9a6a0358cb4b24f610422c0d`  
		Last Modified: Wed, 23 Jun 2021 09:00:49 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8546cea7524de1363f2b74697e2d6f506f38275ca862f821f175a55676c9e45f`  
		Last Modified: Wed, 23 Jun 2021 09:00:49 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-buster` - linux; arm variant v7

```console
$ docker pull redis@sha256:63cd2aeeb92a36bb3ebca995ba74d74e58fa588dd0e12797c0720968e5a90f6c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33496272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df0b976e6584195a5abf8969502c13de24e16d17a4e446aa8dca0c2a273d1460`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:31 GMT
ADD file:8d200a3bbe985ff355343675c5555852f27550a9e367969df6bc98034efb8fd4 in / 
# Wed, 23 Jun 2021 00:20:31 GMT
CMD ["bash"]
# Thu, 24 Jun 2021 07:07:45 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 24 Jun 2021 07:07:46 GMT
ENV GOSU_VERSION=1.12
# Thu, 24 Jun 2021 07:08:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 24 Jun 2021 07:08:15 GMT
ENV REDIS_VERSION=6.2.4
# Thu, 24 Jun 2021 07:08:15 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.4.tar.gz
# Thu, 24 Jun 2021 07:08:15 GMT
ENV REDIS_DOWNLOAD_SHA=ba32c406a10fc2c09426e2be2787d74ff204eb3a2e496d87cff76a476b6ae16e
# Thu, 24 Jun 2021 07:09:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 24 Jun 2021 07:09:47 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 24 Jun 2021 07:09:48 GMT
VOLUME [/data]
# Thu, 24 Jun 2021 07:09:48 GMT
WORKDIR /data
# Thu, 24 Jun 2021 07:09:49 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 24 Jun 2021 07:09:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Jun 2021 07:09:49 GMT
EXPOSE 6379
# Thu, 24 Jun 2021 07:09:50 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:8452be1adf00f91570fe21a8e61aaf4c12e014daf67d7de65d984f4e8ecca2f1`  
		Last Modified: Wed, 23 Jun 2021 00:31:49 GMT  
		Size: 22.7 MB (22746055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa4e6aa3026b7ee1d9e897f724c841a133a268a887e189c1fd687596045f295`  
		Last Modified: Thu, 24 Jun 2021 07:20:48 GMT  
		Size: 1.7 KB (1722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a70dd0d5948c481f522bae9d8fb2ced7b9a24ccedd87557fe202fdb7f34bef`  
		Last Modified: Thu, 24 Jun 2021 07:20:49 GMT  
		Size: 1.4 MB (1368334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93cf8c194e6470eb34c1f93cd95e6feea61d950f10abb42f1a69dcab5dbfe765`  
		Last Modified: Thu, 24 Jun 2021 07:20:54 GMT  
		Size: 9.4 MB (9379617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e73876ff6af81cd8255dbf5014a6c497d2e4bf22318963578ca05c0cd15f2d8b`  
		Last Modified: Thu, 24 Jun 2021 07:20:48 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b234c5b8b26962b7a60eca4086ed248a4e67ea2813dda65bebe3868422d4b88`  
		Last Modified: Thu, 24 Jun 2021 07:20:48 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-buster` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:c1c24ce3cfd45e9aa13bd57ca1d5d1ab8dbc0f9b56bd04eb5744d37d2469bac5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37263459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cad8cf27ff34c620e208a2fafd6e6dc487f46ea02ba7ba2d21220a698e1d674a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:40 GMT
ADD file:beee00b59da720f68e12e2ba2a8134207c80c777ddb4ceb03c71e3e4c3f51c93 in / 
# Tue, 22 Jun 2021 23:49:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 12:45:39 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Wed, 23 Jun 2021 12:45:39 GMT
ENV GOSU_VERSION=1.12
# Wed, 23 Jun 2021 12:45:55 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 23 Jun 2021 12:45:55 GMT
ENV REDIS_VERSION=6.2.4
# Wed, 23 Jun 2021 12:45:55 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.4.tar.gz
# Wed, 23 Jun 2021 12:45:55 GMT
ENV REDIS_DOWNLOAD_SHA=ba32c406a10fc2c09426e2be2787d74ff204eb3a2e496d87cff76a476b6ae16e
# Wed, 23 Jun 2021 12:46:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Wed, 23 Jun 2021 12:46:42 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 23 Jun 2021 12:46:42 GMT
VOLUME [/data]
# Wed, 23 Jun 2021 12:46:42 GMT
WORKDIR /data
# Wed, 23 Jun 2021 12:46:42 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Wed, 23 Jun 2021 12:46:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 12:46:43 GMT
EXPOSE 6379
# Wed, 23 Jun 2021 12:46:43 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:448f6bf000e31217a7c202c659b03b7f8ac8d3ae6b03ef7a2f8339be2f00ff4a`  
		Last Modified: Tue, 22 Jun 2021 23:55:25 GMT  
		Size: 25.9 MB (25914993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1563d96d61100146ffade014fdd0cd089e3954e30d017c5e05237af88f30d86`  
		Last Modified: Wed, 23 Jun 2021 12:50:26 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39898690e366ac2c1fa9e0222407bd019fa76098f28772ca5b89bebeb2a79c88`  
		Last Modified: Wed, 23 Jun 2021 12:50:27 GMT  
		Size: 1.4 MB (1352992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c1f534c176dbc460cee3a32b63a10c83f08131f8e5a959d3f9387a7188acdd`  
		Last Modified: Wed, 23 Jun 2021 12:50:29 GMT  
		Size: 10.0 MB (9993198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:677225c5285bdb3afddf940c1b141bf19db8057d5d0ecb085b903c2649be2a34`  
		Last Modified: Wed, 23 Jun 2021 12:50:26 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f57391477f5117aca72c5c13d658e3dec17d6818f4d8bc4bb45978a2402a28d5`  
		Last Modified: Wed, 23 Jun 2021 12:50:27 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-buster` - linux; 386

```console
$ docker pull redis@sha256:6a855045a9e9306416f59b101b005d08104e99e57ebfbfe51f0184829365f6c5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.9 MB (38924964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3cbb4e8700f03c69727878c1af0995aed18a8bfe69967e071ea40e0785fefaf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Tue, 22 Jun 2021 23:39:35 GMT
ADD file:48f656ac6733911048b3de850490438d0233b3badc11861fca62062d4edfaf40 in / 
# Tue, 22 Jun 2021 23:39:35 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 13:19:37 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Wed, 23 Jun 2021 13:19:37 GMT
ENV GOSU_VERSION=1.12
# Wed, 23 Jun 2021 13:19:58 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 23 Jun 2021 13:19:58 GMT
ENV REDIS_VERSION=6.2.4
# Wed, 23 Jun 2021 13:19:59 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.4.tar.gz
# Wed, 23 Jun 2021 13:19:59 GMT
ENV REDIS_DOWNLOAD_SHA=ba32c406a10fc2c09426e2be2787d74ff204eb3a2e496d87cff76a476b6ae16e
# Wed, 23 Jun 2021 13:21:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Wed, 23 Jun 2021 13:21:09 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 23 Jun 2021 13:21:10 GMT
VOLUME [/data]
# Wed, 23 Jun 2021 13:21:10 GMT
WORKDIR /data
# Wed, 23 Jun 2021 13:21:10 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Wed, 23 Jun 2021 13:21:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 13:21:11 GMT
EXPOSE 6379
# Wed, 23 Jun 2021 13:21:11 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:33af2dcb865e65d53cdeb843b67a0ef62151fa32df292293e7c6b0eb728ac5ac`  
		Last Modified: Tue, 22 Jun 2021 23:46:23 GMT  
		Size: 27.8 MB (27797411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10dda5366e4f224e40b98dadb46e3b952f849dee82ff949fe5ed280f10340e5`  
		Last Modified: Wed, 23 Jun 2021 13:26:22 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfd652d72ae3793a2a8950dd11d131c01c81922b71a752aa90c08ddd96530e5a`  
		Last Modified: Wed, 23 Jun 2021 13:26:23 GMT  
		Size: 1.4 MB (1387649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a065ec216b322aefcf374779c52c4eb1cc40d22d1ccd948f37946282f537a102`  
		Last Modified: Wed, 23 Jun 2021 13:26:25 GMT  
		Size: 9.7 MB (9737636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0283a9e2b3efb137e65c6a0629d255e76ccfad3318526a3f5c17bfc4670082c`  
		Last Modified: Wed, 23 Jun 2021 13:26:23 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f9ba1ceade79e6354690ab32a4775e7839a10324b16e045cd125e3aa8e9501`  
		Last Modified: Wed, 23 Jun 2021 13:26:22 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-buster` - linux; mips64le

```console
$ docker pull redis@sha256:97786c9f705d658af1d8e06ebe9bb551495af786e9ca860cd36f351c044ebf1c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.1 MB (37129751 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcb97679e7caf2c8faf8dfbe7f950c653b76f9c9ddb2a4908c151321cd21055c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 23 Jun 2021 00:09:29 GMT
ADD file:ca8422268fc66c67d19fd3a33a14a9bd6280ef21404677767ffd561a8ecf6724 in / 
# Wed, 23 Jun 2021 00:09:30 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 16:35:08 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Wed, 23 Jun 2021 16:35:09 GMT
ENV GOSU_VERSION=1.12
# Wed, 23 Jun 2021 16:35:35 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 23 Jun 2021 16:35:35 GMT
ENV REDIS_VERSION=6.2.4
# Wed, 23 Jun 2021 16:35:35 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.4.tar.gz
# Wed, 23 Jun 2021 16:35:35 GMT
ENV REDIS_DOWNLOAD_SHA=ba32c406a10fc2c09426e2be2787d74ff204eb3a2e496d87cff76a476b6ae16e
# Wed, 23 Jun 2021 16:38:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Wed, 23 Jun 2021 16:38:39 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 23 Jun 2021 16:38:39 GMT
VOLUME [/data]
# Wed, 23 Jun 2021 16:38:39 GMT
WORKDIR /data
# Wed, 23 Jun 2021 16:38:40 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Wed, 23 Jun 2021 16:38:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 16:38:40 GMT
EXPOSE 6379
# Wed, 23 Jun 2021 16:38:40 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:4b9d1870c33c63bfde89c401b4af9582fbbff99d4036171a7a456706bf805d6d`  
		Last Modified: Wed, 23 Jun 2021 00:15:49 GMT  
		Size: 25.8 MB (25812890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d181ed90f23c743de8654456a879573ce360882b14612c989081edd209cc16`  
		Last Modified: Wed, 23 Jun 2021 16:45:13 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2678054ec82e66ce71e80892634395e84858b128f43f68527e70cda843fe2db4`  
		Last Modified: Wed, 23 Jun 2021 16:45:14 GMT  
		Size: 1.3 MB (1305641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45270e08f8aebdcf58dbf0fe3b20a181d04fb6580847b4329e3be7002d38e81f`  
		Last Modified: Wed, 23 Jun 2021 16:45:21 GMT  
		Size: 10.0 MB (10008981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eef98488d893fbef7e1aa24d115b8234afacc0865aa58d59c00ad73eb1ebd01`  
		Last Modified: Wed, 23 Jun 2021 16:45:13 GMT  
		Size: 97.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bac1cc82bc012ca330a81a322dda53a626b50ff503303e74c8eb6ec06b980b3`  
		Last Modified: Wed, 23 Jun 2021 16:45:13 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-buster` - linux; ppc64le

```console
$ docker pull redis@sha256:7df22b25ff1cb76cd66e8d49b4adc2eb20275d62c82e616d4c37bf7a659f31f0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.6 MB (42644003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c0b4d39429822b159cc3a822e3a958d138c3e036373be7ee15339c7facf057c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 23 Jun 2021 00:30:38 GMT
ADD file:e599654230c9fe95fe2c591dbe60e8a0a886cd053b6117230fbae47561145731 in / 
# Wed, 23 Jun 2021 00:30:46 GMT
CMD ["bash"]
# Thu, 08 Jul 2021 17:17:26 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 08 Jul 2021 17:17:34 GMT
ENV GOSU_VERSION=1.12
# Thu, 08 Jul 2021 17:19:44 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 08 Jul 2021 17:19:52 GMT
ENV REDIS_VERSION=6.2.4
# Thu, 08 Jul 2021 17:19:57 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.4.tar.gz
# Thu, 08 Jul 2021 17:20:01 GMT
ENV REDIS_DOWNLOAD_SHA=ba32c406a10fc2c09426e2be2787d74ff204eb3a2e496d87cff76a476b6ae16e
# Thu, 08 Jul 2021 17:23:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 08 Jul 2021 17:24:07 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 08 Jul 2021 17:24:09 GMT
VOLUME [/data]
# Thu, 08 Jul 2021 17:24:12 GMT
WORKDIR /data
# Thu, 08 Jul 2021 17:24:16 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 08 Jul 2021 17:24:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 17:24:22 GMT
EXPOSE 6379
# Thu, 08 Jul 2021 17:24:26 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:f9cb1946299ce1824ee44809cd0c8b419528fee2f0f89e86400787a14b666f59`  
		Last Modified: Wed, 23 Jun 2021 00:37:07 GMT  
		Size: 30.6 MB (30553627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8f8fa75078ed0168a19669dd6391a9f19e0c7464a9ca89a7697ad4c4a69f25`  
		Last Modified: Thu, 08 Jul 2021 17:40:36 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0758d61c0fb1eadcca2becf530af874142ff63591ce5086789ee305622eb90f7`  
		Last Modified: Thu, 08 Jul 2021 17:40:37 GMT  
		Size: 1.3 MB (1335592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b918aab713df7f402ae80fbf6523477910fa9246392593483e7b824fd145f0b`  
		Last Modified: Thu, 08 Jul 2021 17:40:39 GMT  
		Size: 10.8 MB (10752498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5922a144a4e086dbddbf2e9cb71c509b1a0096af20192d2d72d9696672fdae4e`  
		Last Modified: Thu, 08 Jul 2021 17:40:36 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3adf417bed1678493e234e9b862370253d845ec6d94c2a84c9af699a87a135e9`  
		Last Modified: Thu, 08 Jul 2021 17:40:36 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:6-buster` - linux; s390x

```console
$ docker pull redis@sha256:41320ff1574da56288c728368eb714417929e19d58abba42818a42acc438420b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37298057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c429c2b089c2e18ca4bf41e87f15416d217efc93e4c6fe101a11ec3a2102d20f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Fri, 09 Jul 2021 02:50:32 GMT
ADD file:a53e5772eefa4592eeff989f279dcc870986db7207b419dc3ae61cae85fce41f in / 
# Fri, 09 Jul 2021 02:50:33 GMT
CMD ["bash"]
# Fri, 09 Jul 2021 20:40:19 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Fri, 09 Jul 2021 20:40:19 GMT
ENV GOSU_VERSION=1.12
# Fri, 09 Jul 2021 20:40:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 09 Jul 2021 20:40:46 GMT
ENV REDIS_VERSION=6.2.4
# Fri, 09 Jul 2021 20:40:47 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.4.tar.gz
# Fri, 09 Jul 2021 20:40:47 GMT
ENV REDIS_DOWNLOAD_SHA=ba32c406a10fc2c09426e2be2787d74ff204eb3a2e496d87cff76a476b6ae16e
# Fri, 09 Jul 2021 20:42:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Fri, 09 Jul 2021 20:42:10 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 09 Jul 2021 20:42:11 GMT
VOLUME [/data]
# Fri, 09 Jul 2021 20:42:11 GMT
WORKDIR /data
# Fri, 09 Jul 2021 20:42:12 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Fri, 09 Jul 2021 20:42:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 09 Jul 2021 20:42:13 GMT
EXPOSE 6379
# Fri, 09 Jul 2021 20:42:14 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:d08eb187b3111e87e1b138f7b93df64c5470da613a64d0adc804e17e12aed4dc`  
		Last Modified: Tue, 22 Jun 2021 23:45:45 GMT  
		Size: 25.8 MB (25760716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24dc593ec181c3d059ba73276304f11d86cf0c7edb59f4630ccc9ea6528465d1`  
		Last Modified: Fri, 09 Jul 2021 20:53:48 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024c56561a653386678302b3a5423dcfa9b6cd895383c6a3aa404e37744f08af`  
		Last Modified: Fri, 09 Jul 2021 20:53:49 GMT  
		Size: 1.4 MB (1404000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fab98ee5d83ff90b5bc902c9fd696decab36b5149c65aa318a779e22a111690`  
		Last Modified: Fri, 09 Jul 2021 20:53:50 GMT  
		Size: 10.1 MB (10131061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:556d2375ee773af0a5c1f7e5067280029b53bc2cf228121b1336e53fe102b13e`  
		Last Modified: Fri, 09 Jul 2021 20:53:48 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82a3062293d5cd26988539e195116a6a0760c5481bf416bae52a5a1d6f84e223`  
		Last Modified: Fri, 09 Jul 2021 20:53:48 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
