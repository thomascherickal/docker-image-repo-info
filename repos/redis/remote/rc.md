## `redis:rc`

```console
$ docker pull redis@sha256:8ba11a1102aa4c2f3f0f9542ccd2ad45b76ebabe63cd12d652e57915efeba518
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `redis:rc` - linux; amd64

```console
$ docker pull redis@sha256:e55ff6f2c8d7dfddf749a68aebcd31dbf32043220f84b9b5e5966ce7eaea5ce0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.0 MB (38046830 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06320b052e263137512983551818430b5ea3293a42fb3ff2cf256482ce37de62`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 26 Feb 2020 00:37:39 GMT
ADD file:e5a364615e0f6961626089c7d658adbf8c8d95b3ae95a390a8bb33875317d434 in / 
# Wed, 26 Feb 2020 00:37:39 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 20:05:10 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Wed, 26 Feb 2020 20:05:10 GMT
ENV GOSU_VERSION=1.11
# Wed, 26 Feb 2020 20:05:23 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 06 Mar 2020 02:30:41 GMT
ENV REDIS_VERSION=6.0-rc2
# Fri, 06 Mar 2020 02:30:41 GMT
ENV REDIS_DOWNLOAD_URL=https://github.com/antirez/redis/archive/6.0-rc2.tar.gz
# Fri, 06 Mar 2020 02:30:41 GMT
ENV REDIS_DOWNLOAD_SHA=ac8ac8aae2c143ba972c386f9852ae40b418dbcecab3841bf7f6d4b71fccd7cb
# Fri, 06 Mar 2020 02:31:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Fri, 06 Mar 2020 02:31:58 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 06 Mar 2020 02:31:58 GMT
VOLUME [/data]
# Fri, 06 Mar 2020 02:31:58 GMT
WORKDIR /data
# Fri, 06 Mar 2020 02:31:59 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Fri, 06 Mar 2020 02:31:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Mar 2020 02:31:59 GMT
EXPOSE 6379
# Fri, 06 Mar 2020 02:32:00 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:68ced04f60ab5c7a5f1d0b0b4e7572c5a4c8cce44866513d30d9df1a15277d6b`  
		Last Modified: Wed, 26 Feb 2020 00:44:23 GMT  
		Size: 27.1 MB (27091819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ecc253967df63c91c05c830bac2fe70ca6310473427da326667b44fdec3374f`  
		Last Modified: Wed, 26 Feb 2020 20:11:48 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:765957bf98d45a3c48bc1565d2cbddfbae12a480404e11a2ad43e0e5c1513a64`  
		Last Modified: Wed, 26 Feb 2020 20:11:49 GMT  
		Size: 1.4 MB (1357665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0415fa01513fe24b846c488460a9f3e8f81bb86c5b15fd4477a8ed6fdca1ab7b`  
		Last Modified: Fri, 06 Mar 2020 02:35:23 GMT  
		Size: 9.6 MB (9595108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:633e7d5f17a271622746a5b4445af5b5bf2b756c3a6495c8e701167e83e652dd`  
		Last Modified: Fri, 06 Mar 2020 02:35:21 GMT  
		Size: 99.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b4b4e91259db92409993d19752d4677d9425bd74aefd041502af26402663d3b`  
		Last Modified: Fri, 06 Mar 2020 02:35:20 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:rc` - linux; arm variant v5

```console
$ docker pull redis@sha256:54ecba9e209763f27038b8c63d74c870a7bd1d0b85d6e5546b8cd5be3b82f147
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35271422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04afb268dee3c3a40f649cb395153faa053aaea6ce06858958ec9829d5a359ce`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 26 Feb 2020 00:47:49 GMT
ADD file:745d3236976c8213b805ca6d14f150561816cd2eeec5aa7e1aaea44d9d5675e9 in / 
# Wed, 26 Feb 2020 00:47:53 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 06:11:36 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Wed, 26 Feb 2020 06:11:39 GMT
ENV GOSU_VERSION=1.11
# Wed, 26 Feb 2020 06:12:21 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 06 Mar 2020 00:51:12 GMT
ENV REDIS_VERSION=6.0-rc2
# Fri, 06 Mar 2020 00:51:13 GMT
ENV REDIS_DOWNLOAD_URL=https://github.com/antirez/redis/archive/6.0-rc2.tar.gz
# Fri, 06 Mar 2020 00:51:13 GMT
ENV REDIS_DOWNLOAD_SHA=ac8ac8aae2c143ba972c386f9852ae40b418dbcecab3841bf7f6d4b71fccd7cb
# Fri, 06 Mar 2020 00:52:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Fri, 06 Mar 2020 00:52:40 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 06 Mar 2020 00:52:41 GMT
VOLUME [/data]
# Fri, 06 Mar 2020 00:52:42 GMT
WORKDIR /data
# Fri, 06 Mar 2020 00:52:43 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Fri, 06 Mar 2020 00:52:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Mar 2020 00:52:44 GMT
EXPOSE 6379
# Fri, 06 Mar 2020 00:52:45 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:d9f9009f908455fa93c5b3e0d3230df44ea75299b2de375ab35b74193f679076`  
		Last Modified: Wed, 26 Feb 2020 00:59:18 GMT  
		Size: 24.8 MB (24830277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7886599d45595e317dc35d78cf5439d6721e93516002f5ab6c483f569121665e`  
		Last Modified: Wed, 26 Feb 2020 06:20:10 GMT  
		Size: 1.7 KB (1727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acca0e683588637378a83fdb243c9a1e527ca9ab161a4195c1ac05504ef85417`  
		Last Modified: Wed, 26 Feb 2020 06:20:11 GMT  
		Size: 1.3 MB (1317132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce5c1b873b64cef3b9078d628323e920b0eef26c036c5af31a5cbe3bc10951ef`  
		Last Modified: Fri, 06 Mar 2020 00:59:40 GMT  
		Size: 9.1 MB (9121744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4c364426774950dc2db13a52d3c6a0ea7e180e38e33d702b47b80595b8de655`  
		Last Modified: Fri, 06 Mar 2020 00:59:37 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:416bcb5fe2a34477dc19b10454942044d7decc7295348e6705757ec74fecc2ac`  
		Last Modified: Fri, 06 Mar 2020 00:59:37 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:rc` - linux; arm variant v7

```console
$ docker pull redis@sha256:d784c4b86e3dbb0a46a05cad4be29b68ef06df2c96c1fc43a4c185af5f75adc5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.9 MB (32897626 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0400486ad8037544d59291129d5f987e573eff5d2307850feff81686bbff8be3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Tue, 31 Mar 2020 01:48:12 GMT
ADD file:8c3ed0df404a6bcaf7583e71796cb4c1f40e87288953a21d4ee5946079c3274f in / 
# Tue, 31 Mar 2020 01:48:13 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 05:21:20 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Tue, 31 Mar 2020 05:21:20 GMT
ENV GOSU_VERSION=1.11
# Tue, 31 Mar 2020 05:21:47 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 31 Mar 2020 05:21:48 GMT
ENV REDIS_VERSION=6.0-rc2
# Tue, 31 Mar 2020 05:21:49 GMT
ENV REDIS_DOWNLOAD_URL=https://github.com/antirez/redis/archive/6.0-rc2.tar.gz
# Tue, 31 Mar 2020 05:21:50 GMT
ENV REDIS_DOWNLOAD_SHA=ac8ac8aae2c143ba972c386f9852ae40b418dbcecab3841bf7f6d4b71fccd7cb
# Tue, 31 Mar 2020 05:22:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Tue, 31 Mar 2020 05:22:57 GMT
RUN mkdir /data && chown redis:redis /data
# Tue, 31 Mar 2020 05:22:57 GMT
VOLUME [/data]
# Tue, 31 Mar 2020 05:22:58 GMT
WORKDIR /data
# Tue, 31 Mar 2020 05:22:58 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Tue, 31 Mar 2020 05:22:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Mar 2020 05:23:00 GMT
EXPOSE 6379
# Tue, 31 Mar 2020 05:23:00 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:98098fa10651fdba12c848231b7428536a120e17637f1f9e0d25c63880483fcc`  
		Last Modified: Tue, 31 Mar 2020 01:56:24 GMT  
		Size: 22.7 MB (22699731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a498080b161ccf8f18c8435b015478362025efee1e11d37a2503fab003342459`  
		Last Modified: Tue, 31 Mar 2020 05:26:27 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c31c436c4b8a133e094c1ea9575174ae6016dfebe20dad740734215cc00ac2ff`  
		Last Modified: Tue, 31 Mar 2020 05:26:27 GMT  
		Size: 1.3 MB (1307646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87626b7bfb0bdbb205d285e857bf902e6eaadf80ea91a5c64edfefe528f49312`  
		Last Modified: Tue, 31 Mar 2020 05:26:30 GMT  
		Size: 8.9 MB (8887979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:785560178ec3c4d42f9a37118303836d5e9e2bf00c63ef6ab85a20ef2ee02b54`  
		Last Modified: Tue, 31 Mar 2020 05:26:27 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2400484d85fb425ae0560fd1b772e04814d79714e59f451e9e14538cdfd3b1`  
		Last Modified: Tue, 31 Mar 2020 05:26:28 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:rc` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:e39ea3755e6b8f4eb3c4bcf4986ab6462985bc6dad3585b4f15cd44285b1b541
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.6 MB (36601478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da8ded25ebc02e274a068b0de86d1c4e9baa28774a676aa10030b9bb195739eb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 26 Feb 2020 00:46:51 GMT
ADD file:a93818b0ffcb2823807811dffd78092a3e3f4981aabf48c3cb75f2fa319ac055 in / 
# Wed, 26 Feb 2020 00:46:55 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 19:01:33 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Wed, 26 Feb 2020 19:01:34 GMT
ENV GOSU_VERSION=1.11
# Wed, 26 Feb 2020 19:01:58 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 06 Mar 2020 01:37:18 GMT
ENV REDIS_VERSION=6.0-rc2
# Fri, 06 Mar 2020 01:37:18 GMT
ENV REDIS_DOWNLOAD_URL=https://github.com/antirez/redis/archive/6.0-rc2.tar.gz
# Fri, 06 Mar 2020 01:37:19 GMT
ENV REDIS_DOWNLOAD_SHA=ac8ac8aae2c143ba972c386f9852ae40b418dbcecab3841bf7f6d4b71fccd7cb
# Fri, 06 Mar 2020 01:38:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Fri, 06 Mar 2020 01:38:31 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 06 Mar 2020 01:38:32 GMT
VOLUME [/data]
# Fri, 06 Mar 2020 01:38:33 GMT
WORKDIR /data
# Fri, 06 Mar 2020 01:38:34 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Fri, 06 Mar 2020 01:38:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Mar 2020 01:38:36 GMT
EXPOSE 6379
# Fri, 06 Mar 2020 01:38:37 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:f338bc35613f66cfaad272234de7b77a91d6c5422855bf6239f2b0ff9d73f0a4`  
		Last Modified: Wed, 26 Feb 2020 00:56:15 GMT  
		Size: 25.9 MB (25851563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d49f96b203f98ac73ecd9ee9dcbd3050716ea5911b43216ed2f553f856144961`  
		Last Modified: Wed, 26 Feb 2020 19:06:14 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac978a3fb28b29b24de4d0f625a8dcd6cced0e68b00348ac282b9fb8b928222`  
		Last Modified: Wed, 26 Feb 2020 19:06:14 GMT  
		Size: 1.3 MB (1290661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a93c2533ff2bd4c616bebf48c5d750568fc09011e2196f14e44ea9bb01561cdd`  
		Last Modified: Fri, 06 Mar 2020 01:41:19 GMT  
		Size: 9.5 MB (9456978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae3b92b18d669f9fa485337a696a9d3bb390e282b6864f5fc15770c39270e257`  
		Last Modified: Fri, 06 Mar 2020 01:41:05 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5cbf73b1da76d055d3949892ec90a6cd9426ad13dda1bc6e93ca05304f3d507`  
		Last Modified: Fri, 06 Mar 2020 01:41:05 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:rc` - linux; 386

```console
$ docker pull redis@sha256:923a6b0b64d39d8fcca4ec5f665b8af0dc41723b7f11a04fdb8b504f273d3ebd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.3 MB (38301625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:132418079b997e54285f8415095844c7a0e11f035d06a2aa552ea34672ecd13b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 26 Feb 2020 00:32:17 GMT
ADD file:08977fa54555a1ed2ae44a3aec04df157092a6c1c1b70ce0407cc2dc2f8bcd76 in / 
# Wed, 26 Feb 2020 00:32:17 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 05:19:06 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Wed, 26 Feb 2020 05:19:06 GMT
ENV GOSU_VERSION=1.11
# Wed, 26 Feb 2020 05:19:20 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 06 Mar 2020 03:10:59 GMT
ENV REDIS_VERSION=6.0-rc2
# Fri, 06 Mar 2020 03:10:59 GMT
ENV REDIS_DOWNLOAD_URL=https://github.com/antirez/redis/archive/6.0-rc2.tar.gz
# Fri, 06 Mar 2020 03:10:59 GMT
ENV REDIS_DOWNLOAD_SHA=ac8ac8aae2c143ba972c386f9852ae40b418dbcecab3841bf7f6d4b71fccd7cb
# Fri, 06 Mar 2020 03:12:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Fri, 06 Mar 2020 03:12:23 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 06 Mar 2020 03:12:23 GMT
VOLUME [/data]
# Fri, 06 Mar 2020 03:12:23 GMT
WORKDIR /data
# Fri, 06 Mar 2020 03:12:23 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Fri, 06 Mar 2020 03:12:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Mar 2020 03:12:24 GMT
EXPOSE 6379
# Fri, 06 Mar 2020 03:12:24 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:1de10f1ae2a5bfd5f34f19421ebd282580e443321e4947cdf5f943875782b018`  
		Last Modified: Wed, 26 Feb 2020 00:38:34 GMT  
		Size: 27.7 MB (27747667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b601c134c02e3ddbaca43b0ac84998b13c790129fc9e1d69b11cafcb335a4b52`  
		Last Modified: Wed, 26 Feb 2020 05:25:12 GMT  
		Size: 1.7 KB (1724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e7fe37cc3ca17d9a6d916ccc4472e576d45c14fc98f2060cd1aaec94b36fe9`  
		Last Modified: Wed, 26 Feb 2020 05:25:13 GMT  
		Size: 1.3 MB (1323356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a9a116b924b7e354b19fb1bbff913fa2f603cf2c0d3e2d234ba28690ec19fbc`  
		Last Modified: Fri, 06 Mar 2020 03:15:05 GMT  
		Size: 9.2 MB (9228369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0b00719191b1f5f2d0ed85caad25584ab481b0f0694c3fa0d3b935276c2d777`  
		Last Modified: Fri, 06 Mar 2020 03:15:02 GMT  
		Size: 99.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58579eda0cbaae86cd673a4f3e6be876fbe7ba0244db5deefdb1e84df1470922`  
		Last Modified: Fri, 06 Mar 2020 03:15:03 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:rc` - linux; ppc64le

```console
$ docker pull redis@sha256:96213d7ef44151fe8aef15ce11766e84fa52cb456e06e6acce3afacbae76669d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.0 MB (41999502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c36110733202d9b4df56e914e0cfc206ad42f5bf3f8ce7e1d01d1a9cf3ad7da8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Wed, 26 Feb 2020 01:31:23 GMT
ADD file:430f1f769b86c60db1b8d2f96ed26c24837b3ff5730264be42a9c0cd8e43df7f in / 
# Wed, 26 Feb 2020 01:31:29 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 18:41:27 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Wed, 26 Feb 2020 18:41:30 GMT
ENV GOSU_VERSION=1.11
# Wed, 26 Feb 2020 18:43:10 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 06 Mar 2020 01:32:07 GMT
ENV REDIS_VERSION=6.0-rc2
# Fri, 06 Mar 2020 01:32:11 GMT
ENV REDIS_DOWNLOAD_URL=https://github.com/antirez/redis/archive/6.0-rc2.tar.gz
# Fri, 06 Mar 2020 01:32:14 GMT
ENV REDIS_DOWNLOAD_SHA=ac8ac8aae2c143ba972c386f9852ae40b418dbcecab3841bf7f6d4b71fccd7cb
# Fri, 06 Mar 2020 01:34:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Fri, 06 Mar 2020 01:35:00 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 06 Mar 2020 01:35:04 GMT
VOLUME [/data]
# Fri, 06 Mar 2020 01:35:09 GMT
WORKDIR /data
# Fri, 06 Mar 2020 01:35:10 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Fri, 06 Mar 2020 01:35:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Mar 2020 01:35:17 GMT
EXPOSE 6379
# Fri, 06 Mar 2020 01:35:19 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:975241fcd2057cc8f4cb8f066d68ed18877152b88da11e682911ccc3bc3da7c4`  
		Last Modified: Wed, 26 Feb 2020 01:52:57 GMT  
		Size: 30.5 MB (30518427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53295c4c47fa7aa3d3ea87b305cf9e732ef5867019e007559af4f3af6bd509fa`  
		Last Modified: Wed, 26 Feb 2020 18:51:18 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c70c5cb1b3b2b906129b50805c2341f281e3df95927f63a55292111a6b0b2140`  
		Last Modified: Wed, 26 Feb 2020 18:51:18 GMT  
		Size: 1.3 MB (1279131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9645bc07e5c569f3c7d6afebe54f9888afbf6c6f8072195531cf9cab4813bb64`  
		Last Modified: Fri, 06 Mar 2020 01:38:20 GMT  
		Size: 10.2 MB (10199673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7ac61ad2761803f5dd6e69646fb3fbae4e624321a4fcd1834c7446a8c96f66`  
		Last Modified: Fri, 06 Mar 2020 01:38:14 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32598bb9d56f52a133d6fdb9133d3fdc39ba56e1eda0a6b6fb752506912ff1f8`  
		Last Modified: Fri, 06 Mar 2020 01:38:14 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:rc` - linux; s390x

```console
$ docker pull redis@sha256:d57f0fc9f29e67949e7302110f451a853aca4fdaefb70bb8881be53658c75ee5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.6 MB (36619382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2969521ef9c441c8e325c270c2933753537c69a2515d6015c4e22c65622aa21c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Tue, 31 Mar 2020 01:09:01 GMT
ADD file:012f7224d56eafd61d4fbf99bc0a12ce4afa4a228fb04a849a9e9398ae8e0969 in / 
# Tue, 31 Mar 2020 01:09:02 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 02:35:37 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Tue, 31 Mar 2020 02:35:37 GMT
ENV GOSU_VERSION=1.11
# Tue, 31 Mar 2020 02:35:50 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dirmngr 		gnupg 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 31 Mar 2020 02:35:50 GMT
ENV REDIS_VERSION=6.0-rc2
# Tue, 31 Mar 2020 02:35:51 GMT
ENV REDIS_DOWNLOAD_URL=https://github.com/antirez/redis/archive/6.0-rc2.tar.gz
# Tue, 31 Mar 2020 02:35:51 GMT
ENV REDIS_DOWNLOAD_SHA=ac8ac8aae2c143ba972c386f9852ae40b418dbcecab3841bf7f6d4b71fccd7cb
# Tue, 31 Mar 2020 02:36:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Tue, 31 Mar 2020 02:36:22 GMT
RUN mkdir /data && chown redis:redis /data
# Tue, 31 Mar 2020 02:36:22 GMT
VOLUME [/data]
# Tue, 31 Mar 2020 02:36:22 GMT
WORKDIR /data
# Tue, 31 Mar 2020 02:36:23 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Tue, 31 Mar 2020 02:36:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Mar 2020 02:36:23 GMT
EXPOSE 6379
# Tue, 31 Mar 2020 02:36:23 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:b59fc323cb12d31b5e0b5e812b5ca8436f3753a6e6cc9004edbac36ffa7be8e0`  
		Last Modified: Tue, 31 Mar 2020 01:12:39 GMT  
		Size: 25.7 MB (25706014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17c6808d8bc4b5e0b26e76f8a656c365b2f57a4ba88b319913aa25694262eeca`  
		Last Modified: Tue, 31 Mar 2020 02:38:03 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d416799a4cc0e85985096fbe9a11d247f524b5cf1ad041f6d98a85efba757014`  
		Last Modified: Tue, 31 Mar 2020 02:38:03 GMT  
		Size: 1.3 MB (1345855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca5e0ca72e9536d542b60f958efa9e15474bbfd62495bb4388694911a070618`  
		Last Modified: Tue, 31 Mar 2020 02:38:04 GMT  
		Size: 9.6 MB (9565233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf7c8a619c22defb931d50d1897d942dc4dc34a5ad7548a2ad835cd3cf5ec103`  
		Last Modified: Tue, 31 Mar 2020 02:38:08 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9b2f8564f0aa9bad60150f8daac201931953997ad57d119b75695a95c66be10`  
		Last Modified: Tue, 31 Mar 2020 02:38:08 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
