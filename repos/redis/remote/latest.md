## `redis:latest`

```console
$ docker pull redis@sha256:9c0cc0c655561a14abdd30b6c9f95c446fd02266ac23ab5ec78cbb3d5f59eabf
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
$ docker pull redis@sha256:5d30f5c16e473549ad7c950b0ac3083039719b1c9749519c50e18017dd4bfc54
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.1 MB (41132291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7faaec68323851b2265bddb239bd9476c7d4e4335e9fd88cbfcc1df374dded2f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Tue, 12 Oct 2021 01:20:42 GMT
ADD file:16dc2c6d1932194edec28d730b004fd6deca3d0f0e1a07bc5b8b6e8a1662f7af in / 
# Tue, 12 Oct 2021 01:20:42 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 09:41:10 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Tue, 12 Oct 2021 09:41:10 GMT
ENV GOSU_VERSION=1.12
# Tue, 12 Oct 2021 09:41:22 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 12 Oct 2021 09:41:22 GMT
ENV REDIS_VERSION=6.2.6
# Tue, 12 Oct 2021 09:41:22 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.6.tar.gz
# Tue, 12 Oct 2021 09:41:23 GMT
ENV REDIS_DOWNLOAD_SHA=5b2b8b7a50111ef395bf1c1d5be11e6e167ac018125055daa8b5c2317ae131ab
# Tue, 12 Oct 2021 09:42:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Tue, 12 Oct 2021 09:42:27 GMT
RUN mkdir /data && chown redis:redis /data
# Tue, 12 Oct 2021 09:42:27 GMT
VOLUME [/data]
# Tue, 12 Oct 2021 09:42:27 GMT
WORKDIR /data
# Tue, 12 Oct 2021 09:42:27 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Tue, 12 Oct 2021 09:42:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Oct 2021 09:42:28 GMT
EXPOSE 6379
# Tue, 12 Oct 2021 09:42:28 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:7d63c13d9b9b6ec5f05a2b07daadacaa9c610d01102a662ae9b1d082105f1ffa`  
		Last Modified: Tue, 12 Oct 2021 01:26:05 GMT  
		Size: 31.4 MB (31357311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2c3b174c5adb1054d2852ab40e7e819e53672f109f9a41b262fb92888b73fb0`  
		Last Modified: Tue, 12 Oct 2021 09:46:59 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283a10257b0f635ab12b2f4990dc8579457b91f92a3f097829c3798866ce146e`  
		Last Modified: Tue, 12 Oct 2021 09:46:59 GMT  
		Size: 1.4 MB (1442376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a08c63a873a0e80c8646f11ff13398a1eed0e8e630a6c3b995a61de974141e5`  
		Last Modified: Tue, 12 Oct 2021 09:47:01 GMT  
		Size: 8.3 MB (8330329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0531663a7f55d313efe69b5c04393ae60e991217ac45a683dfd0b46664a96373`  
		Last Modified: Tue, 12 Oct 2021 09:46:59 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf50efb265cd3aca469198518d776536f376863307b6ac4a5c06b864fb1ebc3`  
		Last Modified: Tue, 12 Oct 2021 09:46:59 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:latest` - linux; arm variant v5

```console
$ docker pull redis@sha256:67d9a6823a30cf26708321e8f97a3329434281de663cf5337d8d12088dc3d992
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.5 MB (38466585 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bef10030795e5e2bbe24334f7a0872c5af16e8f7c72d6e94438c5e759da63b6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Tue, 28 Sep 2021 01:50:38 GMT
ADD file:da0067258fc1c6a50273e6b3b2673e88fad974a5a1fe4d5eecfeca2df1ff54b3 in / 
# Tue, 28 Sep 2021 01:50:39 GMT
CMD ["bash"]
# Thu, 07 Oct 2021 21:59:21 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 07 Oct 2021 21:59:21 GMT
ENV GOSU_VERSION=1.12
# Thu, 07 Oct 2021 21:59:53 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 07 Oct 2021 21:59:54 GMT
ENV REDIS_VERSION=6.2.6
# Thu, 07 Oct 2021 21:59:54 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.6.tar.gz
# Thu, 07 Oct 2021 21:59:55 GMT
ENV REDIS_DOWNLOAD_SHA=5b2b8b7a50111ef395bf1c1d5be11e6e167ac018125055daa8b5c2317ae131ab
# Thu, 07 Oct 2021 22:01:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 07 Oct 2021 22:01:37 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 07 Oct 2021 22:01:38 GMT
VOLUME [/data]
# Thu, 07 Oct 2021 22:01:38 GMT
WORKDIR /data
# Thu, 07 Oct 2021 22:01:39 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 07 Oct 2021 22:01:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Oct 2021 22:01:40 GMT
EXPOSE 6379
# Thu, 07 Oct 2021 22:01:40 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:86f2b8be18fc44e8eb430e2c472979a79cda6eb6fa3add10cc8c5d8764eb90ac`  
		Last Modified: Tue, 28 Sep 2021 02:06:35 GMT  
		Size: 28.9 MB (28910670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca9322fc1fac20562a1921894a919047465d65607833f41d220789549da545d`  
		Last Modified: Thu, 07 Oct 2021 22:06:59 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0865f7ab3c868402609d9ab12f69c8ee08ea578f458b5d8661bc3a7e0d44ea51`  
		Last Modified: Thu, 07 Oct 2021 22:07:00 GMT  
		Size: 1.4 MB (1402326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:867ba0513d6cf06fb3fc6058ddd66a5d6a31529167419f98a82c616e79e2c5e1`  
		Last Modified: Thu, 07 Oct 2021 22:07:04 GMT  
		Size: 8.2 MB (8151321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009d73e42f8a35164300c58cffe1fd70c972f6d4b84e0806bcb42a4a8781c966`  
		Last Modified: Thu, 07 Oct 2021 22:06:59 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7674919cf01ad4ee9bb02a0f0c15dcf4d72a363881510de050e09b2bc51a5b50`  
		Last Modified: Thu, 07 Oct 2021 22:06:59 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:latest` - linux; arm variant v7

```console
$ docker pull redis@sha256:71642754957d40b31eed8582b71d8cc803e6e3d63c8dd3035d0d3c0abc70a6c0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.0 MB (35958753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:382d947f08a2c9ae9e917434d9a4d800600ba93089320718a1265c44c85d2b79`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Thu, 30 Sep 2021 18:03:01 GMT
ADD file:129e2106788d883a456b145d9aff00c3003ee3480901a30318933b46961d31f3 in / 
# Thu, 30 Sep 2021 18:03:02 GMT
CMD ["bash"]
# Thu, 07 Oct 2021 22:17:04 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 07 Oct 2021 22:17:05 GMT
ENV GOSU_VERSION=1.12
# Thu, 07 Oct 2021 22:17:33 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 07 Oct 2021 22:17:33 GMT
ENV REDIS_VERSION=6.2.6
# Thu, 07 Oct 2021 22:17:33 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.6.tar.gz
# Thu, 07 Oct 2021 22:17:34 GMT
ENV REDIS_DOWNLOAD_SHA=5b2b8b7a50111ef395bf1c1d5be11e6e167ac018125055daa8b5c2317ae131ab
# Thu, 07 Oct 2021 22:19:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 07 Oct 2021 22:19:06 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 07 Oct 2021 22:19:06 GMT
VOLUME [/data]
# Thu, 07 Oct 2021 22:19:07 GMT
WORKDIR /data
# Thu, 07 Oct 2021 22:19:08 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 07 Oct 2021 22:19:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Oct 2021 22:19:08 GMT
EXPOSE 6379
# Thu, 07 Oct 2021 22:19:09 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:aad43ac6bd46b2cab91485c8f1dac6a985df690af3e431e9e0b9fd57ad5ed423`  
		Last Modified: Thu, 30 Sep 2021 18:19:26 GMT  
		Size: 26.6 MB (26571924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b87fbfeb09b715c5c1386db714385d0eb9ba76740e429730ff8641f184817adb`  
		Last Modified: Thu, 07 Oct 2021 22:26:19 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5c3b5190f52ee32c8240a2d769a213d5e56aa16b2206b3aeb42705339127ff`  
		Last Modified: Thu, 07 Oct 2021 22:26:20 GMT  
		Size: 1.4 MB (1394055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd12fc46901699122debcf70cca8abd405ddb6ca1dbdc4ec592a00dab68e4677`  
		Last Modified: Thu, 07 Oct 2021 22:26:23 GMT  
		Size: 8.0 MB (7990507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9c94018528b1f74c84d2b8bbd5f4d44ab8ff9cd11c328dfa8c6795801b09ec4`  
		Last Modified: Thu, 07 Oct 2021 22:26:19 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d050e089bf035a36c838245ec5a2b4f4db7525ee056428c60bf49d0d90189c05`  
		Last Modified: Thu, 07 Oct 2021 22:26:19 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:latest` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:9013029da6a9bad604708012ae951dba36551fafc3aaf7990483e3c6129fd30d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.8 MB (39798026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b90c8df2167d977ecc4f1acdd324d5e2d94824216821ef26179b8f9650779b4e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:43 GMT
ADD file:6472ab63529e688735f77634402740e08fdbd5bfa788c150915027993df7e8ec in / 
# Tue, 28 Sep 2021 01:40:44 GMT
CMD ["bash"]
# Thu, 07 Oct 2021 22:04:58 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 07 Oct 2021 22:04:59 GMT
ENV GOSU_VERSION=1.12
# Thu, 07 Oct 2021 22:05:10 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 07 Oct 2021 22:05:10 GMT
ENV REDIS_VERSION=6.2.6
# Thu, 07 Oct 2021 22:05:10 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.6.tar.gz
# Thu, 07 Oct 2021 22:05:10 GMT
ENV REDIS_DOWNLOAD_SHA=5b2b8b7a50111ef395bf1c1d5be11e6e167ac018125055daa8b5c2317ae131ab
# Thu, 07 Oct 2021 22:06:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 07 Oct 2021 22:06:01 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 07 Oct 2021 22:06:02 GMT
VOLUME [/data]
# Thu, 07 Oct 2021 22:06:02 GMT
WORKDIR /data
# Thu, 07 Oct 2021 22:06:02 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 07 Oct 2021 22:06:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Oct 2021 22:06:02 GMT
EXPOSE 6379
# Thu, 07 Oct 2021 22:06:03 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:2f8871a8654eb1158cb626f8dc69992dba7e4bd8796fae6aa7cf967f951f5fe9`  
		Last Modified: Tue, 28 Sep 2021 01:48:25 GMT  
		Size: 30.1 MB (30055408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c57e4e320cf6c2981fc423d2da6b055678cb495df32bbea22d37cb0537585e2`  
		Last Modified: Thu, 07 Oct 2021 22:09:42 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6054a0eb6707dc288f9ce2b655bf5125a97f81fb2b2cf08340859a70303da582`  
		Last Modified: Thu, 07 Oct 2021 22:09:42 GMT  
		Size: 1.4 MB (1378430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc6e8d232c7f96854bec16dfc62c0e12dbd8a87c04799e188d2f5e13b04596be`  
		Last Modified: Thu, 07 Oct 2021 22:09:44 GMT  
		Size: 8.4 MB (8361908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aacb6223d43f571ef24373b2472e731c6df22e8a1f0f730e1c8a71d5d2bb6607`  
		Last Modified: Thu, 07 Oct 2021 22:09:42 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b2cf2c79df5bd8688d0304ab43a1cda920b094232f97ee303f91c1ca77a5b0b`  
		Last Modified: Thu, 07 Oct 2021 22:09:42 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:latest` - linux; 386

```console
$ docker pull redis@sha256:8c32b998a8731b362595a154c64013933abfb4446b58037c2f73864b635d0e13
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.8 MB (41778650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c8339248ffff412885a8882e7e7454812a86ca7601cfe8e5f6268ea62902201`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Tue, 28 Sep 2021 01:40:08 GMT
ADD file:8466bd8df052ea7fa26e49575ac95fd4934ddafdad54a9736ac2bd8e7fc6e735 in / 
# Tue, 28 Sep 2021 01:40:08 GMT
CMD ["bash"]
# Thu, 07 Oct 2021 20:52:21 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 07 Oct 2021 20:52:21 GMT
ENV GOSU_VERSION=1.12
# Thu, 07 Oct 2021 20:52:35 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 07 Oct 2021 20:52:36 GMT
ENV REDIS_VERSION=6.2.6
# Thu, 07 Oct 2021 20:52:36 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.6.tar.gz
# Thu, 07 Oct 2021 20:52:36 GMT
ENV REDIS_DOWNLOAD_SHA=5b2b8b7a50111ef395bf1c1d5be11e6e167ac018125055daa8b5c2317ae131ab
# Thu, 07 Oct 2021 20:53:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 07 Oct 2021 20:53:50 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 07 Oct 2021 20:53:50 GMT
VOLUME [/data]
# Thu, 07 Oct 2021 20:53:50 GMT
WORKDIR /data
# Thu, 07 Oct 2021 20:53:51 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 07 Oct 2021 20:53:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Oct 2021 20:53:51 GMT
EXPOSE 6379
# Thu, 07 Oct 2021 20:53:51 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:e79fce1f6442094a82dc5f6b4d1aa352e04aae39bba821c9021f6da08b1cacaf`  
		Last Modified: Tue, 28 Sep 2021 01:49:07 GMT  
		Size: 32.4 MB (32380160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1dab74a58b22b019d99fb261efb2dff6105ef3e96e616e7ecae897b28210ee`  
		Last Modified: Thu, 07 Oct 2021 20:58:21 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a83e6528dc785a1a6841e219b86bd10ba700eee8a469e78aa6658ec6ab284825`  
		Last Modified: Thu, 07 Oct 2021 20:58:22 GMT  
		Size: 1.4 MB (1413346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee5419e8d0d2191536edd01cd5d866fc816e4e8914e3647de8fd7d21264244f`  
		Last Modified: Thu, 07 Oct 2021 20:58:23 GMT  
		Size: 8.0 MB (7982880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a5b7a46db0e8fa99967d4fb1875b368036b500134c4fd677d68a9b004c0695c`  
		Last Modified: Thu, 07 Oct 2021 20:58:21 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adde60d48a85ccde382f5611d447655a4e61baea7d1f3f967ba85bdc5f14b0a3`  
		Last Modified: Thu, 07 Oct 2021 20:58:21 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:latest` - linux; mips64le

```console
$ docker pull redis@sha256:944694487329dc1db067106ef9458f5df99402f5246c40e8b02cb516c556f9b9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.6 MB (39640455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b8c49c6033fb722bd145e1d78b34451397e5b7cffb8f083ecd752a577299261`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Tue, 28 Sep 2021 02:10:40 GMT
ADD file:43593ef3d79c9b74a92e318d44aacb578f6f8d835dd72665e057bbfe73df1a93 in / 
# Tue, 28 Sep 2021 02:10:41 GMT
CMD ["bash"]
# Thu, 07 Oct 2021 20:14:44 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 07 Oct 2021 20:14:45 GMT
ENV GOSU_VERSION=1.12
# Thu, 07 Oct 2021 20:15:17 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 07 Oct 2021 20:15:17 GMT
ENV REDIS_VERSION=6.2.6
# Thu, 07 Oct 2021 20:15:17 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.6.tar.gz
# Thu, 07 Oct 2021 20:15:18 GMT
ENV REDIS_DOWNLOAD_SHA=5b2b8b7a50111ef395bf1c1d5be11e6e167ac018125055daa8b5c2317ae131ab
# Thu, 07 Oct 2021 20:18:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 07 Oct 2021 20:18:28 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 07 Oct 2021 20:18:29 GMT
VOLUME [/data]
# Thu, 07 Oct 2021 20:18:29 GMT
WORKDIR /data
# Thu, 07 Oct 2021 20:18:29 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 07 Oct 2021 20:18:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Oct 2021 20:18:30 GMT
EXPOSE 6379
# Thu, 07 Oct 2021 20:18:30 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:1f46ea49e27fccc580c8910db39ba7f51ae208a8d24d46a33140afa92ea3d955`  
		Last Modified: Tue, 28 Sep 2021 02:20:45 GMT  
		Size: 29.6 MB (29627871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff7455b351251e3574e185fead1aaf426cd358e283a5bdf112256c8cd784269`  
		Last Modified: Thu, 07 Oct 2021 20:25:17 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9f6e90aa3b254c78e19bc514ccd33afb485e684108bae0db40c1e6ec7d86972`  
		Last Modified: Thu, 07 Oct 2021 20:25:18 GMT  
		Size: 1.3 MB (1330980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd71076bc67ec837aea7ea5152c159a512af4baf6a5333e86f0a1b780e2d3f6`  
		Last Modified: Thu, 07 Oct 2021 20:25:24 GMT  
		Size: 8.7 MB (8679361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d7f72ddb547ef0771933f374f68a41fe1a811d0f0f4dd1e7731e429424cef1`  
		Last Modified: Thu, 07 Oct 2021 20:25:17 GMT  
		Size: 98.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3334420f98f5eb4b4ee807358b45566187b12276d0ba4687bc066e9866e4b632`  
		Last Modified: Thu, 07 Oct 2021 20:25:17 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:latest` - linux; ppc64le

```console
$ docker pull redis@sha256:4bfcd8bc8005356bc5f305764ad3803ea4c89e5a5514144a2fe4f1281fe4b704
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.5 MB (45536562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:650b2fc359a164e920c63b58dbf8f25d6748f98c64f81c62606596955b162524`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Mon, 04 Oct 2021 17:55:01 GMT
ADD file:f4b696a766a0d9a808c171a1d5db4f0877b0a784649d63bf461dfcf54b532239 in / 
# Mon, 04 Oct 2021 17:55:06 GMT
CMD ["bash"]
# Thu, 07 Oct 2021 23:14:01 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Thu, 07 Oct 2021 23:14:04 GMT
ENV GOSU_VERSION=1.12
# Thu, 07 Oct 2021 23:15:25 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 07 Oct 2021 23:15:27 GMT
ENV REDIS_VERSION=6.2.6
# Thu, 07 Oct 2021 23:15:29 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.6.tar.gz
# Thu, 07 Oct 2021 23:15:32 GMT
ENV REDIS_DOWNLOAD_SHA=5b2b8b7a50111ef395bf1c1d5be11e6e167ac018125055daa8b5c2317ae131ab
# Thu, 07 Oct 2021 23:18:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 07 Oct 2021 23:18:48 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 07 Oct 2021 23:18:50 GMT
VOLUME [/data]
# Thu, 07 Oct 2021 23:18:52 GMT
WORKDIR /data
# Thu, 07 Oct 2021 23:18:54 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 07 Oct 2021 23:18:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Oct 2021 23:18:59 GMT
EXPOSE 6379
# Thu, 07 Oct 2021 23:19:06 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:c3b7af0ed242d09d9fee2dfc48d4553d58ad90c5fb862ab58fb89e2d04c5b922`  
		Last Modified: Mon, 04 Oct 2021 18:07:32 GMT  
		Size: 35.3 MB (35272408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:880524651781169d23b58460167d03798148fc51dbd253e4fdc20c2f21adc8c2`  
		Last Modified: Thu, 07 Oct 2021 23:27:12 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26fd402769115b43e94bcc6d7908db58c48b02a9f4d90dba09396d2e643a155b`  
		Last Modified: Thu, 07 Oct 2021 23:27:12 GMT  
		Size: 1.4 MB (1361317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:141826f9de9242e0fd2e7d032e6d84a49300aabcc7d78a48753ab4cf4efd946f`  
		Last Modified: Thu, 07 Oct 2021 23:27:14 GMT  
		Size: 8.9 MB (8900553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7264c8a32e097b23d3a5947b2499ab152a51f2ef308e9f57d34be38a971ea2ce`  
		Last Modified: Thu, 07 Oct 2021 23:27:12 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4101d60dd7e22776ce9e3ce425086f08d58f5c87cce6f4d7c951c8b991cca30d`  
		Last Modified: Thu, 07 Oct 2021 23:27:11 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:latest` - linux; s390x

```console
$ docker pull redis@sha256:339ffd500031ba179d9c9bd5d891f90d1aaa5bcb4637ebb31d96380782661b1a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.8 MB (39760893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f15dfb1258f4503d49cdbb7b76985948e315bcc2c7b70913054ea0b33b3172e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["redis-server"]`

```dockerfile
# Tue, 12 Oct 2021 00:42:27 GMT
ADD file:6038dd6db57fb05c3d39c02c3379667ccd2989e7667ff773a8020fe6a69a760c in / 
# Tue, 12 Oct 2021 00:42:29 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 03:57:22 GMT
RUN groupadd -r -g 999 redis && useradd -r -g redis -u 999 redis
# Tue, 12 Oct 2021 03:57:22 GMT
ENV GOSU_VERSION=1.12
# Tue, 12 Oct 2021 03:57:30 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates dirmngr gnupg wget; 	rm -rf /var/lib/apt/lists/*; 	dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 	apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 12 Oct 2021 03:57:31 GMT
ENV REDIS_VERSION=6.2.6
# Tue, 12 Oct 2021 03:57:31 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-6.2.6.tar.gz
# Tue, 12 Oct 2021 03:57:31 GMT
ENV REDIS_DOWNLOAD_SHA=5b2b8b7a50111ef395bf1c1d5be11e6e167ac018125055daa8b5c2317ae131ab
# Tue, 12 Oct 2021 03:58:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		libssl-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -E '^ *createBoolConfig[(]"protected-mode",.*, *1 *,.*[)],$' /usr/src/redis/src/config.c; 	sed -ri 's!^( *createBoolConfig[(]"protected-mode",.*, *)1( *,.*[)],)$!\10\2!' /usr/src/redis/src/config.c; 	grep -E '^ *createBoolConfig[(]"protected-mode",.*, *0 *,.*[)],$' /usr/src/redis/src/config.c; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		export BUILD_TLS=yes; 	make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Tue, 12 Oct 2021 03:58:06 GMT
RUN mkdir /data && chown redis:redis /data
# Tue, 12 Oct 2021 03:58:06 GMT
VOLUME [/data]
# Tue, 12 Oct 2021 03:58:06 GMT
WORKDIR /data
# Tue, 12 Oct 2021 03:58:06 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Tue, 12 Oct 2021 03:58:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Oct 2021 03:58:06 GMT
EXPOSE 6379
# Tue, 12 Oct 2021 03:58:07 GMT
CMD ["redis-server"]
```

-	Layers:
	-	`sha256:ded751c48f72503973be01be2794cc039490f22b039b8ac106e9f17de4980742`  
		Last Modified: Tue, 12 Oct 2021 00:48:05 GMT  
		Size: 29.6 MB (29641215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98386a1364a2f66300ddad41aae2a80dfeb46d1713150409c2389667d3a843f6`  
		Last Modified: Tue, 12 Oct 2021 04:01:11 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4625e11cc10130d18306bbf5d90ccf110f16ca25379ebb1f991c2efd2b054248`  
		Last Modified: Tue, 12 Oct 2021 04:01:11 GMT  
		Size: 1.4 MB (1429170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e0db9aa599212d0eb07db385639b57eed9ac5e50ddb36fcf4b066350ebfad0`  
		Last Modified: Tue, 12 Oct 2021 04:01:12 GMT  
		Size: 8.7 MB (8688230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ccc5bc404f07cb6b030f802362894d2634a56fc4e3d4af749ed264a361bf95`  
		Last Modified: Tue, 12 Oct 2021 04:01:11 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9876266500c5b02b62c89df238dab066f397dd4c27109df1aecf3aa91bbec164`  
		Last Modified: Tue, 12 Oct 2021 04:01:11 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
