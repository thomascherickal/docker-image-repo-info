## `redis:5-buster`

```console
$ docker pull redis@sha256:3dd5f850c693b941c8355f9fdacc5edaa2b5542e36595401f55c5d77420939a6
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

### `redis:5-buster` - linux; amd64

```console
$ docker pull redis@sha256:187244c6bc6ac03a9a00ad275798a16dde3091eea2136af70396be939928c110
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35920503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aec43d10ed3b8db033b6429837ec2e600c682282112b6ae7682eb9b1a5f42449`
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
# Wed, 23 Jun 2021 16:37:56 GMT
ENV REDIS_VERSION=5.0.12
# Wed, 23 Jun 2021 16:37:57 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.12.tar.gz
# Wed, 23 Jun 2021 16:37:57 GMT
ENV REDIS_DOWNLOAD_SHA=7040eba5910f7c3d38f05ea5a1d88b480488215bdbd2e10ec70d18380108e31e
# Wed, 23 Jun 2021 16:38:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Wed, 23 Jun 2021 16:38:57 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 23 Jun 2021 16:38:58 GMT
VOLUME [/data]
# Wed, 23 Jun 2021 16:38:58 GMT
WORKDIR /data
# Wed, 23 Jun 2021 16:38:59 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Wed, 23 Jun 2021 16:38:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 16:38:59 GMT
EXPOSE 6379
# Wed, 23 Jun 2021 16:39:00 GMT
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
	-	`sha256:3608e9786a516281856b848eaaf9941a4061d604bbd822ec27d39b0cbc196287`  
		Last Modified: Wed, 23 Jun 2021 16:42:23 GMT  
		Size: 7.4 MB (7354408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f881640d21d85f7185739be676d1169526e3db4ed5b06421f7badc6c93dd79d6`  
		Last Modified: Wed, 23 Jun 2021 16:42:21 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95a8978f46d8c5f4dcc9be72a128880866a94f941f2e1dfc551e77dfb11ac2a3`  
		Last Modified: Wed, 23 Jun 2021 16:42:21 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-buster` - linux; arm variant v5

```console
$ docker pull redis@sha256:f24092a686b0d79fe295edda59d9ced2da43415658594b70ffdb18445ab776b2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.4 MB (33440145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66e5de1f6f479549cea2666c58eec278c3cfaebd2425f729e0579efe21c2c564`
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
# Wed, 23 Jun 2021 08:57:41 GMT
ENV REDIS_VERSION=5.0.12
# Wed, 23 Jun 2021 08:57:41 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.12.tar.gz
# Wed, 23 Jun 2021 08:57:41 GMT
ENV REDIS_DOWNLOAD_SHA=7040eba5910f7c3d38f05ea5a1d88b480488215bdbd2e10ec70d18380108e31e
# Wed, 23 Jun 2021 08:59:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Wed, 23 Jun 2021 08:59:14 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 23 Jun 2021 08:59:14 GMT
VOLUME [/data]
# Wed, 23 Jun 2021 08:59:15 GMT
WORKDIR /data
# Wed, 23 Jun 2021 08:59:15 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Wed, 23 Jun 2021 08:59:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 08:59:16 GMT
EXPOSE 6379
# Wed, 23 Jun 2021 08:59:16 GMT
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
	-	`sha256:acb5a5402d162f2dcc89ad5b306ad90d438f0b1d73d56eb4f979523240fab396`  
		Last Modified: Wed, 23 Jun 2021 09:02:03 GMT  
		Size: 7.2 MB (7182706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8e080c6a0c8fc85be0c5f516f5bfb11f2910ebf871d60394aa218652305ec01`  
		Last Modified: Wed, 23 Jun 2021 09:01:58 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9689d4ea225aff23c1339a4b6ed4cb0f1a58e7019ebaff9d3b9fcf544cb12764`  
		Last Modified: Wed, 23 Jun 2021 09:01:58 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-buster` - linux; arm variant v7

```console
$ docker pull redis@sha256:c6d47a0b1dd8b43c51ac255264afe8dcc6718e9d63ff7ae7386a815515e12772
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31155634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83dca8235b11e983ad2b523eacf2ce047370330a3da481b9f49f8ef856429ec1`
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
# Thu, 24 Jun 2021 07:15:03 GMT
ENV REDIS_VERSION=5.0.12
# Thu, 24 Jun 2021 07:15:03 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.12.tar.gz
# Thu, 24 Jun 2021 07:15:04 GMT
ENV REDIS_DOWNLOAD_SHA=7040eba5910f7c3d38f05ea5a1d88b480488215bdbd2e10ec70d18380108e31e
# Thu, 24 Jun 2021 07:16:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 24 Jun 2021 07:16:29 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 24 Jun 2021 07:16:30 GMT
VOLUME [/data]
# Thu, 24 Jun 2021 07:16:30 GMT
WORKDIR /data
# Thu, 24 Jun 2021 07:16:31 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 24 Jun 2021 07:16:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Jun 2021 07:16:32 GMT
EXPOSE 6379
# Thu, 24 Jun 2021 07:16:32 GMT
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
	-	`sha256:c2df3f4495e220a622896951d96e217f2b97b935d5b3123713ca29d05962f9e2`  
		Last Modified: Thu, 24 Jun 2021 07:23:08 GMT  
		Size: 7.0 MB (7038980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb301fa4071422729c52aa98f9e19b106a2d2402a0ad4b1ead09e8e146865ca`  
		Last Modified: Thu, 24 Jun 2021 07:23:03 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5402cf4bebcac8dc78d899c1e3d70f01e1d36f6afddd6bac14a1a43a55a89e52`  
		Last Modified: Thu, 24 Jun 2021 07:23:03 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-buster` - linux; arm64 variant v8

```console
$ docker pull redis@sha256:a6b3dea248895274c6ada962ac732ca605884762eccbd370bf448e8f17092b0f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.6 MB (34635329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4da7c7928ba0162ce671fbdf663bd5e5c38751bbb9b6538f6a9ca259989d1d63`
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
# Wed, 23 Jun 2021 12:48:06 GMT
ENV REDIS_VERSION=5.0.12
# Wed, 23 Jun 2021 12:48:06 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.12.tar.gz
# Wed, 23 Jun 2021 12:48:06 GMT
ENV REDIS_DOWNLOAD_SHA=7040eba5910f7c3d38f05ea5a1d88b480488215bdbd2e10ec70d18380108e31e
# Wed, 23 Jun 2021 12:48:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Wed, 23 Jun 2021 12:48:53 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 23 Jun 2021 12:48:54 GMT
VOLUME [/data]
# Wed, 23 Jun 2021 12:48:54 GMT
WORKDIR /data
# Wed, 23 Jun 2021 12:48:54 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Wed, 23 Jun 2021 12:48:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 12:48:54 GMT
EXPOSE 6379
# Wed, 23 Jun 2021 12:48:55 GMT
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
	-	`sha256:8e20ce7c3ac1fdb13069c890dfe38edec6a268168b7f173054999d2b0a137b5d`  
		Last Modified: Wed, 23 Jun 2021 12:51:32 GMT  
		Size: 7.4 MB (7365069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f13d23954fc04c2d3d08dd4e7872259c63a1808a35489caf8a060302dc571617`  
		Last Modified: Wed, 23 Jun 2021 12:51:30 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5975da0ee683b0e12dfa5acf1dd91523a33fb082b7572078f292cd6b3231dbd6`  
		Last Modified: Wed, 23 Jun 2021 12:51:30 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-buster` - linux; 386

```console
$ docker pull redis@sha256:e06b4d815ab73f629cb80d13c415adf537c0754ffb709d481d4f3d7e78dc8906
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.2 MB (36206220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f83dcf263d7beb0474bbe8178c61414ba21e574e7007d2250b60a67ac400800c`
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
# Wed, 23 Jun 2021 13:23:04 GMT
ENV REDIS_VERSION=5.0.12
# Wed, 23 Jun 2021 13:23:04 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.12.tar.gz
# Wed, 23 Jun 2021 13:23:04 GMT
ENV REDIS_DOWNLOAD_SHA=7040eba5910f7c3d38f05ea5a1d88b480488215bdbd2e10ec70d18380108e31e
# Wed, 23 Jun 2021 13:24:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Wed, 23 Jun 2021 13:24:35 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 23 Jun 2021 13:24:35 GMT
VOLUME [/data]
# Wed, 23 Jun 2021 13:24:35 GMT
WORKDIR /data
# Wed, 23 Jun 2021 13:24:36 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Wed, 23 Jun 2021 13:24:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 13:24:36 GMT
EXPOSE 6379
# Wed, 23 Jun 2021 13:24:36 GMT
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
	-	`sha256:6fc6170f1042ab636fae0b985e2eb9afa18ab74a56b8a06f53af4f31b0fdebc1`  
		Last Modified: Wed, 23 Jun 2021 13:27:41 GMT  
		Size: 7.0 MB (7018889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c858dadcdf962c124841fb3c3e30802c73686e4c93b7624128e2e1b969a35ac`  
		Last Modified: Wed, 23 Jun 2021 13:27:39 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9635d9cfb7c8f2d2d4093bf06e386fff1011ef1f713aaec8f5587452ddd08396`  
		Last Modified: Wed, 23 Jun 2021 13:27:39 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-buster` - linux; mips64le

```console
$ docker pull redis@sha256:058adc1c420f96bae6d5c378add6ea0cf70cc10875a836ce80c594fca148d386
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34790918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e90a1f6754fc7a739b38726a890528f5f2f2f7e611a8bfc8cf730a6bdb689c0`
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
# Wed, 23 Jun 2021 16:42:00 GMT
ENV REDIS_VERSION=5.0.12
# Wed, 23 Jun 2021 16:42:00 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.12.tar.gz
# Wed, 23 Jun 2021 16:42:00 GMT
ENV REDIS_DOWNLOAD_SHA=7040eba5910f7c3d38f05ea5a1d88b480488215bdbd2e10ec70d18380108e31e
# Wed, 23 Jun 2021 16:44:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Wed, 23 Jun 2021 16:44:48 GMT
RUN mkdir /data && chown redis:redis /data
# Wed, 23 Jun 2021 16:44:48 GMT
VOLUME [/data]
# Wed, 23 Jun 2021 16:44:49 GMT
WORKDIR /data
# Wed, 23 Jun 2021 16:44:49 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Wed, 23 Jun 2021 16:44:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 16:44:50 GMT
EXPOSE 6379
# Wed, 23 Jun 2021 16:44:50 GMT
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
	-	`sha256:fd67a469b7e1d284ee66ed730de08935e536b16890e0b677ec3bc3f10b2357b9`  
		Last Modified: Wed, 23 Jun 2021 16:46:20 GMT  
		Size: 7.7 MB (7670148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61e21018df712e5d26e7d32b9e4a42498808c5a6ea24fdb7d1c55575fd4acc7`  
		Last Modified: Wed, 23 Jun 2021 16:46:14 GMT  
		Size: 97.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:783ef907bc4a792ac41f6bf5f728c8324fc79982a1442bb17af350568e439949`  
		Last Modified: Wed, 23 Jun 2021 16:46:14 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-buster` - linux; ppc64le

```console
$ docker pull redis@sha256:2b03d13a165088282d560b2bbadb22355f981eba818c23402bb1d14baea76e76
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.7 MB (39738560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:379333f51ea9ea19ed77a6828d37d5013aaccdb77cb375878883ff30efa9bf99`
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
# Thu, 08 Jul 2021 17:33:20 GMT
ENV REDIS_VERSION=5.0.12
# Thu, 08 Jul 2021 17:33:23 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.12.tar.gz
# Thu, 08 Jul 2021 17:33:26 GMT
ENV REDIS_DOWNLOAD_SHA=7040eba5910f7c3d38f05ea5a1d88b480488215bdbd2e10ec70d18380108e31e
# Thu, 08 Jul 2021 17:37:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Thu, 08 Jul 2021 17:37:32 GMT
RUN mkdir /data && chown redis:redis /data
# Thu, 08 Jul 2021 17:37:38 GMT
VOLUME [/data]
# Thu, 08 Jul 2021 17:37:43 GMT
WORKDIR /data
# Thu, 08 Jul 2021 17:37:45 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Thu, 08 Jul 2021 17:37:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 17:37:55 GMT
EXPOSE 6379
# Thu, 08 Jul 2021 17:37:59 GMT
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
	-	`sha256:df452bf7b43738b619bb478bba162305b9fd995399b3f6aa4d4d1d1bfa9e8f4b`  
		Last Modified: Thu, 08 Jul 2021 17:41:44 GMT  
		Size: 7.8 MB (7847057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c516a8165fda4c673424a6c909b7ccebf48425dca12ead8679962904835fde`  
		Last Modified: Thu, 08 Jul 2021 17:41:42 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec03e4d2f479ed310c2df2117d1757a0b1627da01e26972ecdc34a413c982fcd`  
		Last Modified: Thu, 08 Jul 2021 17:41:42 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redis:5-buster` - linux; s390x

```console
$ docker pull redis@sha256:5207cdd737c5fd574ff711efde072718ed08fa566aceed1c9657c13ec64b88f0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34802681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:192334fcbc7b6b738ed97a7154f79f53335bbd9fb08ec689062a2c77287e849c`
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
# Fri, 09 Jul 2021 20:45:22 GMT
ENV REDIS_VERSION=5.0.12
# Fri, 09 Jul 2021 20:45:23 GMT
ENV REDIS_DOWNLOAD_URL=http://download.redis.io/releases/redis-5.0.12.tar.gz
# Fri, 09 Jul 2021 20:45:23 GMT
ENV REDIS_DOWNLOAD_SHA=7040eba5910f7c3d38f05ea5a1d88b480488215bdbd2e10ec70d18380108e31e
# Fri, 09 Jul 2021 20:46:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				dpkg-dev 		gcc 		libc6-dev 		make 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O redis.tar.gz "$REDIS_DOWNLOAD_URL"; 	echo "$REDIS_DOWNLOAD_SHA *redis.tar.gz" | sha256sum -c -; 	mkdir -p /usr/src/redis; 	tar -xzf redis.tar.gz -C /usr/src/redis --strip-components=1; 	rm redis.tar.gz; 		grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 1$' /usr/src/redis/src/server.h; 	sed -ri 's!^(#define CONFIG_DEFAULT_PROTECTED_MODE) 1$!\1 0!' /usr/src/redis/src/server.h; 	grep -q '^#define CONFIG_DEFAULT_PROTECTED_MODE 0$' /usr/src/redis/src/server.h; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	extraJemallocConfigureFlags="--build=$gnuArch"; 	dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64 | i386 | x32) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=12" ;; 		*) extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-page=16" ;; 	esac; 	extraJemallocConfigureFlags="$extraJemallocConfigureFlags --with-lg-hugepage=21"; 	grep -F 'cd jemalloc && ./configure ' /usr/src/redis/deps/Makefile; 	sed -ri 's!cd jemalloc && ./configure !&'"$extraJemallocConfigureFlags"' !' /usr/src/redis/deps/Makefile; 	grep -F "cd jemalloc && ./configure $extraJemallocConfigureFlags " /usr/src/redis/deps/Makefile; 		make -C /usr/src/redis -j "$(nproc)" all; 	make -C /usr/src/redis install; 		serverMd5="$(md5sum /usr/local/bin/redis-server | cut -d' ' -f1)"; export serverMd5; 	find /usr/local/bin/redis* -maxdepth 0 		-type f -not -name redis-server 		-exec sh -eux -c ' 			md5="$(md5sum "$1" | cut -d" " -f1)"; 			test "$md5" = "$serverMd5"; 		' -- '{}' ';' 		-exec ln -svfT 'redis-server' '{}' ';' 	; 		rm -r /usr/src/redis; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		redis-cli --version; 	redis-server --version
# Fri, 09 Jul 2021 20:46:08 GMT
RUN mkdir /data && chown redis:redis /data
# Fri, 09 Jul 2021 20:46:08 GMT
VOLUME [/data]
# Fri, 09 Jul 2021 20:46:08 GMT
WORKDIR /data
# Fri, 09 Jul 2021 20:46:09 GMT
COPY file:df205a0ef6e6df8947ce0a7ae9e37b6a5588035647f38a49b8b07321003a8a01 in /usr/local/bin/ 
# Fri, 09 Jul 2021 20:46:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 09 Jul 2021 20:46:09 GMT
EXPOSE 6379
# Fri, 09 Jul 2021 20:46:10 GMT
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
	-	`sha256:9d187f0aac0396729fa090fbd7b43069a11301e74c00eca4db3061fc9f0de4ba`  
		Last Modified: Fri, 09 Jul 2021 20:55:49 GMT  
		Size: 7.6 MB (7635684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f62261531b61573da2cd7eb18e15af648a33df8507227f81e86937d9662ae49`  
		Last Modified: Fri, 09 Jul 2021 20:55:48 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a56aefb84d2e3e850ba002c3ab430114953c183b4b960d20c374e3cc79752ac`  
		Last Modified: Fri, 09 Jul 2021 20:55:48 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
