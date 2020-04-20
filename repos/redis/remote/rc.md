## `redis:rc`

```console
$ docker pull redis@sha256:4abc3cba6b0cd54778c297d5fa58dea24823092085532259cca0e17c7bcb8957
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

### `redis:rc` - linux; amd64

```console
$ docker pull redis@sha256:fcc8b652810cf40ad043f677045589e1397334e1280747851e9b10d214710c74
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.1 MB (38142556 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a90241ac749e91f9f6dcede80d9fbc6b4608b773c12fb1bd9bae357e90d64fa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 16 Apr 2020 03:22:36 GMT
ADD file:865f9041e12eb341f0a394764ddc11db49cbc8b91d4fb57c6fb1960b68b1bb41 in / 
# Thu, 16 Apr 2020 03:22:36 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 20:53:59 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 16 Apr 2020 20:53:59 GMT
ENV GOSU_VERSION=1.12
# Thu, 16 Apr 2020 20:54:13 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 20 Apr 2020 18:31:54 GMT
ENV REDIS_VERSION=6.0-rc4
# Mon, 20 Apr 2020 18:31:54 GMT
ENV REDIS_DOWNLOAD_URL=https://github.com/antirez/redis/archive/6.0-rc4.tar.gz
# Mon, 20 Apr 2020 18:31:55 GMT
ENV REDIS_DOWNLOAD_SHA=dac1ad1253337c06adf2af7f6ec7d2f54371e6b37b3c3d1c9d8fb4b7713d12a7
# Mon, 20 Apr 2020 18:33:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Mon, 20 Apr 2020 18:33:07 GMT
RUN mkdir /data && chown redis:redis /data
# Mon, 20 Apr 2020 18:33:07 GMT
VOLUME [/data]
# Mon, 20 Apr 2020 18:33:07 GMT
WORKDIR /data
# Mon, 20 Apr 2020 18:33:08 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Mon, 20 Apr 2020 18:33:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 20 Apr 2020 18:33:08 GMT
EXPOSE 6379
# Mon, 20 Apr 2020 18:33:08 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:123275d6e508d282237a22fefa5aef822b719a06496444ea89efa65da523fc4b`  
		Last Modified: Thu, 16 Apr 2020 03:31:44 GMT  
		Size: 27.1 MB (27098147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2edbd6a658e04d559c1bec36d838006bbdcb39d8fb9033ed43d2014ac497774`  
		Last Modified: Thu, 16 Apr 2020 21:01:17 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66960bede47c1a193710cf8bfa7bf5f50bc46374260923df1db1c423b52153ac`  
		Last Modified: Thu, 16 Apr 2020 21:01:17 GMT  
		Size: 1.4 MB (1417708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009c94826ab1e05bfe7ce40fc44ef455f80ebc66acdb0cf510bdacf1a128cd27`  
		Last Modified: Mon, 20 Apr 2020 18:39:46 GMT  
		Size: 9.6 MB (9624462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:396cab04d9f902ad0373deef5877ea22b3785dcc041dee66c4e0cddb81533bcd`  
		Last Modified: Mon, 20 Apr 2020 18:39:44 GMT  
		Size: 98.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:146790184cc837ccc88d91d3f234e2869780810c5c351a8a9d0dbfae65851ca0`  
		Last Modified: Mon, 20 Apr 2020 18:39:44 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:rc` - linux; arm variant v5

```console
$ docker pull redis@sha256:fe03fdcfff8d3d657cb5b633323a93a1997fb776fb4f9412dbab7a33369d8d19
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.4 MB (35351761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:343d5a4c12538ab3a155bfefd5b7607d7d5599e9b7ab674d92013df0c93e1d2e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 16 Apr 2020 00:50:14 GMT
ADD file:761a556ec2a7d8c742c860e429c9b9ba3f7abfcd9383c6b3767499de6dcad4bc in / 
# Thu, 16 Apr 2020 00:50:15 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:59:29 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 16 Apr 2020 20:17:57 GMT
ENV GOSU_VERSION=1.12
# Thu, 16 Apr 2020 20:18:43 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 16 Apr 2020 20:18:45 GMT
ENV REDIS_VERSION=6.0-rc3
# Thu, 16 Apr 2020 20:18:45 GMT
ENV REDIS_DOWNLOAD_URL=https://github.com/antirez/redis/archive/6.0-rc3.tar.gz
# Thu, 16 Apr 2020 20:18:46 GMT
ENV REDIS_DOWNLOAD_SHA=a81f92ed0aeb2ecab1488ce916725da1283fa86c3ff43828430e77ce8e612534
# Thu, 16 Apr 2020 20:20:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 16 Apr 2020 20:20:08 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 16 Apr 2020 20:20:09 GMT
VOLUME [/data]
# Thu, 16 Apr 2020 20:20:10 GMT
WORKDIR /data
# Thu, 16 Apr 2020 20:20:11 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 16 Apr 2020 20:20:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Apr 2020 20:20:12 GMT
EXPOSE 6379
# Thu, 16 Apr 2020 20:20:13 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:600369660a591bc9594fcf333a847fe997901785f7032d3ad2822b2812c13243`  
		Last Modified: Thu, 16 Apr 2020 00:58:26 GMT  
		Size: 24.8 MB (24836437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:229376286c6540047b204d37150dcf019406869f7f4ff7a0ce2c085affd17c98`  
		Last Modified: Thu, 16 Apr 2020 07:06:43 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40abfc675fdacf8461c3a2e93c5808599a4464b87fbeb96eb0aaee04b74d94b0`  
		Last Modified: Thu, 16 Apr 2020 20:25:09 GMT  
		Size: 1.4 MB (1376090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7595a34901fbbf582fe8994e10abbd5a99791175dd13a053d4992ca5e2a6e700`  
		Last Modified: Thu, 16 Apr 2020 20:25:12 GMT  
		Size: 9.1 MB (9136967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b901ad6e3b1c92ffaa10c909632d755b0c4bf3b681297c6c0354cd879c9ccd7`  
		Last Modified: Thu, 16 Apr 2020 20:25:09 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b567c656b44f8cd65a248e437e5ff7955da018871cf20b8711c6b1f1ded124b2`  
		Last Modified: Thu, 16 Apr 2020 20:25:09 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:rc` - linux; arm variant v7

```console
$ docker pull redis@sha256:7a42f6a45f6bd05d76726fa09230f908cc59570360b44d91776ef5cc87e67f91
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32975742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:015e8e2172f3294c09a1eb2f6c51009215ec3a2f6149b98f0a0e919fb9288251`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 16 Apr 2020 00:59:45 GMT
ADD file:e346a36a456d66d8019344b5f7d60df8b5b24aea1461c19838982135ad1f4d7d in / 
# Thu, 16 Apr 2020 00:59:47 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 13:21:42 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Fri, 17 Apr 2020 08:27:23 GMT
ENV GOSU_VERSION=1.12
# Fri, 17 Apr 2020 08:27:53 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 17 Apr 2020 08:27:54 GMT
ENV REDIS_VERSION=6.0-rc3
# Fri, 17 Apr 2020 08:27:55 GMT
ENV REDIS_DOWNLOAD_URL=https://github.com/antirez/redis/archive/6.0-rc3.tar.gz
# Fri, 17 Apr 2020 08:27:56 GMT
ENV REDIS_DOWNLOAD_SHA=a81f92ed0aeb2ecab1488ce916725da1283fa86c3ff43828430e77ce8e612534
# Fri, 17 Apr 2020 08:29:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Fri, 17 Apr 2020 08:29:12 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 17 Apr 2020 08:29:13 GMT
VOLUME [/data]
# Fri, 17 Apr 2020 08:29:14 GMT
WORKDIR /data
# Fri, 17 Apr 2020 08:29:15 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Fri, 17 Apr 2020 08:29:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 17 Apr 2020 08:29:18 GMT
EXPOSE 6379
# Fri, 17 Apr 2020 08:29:19 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:838dc71644c10eab485c4bdfa3879e0fb9e72426de1239cfac1d4c05c23db7be`  
		Last Modified: Thu, 16 Apr 2020 01:08:59 GMT  
		Size: 22.7 MB (22705228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c62ce5bbe09f192518a9390c16060106ee5880db10ca593b8965ff3f14316886`  
		Last Modified: Thu, 16 Apr 2020 13:26:33 GMT  
		Size: 1.7 KB (1724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb881abf113b785134c66a0b49e2f10c633c42ddceb143e5e480d14072ea0c16`  
		Last Modified: Fri, 17 Apr 2020 08:33:17 GMT  
		Size: 1.4 MB (1368136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f064475e169ff0bf8faf124c32b0d91edf5213b6c1ac538e8b8d74638376cce`  
		Last Modified: Fri, 17 Apr 2020 08:33:20 GMT  
		Size: 8.9 MB (8900110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:939ed1b22b7546855e0245bb4c2696bb08dcdc9363988dc7f6558a9cfe5e98fa`  
		Last Modified: Fri, 17 Apr 2020 08:33:17 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:481a3e4caf8f68f97b50ee7172f061423ba88d1cab8b252fe332dac5d12c5ab8`  
		Last Modified: Fri, 17 Apr 2020 08:33:17 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:rc` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:3b99ad83be1a63878e040d3cde38e1625617426ebfbb0121d0f564a71df0ba13
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.7 MB (36699398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a179c89d93328f386acec008130042c9f53f758de43f900a3ebfacc1fd5a491b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 16 Apr 2020 02:41:52 GMT
ADD file:1aab17002a9095c31dd6928277a045cb26846ac58c3d2d63316332c99a5f90bd in / 
# Thu, 16 Apr 2020 02:41:57 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 18:59:21 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 16 Apr 2020 18:59:22 GMT
ENV GOSU_VERSION=1.12
# Thu, 16 Apr 2020 18:59:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 20 Apr 2020 18:24:23 GMT
ENV REDIS_VERSION=6.0-rc4
# Mon, 20 Apr 2020 18:24:27 GMT
ENV REDIS_DOWNLOAD_URL=https://github.com/antirez/redis/archive/6.0-rc4.tar.gz
# Mon, 20 Apr 2020 18:24:30 GMT
ENV REDIS_DOWNLOAD_SHA=dac1ad1253337c06adf2af7f6ec7d2f54371e6b37b3c3d1c9d8fb4b7713d12a7
# Mon, 20 Apr 2020 18:26:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Mon, 20 Apr 2020 18:27:03 GMT
RUN mkdir /data && chown redis:redis /data
# Mon, 20 Apr 2020 18:27:05 GMT
VOLUME [/data]
# Mon, 20 Apr 2020 18:27:10 GMT
WORKDIR /data
# Mon, 20 Apr 2020 18:27:11 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Mon, 20 Apr 2020 18:27:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 20 Apr 2020 18:27:16 GMT
EXPOSE 6379
# Mon, 20 Apr 2020 18:27:19 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:3d48095d71a365b5910cea98e5566c152a3f9aa11657560568259bf93ff2f4cb`  
		Last Modified: Thu, 16 Apr 2020 02:48:58 GMT  
		Size: 25.9 MB (25857715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:773882920678246b0738b0c84fe9b851fb4cf0c39bad7f78cdb329c31e214fe2`  
		Last Modified: Thu, 16 Apr 2020 19:04:54 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04905edf724bdcc5c1b0b9e01fe82619d3987b1b95d122b6e38fca03d351a84`  
		Last Modified: Thu, 16 Apr 2020 19:04:54 GMT  
		Size: 1.4 MB (1352859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ed0656092a5cc775535ee61134b11e522fc972fc8bb1391526643d710dd68a`  
		Last Modified: Mon, 20 Apr 2020 18:34:39 GMT  
		Size: 9.5 MB (9486547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9fd2750561a13a904f71d4ab5a685dbbf49aadd2a7d0ef4140244fe1cd9bd75`  
		Last Modified: Mon, 20 Apr 2020 18:34:38 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e48e0955b9e9bb75bfab971c8932231ee8af3956747f69c5d40d0f6055d88031`  
		Last Modified: Mon, 20 Apr 2020 18:34:38 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:rc` - linux; 386

```console
$ docker pull redis@sha256:fdeee0f71b970e9f5d325a843982600b6811ffb972ee429d621a6c3f2a8a2ddf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.4 MB (38400587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55bc23ed3c0cde5391fb5e0b9f679f7cf0c3fa861f05d8ed38c5e9e50be293c0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 16 Apr 2020 01:39:55 GMT
ADD file:ab0bbfba6c4b56420ffffc6cdddcc4592fff018f0cd07578c7dc0a5faa49df2f in / 
# Thu, 16 Apr 2020 01:39:56 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 18:48:13 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 16 Apr 2020 18:48:13 GMT
ENV GOSU_VERSION=1.12
# Thu, 16 Apr 2020 18:48:33 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 20 Apr 2020 18:03:11 GMT
ENV REDIS_VERSION=6.0-rc4
# Mon, 20 Apr 2020 18:03:11 GMT
ENV REDIS_DOWNLOAD_URL=https://github.com/antirez/redis/archive/6.0-rc4.tar.gz
# Mon, 20 Apr 2020 18:03:11 GMT
ENV REDIS_DOWNLOAD_SHA=dac1ad1253337c06adf2af7f6ec7d2f54371e6b37b3c3d1c9d8fb4b7713d12a7
# Mon, 20 Apr 2020 18:04:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Mon, 20 Apr 2020 18:04:36 GMT
RUN mkdir /data && chown redis:redis /data
# Mon, 20 Apr 2020 18:04:37 GMT
VOLUME [/data]
# Mon, 20 Apr 2020 18:04:37 GMT
WORKDIR /data
# Mon, 20 Apr 2020 18:04:37 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Mon, 20 Apr 2020 18:04:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 20 Apr 2020 18:04:37 GMT
EXPOSE 6379
# Mon, 20 Apr 2020 18:04:38 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:75bc60a98e6523be3fadd9128c1a630cb5cbd2d2d813ee5e99dc146a3de22254`  
		Last Modified: Thu, 16 Apr 2020 01:46:20 GMT  
		Size: 27.8 MB (27753976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:480c59671a8d31c11d74d3d995023ee54099bd645d1953b8278069fa0cfc8c68`  
		Last Modified: Thu, 16 Apr 2020 18:53:14 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67716918bb5033f981e8697a437a9466cc65073f3f8568aa781d0e78a1ba223b`  
		Last Modified: Thu, 16 Apr 2020 18:53:15 GMT  
		Size: 1.4 MB (1387415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03d110b60cf828829d86f42caafd31af290396da12b7517ea84c33d1eca3bfc`  
		Last Modified: Mon, 20 Apr 2020 18:10:25 GMT  
		Size: 9.3 MB (9256964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c95b6178e3f731ae33531bd50378f4a95d6cf9006dd005a53b30c36c518d71a`  
		Last Modified: Mon, 20 Apr 2020 18:10:23 GMT  
		Size: 99.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252926c288739dec5a4b3f4f3fb28aafca4c26950be3455b440ef195c46f3ed2`  
		Last Modified: Mon, 20 Apr 2020 18:10:23 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:rc` - linux; mips64le

```console
$ docker pull redis@sha256:e6985cdc0d1641c29662f534e2ba4c11ffdc7279ee33d0bfed7de89935840c89
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.6 MB (36562862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c54c3fff9791e64c08238af261a11c6ce985c8b5e79f618e201ceb193319020`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 16 Apr 2020 03:30:32 GMT
ADD file:1324f1b90326c771ad3fbeba783010d46ba465c130b2b400ff60232e52bc4bbb in / 
# Thu, 16 Apr 2020 03:30:33 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:24:19 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 16 Apr 2020 19:46:31 GMT
ENV GOSU_VERSION=1.12
# Thu, 16 Apr 2020 19:46:59 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 16 Apr 2020 19:46:59 GMT
ENV REDIS_VERSION=6.0-rc3
# Thu, 16 Apr 2020 19:47:00 GMT
ENV REDIS_DOWNLOAD_URL=https://github.com/antirez/redis/archive/6.0-rc3.tar.gz
# Thu, 16 Apr 2020 19:47:00 GMT
ENV REDIS_DOWNLOAD_SHA=a81f92ed0aeb2ecab1488ce916725da1283fa86c3ff43828430e77ce8e612534
# Thu, 16 Apr 2020 19:50:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 16 Apr 2020 19:50:30 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 16 Apr 2020 19:50:31 GMT
VOLUME [/data]
# Thu, 16 Apr 2020 19:50:31 GMT
WORKDIR /data
# Thu, 16 Apr 2020 19:50:31 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 16 Apr 2020 19:50:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Apr 2020 19:50:32 GMT
EXPOSE 6379
# Thu, 16 Apr 2020 19:50:32 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:9d68bbb6bb3e325311e23872a0324580a3e32aea907701fa94bab81e80ff88c4`  
		Last Modified: Thu, 16 Apr 2020 03:56:50 GMT  
		Size: 25.8 MB (25762172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c3eb7c6a1ed9071e27a712bf3b37a8b090ae44838e7aa7778d53f8fd236fac`  
		Last Modified: Thu, 16 Apr 2020 19:56:32 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b694cc8e6c5f7d347ce3e406178fe732292d6e0b10de86c066744f63331dca`  
		Last Modified: Thu, 16 Apr 2020 19:56:34 GMT  
		Size: 1.3 MB (1305461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca87adcd9f134cfd086e0cb626bbcbf1895ff47ae26630c22c63a75fea19b224`  
		Last Modified: Thu, 16 Apr 2020 19:56:41 GMT  
		Size: 9.5 MB (9492992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ab6ba41cee47da41077abdcd349521de406c92aa3dadaebe2797fa0ac7eabe3`  
		Last Modified: Thu, 16 Apr 2020 19:56:32 GMT  
		Size: 97.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c86dc5ca9760236b4c6b2808ce9e50ae9dfed9aa03cdcc7b3d5c384ac4e89d9`  
		Last Modified: Thu, 16 Apr 2020 19:56:32 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:rc` - linux; ppc64le

```console
$ docker pull redis@sha256:58b03214e89143d1ba573b8d4ec76e7277809e90f955e2f5c9aa7a5b8a25695a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42077488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13bc1b6e5e6a8a0cd64de80ccf95c7f01cf982b3c1a8b6d18688ea774600067c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 16 Apr 2020 01:38:30 GMT
ADD file:9beea54416432abbd09d26b965c3c8e5bea8e233113f9bc308294c0008ee886f in / 
# Thu, 16 Apr 2020 01:38:39 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 07:22:15 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Fri, 17 Apr 2020 02:44:47 GMT
ENV GOSU_VERSION=1.12
# Fri, 17 Apr 2020 02:46:08 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 17 Apr 2020 02:46:10 GMT
ENV REDIS_VERSION=6.0-rc3
# Fri, 17 Apr 2020 02:46:14 GMT
ENV REDIS_DOWNLOAD_URL=https://github.com/antirez/redis/archive/6.0-rc3.tar.gz
# Fri, 17 Apr 2020 02:46:16 GMT
ENV REDIS_DOWNLOAD_SHA=a81f92ed0aeb2ecab1488ce916725da1283fa86c3ff43828430e77ce8e612534
# Fri, 17 Apr 2020 02:48:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Fri, 17 Apr 2020 02:48:28 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 17 Apr 2020 02:48:32 GMT
VOLUME [/data]
# Fri, 17 Apr 2020 02:48:35 GMT
WORKDIR /data
# Fri, 17 Apr 2020 02:48:37 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Fri, 17 Apr 2020 02:48:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 17 Apr 2020 02:48:42 GMT
EXPOSE 6379
# Fri, 17 Apr 2020 02:48:44 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:f268991f8af64097bbfefa3f01dd3fdb7f715051a3681f352504a3ecaa9d3596`  
		Last Modified: Thu, 16 Apr 2020 01:54:39 GMT  
		Size: 30.5 MB (30524651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a89977e978b6e4b52cd3afcd5f61ecb22125b95db7f2e6bc3c332ac0b2ed17a4`  
		Last Modified: Thu, 16 Apr 2020 07:33:47 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fca67d84d55dd14c3b61e0683dd5807b3685b11817b54757a4fd4d528fe8d7f`  
		Last Modified: Fri, 17 Apr 2020 02:55:08 GMT  
		Size: 1.3 MB (1335293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4e7a8b85c51a6aaf3a0c549f6adfad336d62906e5d438d335ab15d5f0502f9`  
		Last Modified: Fri, 17 Apr 2020 02:55:10 GMT  
		Size: 10.2 MB (10215270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e990f5259e911963a767c6991803417c2859b0c80b97b61e921a68ff4fab25`  
		Last Modified: Fri, 17 Apr 2020 02:55:07 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3322fa64f3c586a17228d73c2ba89a24e7b4c744828f39e00331514375257d7`  
		Last Modified: Fri, 17 Apr 2020 02:55:07 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:rc` - linux; s390x

```console
$ docker pull redis@sha256:67c11521c347562d7082ef5fb44c73d09adf6f2b351bcb18abaa14843c3397d0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.7 MB (36701026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:417ce123d48e89878f062ee07227576ba5c457b77d51f17803e4b33703c869e0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 16 Apr 2020 00:42:19 GMT
ADD file:f328b5d6dce2eaf00360542c1e3280958b818268b9150b12ffd1fddf030daf2f in / 
# Thu, 16 Apr 2020 00:42:20 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 08:41:53 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 16 Apr 2020 20:08:23 GMT
ENV GOSU_VERSION=1.12
# Thu, 16 Apr 2020 20:08:32 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 16 Apr 2020 20:08:32 GMT
ENV REDIS_VERSION=6.0-rc3
# Thu, 16 Apr 2020 20:08:32 GMT
ENV REDIS_DOWNLOAD_URL=https://github.com/antirez/redis/archive/6.0-rc3.tar.gz
# Thu, 16 Apr 2020 20:08:32 GMT
ENV REDIS_DOWNLOAD_SHA=a81f92ed0aeb2ecab1488ce916725da1283fa86c3ff43828430e77ce8e612534
# Thu, 16 Apr 2020 20:09:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 16 Apr 2020 20:09:08 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 16 Apr 2020 20:09:08 GMT
VOLUME [/data]
# Thu, 16 Apr 2020 20:09:08 GMT
WORKDIR /data
# Thu, 16 Apr 2020 20:09:09 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 16 Apr 2020 20:09:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Apr 2020 20:09:09 GMT
EXPOSE 6379
# Thu, 16 Apr 2020 20:09:09 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:043f95f5412a986fb082b0193860bb9c0388c2fbcb5e8bf5bcbbeefb0e45c9c5`  
		Last Modified: Thu, 16 Apr 2020 00:46:19 GMT  
		Size: 25.7 MB (25712234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7252bb7c6713c7896b021e6fdbb2c4ccd49d7c163dc9eed0b68d9001d0333d9`  
		Last Modified: Thu, 16 Apr 2020 08:44:34 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:100f02751c508c26b726472e2fffa3c32b8f7c0916d8d811ac8498af5e9e6202`  
		Last Modified: Thu, 16 Apr 2020 20:10:52 GMT  
		Size: 1.4 MB (1403637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb29be3e1dc8706ffa9d893394582dbac8c6a54dfe72aa17c0c854a396acce7`  
		Last Modified: Thu, 16 Apr 2020 20:10:53 GMT  
		Size: 9.6 MB (9582879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc504fb3a0b0bc4294e87603750d3295403379271ff966c98680be1225a203ce`  
		Last Modified: Thu, 16 Apr 2020 20:10:58 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679dba8944e3933e3f98065bb0b6703d98d1c18554d848a8d310860e6c2304b9`  
		Last Modified: Thu, 16 Apr 2020 20:10:51 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
