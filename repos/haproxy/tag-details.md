<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `haproxy`

-	[`haproxy:1.7`](#haproxy17)
-	[`haproxy:1.7-alpine`](#haproxy17-alpine)
-	[`haproxy:1.7.14`](#haproxy1714)
-	[`haproxy:1.7.14-alpine`](#haproxy1714-alpine)
-	[`haproxy:1.8`](#haproxy18)
-	[`haproxy:1.8-alpine`](#haproxy18-alpine)
-	[`haproxy:1.8.30`](#haproxy1830)
-	[`haproxy:1.8.30-alpine`](#haproxy1830-alpine)
-	[`haproxy:2.0`](#haproxy20)
-	[`haproxy:2.0-alpine`](#haproxy20-alpine)
-	[`haproxy:2.0.23`](#haproxy2023)
-	[`haproxy:2.0.23-alpine`](#haproxy2023-alpine)
-	[`haproxy:2.2`](#haproxy22)
-	[`haproxy:2.2-alpine`](#haproxy22-alpine)
-	[`haproxy:2.2.15`](#haproxy2215)
-	[`haproxy:2.2.15-alpine`](#haproxy2215-alpine)
-	[`haproxy:2.3`](#haproxy23)
-	[`haproxy:2.3-alpine`](#haproxy23-alpine)
-	[`haproxy:2.3.12`](#haproxy2312)
-	[`haproxy:2.3.12-alpine`](#haproxy2312-alpine)
-	[`haproxy:2.4`](#haproxy24)
-	[`haproxy:2.4-alpine`](#haproxy24-alpine)
-	[`haproxy:2.4.2`](#haproxy242)
-	[`haproxy:2.4.2-alpine`](#haproxy242-alpine)
-	[`haproxy:2.5-dev`](#haproxy25-dev)
-	[`haproxy:2.5-dev-alpine`](#haproxy25-dev-alpine)
-	[`haproxy:2.5-dev2`](#haproxy25-dev2)
-	[`haproxy:2.5-dev2-alpine`](#haproxy25-dev2-alpine)
-	[`haproxy:alpine`](#haproxyalpine)
-	[`haproxy:latest`](#haproxylatest)
-	[`haproxy:lts`](#haproxylts)
-	[`haproxy:lts-alpine`](#haproxylts-alpine)

## `haproxy:1.7`

```console
$ docker pull haproxy@sha256:4c8908c0072a73ef6f5fe77aa0f7ea511cefdd50d8509ff0b43ba13f3f104066
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

### `haproxy:1.7` - linux; amd64

```console
$ docker pull haproxy@sha256:3d461dbce17a816277f813d59fdcad592d9b5c8188fbca83908b1e3db59f10d9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.5 MB (32541296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9be1737d9bbe86e16c10fcb2f8eb938d2c06640bc27138fd5ad117f811bac40b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 06:19:17 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 23 Jun 2021 06:27:30 GMT
ENV HAPROXY_VERSION=1.7.14
# Wed, 23 Jun 2021 06:27:30 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Wed, 23 Jun 2021 06:27:30 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Wed, 23 Jun 2021 06:28:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 23 Jun 2021 06:28:13 GMT
STOPSIGNAL SIGUSR1
# Wed, 23 Jun 2021 06:28:13 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Wed, 23 Jun 2021 06:28:14 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 23 Jun 2021 06:28:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 06:28:15 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91332cb81883405a321c1a2d2144bdd0aef8d1c69f90fdf0cf219982161b6e6e`  
		Last Modified: Wed, 23 Jun 2021 06:29:07 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:665e7a14a17f6fe1b65bc8010c568864f830e8a937c5707f6e68c2724a2f1415`  
		Last Modified: Wed, 23 Jun 2021 06:30:37 GMT  
		Size: 5.4 MB (5393475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dccd5cee97007600fc7a9cad5980265f2cead92d390911c5f2aa5e8879a064bb`  
		Last Modified: Wed, 23 Jun 2021 06:30:36 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5688c2df927a2c9a7dbe90061cbd2d45c426d7af4a2f47c03eb9be039e223728`  
		Last Modified: Wed, 23 Jun 2021 06:30:36 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:eb40db1ad848dbcc5322aa69af01d4789b1246328750535ca3cf348c84b7c431
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.9 MB (29901157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e146711fa968989fe60f3dd8be14de2800be27104e98a634f3583255612c848`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 22 Jun 2021 23:50:09 GMT
ADD file:78d4ced31112d85490c684f350aceeebfc72a804262c7ad3e033257e3894f5c4 in / 
# Tue, 22 Jun 2021 23:50:11 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:15:11 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 23 Jun 2021 05:21:52 GMT
ENV HAPROXY_VERSION=1.7.14
# Wed, 23 Jun 2021 05:21:53 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Wed, 23 Jun 2021 05:21:53 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Wed, 23 Jun 2021 05:22:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 23 Jun 2021 05:22:42 GMT
STOPSIGNAL SIGUSR1
# Wed, 23 Jun 2021 05:22:42 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Wed, 23 Jun 2021 05:22:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 23 Jun 2021 05:22:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 05:22:44 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:532d6df30af5174ac6e1b379c32b8f464d44651ac060376a560c4a76a87704a7`  
		Last Modified: Wed, 23 Jun 2021 00:01:46 GMT  
		Size: 24.9 MB (24878945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48649e3d7de4cd80d3a9a34c725a2935be904ff90e99ea6c8e4bb6e1e7a4eeb7`  
		Last Modified: Wed, 23 Jun 2021 05:24:11 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:170f6401c23b3b6db35408132d6b6487f4b6e7ccdc9b6a384426636adc787dac`  
		Last Modified: Wed, 23 Jun 2021 05:26:11 GMT  
		Size: 5.0 MB (5020242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba60f03140a88c98fd76bbf209b30e2c635f793d650ef0a5fabf88df6fa84358`  
		Last Modified: Wed, 23 Jun 2021 05:26:07 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed57b998443ddcd697a62040539bf6500f70cde810b550776a396497e19abbc4`  
		Last Modified: Wed, 23 Jun 2021 05:26:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:5bf1be3afe675072cef4473312e51c4ed9b3dd1efee0090f9da55a02234fbfd7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.6 MB (27640225 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8aae63f0809a60888ba04d9fa70fdc6d5f0224aaaf6941fd7a422cb9130b911`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:31 GMT
ADD file:8d200a3bbe985ff355343675c5555852f27550a9e367969df6bc98034efb8fd4 in / 
# Wed, 23 Jun 2021 00:20:31 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:21:41 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 23 Jun 2021 05:32:03 GMT
ENV HAPROXY_VERSION=1.7.14
# Wed, 23 Jun 2021 05:32:04 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Wed, 23 Jun 2021 05:32:04 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Wed, 23 Jun 2021 05:32:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 23 Jun 2021 05:32:49 GMT
STOPSIGNAL SIGUSR1
# Wed, 23 Jun 2021 05:32:49 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Wed, 23 Jun 2021 05:32:51 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 23 Jun 2021 05:32:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 05:32:52 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:8452be1adf00f91570fe21a8e61aaf4c12e014daf67d7de65d984f4e8ecca2f1`  
		Last Modified: Wed, 23 Jun 2021 00:31:49 GMT  
		Size: 22.7 MB (22746055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed1c9c92d0076fd4bf40503e3f47102509a5b99d182f4dd9e81e64d0a7e0b8a`  
		Last Modified: Wed, 23 Jun 2021 05:35:48 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4ddb74c7a1350f6335ed180208075ce88a1db859fc405d7ddda0dc47b98b94`  
		Last Modified: Wed, 23 Jun 2021 05:39:21 GMT  
		Size: 4.9 MB (4892197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f289bf8c6c4e11830a6c2920e1a656b5c46f9b454a21d57c1129f9aa35260df8`  
		Last Modified: Wed, 23 Jun 2021 05:39:18 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6062074497a0994f1f648d5799560f3e732d12502b938eab4525d2b3b22ec9a`  
		Last Modified: Wed, 23 Jun 2021 05:39:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:9fcc85c1fd689edcc3a6f03204170145bc9757478534a5d5554d613d2e17060e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31197976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d018078b9507ee49d00dec4231d3217d31540e91104da7161eebf1dfa60865b6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:40 GMT
ADD file:beee00b59da720f68e12e2ba2a8134207c80c777ddb4ceb03c71e3e4c3f51c93 in / 
# Tue, 22 Jun 2021 23:49:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 03:19:31 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 23 Jun 2021 03:24:30 GMT
ENV HAPROXY_VERSION=1.7.14
# Wed, 23 Jun 2021 03:24:30 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Wed, 23 Jun 2021 03:24:31 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Wed, 23 Jun 2021 03:24:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 23 Jun 2021 03:24:56 GMT
STOPSIGNAL SIGUSR1
# Wed, 23 Jun 2021 03:24:56 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Wed, 23 Jun 2021 03:24:57 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 23 Jun 2021 03:24:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 03:24:57 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:448f6bf000e31217a7c202c659b03b7f8ac8d3ae6b03ef7a2f8339be2f00ff4a`  
		Last Modified: Tue, 22 Jun 2021 23:55:25 GMT  
		Size: 25.9 MB (25914993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b05ad81dc8a7d67656235988f0e5fb72c374c7d8df44c105b91d712e06c4ac`  
		Last Modified: Wed, 23 Jun 2021 03:26:16 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edc87e3339ee885225543831e8b2dfda8cba3610676e3993a8f31b171486cbd1`  
		Last Modified: Wed, 23 Jun 2021 03:27:52 GMT  
		Size: 5.3 MB (5281010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0335c8e3127a6be5a9f7c49aef80a03c093fd5412a108693b1434c203d69162`  
		Last Modified: Wed, 23 Jun 2021 03:27:51 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41c07a18fd101002b18aaac65e6f589572bfd53f3de33de84f208568b9e23eea`  
		Last Modified: Wed, 23 Jun 2021 03:27:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7` - linux; 386

```console
$ docker pull haproxy@sha256:7385f826a4450550dadc352efa8c933a2b50bdb03eb28997452b0fc310bfc70e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.1 MB (33123397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6daa1c38e094d95fd74d0009b946bca8dfb85a4376792393de8731069959803`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 22 Jun 2021 23:39:35 GMT
ADD file:48f656ac6733911048b3de850490438d0233b3badc11861fca62062d4edfaf40 in / 
# Tue, 22 Jun 2021 23:39:35 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:23:13 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 23 Jun 2021 00:30:01 GMT
ENV HAPROXY_VERSION=1.7.14
# Wed, 23 Jun 2021 00:30:01 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Wed, 23 Jun 2021 00:30:01 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Wed, 23 Jun 2021 00:30:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 23 Jun 2021 00:30:34 GMT
STOPSIGNAL SIGUSR1
# Wed, 23 Jun 2021 00:30:35 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Wed, 23 Jun 2021 00:30:35 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 23 Jun 2021 00:30:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 00:30:36 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:33af2dcb865e65d53cdeb843b67a0ef62151fa32df292293e7c6b0eb728ac5ac`  
		Last Modified: Tue, 22 Jun 2021 23:46:23 GMT  
		Size: 27.8 MB (27797411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a6e4d42b23996eb7d8a1baa85ee19828c2667fd4a2dca6eb1040b266680e9f`  
		Last Modified: Wed, 23 Jun 2021 00:32:00 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b27b997e8598f8116677e406f452f79707677c4b1df6495585abbc1f29238ad`  
		Last Modified: Wed, 23 Jun 2021 00:33:38 GMT  
		Size: 5.3 MB (5324016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f072c4b4c9ec2e76fb216777fac9153f6dcf22a5685ebdf52bbffdd97acfc05b`  
		Last Modified: Wed, 23 Jun 2021 00:33:36 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eee6b076bba5aada707e31ff5f8d84e272f47e3a9370c00532d0ab727eb5383`  
		Last Modified: Wed, 23 Jun 2021 00:33:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7` - linux; mips64le

```console
$ docker pull haproxy@sha256:37fbe8b99980c76d6738dd65c4258ec5b78ba6423298e3405ea3e63e6771773f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.8 MB (30842533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3abb2ea5d80b752c7bf7e8c17369ab97a8361783739a6a0ee92602fd9b633bdf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 22 Jul 2021 00:09:45 GMT
ADD file:1f77b9001c4977ba733be674fc5eb4b85130f1dea8a7b39d545b70f9c107695f in / 
# Thu, 22 Jul 2021 00:09:46 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:07:49 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 22 Jul 2021 01:22:40 GMT
ENV HAPROXY_VERSION=1.7.14
# Thu, 22 Jul 2021 01:22:40 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Thu, 22 Jul 2021 01:22:41 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Thu, 22 Jul 2021 01:24:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 22 Jul 2021 01:24:06 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 01:24:06 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Thu, 22 Jul 2021 01:24:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Jul 2021 01:24:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 01:24:09 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:99ee621d0b0485e9de65aa19604aa2453d19ea7fc86b22c5b77c1bab74e3cb42`  
		Last Modified: Thu, 22 Jul 2021 00:16:11 GMT  
		Size: 25.8 MB (25812771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f444627794f98947a9df95ec5d19b2a1cd6c151ed438982b1dc0b89f5eaf19e`  
		Last Modified: Thu, 22 Jul 2021 01:24:39 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad8199dbb9f3f9e98bbd8dea7146b6ba797f846c74e703dea2dfa9e753c72da3`  
		Last Modified: Thu, 22 Jul 2021 01:26:25 GMT  
		Size: 5.0 MB (5027791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4ffe21fcf7ac71e04543b553d963d67c0c0d26535369b460875de7f653247e`  
		Last Modified: Thu, 22 Jul 2021 01:26:21 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244dceab14585bfcb12416cb1018527be5ecfeae00575b4b183ff3cac009a55c`  
		Last Modified: Thu, 22 Jul 2021 01:26:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7` - linux; ppc64le

```console
$ docker pull haproxy@sha256:1abfbe399c3e8807e50431c134c8b97d0cf2eced31e8d532dcacd8cefccc8ab7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36266404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:719f475fb89a446baf503d2feb34d7b5814d2c8a6c5fd9561842e9a8e963316d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 22 Jul 2021 00:19:04 GMT
ADD file:3a6bd6ce3eff98b88a13de5d0f26cff0b026f876674204dbad6f84fafcf145b1 in / 
# Thu, 22 Jul 2021 00:19:13 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 02:52:46 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 22 Jul 2021 03:33:15 GMT
ENV HAPROXY_VERSION=1.7.14
# Thu, 22 Jul 2021 03:33:21 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Thu, 22 Jul 2021 03:33:25 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Thu, 22 Jul 2021 03:37:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 22 Jul 2021 03:37:47 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 03:37:51 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Thu, 22 Jul 2021 03:38:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Jul 2021 03:38:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 03:38:19 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:1130517d52da84a09f9465006bddab5e49afd398860890eab6274fd0bff32371`  
		Last Modified: Thu, 22 Jul 2021 00:27:49 GMT  
		Size: 30.6 MB (30553709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251bf3fe1d4bbe9c27e393cd8ddc550b56cec90eb916bf9bec24d657c9f6556f`  
		Last Modified: Thu, 22 Jul 2021 03:40:01 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a29f6d6804eb054d0c618384a92189f202e0cf1932e49b2a2582a675fa5b0ff2`  
		Last Modified: Thu, 22 Jul 2021 03:43:02 GMT  
		Size: 5.7 MB (5710724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0445214d7e223706b47751dd070f47e33c533caa0278329641fdc4db7390015d`  
		Last Modified: Thu, 22 Jul 2021 03:43:01 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f703a80a7b00ccb9b5604f68c2050f000ed0da1cad292175530b03014a713ff`  
		Last Modified: Thu, 22 Jul 2021 03:43:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7` - linux; s390x

```console
$ docker pull haproxy@sha256:7e952ce5ecc34758ff5e94aeca5a3831c9ddd602005fb1a19302b5bfbcdb1872
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.9 MB (30891864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5dc3a063fcda3f6020320a2d0abb1ea67604a8bfc767ae1bd3d4d3fa67ea762`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 22 Jul 2021 00:42:45 GMT
ADD file:1ab999eb6f80d8ce91ce3a173e23fd2710f2779117bba29037eaa82aadcbf6ed in / 
# Thu, 22 Jul 2021 00:42:48 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:30:19 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 22 Jul 2021 01:38:31 GMT
ENV HAPROXY_VERSION=1.7.14
# Thu, 22 Jul 2021 01:38:32 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Thu, 22 Jul 2021 01:38:32 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Thu, 22 Jul 2021 01:38:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 22 Jul 2021 01:38:58 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 01:38:58 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Thu, 22 Jul 2021 01:38:59 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Jul 2021 01:39:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 01:39:00 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:7a50fdd85ff244c1465e71c51354d055e3df0b90ff5faad28cc22d9ecde9daf3`  
		Last Modified: Thu, 22 Jul 2021 00:48:13 GMT  
		Size: 25.8 MB (25760761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05fb34d1ed21b67502665114a7ae60445472fc7bafa620bbf6c79b7df85a01d4`  
		Last Modified: Thu, 22 Jul 2021 01:39:54 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d133f88f7bf0d9f7fd35aeb02cf4e3d54fa2264868d3553fed415864b067e204`  
		Last Modified: Thu, 22 Jul 2021 01:40:57 GMT  
		Size: 5.1 MB (5129131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a088aeea9fbccb475252ae3098ca841aaa5f0cc910d40d58cd65bb04654d54f1`  
		Last Modified: Thu, 22 Jul 2021 01:40:56 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be65e63201a559c73a322bea91f4ef1b8bc5c4e54994efe33d142261911d9993`  
		Last Modified: Thu, 22 Jul 2021 01:40:56 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:1.7-alpine`

```console
$ docker pull haproxy@sha256:f8946d8c90ff0e2f7c56e1f8d5afe87356b7864db3713a4558c987b5b264e8ce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `haproxy:1.7-alpine` - linux; amd64

```console
$ docker pull haproxy@sha256:585430cbbec0b6df064587170ed3ac0104e263290ffc6f6d63dfeb3d263437f7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.5 MB (3547528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f57f9af8fae5238962a097fdf78d150e3d0cc1160c1495149e0011cdd22cf77`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:42:45 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 21:42:45 GMT
ENV HAPROXY_VERSION=1.7.14
# Wed, 14 Apr 2021 21:42:45 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Wed, 14 Apr 2021 21:42:46 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Wed, 14 Apr 2021 21:42:57 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		CFLAGS+="-Wno-address-of-packed-member" 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 21:42:57 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 21:42:57 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Wed, 14 Apr 2021 21:42:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 21:42:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 21:42:58 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e79a8d3da5b7b8e6a180e6fa428bf4a36b8f8bc0e3675927aeb0860a92747561`  
		Last Modified: Wed, 14 Apr 2021 21:44:42 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ba53b9604ae0a19fc162eca377f3de4c0deb844929aa614806d7566b55d42e`  
		Last Modified: Wed, 14 Apr 2021 21:44:43 GMT  
		Size: 745.2 KB (745185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f8509370c0a2bc5abc5c0de684ae960d3917ef4fae3de452c52e6a83619de90`  
		Last Modified: Wed, 14 Apr 2021 21:44:42 GMT  
		Size: 471.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0bf7494a1e4cf18a66f609c0be15d90d5ec36c6eeb05c116acbd0f00ae4cc08`  
		Last Modified: Wed, 14 Apr 2021 21:44:42 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7-alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:91f9984cff0f997f604f6ce233ded4cfa3c3f29a81bb40820a2575e3943cb5d4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 MB (3326550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1be9c767dd4ef5c7d0d34901388b0853c249afbdf3b7ba7a4ae92e5bbc49f1dd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:41 GMT
ADD file:82fa6a18d24e3f535c9061d2e111d63fe6d8a27710bb34a17b326e605ff478be in / 
# Tue, 15 Jun 2021 22:57:41 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 02:07:10 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 26 Jun 2021 02:07:11 GMT
ENV HAPROXY_VERSION=1.7.14
# Sat, 26 Jun 2021 02:07:11 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Sat, 26 Jun 2021 02:07:11 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Sat, 26 Jun 2021 02:07:22 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		CFLAGS+="-Wno-address-of-packed-member" 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Sat, 26 Jun 2021 02:07:22 GMT
STOPSIGNAL SIGUSR1
# Sat, 26 Jun 2021 02:07:22 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Sat, 26 Jun 2021 02:07:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 26 Jun 2021 02:07:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 26 Jun 2021 02:07:25 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:b452d2916bdfd021add56f1eda6bdea35400671ef07b38316ef82fce92a88fee`  
		Last Modified: Wed, 14 Apr 2021 18:50:38 GMT  
		Size: 2.6 MB (2605253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a05b743ec9c1837f79c05c9452399bfadd3685ca356e39a4ac0174ec2665746`  
		Last Modified: Sat, 26 Jun 2021 02:10:27 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05bd299854cacd425e8755710904f3d353783e60ec749be773219c41d2e757b`  
		Last Modified: Sat, 26 Jun 2021 02:10:28 GMT  
		Size: 719.5 KB (719514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dff269165ac7f44366828c20581f0b035832210ce9159ec3c8a598e82afbdcf`  
		Last Modified: Sat, 26 Jun 2021 02:10:27 GMT  
		Size: 471.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62ddda44eae920d7f56d9e92d7557d2370026c4490bc16f6fe25e5df292656bc`  
		Last Modified: Sat, 26 Jun 2021 02:10:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:730742ef2cc680d0e454c5cfbd1faccca1d6e284468edc849b6b4f0482b19fb1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3087785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dec4cce6aaff89d1dbd9d98f0347ca66ed949280cf15ee68ddeb220ab6fb0fd2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:24 GMT
ADD file:d844cc7b5e00fb62be39d903a2fb4a08f700e75112c8eef1f31101e846ed010d in / 
# Tue, 15 Jun 2021 23:15:25 GMT
CMD ["/bin/sh"]
# Wed, 23 Jun 2021 05:33:03 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 23 Jun 2021 05:33:03 GMT
ENV HAPROXY_VERSION=1.7.14
# Wed, 23 Jun 2021 05:33:04 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Wed, 23 Jun 2021 05:33:04 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Wed, 23 Jun 2021 05:33:13 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		CFLAGS+="-Wno-address-of-packed-member" 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 23 Jun 2021 05:33:14 GMT
STOPSIGNAL SIGUSR1
# Wed, 23 Jun 2021 05:33:14 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Wed, 23 Jun 2021 05:33:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 23 Jun 2021 05:33:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 05:33:17 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:420c7481a3a76d5d12df768d2745ddbe40357df0af780c756a5a7d1f2a43d288`  
		Last Modified: Wed, 14 Apr 2021 18:58:46 GMT  
		Size: 2.4 MB (2409178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219b731e720358ea220ab0b84f59dc8e955bb18ba7c4eb089513b4783634b986`  
		Last Modified: Wed, 23 Jun 2021 05:39:33 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7936d9d658902da2de485e2a3fc5f5f05752af2cae009319dd67972a2b540ae0`  
		Last Modified: Wed, 23 Jun 2021 05:39:34 GMT  
		Size: 676.8 KB (676828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db1af767e65d361f3fd7fe106f74be83f294b60e16b787ced30269303f532b2f`  
		Last Modified: Wed, 23 Jun 2021 05:39:34 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ba8f0c2f3d14fd082ba95123c20fb368092ca171e14a376dbcf9df1eca7b5f`  
		Last Modified: Wed, 23 Jun 2021 05:39:34 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:3b4ac8f17466e2cf4a7004feafd5b7cee86b6e30087536f50a9b12d55be267f7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3433872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74f64a229633dc7acec39aef12cd9f9c41584d983324089e445db79138c64072`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:09 GMT
ADD file:3db1e10ac5ebf1cb34939eff736f1384f7d3b17355758cec361489fa7a7e19ca in / 
# Tue, 15 Jun 2021 21:45:09 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 00:43:10 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 00:43:11 GMT
ENV HAPROXY_VERSION=1.7.14
# Wed, 16 Jun 2021 00:43:11 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Wed, 16 Jun 2021 00:43:11 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Wed, 16 Jun 2021 00:43:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		CFLAGS+="-Wno-address-of-packed-member" 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 16 Jun 2021 00:43:21 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 00:43:21 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Wed, 16 Jun 2021 00:43:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 16 Jun 2021 00:43:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 00:43:22 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:d2f70382dc9a1658ea3491d7ab4439c22087e426c00e3eb7daf825b83be4ba9c`  
		Last Modified: Wed, 14 Apr 2021 18:43:55 GMT  
		Size: 2.7 MB (2710694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbb4bfb14121f961d3230a88ceb1a660109674eb24f1088819024b4bd0f8cc7f`  
		Last Modified: Wed, 16 Jun 2021 00:47:43 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef801df0b3ae859e0088c74f1a65addffad28b7c01a66c68d847d5d61204a19d`  
		Last Modified: Wed, 16 Jun 2021 00:47:43 GMT  
		Size: 721.4 KB (721396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f68775e45e48621557a43d77a6338d9bb9d0d51b9c6615395c680db228871a5c`  
		Last Modified: Wed, 16 Jun 2021 00:47:43 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:387532a80388b0ddbb57e419c705ff30e5864b36174a19124199c509b2d702db`  
		Last Modified: Wed, 16 Jun 2021 00:47:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7-alpine` - linux; 386

```console
$ docker pull haproxy@sha256:7dc566502e4e5dbea0dad303fdc2db644d953f649231265c88f7cbdfa60917d2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3554460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:690a2df6ec30f31b2a79bdb3b11ff3c1c9e023e4aa2686f5a23e75dc0768be2d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:36 GMT
ADD file:0a694887033953f24197dedcb1098d28a4b6e539b29386f53d82262107e208fb in / 
# Wed, 14 Apr 2021 18:38:36 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 01:58:28 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 15 Apr 2021 01:58:28 GMT
ENV HAPROXY_VERSION=1.7.14
# Thu, 15 Apr 2021 01:58:28 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Thu, 15 Apr 2021 01:58:29 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Thu, 15 Apr 2021 01:58:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		CFLAGS+="-Wno-address-of-packed-member" 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 15 Apr 2021 01:58:48 GMT
STOPSIGNAL SIGUSR1
# Thu, 15 Apr 2021 01:58:49 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Thu, 15 Apr 2021 01:58:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 15 Apr 2021 01:58:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Apr 2021 01:58:51 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:7aa04a8f7710c18952348aa54b4346438ad013c87b6f7d476eb21ad756359bc3`  
		Last Modified: Wed, 14 Apr 2021 18:39:43 GMT  
		Size: 2.8 MB (2795795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db648b1d7e93e227e16c4834283e47159a9936ec09ac5b9780d187cb637ad929`  
		Last Modified: Thu, 15 Apr 2021 02:02:01 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6787122459115456ff00e91ee6135f1f51626400da66666caa0d4cb3eb27f2f4`  
		Last Modified: Thu, 15 Apr 2021 02:02:02 GMT  
		Size: 756.9 KB (756887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcb198f7789a97df234ecbc39c81d894b8dfa1d442612d05a674847be086f20`  
		Last Modified: Thu, 15 Apr 2021 02:02:01 GMT  
		Size: 471.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bdc70581f273a2514b63c4f025e6c0c6c47a03f53e17515e7c9c87ab1ba177c`  
		Last Modified: Thu, 15 Apr 2021 02:02:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7-alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:459d63194d7b01ddcb195de78eb793892ab562781fec05eecee270b8f03276cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3573881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5e6ee03859c7016b8a01fd51a213bc309e4b2d60a69a08718d6b997af34fc46`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:31:22 GMT
ADD file:f8b081207f6d35f8ebd06aa471e350644151d183801f678def586d8f37e81366 in / 
# Wed, 14 Apr 2021 19:31:29 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 13:41:41 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 26 Jun 2021 13:41:47 GMT
ENV HAPROXY_VERSION=1.7.14
# Sat, 26 Jun 2021 13:41:58 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Sat, 26 Jun 2021 13:42:04 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Sat, 26 Jun 2021 13:42:24 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		CFLAGS+="-Wno-address-of-packed-member" 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Sat, 26 Jun 2021 13:42:27 GMT
STOPSIGNAL SIGUSR1
# Sat, 26 Jun 2021 13:42:29 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Sat, 26 Jun 2021 13:42:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 26 Jun 2021 13:42:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 26 Jun 2021 13:42:50 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:45707b9629c4ab8c6046680737229218fe844f38d08e5458b24605e1dbfd2709`  
		Last Modified: Wed, 14 Apr 2021 19:32:50 GMT  
		Size: 2.8 MB (2806750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5771c4fe7d869db103cc77efdc165ce9265d1ee4bc36d70c05ac4e3004ca0267`  
		Last Modified: Sat, 26 Jun 2021 13:45:44 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d56e2659d9cda5347edd6ccb43cccf9c9ae144b43809eab9bbea6819eaea9958`  
		Last Modified: Sat, 26 Jun 2021 13:45:44 GMT  
		Size: 765.3 KB (765348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9bd0e264bbb8971cc49f45b4e8ff68fb85a7bfacba78333197b0791e4f6b45d`  
		Last Modified: Sat, 26 Jun 2021 13:45:44 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdd4596344ad24fd4cf8972b71852429f90aedb5388f081702058cf3d14d265f`  
		Last Modified: Sat, 26 Jun 2021 13:45:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7-alpine` - linux; s390x

```console
$ docker pull haproxy@sha256:6b2504fbe06664541dd59d3b8809930cbcd6585dfdf3b637a8fc5ba0783a7993
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 MB (3346074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98c431c126e8d54885589edcf0d5221d922acbad33a29eae7c53617e537fd890`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:42 GMT
ADD file:c73a5ff435939cdc9d621ee9dc2aa5a54a5f5e0241caae8dc948c03c423d9fef in / 
# Wed, 14 Apr 2021 18:41:42 GMT
CMD ["/bin/sh"]
# Sun, 27 Jun 2021 12:29:55 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sun, 27 Jun 2021 12:29:55 GMT
ENV HAPROXY_VERSION=1.7.14
# Sun, 27 Jun 2021 12:29:55 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Sun, 27 Jun 2021 12:29:56 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Sun, 27 Jun 2021 12:30:06 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		CFLAGS+="-Wno-address-of-packed-member" 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Sun, 27 Jun 2021 12:30:07 GMT
STOPSIGNAL SIGUSR1
# Sun, 27 Jun 2021 12:30:07 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Sun, 27 Jun 2021 12:30:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sun, 27 Jun 2021 12:30:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 27 Jun 2021 12:30:09 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:27efec644c4207cbc4d1400f84f3402937aab5ce72489976148896e42a219820`  
		Last Modified: Wed, 14 Apr 2021 18:42:24 GMT  
		Size: 2.6 MB (2568428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea6c7bde2ce3e4d74b134428300d84e9f2ded4d30d9ddee89b700aa24fbe5607`  
		Last Modified: Sun, 27 Jun 2021 12:32:10 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c1177990fb0b3d7598ea9469e3e3ee69da1e158fac0f1b62d83ee23eae7a384`  
		Last Modified: Sun, 27 Jun 2021 12:32:10 GMT  
		Size: 775.9 KB (775868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed496a9835e310f3e327110254c5c3904c24bdbb8aa16df6e9ea257aef5d77e8`  
		Last Modified: Sun, 27 Jun 2021 12:32:10 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e94ca8a219fa47fbf152d8ba693c278a9cfa3d12f636283f1196b321d878d8`  
		Last Modified: Sun, 27 Jun 2021 12:32:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:1.7.14`

```console
$ docker pull haproxy@sha256:4c8908c0072a73ef6f5fe77aa0f7ea511cefdd50d8509ff0b43ba13f3f104066
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

### `haproxy:1.7.14` - linux; amd64

```console
$ docker pull haproxy@sha256:3d461dbce17a816277f813d59fdcad592d9b5c8188fbca83908b1e3db59f10d9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.5 MB (32541296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9be1737d9bbe86e16c10fcb2f8eb938d2c06640bc27138fd5ad117f811bac40b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 06:19:17 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 23 Jun 2021 06:27:30 GMT
ENV HAPROXY_VERSION=1.7.14
# Wed, 23 Jun 2021 06:27:30 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Wed, 23 Jun 2021 06:27:30 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Wed, 23 Jun 2021 06:28:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 23 Jun 2021 06:28:13 GMT
STOPSIGNAL SIGUSR1
# Wed, 23 Jun 2021 06:28:13 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Wed, 23 Jun 2021 06:28:14 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 23 Jun 2021 06:28:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 06:28:15 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91332cb81883405a321c1a2d2144bdd0aef8d1c69f90fdf0cf219982161b6e6e`  
		Last Modified: Wed, 23 Jun 2021 06:29:07 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:665e7a14a17f6fe1b65bc8010c568864f830e8a937c5707f6e68c2724a2f1415`  
		Last Modified: Wed, 23 Jun 2021 06:30:37 GMT  
		Size: 5.4 MB (5393475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dccd5cee97007600fc7a9cad5980265f2cead92d390911c5f2aa5e8879a064bb`  
		Last Modified: Wed, 23 Jun 2021 06:30:36 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5688c2df927a2c9a7dbe90061cbd2d45c426d7af4a2f47c03eb9be039e223728`  
		Last Modified: Wed, 23 Jun 2021 06:30:36 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7.14` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:eb40db1ad848dbcc5322aa69af01d4789b1246328750535ca3cf348c84b7c431
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.9 MB (29901157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e146711fa968989fe60f3dd8be14de2800be27104e98a634f3583255612c848`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 22 Jun 2021 23:50:09 GMT
ADD file:78d4ced31112d85490c684f350aceeebfc72a804262c7ad3e033257e3894f5c4 in / 
# Tue, 22 Jun 2021 23:50:11 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:15:11 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 23 Jun 2021 05:21:52 GMT
ENV HAPROXY_VERSION=1.7.14
# Wed, 23 Jun 2021 05:21:53 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Wed, 23 Jun 2021 05:21:53 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Wed, 23 Jun 2021 05:22:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 23 Jun 2021 05:22:42 GMT
STOPSIGNAL SIGUSR1
# Wed, 23 Jun 2021 05:22:42 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Wed, 23 Jun 2021 05:22:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 23 Jun 2021 05:22:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 05:22:44 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:532d6df30af5174ac6e1b379c32b8f464d44651ac060376a560c4a76a87704a7`  
		Last Modified: Wed, 23 Jun 2021 00:01:46 GMT  
		Size: 24.9 MB (24878945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48649e3d7de4cd80d3a9a34c725a2935be904ff90e99ea6c8e4bb6e1e7a4eeb7`  
		Last Modified: Wed, 23 Jun 2021 05:24:11 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:170f6401c23b3b6db35408132d6b6487f4b6e7ccdc9b6a384426636adc787dac`  
		Last Modified: Wed, 23 Jun 2021 05:26:11 GMT  
		Size: 5.0 MB (5020242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba60f03140a88c98fd76bbf209b30e2c635f793d650ef0a5fabf88df6fa84358`  
		Last Modified: Wed, 23 Jun 2021 05:26:07 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed57b998443ddcd697a62040539bf6500f70cde810b550776a396497e19abbc4`  
		Last Modified: Wed, 23 Jun 2021 05:26:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7.14` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:5bf1be3afe675072cef4473312e51c4ed9b3dd1efee0090f9da55a02234fbfd7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.6 MB (27640225 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8aae63f0809a60888ba04d9fa70fdc6d5f0224aaaf6941fd7a422cb9130b911`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:31 GMT
ADD file:8d200a3bbe985ff355343675c5555852f27550a9e367969df6bc98034efb8fd4 in / 
# Wed, 23 Jun 2021 00:20:31 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:21:41 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 23 Jun 2021 05:32:03 GMT
ENV HAPROXY_VERSION=1.7.14
# Wed, 23 Jun 2021 05:32:04 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Wed, 23 Jun 2021 05:32:04 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Wed, 23 Jun 2021 05:32:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 23 Jun 2021 05:32:49 GMT
STOPSIGNAL SIGUSR1
# Wed, 23 Jun 2021 05:32:49 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Wed, 23 Jun 2021 05:32:51 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 23 Jun 2021 05:32:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 05:32:52 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:8452be1adf00f91570fe21a8e61aaf4c12e014daf67d7de65d984f4e8ecca2f1`  
		Last Modified: Wed, 23 Jun 2021 00:31:49 GMT  
		Size: 22.7 MB (22746055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed1c9c92d0076fd4bf40503e3f47102509a5b99d182f4dd9e81e64d0a7e0b8a`  
		Last Modified: Wed, 23 Jun 2021 05:35:48 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae4ddb74c7a1350f6335ed180208075ce88a1db859fc405d7ddda0dc47b98b94`  
		Last Modified: Wed, 23 Jun 2021 05:39:21 GMT  
		Size: 4.9 MB (4892197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f289bf8c6c4e11830a6c2920e1a656b5c46f9b454a21d57c1129f9aa35260df8`  
		Last Modified: Wed, 23 Jun 2021 05:39:18 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6062074497a0994f1f648d5799560f3e732d12502b938eab4525d2b3b22ec9a`  
		Last Modified: Wed, 23 Jun 2021 05:39:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7.14` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:9fcc85c1fd689edcc3a6f03204170145bc9757478534a5d5554d613d2e17060e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31197976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d018078b9507ee49d00dec4231d3217d31540e91104da7161eebf1dfa60865b6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:40 GMT
ADD file:beee00b59da720f68e12e2ba2a8134207c80c777ddb4ceb03c71e3e4c3f51c93 in / 
# Tue, 22 Jun 2021 23:49:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 03:19:31 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 23 Jun 2021 03:24:30 GMT
ENV HAPROXY_VERSION=1.7.14
# Wed, 23 Jun 2021 03:24:30 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Wed, 23 Jun 2021 03:24:31 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Wed, 23 Jun 2021 03:24:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 23 Jun 2021 03:24:56 GMT
STOPSIGNAL SIGUSR1
# Wed, 23 Jun 2021 03:24:56 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Wed, 23 Jun 2021 03:24:57 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 23 Jun 2021 03:24:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 03:24:57 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:448f6bf000e31217a7c202c659b03b7f8ac8d3ae6b03ef7a2f8339be2f00ff4a`  
		Last Modified: Tue, 22 Jun 2021 23:55:25 GMT  
		Size: 25.9 MB (25914993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b05ad81dc8a7d67656235988f0e5fb72c374c7d8df44c105b91d712e06c4ac`  
		Last Modified: Wed, 23 Jun 2021 03:26:16 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edc87e3339ee885225543831e8b2dfda8cba3610676e3993a8f31b171486cbd1`  
		Last Modified: Wed, 23 Jun 2021 03:27:52 GMT  
		Size: 5.3 MB (5281010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0335c8e3127a6be5a9f7c49aef80a03c093fd5412a108693b1434c203d69162`  
		Last Modified: Wed, 23 Jun 2021 03:27:51 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41c07a18fd101002b18aaac65e6f589572bfd53f3de33de84f208568b9e23eea`  
		Last Modified: Wed, 23 Jun 2021 03:27:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7.14` - linux; 386

```console
$ docker pull haproxy@sha256:7385f826a4450550dadc352efa8c933a2b50bdb03eb28997452b0fc310bfc70e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.1 MB (33123397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6daa1c38e094d95fd74d0009b946bca8dfb85a4376792393de8731069959803`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 22 Jun 2021 23:39:35 GMT
ADD file:48f656ac6733911048b3de850490438d0233b3badc11861fca62062d4edfaf40 in / 
# Tue, 22 Jun 2021 23:39:35 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:23:13 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 23 Jun 2021 00:30:01 GMT
ENV HAPROXY_VERSION=1.7.14
# Wed, 23 Jun 2021 00:30:01 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Wed, 23 Jun 2021 00:30:01 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Wed, 23 Jun 2021 00:30:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 23 Jun 2021 00:30:34 GMT
STOPSIGNAL SIGUSR1
# Wed, 23 Jun 2021 00:30:35 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Wed, 23 Jun 2021 00:30:35 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 23 Jun 2021 00:30:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 00:30:36 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:33af2dcb865e65d53cdeb843b67a0ef62151fa32df292293e7c6b0eb728ac5ac`  
		Last Modified: Tue, 22 Jun 2021 23:46:23 GMT  
		Size: 27.8 MB (27797411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a6e4d42b23996eb7d8a1baa85ee19828c2667fd4a2dca6eb1040b266680e9f`  
		Last Modified: Wed, 23 Jun 2021 00:32:00 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b27b997e8598f8116677e406f452f79707677c4b1df6495585abbc1f29238ad`  
		Last Modified: Wed, 23 Jun 2021 00:33:38 GMT  
		Size: 5.3 MB (5324016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f072c4b4c9ec2e76fb216777fac9153f6dcf22a5685ebdf52bbffdd97acfc05b`  
		Last Modified: Wed, 23 Jun 2021 00:33:36 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eee6b076bba5aada707e31ff5f8d84e272f47e3a9370c00532d0ab727eb5383`  
		Last Modified: Wed, 23 Jun 2021 00:33:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7.14` - linux; mips64le

```console
$ docker pull haproxy@sha256:37fbe8b99980c76d6738dd65c4258ec5b78ba6423298e3405ea3e63e6771773f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.8 MB (30842533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3abb2ea5d80b752c7bf7e8c17369ab97a8361783739a6a0ee92602fd9b633bdf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 22 Jul 2021 00:09:45 GMT
ADD file:1f77b9001c4977ba733be674fc5eb4b85130f1dea8a7b39d545b70f9c107695f in / 
# Thu, 22 Jul 2021 00:09:46 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:07:49 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 22 Jul 2021 01:22:40 GMT
ENV HAPROXY_VERSION=1.7.14
# Thu, 22 Jul 2021 01:22:40 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Thu, 22 Jul 2021 01:22:41 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Thu, 22 Jul 2021 01:24:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 22 Jul 2021 01:24:06 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 01:24:06 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Thu, 22 Jul 2021 01:24:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Jul 2021 01:24:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 01:24:09 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:99ee621d0b0485e9de65aa19604aa2453d19ea7fc86b22c5b77c1bab74e3cb42`  
		Last Modified: Thu, 22 Jul 2021 00:16:11 GMT  
		Size: 25.8 MB (25812771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f444627794f98947a9df95ec5d19b2a1cd6c151ed438982b1dc0b89f5eaf19e`  
		Last Modified: Thu, 22 Jul 2021 01:24:39 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad8199dbb9f3f9e98bbd8dea7146b6ba797f846c74e703dea2dfa9e753c72da3`  
		Last Modified: Thu, 22 Jul 2021 01:26:25 GMT  
		Size: 5.0 MB (5027791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4ffe21fcf7ac71e04543b553d963d67c0c0d26535369b460875de7f653247e`  
		Last Modified: Thu, 22 Jul 2021 01:26:21 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244dceab14585bfcb12416cb1018527be5ecfeae00575b4b183ff3cac009a55c`  
		Last Modified: Thu, 22 Jul 2021 01:26:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7.14` - linux; ppc64le

```console
$ docker pull haproxy@sha256:1abfbe399c3e8807e50431c134c8b97d0cf2eced31e8d532dcacd8cefccc8ab7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36266404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:719f475fb89a446baf503d2feb34d7b5814d2c8a6c5fd9561842e9a8e963316d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 22 Jul 2021 00:19:04 GMT
ADD file:3a6bd6ce3eff98b88a13de5d0f26cff0b026f876674204dbad6f84fafcf145b1 in / 
# Thu, 22 Jul 2021 00:19:13 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 02:52:46 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 22 Jul 2021 03:33:15 GMT
ENV HAPROXY_VERSION=1.7.14
# Thu, 22 Jul 2021 03:33:21 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Thu, 22 Jul 2021 03:33:25 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Thu, 22 Jul 2021 03:37:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 22 Jul 2021 03:37:47 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 03:37:51 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Thu, 22 Jul 2021 03:38:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Jul 2021 03:38:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 03:38:19 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:1130517d52da84a09f9465006bddab5e49afd398860890eab6274fd0bff32371`  
		Last Modified: Thu, 22 Jul 2021 00:27:49 GMT  
		Size: 30.6 MB (30553709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251bf3fe1d4bbe9c27e393cd8ddc550b56cec90eb916bf9bec24d657c9f6556f`  
		Last Modified: Thu, 22 Jul 2021 03:40:01 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a29f6d6804eb054d0c618384a92189f202e0cf1932e49b2a2582a675fa5b0ff2`  
		Last Modified: Thu, 22 Jul 2021 03:43:02 GMT  
		Size: 5.7 MB (5710724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0445214d7e223706b47751dd070f47e33c533caa0278329641fdc4db7390015d`  
		Last Modified: Thu, 22 Jul 2021 03:43:01 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f703a80a7b00ccb9b5604f68c2050f000ed0da1cad292175530b03014a713ff`  
		Last Modified: Thu, 22 Jul 2021 03:43:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7.14` - linux; s390x

```console
$ docker pull haproxy@sha256:7e952ce5ecc34758ff5e94aeca5a3831c9ddd602005fb1a19302b5bfbcdb1872
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.9 MB (30891864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5dc3a063fcda3f6020320a2d0abb1ea67604a8bfc767ae1bd3d4d3fa67ea762`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 22 Jul 2021 00:42:45 GMT
ADD file:1ab999eb6f80d8ce91ce3a173e23fd2710f2779117bba29037eaa82aadcbf6ed in / 
# Thu, 22 Jul 2021 00:42:48 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:30:19 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 22 Jul 2021 01:38:31 GMT
ENV HAPROXY_VERSION=1.7.14
# Thu, 22 Jul 2021 01:38:32 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Thu, 22 Jul 2021 01:38:32 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Thu, 22 Jul 2021 01:38:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 22 Jul 2021 01:38:58 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 01:38:58 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Thu, 22 Jul 2021 01:38:59 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Jul 2021 01:39:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 01:39:00 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:7a50fdd85ff244c1465e71c51354d055e3df0b90ff5faad28cc22d9ecde9daf3`  
		Last Modified: Thu, 22 Jul 2021 00:48:13 GMT  
		Size: 25.8 MB (25760761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05fb34d1ed21b67502665114a7ae60445472fc7bafa620bbf6c79b7df85a01d4`  
		Last Modified: Thu, 22 Jul 2021 01:39:54 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d133f88f7bf0d9f7fd35aeb02cf4e3d54fa2264868d3553fed415864b067e204`  
		Last Modified: Thu, 22 Jul 2021 01:40:57 GMT  
		Size: 5.1 MB (5129131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a088aeea9fbccb475252ae3098ca841aaa5f0cc910d40d58cd65bb04654d54f1`  
		Last Modified: Thu, 22 Jul 2021 01:40:56 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be65e63201a559c73a322bea91f4ef1b8bc5c4e54994efe33d142261911d9993`  
		Last Modified: Thu, 22 Jul 2021 01:40:56 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:1.7.14-alpine`

```console
$ docker pull haproxy@sha256:f8946d8c90ff0e2f7c56e1f8d5afe87356b7864db3713a4558c987b5b264e8ce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `haproxy:1.7.14-alpine` - linux; amd64

```console
$ docker pull haproxy@sha256:585430cbbec0b6df064587170ed3ac0104e263290ffc6f6d63dfeb3d263437f7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.5 MB (3547528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f57f9af8fae5238962a097fdf78d150e3d0cc1160c1495149e0011cdd22cf77`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:42:45 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 21:42:45 GMT
ENV HAPROXY_VERSION=1.7.14
# Wed, 14 Apr 2021 21:42:45 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Wed, 14 Apr 2021 21:42:46 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Wed, 14 Apr 2021 21:42:57 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		CFLAGS+="-Wno-address-of-packed-member" 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 21:42:57 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 21:42:57 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Wed, 14 Apr 2021 21:42:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 21:42:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 21:42:58 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e79a8d3da5b7b8e6a180e6fa428bf4a36b8f8bc0e3675927aeb0860a92747561`  
		Last Modified: Wed, 14 Apr 2021 21:44:42 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ba53b9604ae0a19fc162eca377f3de4c0deb844929aa614806d7566b55d42e`  
		Last Modified: Wed, 14 Apr 2021 21:44:43 GMT  
		Size: 745.2 KB (745185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f8509370c0a2bc5abc5c0de684ae960d3917ef4fae3de452c52e6a83619de90`  
		Last Modified: Wed, 14 Apr 2021 21:44:42 GMT  
		Size: 471.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0bf7494a1e4cf18a66f609c0be15d90d5ec36c6eeb05c116acbd0f00ae4cc08`  
		Last Modified: Wed, 14 Apr 2021 21:44:42 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7.14-alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:91f9984cff0f997f604f6ce233ded4cfa3c3f29a81bb40820a2575e3943cb5d4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 MB (3326550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1be9c767dd4ef5c7d0d34901388b0853c249afbdf3b7ba7a4ae92e5bbc49f1dd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:41 GMT
ADD file:82fa6a18d24e3f535c9061d2e111d63fe6d8a27710bb34a17b326e605ff478be in / 
# Tue, 15 Jun 2021 22:57:41 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 02:07:10 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 26 Jun 2021 02:07:11 GMT
ENV HAPROXY_VERSION=1.7.14
# Sat, 26 Jun 2021 02:07:11 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Sat, 26 Jun 2021 02:07:11 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Sat, 26 Jun 2021 02:07:22 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		CFLAGS+="-Wno-address-of-packed-member" 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Sat, 26 Jun 2021 02:07:22 GMT
STOPSIGNAL SIGUSR1
# Sat, 26 Jun 2021 02:07:22 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Sat, 26 Jun 2021 02:07:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 26 Jun 2021 02:07:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 26 Jun 2021 02:07:25 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:b452d2916bdfd021add56f1eda6bdea35400671ef07b38316ef82fce92a88fee`  
		Last Modified: Wed, 14 Apr 2021 18:50:38 GMT  
		Size: 2.6 MB (2605253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a05b743ec9c1837f79c05c9452399bfadd3685ca356e39a4ac0174ec2665746`  
		Last Modified: Sat, 26 Jun 2021 02:10:27 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05bd299854cacd425e8755710904f3d353783e60ec749be773219c41d2e757b`  
		Last Modified: Sat, 26 Jun 2021 02:10:28 GMT  
		Size: 719.5 KB (719514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dff269165ac7f44366828c20581f0b035832210ce9159ec3c8a598e82afbdcf`  
		Last Modified: Sat, 26 Jun 2021 02:10:27 GMT  
		Size: 471.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62ddda44eae920d7f56d9e92d7557d2370026c4490bc16f6fe25e5df292656bc`  
		Last Modified: Sat, 26 Jun 2021 02:10:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7.14-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:730742ef2cc680d0e454c5cfbd1faccca1d6e284468edc849b6b4f0482b19fb1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3087785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dec4cce6aaff89d1dbd9d98f0347ca66ed949280cf15ee68ddeb220ab6fb0fd2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:24 GMT
ADD file:d844cc7b5e00fb62be39d903a2fb4a08f700e75112c8eef1f31101e846ed010d in / 
# Tue, 15 Jun 2021 23:15:25 GMT
CMD ["/bin/sh"]
# Wed, 23 Jun 2021 05:33:03 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 23 Jun 2021 05:33:03 GMT
ENV HAPROXY_VERSION=1.7.14
# Wed, 23 Jun 2021 05:33:04 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Wed, 23 Jun 2021 05:33:04 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Wed, 23 Jun 2021 05:33:13 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		CFLAGS+="-Wno-address-of-packed-member" 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 23 Jun 2021 05:33:14 GMT
STOPSIGNAL SIGUSR1
# Wed, 23 Jun 2021 05:33:14 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Wed, 23 Jun 2021 05:33:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 23 Jun 2021 05:33:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 05:33:17 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:420c7481a3a76d5d12df768d2745ddbe40357df0af780c756a5a7d1f2a43d288`  
		Last Modified: Wed, 14 Apr 2021 18:58:46 GMT  
		Size: 2.4 MB (2409178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:219b731e720358ea220ab0b84f59dc8e955bb18ba7c4eb089513b4783634b986`  
		Last Modified: Wed, 23 Jun 2021 05:39:33 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7936d9d658902da2de485e2a3fc5f5f05752af2cae009319dd67972a2b540ae0`  
		Last Modified: Wed, 23 Jun 2021 05:39:34 GMT  
		Size: 676.8 KB (676828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db1af767e65d361f3fd7fe106f74be83f294b60e16b787ced30269303f532b2f`  
		Last Modified: Wed, 23 Jun 2021 05:39:34 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ba8f0c2f3d14fd082ba95123c20fb368092ca171e14a376dbcf9df1eca7b5f`  
		Last Modified: Wed, 23 Jun 2021 05:39:34 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7.14-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:3b4ac8f17466e2cf4a7004feafd5b7cee86b6e30087536f50a9b12d55be267f7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3433872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74f64a229633dc7acec39aef12cd9f9c41584d983324089e445db79138c64072`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:09 GMT
ADD file:3db1e10ac5ebf1cb34939eff736f1384f7d3b17355758cec361489fa7a7e19ca in / 
# Tue, 15 Jun 2021 21:45:09 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 00:43:10 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 00:43:11 GMT
ENV HAPROXY_VERSION=1.7.14
# Wed, 16 Jun 2021 00:43:11 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Wed, 16 Jun 2021 00:43:11 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Wed, 16 Jun 2021 00:43:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		CFLAGS+="-Wno-address-of-packed-member" 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 16 Jun 2021 00:43:21 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 00:43:21 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Wed, 16 Jun 2021 00:43:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 16 Jun 2021 00:43:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 00:43:22 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:d2f70382dc9a1658ea3491d7ab4439c22087e426c00e3eb7daf825b83be4ba9c`  
		Last Modified: Wed, 14 Apr 2021 18:43:55 GMT  
		Size: 2.7 MB (2710694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbb4bfb14121f961d3230a88ceb1a660109674eb24f1088819024b4bd0f8cc7f`  
		Last Modified: Wed, 16 Jun 2021 00:47:43 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef801df0b3ae859e0088c74f1a65addffad28b7c01a66c68d847d5d61204a19d`  
		Last Modified: Wed, 16 Jun 2021 00:47:43 GMT  
		Size: 721.4 KB (721396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f68775e45e48621557a43d77a6338d9bb9d0d51b9c6615395c680db228871a5c`  
		Last Modified: Wed, 16 Jun 2021 00:47:43 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:387532a80388b0ddbb57e419c705ff30e5864b36174a19124199c509b2d702db`  
		Last Modified: Wed, 16 Jun 2021 00:47:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7.14-alpine` - linux; 386

```console
$ docker pull haproxy@sha256:7dc566502e4e5dbea0dad303fdc2db644d953f649231265c88f7cbdfa60917d2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3554460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:690a2df6ec30f31b2a79bdb3b11ff3c1c9e023e4aa2686f5a23e75dc0768be2d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:36 GMT
ADD file:0a694887033953f24197dedcb1098d28a4b6e539b29386f53d82262107e208fb in / 
# Wed, 14 Apr 2021 18:38:36 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 01:58:28 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 15 Apr 2021 01:58:28 GMT
ENV HAPROXY_VERSION=1.7.14
# Thu, 15 Apr 2021 01:58:28 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Thu, 15 Apr 2021 01:58:29 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Thu, 15 Apr 2021 01:58:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		CFLAGS+="-Wno-address-of-packed-member" 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 15 Apr 2021 01:58:48 GMT
STOPSIGNAL SIGUSR1
# Thu, 15 Apr 2021 01:58:49 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Thu, 15 Apr 2021 01:58:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 15 Apr 2021 01:58:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Apr 2021 01:58:51 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:7aa04a8f7710c18952348aa54b4346438ad013c87b6f7d476eb21ad756359bc3`  
		Last Modified: Wed, 14 Apr 2021 18:39:43 GMT  
		Size: 2.8 MB (2795795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db648b1d7e93e227e16c4834283e47159a9936ec09ac5b9780d187cb637ad929`  
		Last Modified: Thu, 15 Apr 2021 02:02:01 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6787122459115456ff00e91ee6135f1f51626400da66666caa0d4cb3eb27f2f4`  
		Last Modified: Thu, 15 Apr 2021 02:02:02 GMT  
		Size: 756.9 KB (756887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcb198f7789a97df234ecbc39c81d894b8dfa1d442612d05a674847be086f20`  
		Last Modified: Thu, 15 Apr 2021 02:02:01 GMT  
		Size: 471.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bdc70581f273a2514b63c4f025e6c0c6c47a03f53e17515e7c9c87ab1ba177c`  
		Last Modified: Thu, 15 Apr 2021 02:02:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7.14-alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:459d63194d7b01ddcb195de78eb793892ab562781fec05eecee270b8f03276cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3573881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5e6ee03859c7016b8a01fd51a213bc309e4b2d60a69a08718d6b997af34fc46`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:31:22 GMT
ADD file:f8b081207f6d35f8ebd06aa471e350644151d183801f678def586d8f37e81366 in / 
# Wed, 14 Apr 2021 19:31:29 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 13:41:41 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 26 Jun 2021 13:41:47 GMT
ENV HAPROXY_VERSION=1.7.14
# Sat, 26 Jun 2021 13:41:58 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Sat, 26 Jun 2021 13:42:04 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Sat, 26 Jun 2021 13:42:24 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		CFLAGS+="-Wno-address-of-packed-member" 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Sat, 26 Jun 2021 13:42:27 GMT
STOPSIGNAL SIGUSR1
# Sat, 26 Jun 2021 13:42:29 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Sat, 26 Jun 2021 13:42:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 26 Jun 2021 13:42:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 26 Jun 2021 13:42:50 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:45707b9629c4ab8c6046680737229218fe844f38d08e5458b24605e1dbfd2709`  
		Last Modified: Wed, 14 Apr 2021 19:32:50 GMT  
		Size: 2.8 MB (2806750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5771c4fe7d869db103cc77efdc165ce9265d1ee4bc36d70c05ac4e3004ca0267`  
		Last Modified: Sat, 26 Jun 2021 13:45:44 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d56e2659d9cda5347edd6ccb43cccf9c9ae144b43809eab9bbea6819eaea9958`  
		Last Modified: Sat, 26 Jun 2021 13:45:44 GMT  
		Size: 765.3 KB (765348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9bd0e264bbb8971cc49f45b4e8ff68fb85a7bfacba78333197b0791e4f6b45d`  
		Last Modified: Sat, 26 Jun 2021 13:45:44 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdd4596344ad24fd4cf8972b71852429f90aedb5388f081702058cf3d14d265f`  
		Last Modified: Sat, 26 Jun 2021 13:45:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7.14-alpine` - linux; s390x

```console
$ docker pull haproxy@sha256:6b2504fbe06664541dd59d3b8809930cbcd6585dfdf3b637a8fc5ba0783a7993
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 MB (3346074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98c431c126e8d54885589edcf0d5221d922acbad33a29eae7c53617e537fd890`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:42 GMT
ADD file:c73a5ff435939cdc9d621ee9dc2aa5a54a5f5e0241caae8dc948c03c423d9fef in / 
# Wed, 14 Apr 2021 18:41:42 GMT
CMD ["/bin/sh"]
# Sun, 27 Jun 2021 12:29:55 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sun, 27 Jun 2021 12:29:55 GMT
ENV HAPROXY_VERSION=1.7.14
# Sun, 27 Jun 2021 12:29:55 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Sun, 27 Jun 2021 12:29:56 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Sun, 27 Jun 2021 12:30:06 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		CFLAGS+="-Wno-address-of-packed-member" 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Sun, 27 Jun 2021 12:30:07 GMT
STOPSIGNAL SIGUSR1
# Sun, 27 Jun 2021 12:30:07 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Sun, 27 Jun 2021 12:30:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sun, 27 Jun 2021 12:30:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 27 Jun 2021 12:30:09 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:27efec644c4207cbc4d1400f84f3402937aab5ce72489976148896e42a219820`  
		Last Modified: Wed, 14 Apr 2021 18:42:24 GMT  
		Size: 2.6 MB (2568428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea6c7bde2ce3e4d74b134428300d84e9f2ded4d30d9ddee89b700aa24fbe5607`  
		Last Modified: Sun, 27 Jun 2021 12:32:10 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c1177990fb0b3d7598ea9469e3e3ee69da1e158fac0f1b62d83ee23eae7a384`  
		Last Modified: Sun, 27 Jun 2021 12:32:10 GMT  
		Size: 775.9 KB (775868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed496a9835e310f3e327110254c5c3904c24bdbb8aa16df6e9ea257aef5d77e8`  
		Last Modified: Sun, 27 Jun 2021 12:32:10 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e94ca8a219fa47fbf152d8ba693c278a9cfa3d12f636283f1196b321d878d8`  
		Last Modified: Sun, 27 Jun 2021 12:32:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:1.8`

```console
$ docker pull haproxy@sha256:39f817cdc6d4dd7b236b2ab1a0e1e8094d735f7ba7cce22afcb062d84a6efb5a
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

### `haproxy:1.8` - linux; amd64

```console
$ docker pull haproxy@sha256:3722851ed931bf31d94450e32d30ce53995833176fb723e6fc6bd05dbeee1833
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33800154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eff256be590bcd7aa144e0a8bd6302e42fa039ad3a0315a5bc068e59ab3d3b3e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 06:19:17 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 23 Jun 2021 06:26:15 GMT
ENV HAPROXY_VERSION=1.8.30
# Wed, 23 Jun 2021 06:26:16 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Wed, 23 Jun 2021 06:26:16 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Wed, 23 Jun 2021 06:27:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 23 Jun 2021 06:27:15 GMT
STOPSIGNAL SIGUSR1
# Wed, 23 Jun 2021 06:27:15 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 23 Jun 2021 06:27:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 23 Jun 2021 06:27:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 06:27:17 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91332cb81883405a321c1a2d2144bdd0aef8d1c69f90fdf0cf219982161b6e6e`  
		Last Modified: Wed, 23 Jun 2021 06:29:07 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1834e88021136e77b613445f458946e4f7a4b9b825905af333615d8b80d4937`  
		Last Modified: Wed, 23 Jun 2021 06:30:24 GMT  
		Size: 6.7 MB (6652353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be5a8071776446234e68c4cbc6bf0971a16ffb4c9645f73d8a86d8aaf4ee4867`  
		Last Modified: Wed, 23 Jun 2021 06:30:23 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e8d7be053cf42dc731cb9550682dfef65bc311ee24670e94de26013d2b7ba02`  
		Last Modified: Wed, 23 Jun 2021 06:30:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:9503a1c3eb6628c761fb14ac3eeedbef80baa48fcecec96384f2f4a3cf172c86
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.1 MB (31112125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c3e36feaeb4a286370c17155be20e8b7ece4204fcc1d9a5c5319d6997586b5b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 22 Jun 2021 23:50:09 GMT
ADD file:78d4ced31112d85490c684f350aceeebfc72a804262c7ad3e033257e3894f5c4 in / 
# Tue, 22 Jun 2021 23:50:11 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:15:11 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 23 Jun 2021 05:20:46 GMT
ENV HAPROXY_VERSION=1.8.30
# Wed, 23 Jun 2021 05:20:46 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Wed, 23 Jun 2021 05:20:47 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Wed, 23 Jun 2021 05:21:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 23 Jun 2021 05:21:37 GMT
STOPSIGNAL SIGUSR1
# Wed, 23 Jun 2021 05:21:37 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 23 Jun 2021 05:21:39 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 23 Jun 2021 05:21:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 05:21:39 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:532d6df30af5174ac6e1b379c32b8f464d44651ac060376a560c4a76a87704a7`  
		Last Modified: Wed, 23 Jun 2021 00:01:46 GMT  
		Size: 24.9 MB (24878945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48649e3d7de4cd80d3a9a34c725a2935be904ff90e99ea6c8e4bb6e1e7a4eeb7`  
		Last Modified: Wed, 23 Jun 2021 05:24:11 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc3dd6789232c458605cbaaa7c798549960214f7a917be6d09b50a160a56ef0c`  
		Last Modified: Wed, 23 Jun 2021 05:25:56 GMT  
		Size: 6.2 MB (6231232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e605d3d155543a0840b26414df9da3eedc76abc199087ab5c493c064202257cf`  
		Last Modified: Wed, 23 Jun 2021 05:25:52 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe96a800a1c1b4beb8174e7b375f121ab502b1c5b04335e9f408391061ef65d`  
		Last Modified: Wed, 23 Jun 2021 05:25:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:d6aad0ea1b82d238046fb58649e31f79356de73ef9e0a1b993580ae2209da0f3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.8 MB (28818881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b466de86d10c7ae44bbdbf238a5cca50d3c8accefe36c48dcc13c91e3e4666e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:31 GMT
ADD file:8d200a3bbe985ff355343675c5555852f27550a9e367969df6bc98034efb8fd4 in / 
# Wed, 23 Jun 2021 00:20:31 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:21:41 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 23 Jun 2021 05:30:20 GMT
ENV HAPROXY_VERSION=1.8.30
# Wed, 23 Jun 2021 05:30:21 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Wed, 23 Jun 2021 05:30:21 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Wed, 23 Jun 2021 05:31:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 23 Jun 2021 05:31:08 GMT
STOPSIGNAL SIGUSR1
# Wed, 23 Jun 2021 05:31:08 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 23 Jun 2021 05:31:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 23 Jun 2021 05:31:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 05:31:10 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:8452be1adf00f91570fe21a8e61aaf4c12e014daf67d7de65d984f4e8ecca2f1`  
		Last Modified: Wed, 23 Jun 2021 00:31:49 GMT  
		Size: 22.7 MB (22746055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed1c9c92d0076fd4bf40503e3f47102509a5b99d182f4dd9e81e64d0a7e0b8a`  
		Last Modified: Wed, 23 Jun 2021 05:35:48 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faefe1906560d2be5bc0d0ff2712dfbb3281753e9fc3c46bf536e932c8cb6b2c`  
		Last Modified: Wed, 23 Jun 2021 05:38:52 GMT  
		Size: 6.1 MB (6070877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa78b9a61872e76b9579ba405a854bd84c35304d7fb85b5f97a898c9b576c902`  
		Last Modified: Wed, 23 Jun 2021 05:38:49 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c24e2f44ba1bc9242d7c8bfec83f249d20cffc351a650807c6e5e6d958b40d11`  
		Last Modified: Wed, 23 Jun 2021 05:38:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:f8eca28dc001d9734c7c3ccec202b734f2f874b2a5314c163642cdcc08d11211
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.4 MB (32370707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ffe3d091b1855a41fc0e5b4dbf130cabc62733a55fd6ff06974a6145adb205c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:40 GMT
ADD file:beee00b59da720f68e12e2ba2a8134207c80c777ddb4ceb03c71e3e4c3f51c93 in / 
# Tue, 22 Jun 2021 23:49:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 03:19:31 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 23 Jun 2021 03:23:49 GMT
ENV HAPROXY_VERSION=1.8.30
# Wed, 23 Jun 2021 03:23:49 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Wed, 23 Jun 2021 03:23:49 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Wed, 23 Jun 2021 03:24:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 23 Jun 2021 03:24:18 GMT
STOPSIGNAL SIGUSR1
# Wed, 23 Jun 2021 03:24:18 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 23 Jun 2021 03:24:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 23 Jun 2021 03:24:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 03:24:19 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:448f6bf000e31217a7c202c659b03b7f8ac8d3ae6b03ef7a2f8339be2f00ff4a`  
		Last Modified: Tue, 22 Jun 2021 23:55:25 GMT  
		Size: 25.9 MB (25914993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b05ad81dc8a7d67656235988f0e5fb72c374c7d8df44c105b91d712e06c4ac`  
		Last Modified: Wed, 23 Jun 2021 03:26:16 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2c08bfd067c99cbb1d435d19d33818c3df5f623311eaecd221541938020c84f`  
		Last Modified: Wed, 23 Jun 2021 03:27:39 GMT  
		Size: 6.5 MB (6453765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c6c10b3a1bbe6240132054604cddbcca782aa44ffe70d2a9e491f7970be096`  
		Last Modified: Wed, 23 Jun 2021 03:27:37 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c24f8961860ba35f878ad8964ecb67f7aae9b185fe26729d278b583104dd7a`  
		Last Modified: Wed, 23 Jun 2021 03:27:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8` - linux; 386

```console
$ docker pull haproxy@sha256:e07d1474fb9df83b62a04484b9318e5fd98e18c8dc07e4eac23f786d84d5fe80
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.4 MB (34376202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db3e086afd7d3a71e10d8394214db534f5178240d835f5ccf933d5f33dd262c1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 22 Jun 2021 23:39:35 GMT
ADD file:48f656ac6733911048b3de850490438d0233b3badc11861fca62062d4edfaf40 in / 
# Tue, 22 Jun 2021 23:39:35 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:23:13 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 23 Jun 2021 00:29:05 GMT
ENV HAPROXY_VERSION=1.8.30
# Wed, 23 Jun 2021 00:29:05 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Wed, 23 Jun 2021 00:29:05 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Wed, 23 Jun 2021 00:29:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 23 Jun 2021 00:29:46 GMT
STOPSIGNAL SIGUSR1
# Wed, 23 Jun 2021 00:29:46 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 23 Jun 2021 00:29:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 23 Jun 2021 00:29:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 00:29:48 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:33af2dcb865e65d53cdeb843b67a0ef62151fa32df292293e7c6b0eb728ac5ac`  
		Last Modified: Tue, 22 Jun 2021 23:46:23 GMT  
		Size: 27.8 MB (27797411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a6e4d42b23996eb7d8a1baa85ee19828c2667fd4a2dca6eb1040b266680e9f`  
		Last Modified: Wed, 23 Jun 2021 00:32:00 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d67d1c978355aadb373e3fe1b77f9e1065923eb5ff8536bcff3410cb8f1f51`  
		Last Modified: Wed, 23 Jun 2021 00:33:24 GMT  
		Size: 6.6 MB (6576842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0b1e867f7abcc7fb8d66782a1c10dba13636bfad410b71970008d1b7857728e`  
		Last Modified: Wed, 23 Jun 2021 00:33:22 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:553ab70dbc8750a6defbe988b674f8893ec3a055c04f3a8a12c99cb61b357e82`  
		Last Modified: Wed, 23 Jun 2021 00:33:22 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8` - linux; mips64le

```console
$ docker pull haproxy@sha256:5e0035aee04a59445c07bd782e49b891df503f854d71b62060fb28f8924735cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.0 MB (31958121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10f90a12c8f2c51d3cc69ccf675cda9066f4654aad83c8a004b0242de7c0308b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 22 Jul 2021 00:09:45 GMT
ADD file:1f77b9001c4977ba733be674fc5eb4b85130f1dea8a7b39d545b70f9c107695f in / 
# Thu, 22 Jul 2021 00:09:46 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:07:49 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 22 Jul 2021 01:20:44 GMT
ENV HAPROXY_VERSION=1.8.30
# Thu, 22 Jul 2021 01:20:44 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Thu, 22 Jul 2021 01:20:45 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Thu, 22 Jul 2021 01:22:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 22 Jul 2021 01:22:24 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 01:22:25 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 01:22:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Jul 2021 01:22:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 01:22:27 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:99ee621d0b0485e9de65aa19604aa2453d19ea7fc86b22c5b77c1bab74e3cb42`  
		Last Modified: Thu, 22 Jul 2021 00:16:11 GMT  
		Size: 25.8 MB (25812771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f444627794f98947a9df95ec5d19b2a1cd6c151ed438982b1dc0b89f5eaf19e`  
		Last Modified: Thu, 22 Jul 2021 01:24:39 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d46cc82c59ba90df41ab86981801c88d5b242e66fc7aaa0569003b886bac162f`  
		Last Modified: Thu, 22 Jul 2021 01:26:11 GMT  
		Size: 6.1 MB (6143400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbf8d59105a91ea0fccdabc10e39943322a0aacee2bd515cdbdf9541acfcbd22`  
		Last Modified: Thu, 22 Jul 2021 01:26:07 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f33dc89159a92c49b873fad357e16c5c49fa05ee528ea6050b127d87a5a9bcba`  
		Last Modified: Thu, 22 Jul 2021 01:26:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8` - linux; ppc64le

```console
$ docker pull haproxy@sha256:9c9c5d4fc5f93dbee548f9174b762d6e39fc83617963316f13346f4c8d04ead3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.5 MB (37499091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:402641a14b43a9ce16acf3c94c54c20b5ab477c9347adbfcc1984b4481960a78`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 22 Jul 2021 00:19:04 GMT
ADD file:3a6bd6ce3eff98b88a13de5d0f26cff0b026f876674204dbad6f84fafcf145b1 in / 
# Thu, 22 Jul 2021 00:19:13 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 02:52:46 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 22 Jul 2021 03:26:30 GMT
ENV HAPROXY_VERSION=1.8.30
# Thu, 22 Jul 2021 03:26:33 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Thu, 22 Jul 2021 03:26:39 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Thu, 22 Jul 2021 03:30:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 22 Jul 2021 03:30:37 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 03:30:40 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 03:30:59 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Jul 2021 03:31:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 03:31:21 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:1130517d52da84a09f9465006bddab5e49afd398860890eab6274fd0bff32371`  
		Last Modified: Thu, 22 Jul 2021 00:27:49 GMT  
		Size: 30.6 MB (30553709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251bf3fe1d4bbe9c27e393cd8ddc550b56cec90eb916bf9bec24d657c9f6556f`  
		Last Modified: Thu, 22 Jul 2021 03:40:01 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61fb3d9553ee91fddb953a713aa848f98a29d3236aedd84ecbd1fe73f7c7d581`  
		Last Modified: Thu, 22 Jul 2021 03:42:35 GMT  
		Size: 6.9 MB (6943432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c01a0da734e2a2af1290ab52e3772103e6555317852d017f2dd3879f97a0e1d1`  
		Last Modified: Thu, 22 Jul 2021 03:42:34 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f04d176b9caab72c3d0269811b1ac352abf634a4234b26c8805e4537d23b3eb4`  
		Last Modified: Thu, 22 Jul 2021 03:42:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8` - linux; s390x

```console
$ docker pull haproxy@sha256:8e73088111f11757c59a8461740bdbc2f7bab33013bf7700ac3454d2e978bedc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.0 MB (31995443 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9eebfda76966708b76fb2dae89132f8ba615135e4152b8caea2e315278109a45`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 22 Jul 2021 00:42:45 GMT
ADD file:1ab999eb6f80d8ce91ce3a173e23fd2710f2779117bba29037eaa82aadcbf6ed in / 
# Thu, 22 Jul 2021 00:42:48 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:30:19 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 22 Jul 2021 01:37:20 GMT
ENV HAPROXY_VERSION=1.8.30
# Thu, 22 Jul 2021 01:37:20 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Thu, 22 Jul 2021 01:37:20 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Thu, 22 Jul 2021 01:37:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 22 Jul 2021 01:37:53 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 01:37:53 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 01:37:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Jul 2021 01:37:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 01:37:55 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:7a50fdd85ff244c1465e71c51354d055e3df0b90ff5faad28cc22d9ecde9daf3`  
		Last Modified: Thu, 22 Jul 2021 00:48:13 GMT  
		Size: 25.8 MB (25760761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05fb34d1ed21b67502665114a7ae60445472fc7bafa620bbf6c79b7df85a01d4`  
		Last Modified: Thu, 22 Jul 2021 01:39:54 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba077cfa7e6e90708c2e07cb142ebaff52f44b3d0ef773086a186972cbe32d7f`  
		Last Modified: Thu, 22 Jul 2021 01:40:48 GMT  
		Size: 6.2 MB (6232733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2660ce19d595d864db2c6c6f43325a1a2a20be5368cfaa6c701e690a2aac7e`  
		Last Modified: Thu, 22 Jul 2021 01:40:47 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8538ab4000f9c186a0d027a7e6670679b4f9baaff4b566b6ad9fbab7e780c88e`  
		Last Modified: Thu, 22 Jul 2021 01:40:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:1.8-alpine`

```console
$ docker pull haproxy@sha256:dcbb69c0300b37b21bfed0591b4a2354dd60fd50676a9e983e48ff89cc3168e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `haproxy:1.8-alpine` - linux; amd64

```console
$ docker pull haproxy@sha256:f3b232552bd860f51dec9c42535811ac466258c20b797bd5793a4ed34710b0eb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6785158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5c0658210c67f673f45588fa4e74b8d64cfbdcf0ebbc8d16f988634826b6243`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 02:48:50 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 26 Jun 2021 02:55:23 GMT
ENV HAPROXY_VERSION=1.8.30
# Sat, 26 Jun 2021 02:55:23 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Sat, 26 Jun 2021 02:55:24 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Sat, 26 Jun 2021 02:55:59 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Sat, 26 Jun 2021 02:55:59 GMT
STOPSIGNAL SIGUSR1
# Sat, 26 Jun 2021 02:55:59 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 26 Jun 2021 02:56:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 26 Jun 2021 02:56:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 26 Jun 2021 02:56:01 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7834d945b9e597e693f56fb0f9847718c1732b738a2f4956ab2c1b66c289d90`  
		Last Modified: Sat, 26 Jun 2021 02:56:43 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1ecd81de9e72663b77e1dd6e22f0c7cebf5866179233f30e0798bc7cd381602`  
		Last Modified: Sat, 26 Jun 2021 02:58:03 GMT  
		Size: 4.0 MB (3971920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26218aedae4800f0c8160e642b0ef5c786f21f8bb74caa2277b2e48663ee4cd7`  
		Last Modified: Sat, 26 Jun 2021 02:58:02 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac82be057b701d7fde1dc34527274379111a89c3ba7ac7021848149175b769d`  
		Last Modified: Sat, 26 Jun 2021 02:58:02 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8-alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:eef25dda2b21939d369ab3c286f7a7670b20d1e497f84d64f28b47b5e3c05c29
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6471518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1adaeb1c210ac9b97c2546b2ad045fd9956e4ae3d0524aa201f6026688c6c13`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:26 GMT
ADD file:c80bc2b093cbc0fc466582ef21cbed377de9fa874aedbf320079525ddacd1200 in / 
# Tue, 15 Jun 2021 22:57:26 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 02:02:51 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 26 Jun 2021 02:06:28 GMT
ENV HAPROXY_VERSION=1.8.30
# Sat, 26 Jun 2021 02:06:28 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Sat, 26 Jun 2021 02:06:29 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Sat, 26 Jun 2021 02:06:54 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Sat, 26 Jun 2021 02:06:54 GMT
STOPSIGNAL SIGUSR1
# Sat, 26 Jun 2021 02:06:55 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 26 Jun 2021 02:06:57 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 26 Jun 2021 02:06:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 26 Jun 2021 02:06:58 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:b4c9a0924271af3466de27804af26420eb58da1466e7eaaba127d178b380fea3`  
		Last Modified: Tue, 15 Jun 2021 22:58:47 GMT  
		Size: 2.6 MB (2624382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85fa2947d9cc2655af4fd4aa21641629e791bcaf309a7095db77d309ddd05dfa`  
		Last Modified: Sat, 26 Jun 2021 02:08:45 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02feb03605dd20aa89b43d7c64818d79c93bbd2169b6255ec60b618528dbfd08`  
		Last Modified: Sat, 26 Jun 2021 02:10:15 GMT  
		Size: 3.8 MB (3845373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe2eb40128bf0b1b44dbabdc6a20c29f7cd638905563b69b9d1762701ae346b`  
		Last Modified: Sat, 26 Jun 2021 02:10:13 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4c27313b1d5aa8a10721ef75f898ec5ccc0348057dca8d376c1c9bdae487b4e`  
		Last Modified: Sat, 26 Jun 2021 02:10:13 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:46af83d39d06c8fd76de1142093c298ae3c39eb1dd63c6f63ec14c2782cb0170
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 MB (6212708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2acd91e1321709510330921fbfcde8ae6def0bf165cf90a56ae3555dc719d81b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:05 GMT
ADD file:416a8b507abdc6bdcb22997a4be0a4170796c3f9f77e315b2dbff2b0a212bc68 in / 
# Tue, 15 Jun 2021 23:15:06 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 05:27:42 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 26 Jun 2021 05:32:43 GMT
ENV HAPROXY_VERSION=1.8.30
# Sat, 26 Jun 2021 05:32:44 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Sat, 26 Jun 2021 05:32:44 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Sat, 26 Jun 2021 05:33:07 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Sat, 26 Jun 2021 05:33:07 GMT
STOPSIGNAL SIGUSR1
# Sat, 26 Jun 2021 05:33:08 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 26 Jun 2021 05:33:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 26 Jun 2021 05:33:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 26 Jun 2021 05:33:10 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:136482bf81d1fa351b424ebb8c7e34d15f2c5ed3fc0b66b544b8312bda3d52d9`  
		Last Modified: Tue, 15 Jun 2021 23:16:40 GMT  
		Size: 2.4 MB (2427917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5464af225bd487370319e7125fb2769222c5c7371d1be737936169d2e5b01c`  
		Last Modified: Sat, 26 Jun 2021 05:35:56 GMT  
		Size: 1.2 KB (1196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aab9ec8bcf10348d452492b90cb9cabb22ecb858ba7225fa20762ea7eb4dc98`  
		Last Modified: Sat, 26 Jun 2021 05:38:01 GMT  
		Size: 3.8 MB (3783021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fec520fafd8f709ca451744b5e511256f74e86bf33a206e5967de0dd5a44186`  
		Last Modified: Sat, 26 Jun 2021 05:37:59 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b987bc055c4030b816776bc7ca8afef215e1aed176143a26016162b013a3d6f4`  
		Last Modified: Sat, 26 Jun 2021 05:37:59 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:07a9bcea642aa9f560cb64f06a0868038749ca783af56a9bb4f36ac4107bafc0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6640622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11d042c52b8656a60215081290a49ddd6cbd061d15f5e90db7cdf49614d34d66`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 21:44:56 GMT
ADD file:6797caacbfe41bfe44000b39ed017016c6fcc492b3d6557cdaba88536df6c876 in / 
# Tue, 15 Jun 2021 21:44:56 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 02:13:15 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 26 Jun 2021 02:19:24 GMT
ENV HAPROXY_VERSION=1.8.30
# Sat, 26 Jun 2021 02:19:24 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Sat, 26 Jun 2021 02:19:25 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Sat, 26 Jun 2021 02:19:55 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Sat, 26 Jun 2021 02:19:55 GMT
STOPSIGNAL SIGUSR1
# Sat, 26 Jun 2021 02:19:55 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 26 Jun 2021 02:19:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 26 Jun 2021 02:19:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 26 Jun 2021 02:19:56 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:58ab47519297212468320b23b8100fc1b2b96e8d342040806ae509a778a0a07a`  
		Last Modified: Tue, 15 Jun 2021 21:46:03 GMT  
		Size: 2.7 MB (2709626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb8dc96e2a4b7f90ae2dbfca981fe199966b64e3426ca1f742499d46ad1aa357`  
		Last Modified: Sat, 26 Jun 2021 02:21:19 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:525ac00355a3bf8695b4b2938d5caf6df3d1361ab42711e606fe9266f20cfed8`  
		Last Modified: Sat, 26 Jun 2021 02:22:56 GMT  
		Size: 3.9 MB (3929229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18d9bba1688452b29053c8dc1e1c0e643b82aa67398d3cd8f950611f14a3d9cd`  
		Last Modified: Sat, 26 Jun 2021 02:22:55 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24cff32256a92b96a96051f8e01eaf62f793fdd215ea1b4b98627630b8327c10`  
		Last Modified: Sat, 26 Jun 2021 02:22:56 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8-alpine` - linux; 386

```console
$ docker pull haproxy@sha256:fdb0dba68cf3696596cc022ce5b2fb08a3d74d35a212f6837027771862d6cbbc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6707928 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66f73625c0bbb39e6da9eca1438f9223033d403ddd2742d37d8477ec2a0800a7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 21:38:30 GMT
ADD file:3b0fe1454491bb05e218b090fd461f2fd39546aa4a53eb3f953ee8eae149ac57 in / 
# Tue, 15 Jun 2021 21:38:30 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 01:39:05 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 26 Jun 2021 01:47:35 GMT
ENV HAPROXY_VERSION=1.8.30
# Sat, 26 Jun 2021 01:47:36 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Sat, 26 Jun 2021 01:47:36 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Sat, 26 Jun 2021 01:48:17 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Sat, 26 Jun 2021 01:48:17 GMT
STOPSIGNAL SIGUSR1
# Sat, 26 Jun 2021 01:48:18 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 26 Jun 2021 01:48:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 26 Jun 2021 01:48:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 26 Jun 2021 01:48:19 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:be21df321efb39c5daf3151073ebff7688e15ea6cd5158878bc9559a5db76ac6`  
		Last Modified: Tue, 15 Jun 2021 21:39:16 GMT  
		Size: 2.8 MB (2820718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc6fe536c8e50a97873c166db7d3b669842dec91d85ce73433028b3b198a1c4`  
		Last Modified: Sat, 26 Jun 2021 01:49:46 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd1f4902d91366e7dff82b364ce7ec81e8e83f5e4624d398725a18d99ae6b0d9`  
		Last Modified: Sat, 26 Jun 2021 01:51:23 GMT  
		Size: 3.9 MB (3885443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f035c3eeefb59488eaedf065702cb1568bf567ae5f40d299944eb7ec226bbc3c`  
		Last Modified: Sat, 26 Jun 2021 01:51:22 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5605ff4c0ad2529b8326ba5796db6d01903974b60fb979558c55ae42d670e2f`  
		Last Modified: Sat, 26 Jun 2021 01:51:22 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8-alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:6e9e11c25c3fca707ed9ada41fec20d0c0a4ffb8404b5e90c169f41fd6ac1360
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6948508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6214d3e887682c126af41f8b831edf7d9482d1e162f78a71123e9604f657ba4f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:27:00 GMT
ADD file:0075aad7a94f0496483442bb2d9fdaa13e9c23087b90638d014b4bc263aa3861 in / 
# Tue, 15 Jun 2021 22:27:03 GMT
CMD ["/bin/sh"]
# Fri, 16 Jul 2021 20:17:57 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 16 Jul 2021 20:35:28 GMT
ENV HAPROXY_VERSION=1.8.30
# Fri, 16 Jul 2021 20:35:40 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Fri, 16 Jul 2021 20:35:46 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Thu, 22 Jul 2021 03:32:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 22 Jul 2021 03:32:29 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 03:32:34 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 03:32:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Jul 2021 03:32:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 03:32:57 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:baf144cfb66ebe9df1969f3b90f1c448beff98edc84de1ccb5d6346195a070d4`  
		Last Modified: Tue, 15 Jun 2021 22:27:38 GMT  
		Size: 2.8 MB (2810478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e907663c9428bbbb731a221721c606bad29e54dac6f0dda85d6aa3175a725e`  
		Last Modified: Thu, 22 Jul 2021 03:40:16 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85501c64c5947653ce918db5aaa027034a8bd1abd2e03c4e3c8b5129505edce9`  
		Last Modified: Thu, 22 Jul 2021 03:42:49 GMT  
		Size: 4.1 MB (4136259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e0d1ca41ccbc912f12ebeb3436a01dbb33c346912815940e90c2fb888aa55df`  
		Last Modified: Thu, 22 Jul 2021 03:42:48 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8118c17b7f479e9cf15caf9bb21b476ce4cadbbeefc2adb65e9c568f9698678`  
		Last Modified: Thu, 22 Jul 2021 03:42:48 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8-alpine` - linux; s390x

```console
$ docker pull haproxy@sha256:56ab7dd8abed67c02b519cf7e49892f4b44431d493327f3aa9c26dd80841daa9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6469626 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e8e380d640dae4d7b5e8eda393c2992736478cf6bda09d77675c7938d34db2c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:54:24 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 20:57:46 GMT
ENV HAPROXY_VERSION=1.8.30
# Wed, 14 Apr 2021 20:57:46 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Wed, 14 Apr 2021 20:57:46 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Wed, 14 Apr 2021 20:58:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 20:58:10 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 20:58:10 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:58:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 20:58:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:58:12 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267275aba58470c82626189a59be76cd169bd245568e2f2545ed1ee64ff8a8ff`  
		Last Modified: Wed, 14 Apr 2021 20:59:06 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aba85d625d72596824b2a38b34880512b279ac65dacc4bb0255d3a8ba92ec8d1`  
		Last Modified: Wed, 14 Apr 2021 20:59:45 GMT  
		Size: 3.9 MB (3865222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6192a99188bab50360cf865945eb38832403ea8911957b387dd76876c1cf394`  
		Last Modified: Wed, 14 Apr 2021 20:59:44 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05bf0cbbc7f550f9e866f9b903fc73a259f80d6f6847435c4168a8af0e5c5987`  
		Last Modified: Wed, 14 Apr 2021 20:59:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:1.8.30`

```console
$ docker pull haproxy@sha256:39f817cdc6d4dd7b236b2ab1a0e1e8094d735f7ba7cce22afcb062d84a6efb5a
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

### `haproxy:1.8.30` - linux; amd64

```console
$ docker pull haproxy@sha256:3722851ed931bf31d94450e32d30ce53995833176fb723e6fc6bd05dbeee1833
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33800154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eff256be590bcd7aa144e0a8bd6302e42fa039ad3a0315a5bc068e59ab3d3b3e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 06:19:17 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 23 Jun 2021 06:26:15 GMT
ENV HAPROXY_VERSION=1.8.30
# Wed, 23 Jun 2021 06:26:16 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Wed, 23 Jun 2021 06:26:16 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Wed, 23 Jun 2021 06:27:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 23 Jun 2021 06:27:15 GMT
STOPSIGNAL SIGUSR1
# Wed, 23 Jun 2021 06:27:15 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 23 Jun 2021 06:27:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 23 Jun 2021 06:27:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 06:27:17 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91332cb81883405a321c1a2d2144bdd0aef8d1c69f90fdf0cf219982161b6e6e`  
		Last Modified: Wed, 23 Jun 2021 06:29:07 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1834e88021136e77b613445f458946e4f7a4b9b825905af333615d8b80d4937`  
		Last Modified: Wed, 23 Jun 2021 06:30:24 GMT  
		Size: 6.7 MB (6652353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be5a8071776446234e68c4cbc6bf0971a16ffb4c9645f73d8a86d8aaf4ee4867`  
		Last Modified: Wed, 23 Jun 2021 06:30:23 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e8d7be053cf42dc731cb9550682dfef65bc311ee24670e94de26013d2b7ba02`  
		Last Modified: Wed, 23 Jun 2021 06:30:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8.30` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:9503a1c3eb6628c761fb14ac3eeedbef80baa48fcecec96384f2f4a3cf172c86
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.1 MB (31112125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c3e36feaeb4a286370c17155be20e8b7ece4204fcc1d9a5c5319d6997586b5b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 22 Jun 2021 23:50:09 GMT
ADD file:78d4ced31112d85490c684f350aceeebfc72a804262c7ad3e033257e3894f5c4 in / 
# Tue, 22 Jun 2021 23:50:11 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:15:11 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 23 Jun 2021 05:20:46 GMT
ENV HAPROXY_VERSION=1.8.30
# Wed, 23 Jun 2021 05:20:46 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Wed, 23 Jun 2021 05:20:47 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Wed, 23 Jun 2021 05:21:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 23 Jun 2021 05:21:37 GMT
STOPSIGNAL SIGUSR1
# Wed, 23 Jun 2021 05:21:37 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 23 Jun 2021 05:21:39 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 23 Jun 2021 05:21:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 05:21:39 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:532d6df30af5174ac6e1b379c32b8f464d44651ac060376a560c4a76a87704a7`  
		Last Modified: Wed, 23 Jun 2021 00:01:46 GMT  
		Size: 24.9 MB (24878945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48649e3d7de4cd80d3a9a34c725a2935be904ff90e99ea6c8e4bb6e1e7a4eeb7`  
		Last Modified: Wed, 23 Jun 2021 05:24:11 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc3dd6789232c458605cbaaa7c798549960214f7a917be6d09b50a160a56ef0c`  
		Last Modified: Wed, 23 Jun 2021 05:25:56 GMT  
		Size: 6.2 MB (6231232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e605d3d155543a0840b26414df9da3eedc76abc199087ab5c493c064202257cf`  
		Last Modified: Wed, 23 Jun 2021 05:25:52 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe96a800a1c1b4beb8174e7b375f121ab502b1c5b04335e9f408391061ef65d`  
		Last Modified: Wed, 23 Jun 2021 05:25:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8.30` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:d6aad0ea1b82d238046fb58649e31f79356de73ef9e0a1b993580ae2209da0f3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.8 MB (28818881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b466de86d10c7ae44bbdbf238a5cca50d3c8accefe36c48dcc13c91e3e4666e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:31 GMT
ADD file:8d200a3bbe985ff355343675c5555852f27550a9e367969df6bc98034efb8fd4 in / 
# Wed, 23 Jun 2021 00:20:31 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:21:41 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 23 Jun 2021 05:30:20 GMT
ENV HAPROXY_VERSION=1.8.30
# Wed, 23 Jun 2021 05:30:21 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Wed, 23 Jun 2021 05:30:21 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Wed, 23 Jun 2021 05:31:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 23 Jun 2021 05:31:08 GMT
STOPSIGNAL SIGUSR1
# Wed, 23 Jun 2021 05:31:08 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 23 Jun 2021 05:31:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 23 Jun 2021 05:31:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 05:31:10 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:8452be1adf00f91570fe21a8e61aaf4c12e014daf67d7de65d984f4e8ecca2f1`  
		Last Modified: Wed, 23 Jun 2021 00:31:49 GMT  
		Size: 22.7 MB (22746055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed1c9c92d0076fd4bf40503e3f47102509a5b99d182f4dd9e81e64d0a7e0b8a`  
		Last Modified: Wed, 23 Jun 2021 05:35:48 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faefe1906560d2be5bc0d0ff2712dfbb3281753e9fc3c46bf536e932c8cb6b2c`  
		Last Modified: Wed, 23 Jun 2021 05:38:52 GMT  
		Size: 6.1 MB (6070877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa78b9a61872e76b9579ba405a854bd84c35304d7fb85b5f97a898c9b576c902`  
		Last Modified: Wed, 23 Jun 2021 05:38:49 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c24e2f44ba1bc9242d7c8bfec83f249d20cffc351a650807c6e5e6d958b40d11`  
		Last Modified: Wed, 23 Jun 2021 05:38:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8.30` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:f8eca28dc001d9734c7c3ccec202b734f2f874b2a5314c163642cdcc08d11211
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.4 MB (32370707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ffe3d091b1855a41fc0e5b4dbf130cabc62733a55fd6ff06974a6145adb205c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:40 GMT
ADD file:beee00b59da720f68e12e2ba2a8134207c80c777ddb4ceb03c71e3e4c3f51c93 in / 
# Tue, 22 Jun 2021 23:49:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 03:19:31 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 23 Jun 2021 03:23:49 GMT
ENV HAPROXY_VERSION=1.8.30
# Wed, 23 Jun 2021 03:23:49 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Wed, 23 Jun 2021 03:23:49 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Wed, 23 Jun 2021 03:24:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 23 Jun 2021 03:24:18 GMT
STOPSIGNAL SIGUSR1
# Wed, 23 Jun 2021 03:24:18 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 23 Jun 2021 03:24:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 23 Jun 2021 03:24:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 03:24:19 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:448f6bf000e31217a7c202c659b03b7f8ac8d3ae6b03ef7a2f8339be2f00ff4a`  
		Last Modified: Tue, 22 Jun 2021 23:55:25 GMT  
		Size: 25.9 MB (25914993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b05ad81dc8a7d67656235988f0e5fb72c374c7d8df44c105b91d712e06c4ac`  
		Last Modified: Wed, 23 Jun 2021 03:26:16 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2c08bfd067c99cbb1d435d19d33818c3df5f623311eaecd221541938020c84f`  
		Last Modified: Wed, 23 Jun 2021 03:27:39 GMT  
		Size: 6.5 MB (6453765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45c6c10b3a1bbe6240132054604cddbcca782aa44ffe70d2a9e491f7970be096`  
		Last Modified: Wed, 23 Jun 2021 03:27:37 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c24f8961860ba35f878ad8964ecb67f7aae9b185fe26729d278b583104dd7a`  
		Last Modified: Wed, 23 Jun 2021 03:27:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8.30` - linux; 386

```console
$ docker pull haproxy@sha256:e07d1474fb9df83b62a04484b9318e5fd98e18c8dc07e4eac23f786d84d5fe80
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.4 MB (34376202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db3e086afd7d3a71e10d8394214db534f5178240d835f5ccf933d5f33dd262c1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 22 Jun 2021 23:39:35 GMT
ADD file:48f656ac6733911048b3de850490438d0233b3badc11861fca62062d4edfaf40 in / 
# Tue, 22 Jun 2021 23:39:35 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:23:13 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 23 Jun 2021 00:29:05 GMT
ENV HAPROXY_VERSION=1.8.30
# Wed, 23 Jun 2021 00:29:05 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Wed, 23 Jun 2021 00:29:05 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Wed, 23 Jun 2021 00:29:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 23 Jun 2021 00:29:46 GMT
STOPSIGNAL SIGUSR1
# Wed, 23 Jun 2021 00:29:46 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 23 Jun 2021 00:29:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 23 Jun 2021 00:29:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Jun 2021 00:29:48 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:33af2dcb865e65d53cdeb843b67a0ef62151fa32df292293e7c6b0eb728ac5ac`  
		Last Modified: Tue, 22 Jun 2021 23:46:23 GMT  
		Size: 27.8 MB (27797411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a6e4d42b23996eb7d8a1baa85ee19828c2667fd4a2dca6eb1040b266680e9f`  
		Last Modified: Wed, 23 Jun 2021 00:32:00 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d67d1c978355aadb373e3fe1b77f9e1065923eb5ff8536bcff3410cb8f1f51`  
		Last Modified: Wed, 23 Jun 2021 00:33:24 GMT  
		Size: 6.6 MB (6576842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0b1e867f7abcc7fb8d66782a1c10dba13636bfad410b71970008d1b7857728e`  
		Last Modified: Wed, 23 Jun 2021 00:33:22 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:553ab70dbc8750a6defbe988b674f8893ec3a055c04f3a8a12c99cb61b357e82`  
		Last Modified: Wed, 23 Jun 2021 00:33:22 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8.30` - linux; mips64le

```console
$ docker pull haproxy@sha256:5e0035aee04a59445c07bd782e49b891df503f854d71b62060fb28f8924735cb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.0 MB (31958121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10f90a12c8f2c51d3cc69ccf675cda9066f4654aad83c8a004b0242de7c0308b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 22 Jul 2021 00:09:45 GMT
ADD file:1f77b9001c4977ba733be674fc5eb4b85130f1dea8a7b39d545b70f9c107695f in / 
# Thu, 22 Jul 2021 00:09:46 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:07:49 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 22 Jul 2021 01:20:44 GMT
ENV HAPROXY_VERSION=1.8.30
# Thu, 22 Jul 2021 01:20:44 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Thu, 22 Jul 2021 01:20:45 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Thu, 22 Jul 2021 01:22:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 22 Jul 2021 01:22:24 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 01:22:25 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 01:22:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Jul 2021 01:22:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 01:22:27 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:99ee621d0b0485e9de65aa19604aa2453d19ea7fc86b22c5b77c1bab74e3cb42`  
		Last Modified: Thu, 22 Jul 2021 00:16:11 GMT  
		Size: 25.8 MB (25812771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f444627794f98947a9df95ec5d19b2a1cd6c151ed438982b1dc0b89f5eaf19e`  
		Last Modified: Thu, 22 Jul 2021 01:24:39 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d46cc82c59ba90df41ab86981801c88d5b242e66fc7aaa0569003b886bac162f`  
		Last Modified: Thu, 22 Jul 2021 01:26:11 GMT  
		Size: 6.1 MB (6143400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbf8d59105a91ea0fccdabc10e39943322a0aacee2bd515cdbdf9541acfcbd22`  
		Last Modified: Thu, 22 Jul 2021 01:26:07 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f33dc89159a92c49b873fad357e16c5c49fa05ee528ea6050b127d87a5a9bcba`  
		Last Modified: Thu, 22 Jul 2021 01:26:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8.30` - linux; ppc64le

```console
$ docker pull haproxy@sha256:9c9c5d4fc5f93dbee548f9174b762d6e39fc83617963316f13346f4c8d04ead3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.5 MB (37499091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:402641a14b43a9ce16acf3c94c54c20b5ab477c9347adbfcc1984b4481960a78`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 22 Jul 2021 00:19:04 GMT
ADD file:3a6bd6ce3eff98b88a13de5d0f26cff0b026f876674204dbad6f84fafcf145b1 in / 
# Thu, 22 Jul 2021 00:19:13 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 02:52:46 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 22 Jul 2021 03:26:30 GMT
ENV HAPROXY_VERSION=1.8.30
# Thu, 22 Jul 2021 03:26:33 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Thu, 22 Jul 2021 03:26:39 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Thu, 22 Jul 2021 03:30:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 22 Jul 2021 03:30:37 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 03:30:40 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 03:30:59 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Jul 2021 03:31:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 03:31:21 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:1130517d52da84a09f9465006bddab5e49afd398860890eab6274fd0bff32371`  
		Last Modified: Thu, 22 Jul 2021 00:27:49 GMT  
		Size: 30.6 MB (30553709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251bf3fe1d4bbe9c27e393cd8ddc550b56cec90eb916bf9bec24d657c9f6556f`  
		Last Modified: Thu, 22 Jul 2021 03:40:01 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61fb3d9553ee91fddb953a713aa848f98a29d3236aedd84ecbd1fe73f7c7d581`  
		Last Modified: Thu, 22 Jul 2021 03:42:35 GMT  
		Size: 6.9 MB (6943432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c01a0da734e2a2af1290ab52e3772103e6555317852d017f2dd3879f97a0e1d1`  
		Last Modified: Thu, 22 Jul 2021 03:42:34 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f04d176b9caab72c3d0269811b1ac352abf634a4234b26c8805e4537d23b3eb4`  
		Last Modified: Thu, 22 Jul 2021 03:42:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8.30` - linux; s390x

```console
$ docker pull haproxy@sha256:8e73088111f11757c59a8461740bdbc2f7bab33013bf7700ac3454d2e978bedc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.0 MB (31995443 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9eebfda76966708b76fb2dae89132f8ba615135e4152b8caea2e315278109a45`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 22 Jul 2021 00:42:45 GMT
ADD file:1ab999eb6f80d8ce91ce3a173e23fd2710f2779117bba29037eaa82aadcbf6ed in / 
# Thu, 22 Jul 2021 00:42:48 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:30:19 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 22 Jul 2021 01:37:20 GMT
ENV HAPROXY_VERSION=1.8.30
# Thu, 22 Jul 2021 01:37:20 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Thu, 22 Jul 2021 01:37:20 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Thu, 22 Jul 2021 01:37:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 22 Jul 2021 01:37:53 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 01:37:53 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 01:37:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Jul 2021 01:37:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 01:37:55 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:7a50fdd85ff244c1465e71c51354d055e3df0b90ff5faad28cc22d9ecde9daf3`  
		Last Modified: Thu, 22 Jul 2021 00:48:13 GMT  
		Size: 25.8 MB (25760761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05fb34d1ed21b67502665114a7ae60445472fc7bafa620bbf6c79b7df85a01d4`  
		Last Modified: Thu, 22 Jul 2021 01:39:54 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba077cfa7e6e90708c2e07cb142ebaff52f44b3d0ef773086a186972cbe32d7f`  
		Last Modified: Thu, 22 Jul 2021 01:40:48 GMT  
		Size: 6.2 MB (6232733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2660ce19d595d864db2c6c6f43325a1a2a20be5368cfaa6c701e690a2aac7e`  
		Last Modified: Thu, 22 Jul 2021 01:40:47 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8538ab4000f9c186a0d027a7e6670679b4f9baaff4b566b6ad9fbab7e780c88e`  
		Last Modified: Thu, 22 Jul 2021 01:40:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:1.8.30-alpine`

```console
$ docker pull haproxy@sha256:dcbb69c0300b37b21bfed0591b4a2354dd60fd50676a9e983e48ff89cc3168e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `haproxy:1.8.30-alpine` - linux; amd64

```console
$ docker pull haproxy@sha256:f3b232552bd860f51dec9c42535811ac466258c20b797bd5793a4ed34710b0eb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6785158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5c0658210c67f673f45588fa4e74b8d64cfbdcf0ebbc8d16f988634826b6243`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 02:48:50 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 26 Jun 2021 02:55:23 GMT
ENV HAPROXY_VERSION=1.8.30
# Sat, 26 Jun 2021 02:55:23 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Sat, 26 Jun 2021 02:55:24 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Sat, 26 Jun 2021 02:55:59 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Sat, 26 Jun 2021 02:55:59 GMT
STOPSIGNAL SIGUSR1
# Sat, 26 Jun 2021 02:55:59 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 26 Jun 2021 02:56:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 26 Jun 2021 02:56:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 26 Jun 2021 02:56:01 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7834d945b9e597e693f56fb0f9847718c1732b738a2f4956ab2c1b66c289d90`  
		Last Modified: Sat, 26 Jun 2021 02:56:43 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1ecd81de9e72663b77e1dd6e22f0c7cebf5866179233f30e0798bc7cd381602`  
		Last Modified: Sat, 26 Jun 2021 02:58:03 GMT  
		Size: 4.0 MB (3971920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26218aedae4800f0c8160e642b0ef5c786f21f8bb74caa2277b2e48663ee4cd7`  
		Last Modified: Sat, 26 Jun 2021 02:58:02 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac82be057b701d7fde1dc34527274379111a89c3ba7ac7021848149175b769d`  
		Last Modified: Sat, 26 Jun 2021 02:58:02 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8.30-alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:eef25dda2b21939d369ab3c286f7a7670b20d1e497f84d64f28b47b5e3c05c29
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6471518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1adaeb1c210ac9b97c2546b2ad045fd9956e4ae3d0524aa201f6026688c6c13`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:26 GMT
ADD file:c80bc2b093cbc0fc466582ef21cbed377de9fa874aedbf320079525ddacd1200 in / 
# Tue, 15 Jun 2021 22:57:26 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 02:02:51 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 26 Jun 2021 02:06:28 GMT
ENV HAPROXY_VERSION=1.8.30
# Sat, 26 Jun 2021 02:06:28 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Sat, 26 Jun 2021 02:06:29 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Sat, 26 Jun 2021 02:06:54 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Sat, 26 Jun 2021 02:06:54 GMT
STOPSIGNAL SIGUSR1
# Sat, 26 Jun 2021 02:06:55 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 26 Jun 2021 02:06:57 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 26 Jun 2021 02:06:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 26 Jun 2021 02:06:58 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:b4c9a0924271af3466de27804af26420eb58da1466e7eaaba127d178b380fea3`  
		Last Modified: Tue, 15 Jun 2021 22:58:47 GMT  
		Size: 2.6 MB (2624382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85fa2947d9cc2655af4fd4aa21641629e791bcaf309a7095db77d309ddd05dfa`  
		Last Modified: Sat, 26 Jun 2021 02:08:45 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02feb03605dd20aa89b43d7c64818d79c93bbd2169b6255ec60b618528dbfd08`  
		Last Modified: Sat, 26 Jun 2021 02:10:15 GMT  
		Size: 3.8 MB (3845373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe2eb40128bf0b1b44dbabdc6a20c29f7cd638905563b69b9d1762701ae346b`  
		Last Modified: Sat, 26 Jun 2021 02:10:13 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4c27313b1d5aa8a10721ef75f898ec5ccc0348057dca8d376c1c9bdae487b4e`  
		Last Modified: Sat, 26 Jun 2021 02:10:13 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8.30-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:46af83d39d06c8fd76de1142093c298ae3c39eb1dd63c6f63ec14c2782cb0170
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 MB (6212708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2acd91e1321709510330921fbfcde8ae6def0bf165cf90a56ae3555dc719d81b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:05 GMT
ADD file:416a8b507abdc6bdcb22997a4be0a4170796c3f9f77e315b2dbff2b0a212bc68 in / 
# Tue, 15 Jun 2021 23:15:06 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 05:27:42 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 26 Jun 2021 05:32:43 GMT
ENV HAPROXY_VERSION=1.8.30
# Sat, 26 Jun 2021 05:32:44 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Sat, 26 Jun 2021 05:32:44 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Sat, 26 Jun 2021 05:33:07 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Sat, 26 Jun 2021 05:33:07 GMT
STOPSIGNAL SIGUSR1
# Sat, 26 Jun 2021 05:33:08 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 26 Jun 2021 05:33:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 26 Jun 2021 05:33:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 26 Jun 2021 05:33:10 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:136482bf81d1fa351b424ebb8c7e34d15f2c5ed3fc0b66b544b8312bda3d52d9`  
		Last Modified: Tue, 15 Jun 2021 23:16:40 GMT  
		Size: 2.4 MB (2427917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5464af225bd487370319e7125fb2769222c5c7371d1be737936169d2e5b01c`  
		Last Modified: Sat, 26 Jun 2021 05:35:56 GMT  
		Size: 1.2 KB (1196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aab9ec8bcf10348d452492b90cb9cabb22ecb858ba7225fa20762ea7eb4dc98`  
		Last Modified: Sat, 26 Jun 2021 05:38:01 GMT  
		Size: 3.8 MB (3783021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fec520fafd8f709ca451744b5e511256f74e86bf33a206e5967de0dd5a44186`  
		Last Modified: Sat, 26 Jun 2021 05:37:59 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b987bc055c4030b816776bc7ca8afef215e1aed176143a26016162b013a3d6f4`  
		Last Modified: Sat, 26 Jun 2021 05:37:59 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8.30-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:07a9bcea642aa9f560cb64f06a0868038749ca783af56a9bb4f36ac4107bafc0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6640622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11d042c52b8656a60215081290a49ddd6cbd061d15f5e90db7cdf49614d34d66`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 21:44:56 GMT
ADD file:6797caacbfe41bfe44000b39ed017016c6fcc492b3d6557cdaba88536df6c876 in / 
# Tue, 15 Jun 2021 21:44:56 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 02:13:15 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 26 Jun 2021 02:19:24 GMT
ENV HAPROXY_VERSION=1.8.30
# Sat, 26 Jun 2021 02:19:24 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Sat, 26 Jun 2021 02:19:25 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Sat, 26 Jun 2021 02:19:55 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Sat, 26 Jun 2021 02:19:55 GMT
STOPSIGNAL SIGUSR1
# Sat, 26 Jun 2021 02:19:55 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 26 Jun 2021 02:19:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 26 Jun 2021 02:19:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 26 Jun 2021 02:19:56 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:58ab47519297212468320b23b8100fc1b2b96e8d342040806ae509a778a0a07a`  
		Last Modified: Tue, 15 Jun 2021 21:46:03 GMT  
		Size: 2.7 MB (2709626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb8dc96e2a4b7f90ae2dbfca981fe199966b64e3426ca1f742499d46ad1aa357`  
		Last Modified: Sat, 26 Jun 2021 02:21:19 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:525ac00355a3bf8695b4b2938d5caf6df3d1361ab42711e606fe9266f20cfed8`  
		Last Modified: Sat, 26 Jun 2021 02:22:56 GMT  
		Size: 3.9 MB (3929229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18d9bba1688452b29053c8dc1e1c0e643b82aa67398d3cd8f950611f14a3d9cd`  
		Last Modified: Sat, 26 Jun 2021 02:22:55 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24cff32256a92b96a96051f8e01eaf62f793fdd215ea1b4b98627630b8327c10`  
		Last Modified: Sat, 26 Jun 2021 02:22:56 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8.30-alpine` - linux; 386

```console
$ docker pull haproxy@sha256:fdb0dba68cf3696596cc022ce5b2fb08a3d74d35a212f6837027771862d6cbbc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6707928 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66f73625c0bbb39e6da9eca1438f9223033d403ddd2742d37d8477ec2a0800a7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 21:38:30 GMT
ADD file:3b0fe1454491bb05e218b090fd461f2fd39546aa4a53eb3f953ee8eae149ac57 in / 
# Tue, 15 Jun 2021 21:38:30 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 01:39:05 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 26 Jun 2021 01:47:35 GMT
ENV HAPROXY_VERSION=1.8.30
# Sat, 26 Jun 2021 01:47:36 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Sat, 26 Jun 2021 01:47:36 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Sat, 26 Jun 2021 01:48:17 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Sat, 26 Jun 2021 01:48:17 GMT
STOPSIGNAL SIGUSR1
# Sat, 26 Jun 2021 01:48:18 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 26 Jun 2021 01:48:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 26 Jun 2021 01:48:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 26 Jun 2021 01:48:19 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:be21df321efb39c5daf3151073ebff7688e15ea6cd5158878bc9559a5db76ac6`  
		Last Modified: Tue, 15 Jun 2021 21:39:16 GMT  
		Size: 2.8 MB (2820718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc6fe536c8e50a97873c166db7d3b669842dec91d85ce73433028b3b198a1c4`  
		Last Modified: Sat, 26 Jun 2021 01:49:46 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd1f4902d91366e7dff82b364ce7ec81e8e83f5e4624d398725a18d99ae6b0d9`  
		Last Modified: Sat, 26 Jun 2021 01:51:23 GMT  
		Size: 3.9 MB (3885443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f035c3eeefb59488eaedf065702cb1568bf567ae5f40d299944eb7ec226bbc3c`  
		Last Modified: Sat, 26 Jun 2021 01:51:22 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5605ff4c0ad2529b8326ba5796db6d01903974b60fb979558c55ae42d670e2f`  
		Last Modified: Sat, 26 Jun 2021 01:51:22 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8.30-alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:6e9e11c25c3fca707ed9ada41fec20d0c0a4ffb8404b5e90c169f41fd6ac1360
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6948508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6214d3e887682c126af41f8b831edf7d9482d1e162f78a71123e9604f657ba4f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:27:00 GMT
ADD file:0075aad7a94f0496483442bb2d9fdaa13e9c23087b90638d014b4bc263aa3861 in / 
# Tue, 15 Jun 2021 22:27:03 GMT
CMD ["/bin/sh"]
# Fri, 16 Jul 2021 20:17:57 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 16 Jul 2021 20:35:28 GMT
ENV HAPROXY_VERSION=1.8.30
# Fri, 16 Jul 2021 20:35:40 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Fri, 16 Jul 2021 20:35:46 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Thu, 22 Jul 2021 03:32:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 22 Jul 2021 03:32:29 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 03:32:34 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 03:32:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Jul 2021 03:32:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 03:32:57 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:baf144cfb66ebe9df1969f3b90f1c448beff98edc84de1ccb5d6346195a070d4`  
		Last Modified: Tue, 15 Jun 2021 22:27:38 GMT  
		Size: 2.8 MB (2810478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e907663c9428bbbb731a221721c606bad29e54dac6f0dda85d6aa3175a725e`  
		Last Modified: Thu, 22 Jul 2021 03:40:16 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85501c64c5947653ce918db5aaa027034a8bd1abd2e03c4e3c8b5129505edce9`  
		Last Modified: Thu, 22 Jul 2021 03:42:49 GMT  
		Size: 4.1 MB (4136259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e0d1ca41ccbc912f12ebeb3436a01dbb33c346912815940e90c2fb888aa55df`  
		Last Modified: Thu, 22 Jul 2021 03:42:48 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8118c17b7f479e9cf15caf9bb21b476ce4cadbbeefc2adb65e9c568f9698678`  
		Last Modified: Thu, 22 Jul 2021 03:42:48 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8.30-alpine` - linux; s390x

```console
$ docker pull haproxy@sha256:56ab7dd8abed67c02b519cf7e49892f4b44431d493327f3aa9c26dd80841daa9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6469626 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e8e380d640dae4d7b5e8eda393c2992736478cf6bda09d77675c7938d34db2c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:54:24 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 20:57:46 GMT
ENV HAPROXY_VERSION=1.8.30
# Wed, 14 Apr 2021 20:57:46 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Wed, 14 Apr 2021 20:57:46 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Wed, 14 Apr 2021 20:58:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 20:58:10 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 20:58:10 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:58:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 20:58:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:58:12 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267275aba58470c82626189a59be76cd169bd245568e2f2545ed1ee64ff8a8ff`  
		Last Modified: Wed, 14 Apr 2021 20:59:06 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aba85d625d72596824b2a38b34880512b279ac65dacc4bb0255d3a8ba92ec8d1`  
		Last Modified: Wed, 14 Apr 2021 20:59:45 GMT  
		Size: 3.9 MB (3865222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6192a99188bab50360cf865945eb38832403ea8911957b387dd76876c1cf394`  
		Last Modified: Wed, 14 Apr 2021 20:59:44 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05bf0cbbc7f550f9e866f9b903fc73a259f80d6f6847435c4168a8af0e5c5987`  
		Last Modified: Wed, 14 Apr 2021 20:59:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.0`

```console
$ docker pull haproxy@sha256:138702b49465b4c9888f54a809d22331230b9dbcaf0627d0423a702c3cf9760c
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

### `haproxy:2.0` - linux; amd64

```console
$ docker pull haproxy@sha256:e23a2254dbea4fce44679c7017a8b2d09f08665c6fc21b0c81d08e86c4cbcb5f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.8 MB (35809252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04015a55056dc92dcbe712fa83cbb1b5d6c99ceb07b6b8dccc82cf445db0d268`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 06:19:17 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 16 Jul 2021 20:22:01 GMT
ENV HAPROXY_VERSION=2.0.23
# Fri, 16 Jul 2021 20:22:01 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.23.tar.gz
# Fri, 16 Jul 2021 20:22:01 GMT
ENV HAPROXY_SHA256=5ddc04e9040a07c647fa4b68fc9da6ec36063d56e12824b356e770dcf677c87a
# Fri, 16 Jul 2021 20:22:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 16 Jul 2021 20:22:54 GMT
STOPSIGNAL SIGUSR1
# Fri, 16 Jul 2021 20:22:55 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 16 Jul 2021 20:22:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 16 Jul 2021 20:22:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jul 2021 20:22:56 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91332cb81883405a321c1a2d2144bdd0aef8d1c69f90fdf0cf219982161b6e6e`  
		Last Modified: Wed, 23 Jun 2021 06:29:07 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a3a75bd4f980d88055f8d6dc5e659eae8aa1d65d1cf09499c3ea3f6dfd0c4f`  
		Last Modified: Fri, 16 Jul 2021 20:25:14 GMT  
		Size: 8.7 MB (8661448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4c86e186785e009b76f53d8371fde694020334f0c7fcee94d2c621f2d80bc6b`  
		Last Modified: Fri, 16 Jul 2021 20:25:12 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715c25c22c1e52db6636c84e959e8dda5d6b95fd721cb4a8e003db69770b10bb`  
		Last Modified: Fri, 16 Jul 2021 20:25:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:1ea758cc14b6f3dfe45650e197d8df22ae573ab3c41e56c3cd122716402b804d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.1 MB (33069410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f93df7025ee4e7be230bf75b5e4e30836f420519916695321a5344c3641023e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 22 Jun 2021 23:50:09 GMT
ADD file:78d4ced31112d85490c684f350aceeebfc72a804262c7ad3e033257e3894f5c4 in / 
# Tue, 22 Jun 2021 23:50:11 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:15:11 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 16 Jul 2021 19:50:26 GMT
ENV HAPROXY_VERSION=2.0.23
# Fri, 16 Jul 2021 19:50:26 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.23.tar.gz
# Fri, 16 Jul 2021 19:50:27 GMT
ENV HAPROXY_SHA256=5ddc04e9040a07c647fa4b68fc9da6ec36063d56e12824b356e770dcf677c87a
# Fri, 16 Jul 2021 19:51:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 16 Jul 2021 19:51:16 GMT
STOPSIGNAL SIGUSR1
# Fri, 16 Jul 2021 19:51:17 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 16 Jul 2021 19:51:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 16 Jul 2021 19:51:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jul 2021 19:51:19 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:532d6df30af5174ac6e1b379c32b8f464d44651ac060376a560c4a76a87704a7`  
		Last Modified: Wed, 23 Jun 2021 00:01:46 GMT  
		Size: 24.9 MB (24878945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48649e3d7de4cd80d3a9a34c725a2935be904ff90e99ea6c8e4bb6e1e7a4eeb7`  
		Last Modified: Wed, 23 Jun 2021 05:24:11 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de179a73ab38812fe744f4984790e412ec57ce2acce04638ffa2a41ed258e0c3`  
		Last Modified: Fri, 16 Jul 2021 19:53:32 GMT  
		Size: 8.2 MB (8188519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eed6b8b10dcb7503a4037f31b3e3c20dbe705c3c2655f9161805cf08db301f3`  
		Last Modified: Fri, 16 Jul 2021 19:53:27 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c8fa2481a0e1635ffa5e396654295801b17a6d6a5be125ff3334ce358731ac5`  
		Last Modified: Fri, 16 Jul 2021 19:53:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:c1040c9ac9c6cd38d8b5e76a57da4913ddf903bf9716f948391413cf12e7319a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.9 MB (30861541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b04744c0c97785732765b8c9a92ca8b89b83d9a69478e097b9e3c706fdf1ba2d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:31 GMT
ADD file:8d200a3bbe985ff355343675c5555852f27550a9e367969df6bc98034efb8fd4 in / 
# Wed, 23 Jun 2021 00:20:31 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:21:41 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 16 Jul 2021 20:38:05 GMT
ENV HAPROXY_VERSION=2.0.23
# Fri, 16 Jul 2021 20:38:05 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.23.tar.gz
# Fri, 16 Jul 2021 20:38:06 GMT
ENV HAPROXY_SHA256=5ddc04e9040a07c647fa4b68fc9da6ec36063d56e12824b356e770dcf677c87a
# Fri, 16 Jul 2021 20:38:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 16 Jul 2021 20:38:51 GMT
STOPSIGNAL SIGUSR1
# Fri, 16 Jul 2021 20:38:52 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 16 Jul 2021 20:38:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 16 Jul 2021 20:38:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jul 2021 20:38:54 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:8452be1adf00f91570fe21a8e61aaf4c12e014daf67d7de65d984f4e8ecca2f1`  
		Last Modified: Wed, 23 Jun 2021 00:31:49 GMT  
		Size: 22.7 MB (22746055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed1c9c92d0076fd4bf40503e3f47102509a5b99d182f4dd9e81e64d0a7e0b8a`  
		Last Modified: Wed, 23 Jun 2021 05:35:48 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a4707ad32ba231e4366e36f1a859edd24952c7e77c200d1737dbe917e32a670`  
		Last Modified: Fri, 16 Jul 2021 20:43:38 GMT  
		Size: 8.1 MB (8113539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aeb934403d774d328050209d2fa7157e7cd0f483fe1ddfaf86630910df0718c`  
		Last Modified: Fri, 16 Jul 2021 20:43:33 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9cec3dc0c28d8cbdb7b25acd084e80b1f1c70c80685d1e921d943171897f959`  
		Last Modified: Fri, 16 Jul 2021 20:43:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:92a27f5848362f34e6b4074caa860fddce95d22fe63bc9e32ce5c79345d4eb12
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.4 MB (34439104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3aa1e7b28a2822eccb53903de5dce966be08997b4d8c562d7a2c70e1cbd04fb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:40 GMT
ADD file:beee00b59da720f68e12e2ba2a8134207c80c777ddb4ceb03c71e3e4c3f51c93 in / 
# Tue, 22 Jun 2021 23:49:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 03:19:31 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 16 Jul 2021 19:42:05 GMT
ENV HAPROXY_VERSION=2.0.23
# Fri, 16 Jul 2021 19:42:05 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.23.tar.gz
# Fri, 16 Jul 2021 19:42:05 GMT
ENV HAPROXY_SHA256=5ddc04e9040a07c647fa4b68fc9da6ec36063d56e12824b356e770dcf677c87a
# Fri, 16 Jul 2021 19:42:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 16 Jul 2021 19:42:40 GMT
STOPSIGNAL SIGUSR1
# Fri, 16 Jul 2021 19:42:41 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 16 Jul 2021 19:42:42 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 16 Jul 2021 19:42:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jul 2021 19:42:42 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:448f6bf000e31217a7c202c659b03b7f8ac8d3ae6b03ef7a2f8339be2f00ff4a`  
		Last Modified: Tue, 22 Jun 2021 23:55:25 GMT  
		Size: 25.9 MB (25914993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b05ad81dc8a7d67656235988f0e5fb72c374c7d8df44c105b91d712e06c4ac`  
		Last Modified: Wed, 23 Jun 2021 03:26:16 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27571973ed676b6b80333392ed3bff443d02940d7391eb5305a2ca15aa7f7171`  
		Last Modified: Fri, 16 Jul 2021 19:45:44 GMT  
		Size: 8.5 MB (8522161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b9e3742d5e38bce45625e755934c9c25c143447d6b53c253b2519619918435`  
		Last Modified: Fri, 16 Jul 2021 19:45:42 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d3a947db69556f61b2d10db26e579d74665e585ea7d17d73b1a612b3542aa8`  
		Last Modified: Fri, 16 Jul 2021 19:45:42 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0` - linux; 386

```console
$ docker pull haproxy@sha256:95e4d43371492ccc71318f3bbf365ad878b3f9996bdda95045e573fd255734a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36299325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2de994a6f5c25434fea01095e252592edac58522cda4982717fd89566cc61946`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 22 Jun 2021 23:39:35 GMT
ADD file:48f656ac6733911048b3de850490438d0233b3badc11861fca62062d4edfaf40 in / 
# Tue, 22 Jun 2021 23:39:35 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:23:13 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 16 Jul 2021 19:42:02 GMT
ENV HAPROXY_VERSION=2.0.23
# Fri, 16 Jul 2021 19:42:02 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.23.tar.gz
# Fri, 16 Jul 2021 19:42:02 GMT
ENV HAPROXY_SHA256=5ddc04e9040a07c647fa4b68fc9da6ec36063d56e12824b356e770dcf677c87a
# Fri, 16 Jul 2021 19:42:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 16 Jul 2021 19:42:51 GMT
STOPSIGNAL SIGUSR1
# Fri, 16 Jul 2021 19:42:51 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 16 Jul 2021 19:42:52 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 16 Jul 2021 19:42:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jul 2021 19:42:52 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:33af2dcb865e65d53cdeb843b67a0ef62151fa32df292293e7c6b0eb728ac5ac`  
		Last Modified: Tue, 22 Jun 2021 23:46:23 GMT  
		Size: 27.8 MB (27797411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a6e4d42b23996eb7d8a1baa85ee19828c2667fd4a2dca6eb1040b266680e9f`  
		Last Modified: Wed, 23 Jun 2021 00:32:00 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c10787c75f23a36f58130786923d1b9c7d2be2b9c2f0c1a29441585915839f`  
		Last Modified: Fri, 16 Jul 2021 19:46:20 GMT  
		Size: 8.5 MB (8499965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d89c48ad14be00161088c14311a315bd124c1827a6fd335ae59c01a6c50169`  
		Last Modified: Fri, 16 Jul 2021 19:46:18 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79347bc64811a94a1f9ab15200d7e967f6a6c727baa14e067be5327432664a4f`  
		Last Modified: Fri, 16 Jul 2021 19:46:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0` - linux; mips64le

```console
$ docker pull haproxy@sha256:a7e464070f23af3cebfb2f0c59a05afbd6fc188899ad57b81e21fc6d41aed554
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (33980886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12e019131fc52eab8cb173b369886c8d17e0c0e45f64271e60e0034e7d1c9164`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 22 Jul 2021 00:09:45 GMT
ADD file:1f77b9001c4977ba733be674fc5eb4b85130f1dea8a7b39d545b70f9c107695f in / 
# Thu, 22 Jul 2021 00:09:46 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:07:49 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 22 Jul 2021 01:18:18 GMT
ENV HAPROXY_VERSION=2.0.23
# Thu, 22 Jul 2021 01:18:18 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.23.tar.gz
# Thu, 22 Jul 2021 01:18:18 GMT
ENV HAPROXY_SHA256=5ddc04e9040a07c647fa4b68fc9da6ec36063d56e12824b356e770dcf677c87a
# Thu, 22 Jul 2021 01:20:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 22 Jul 2021 01:20:27 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 01:20:28 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 01:20:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Jul 2021 01:20:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 01:20:30 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:99ee621d0b0485e9de65aa19604aa2453d19ea7fc86b22c5b77c1bab74e3cb42`  
		Last Modified: Thu, 22 Jul 2021 00:16:11 GMT  
		Size: 25.8 MB (25812771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f444627794f98947a9df95ec5d19b2a1cd6c151ed438982b1dc0b89f5eaf19e`  
		Last Modified: Thu, 22 Jul 2021 01:24:39 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f3fbdf3d24084b506b77df980ed801fd6591161d93020ae86b0ac1a61ef51f0`  
		Last Modified: Thu, 22 Jul 2021 01:25:57 GMT  
		Size: 8.2 MB (8166166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99bf2632263ce35635f645c39391e1e69eeaf0060511034d7208473afae08e46`  
		Last Modified: Thu, 22 Jul 2021 01:25:51 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ddaa89cefd98b83df09b7ba1939792e7086ab48488f57c5a10f6f36623034a2`  
		Last Modified: Thu, 22 Jul 2021 01:25:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0` - linux; ppc64le

```console
$ docker pull haproxy@sha256:4f3791fd7a97745942e986039df47ad7253611c3cfcbc2058e985a9dfc488683
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39530637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d25faf283d1d4f4d134d17d01081d2e0962225dc772f73e1f131d8521afa03ff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 22 Jul 2021 00:19:04 GMT
ADD file:3a6bd6ce3eff98b88a13de5d0f26cff0b026f876674204dbad6f84fafcf145b1 in / 
# Thu, 22 Jul 2021 00:19:13 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 02:52:46 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 22 Jul 2021 03:19:53 GMT
ENV HAPROXY_VERSION=2.0.23
# Thu, 22 Jul 2021 03:20:00 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.23.tar.gz
# Thu, 22 Jul 2021 03:20:02 GMT
ENV HAPROXY_SHA256=5ddc04e9040a07c647fa4b68fc9da6ec36063d56e12824b356e770dcf677c87a
# Thu, 22 Jul 2021 03:24:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 22 Jul 2021 03:24:19 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 03:24:22 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 03:24:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Jul 2021 03:24:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 03:24:42 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:1130517d52da84a09f9465006bddab5e49afd398860890eab6274fd0bff32371`  
		Last Modified: Thu, 22 Jul 2021 00:27:49 GMT  
		Size: 30.6 MB (30553709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251bf3fe1d4bbe9c27e393cd8ddc550b56cec90eb916bf9bec24d657c9f6556f`  
		Last Modified: Thu, 22 Jul 2021 03:40:01 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c55c238bc1907043b37b9d8cb6291f274fa835260ca9cac932d3d874bd8b7b0`  
		Last Modified: Thu, 22 Jul 2021 03:42:07 GMT  
		Size: 9.0 MB (8974978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbde6ae5ee13fdc489d2f1bd57efb16e74502018edf256b8a96701350bcc3a66`  
		Last Modified: Thu, 22 Jul 2021 03:42:06 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:954fbe9c0656b0b9294f95c8c9b345dd787fecfcb7c68c95c7ea6d954450cb37`  
		Last Modified: Thu, 22 Jul 2021 03:42:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0` - linux; s390x

```console
$ docker pull haproxy@sha256:916e33a3d363209003f80014e34e500d5c59578f595c3a341cab79ecb8c42619
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (34024632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98a02cae6f0544ced632fbd992d3b5c4c2d70b26efa9ef284a8fff5136b3fc53`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 22 Jul 2021 00:42:45 GMT
ADD file:1ab999eb6f80d8ce91ce3a173e23fd2710f2779117bba29037eaa82aadcbf6ed in / 
# Thu, 22 Jul 2021 00:42:48 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:30:19 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 22 Jul 2021 01:35:55 GMT
ENV HAPROXY_VERSION=2.0.23
# Thu, 22 Jul 2021 01:35:55 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.23.tar.gz
# Thu, 22 Jul 2021 01:35:56 GMT
ENV HAPROXY_SHA256=5ddc04e9040a07c647fa4b68fc9da6ec36063d56e12824b356e770dcf677c87a
# Thu, 22 Jul 2021 01:36:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 22 Jul 2021 01:36:36 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 01:36:37 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 01:36:38 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Jul 2021 01:36:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 01:36:38 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:7a50fdd85ff244c1465e71c51354d055e3df0b90ff5faad28cc22d9ecde9daf3`  
		Last Modified: Thu, 22 Jul 2021 00:48:13 GMT  
		Size: 25.8 MB (25760761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05fb34d1ed21b67502665114a7ae60445472fc7bafa620bbf6c79b7df85a01d4`  
		Last Modified: Thu, 22 Jul 2021 01:39:54 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bab0b3e4d539350140e6dd3ea43e7cef0280ff75d00866201b6634ccf26c698e`  
		Last Modified: Thu, 22 Jul 2021 01:40:39 GMT  
		Size: 8.3 MB (8261922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb12d95dcae6f2a60a850c017c8df27d6cb67de4a641154af2d805c9730ee2ca`  
		Last Modified: Thu, 22 Jul 2021 01:40:38 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f9933e89a89dc17bd9122153d663c16017e600e89b9335e33d7ec68048fe189`  
		Last Modified: Thu, 22 Jul 2021 01:40:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.0-alpine`

```console
$ docker pull haproxy@sha256:52f641d108564795e68eccbe825d643cbbb7bb80852c6cbfdc3de292c7dfe6c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `haproxy:2.0-alpine` - linux; amd64

```console
$ docker pull haproxy@sha256:657d634a900142d3a96c90bccbb68bf1ee0d5069d9de3ede94441fe3ee7b1446
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8670230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7215f9d9dac129b8f0c78a04814c97f31872ab1daa5759035503900699d5cc73`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 02:48:50 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 16 Jul 2021 20:23:01 GMT
ENV HAPROXY_VERSION=2.0.23
# Fri, 16 Jul 2021 20:23:01 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.23.tar.gz
# Fri, 16 Jul 2021 20:23:01 GMT
ENV HAPROXY_SHA256=5ddc04e9040a07c647fa4b68fc9da6ec36063d56e12824b356e770dcf677c87a
# Fri, 16 Jul 2021 20:23:54 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 16 Jul 2021 20:23:55 GMT
STOPSIGNAL SIGUSR1
# Fri, 16 Jul 2021 20:23:55 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 16 Jul 2021 20:23:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 16 Jul 2021 20:23:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jul 2021 20:23:56 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7834d945b9e597e693f56fb0f9847718c1732b738a2f4956ab2c1b66c289d90`  
		Last Modified: Sat, 26 Jun 2021 02:56:43 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf810fd8955797371ff4970318e4052e9909d569596a1ff0a105d243c48b88da`  
		Last Modified: Fri, 16 Jul 2021 20:25:25 GMT  
		Size: 5.9 MB (5856986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73eecfee78d7d1e2487332b5a2ce41103f0d341f85212cc9846964e4ccf8742d`  
		Last Modified: Fri, 16 Jul 2021 20:25:24 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d0c6db4f430ca2862389ecdb9f7284085b7d6ac045c94b30f1a33e81e591a63`  
		Last Modified: Fri, 16 Jul 2021 20:25:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0-alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:13057810b2adfa48c3f605260c004b456dc99cecccefefcd9500d03c98ddb505
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8327525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46f6b2b809d02bf3208c1d92f4389ec4b3e4ce054da8aed4ad9871e3163902d9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:26 GMT
ADD file:c80bc2b093cbc0fc466582ef21cbed377de9fa874aedbf320079525ddacd1200 in / 
# Tue, 15 Jun 2021 22:57:26 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 02:02:51 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 16 Jul 2021 19:52:33 GMT
ENV HAPROXY_VERSION=2.0.23
# Fri, 16 Jul 2021 19:52:33 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.23.tar.gz
# Fri, 16 Jul 2021 19:52:33 GMT
ENV HAPROXY_SHA256=5ddc04e9040a07c647fa4b68fc9da6ec36063d56e12824b356e770dcf677c87a
# Fri, 16 Jul 2021 19:52:56 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 16 Jul 2021 19:52:57 GMT
STOPSIGNAL SIGUSR1
# Fri, 16 Jul 2021 19:52:57 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 16 Jul 2021 19:52:59 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 16 Jul 2021 19:52:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jul 2021 19:53:00 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:b4c9a0924271af3466de27804af26420eb58da1466e7eaaba127d178b380fea3`  
		Last Modified: Tue, 15 Jun 2021 22:58:47 GMT  
		Size: 2.6 MB (2624382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85fa2947d9cc2655af4fd4aa21641629e791bcaf309a7095db77d309ddd05dfa`  
		Last Modified: Sat, 26 Jun 2021 02:08:45 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9756c72b35754f6a91e5f930a9d42bb57863c3ed5c753ab23a197c3f7de2a667`  
		Last Modified: Fri, 16 Jul 2021 19:55:05 GMT  
		Size: 5.7 MB (5701377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2992efc609d9957220262aec7662fbaa3207913556ad6c2a70a34521f172f9f`  
		Last Modified: Fri, 16 Jul 2021 19:55:02 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dcc04e669898be9be46cb1aa718ac715c114ad288d15c344d0208af3a4b26b5`  
		Last Modified: Fri, 16 Jul 2021 19:55:02 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:4027076637468b8e8412e5b3eaea7c08e177ec7c704ca362de863199b729e040
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8108123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad0d25c1c58b9ab434d7c216f535a5901591bfff7e4de3938f31c806b98a18fd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:05 GMT
ADD file:416a8b507abdc6bdcb22997a4be0a4170796c3f9f77e315b2dbff2b0a212bc68 in / 
# Tue, 15 Jun 2021 23:15:06 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 05:27:42 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 16 Jul 2021 20:39:11 GMT
ENV HAPROXY_VERSION=2.0.23
# Fri, 16 Jul 2021 20:39:11 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.23.tar.gz
# Fri, 16 Jul 2021 20:39:12 GMT
ENV HAPROXY_SHA256=5ddc04e9040a07c647fa4b68fc9da6ec36063d56e12824b356e770dcf677c87a
# Fri, 16 Jul 2021 20:39:33 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 16 Jul 2021 20:39:34 GMT
STOPSIGNAL SIGUSR1
# Fri, 16 Jul 2021 20:39:34 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 16 Jul 2021 20:39:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 16 Jul 2021 20:39:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jul 2021 20:39:37 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:136482bf81d1fa351b424ebb8c7e34d15f2c5ed3fc0b66b544b8312bda3d52d9`  
		Last Modified: Tue, 15 Jun 2021 23:16:40 GMT  
		Size: 2.4 MB (2427917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5464af225bd487370319e7125fb2769222c5c7371d1be737936169d2e5b01c`  
		Last Modified: Sat, 26 Jun 2021 05:35:56 GMT  
		Size: 1.2 KB (1196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c492ba23364ced5d240104278dc33640247764256605ff8f1b547099a187dcc`  
		Last Modified: Fri, 16 Jul 2021 20:43:53 GMT  
		Size: 5.7 MB (5678440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e32e313e881b9a57a54a5fdb9c0003ce9f18ce93c6fcc4c301afc8d82f891ef7`  
		Last Modified: Fri, 16 Jul 2021 20:43:50 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c355fced946247b83b3d173c997dc1f5de85918ed61785fb3de4102a8d1158b`  
		Last Modified: Fri, 16 Jul 2021 20:43:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:68fcca71ebfc1caa49f7a51bbb49863d85511a0af6e15635bbf13fa136b95cb7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8565065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52ea6d4fcb48cc14cada74f76e1732a8f44bae8dc2f50c6486acabc57cc627de`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 21:44:56 GMT
ADD file:6797caacbfe41bfe44000b39ed017016c6fcc492b3d6557cdaba88536df6c876 in / 
# Tue, 15 Jun 2021 21:44:56 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 02:13:15 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 16 Jul 2021 19:42:49 GMT
ENV HAPROXY_VERSION=2.0.23
# Fri, 16 Jul 2021 19:42:49 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.23.tar.gz
# Fri, 16 Jul 2021 19:42:49 GMT
ENV HAPROXY_SHA256=5ddc04e9040a07c647fa4b68fc9da6ec36063d56e12824b356e770dcf677c87a
# Fri, 16 Jul 2021 19:43:31 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 16 Jul 2021 19:43:31 GMT
STOPSIGNAL SIGUSR1
# Fri, 16 Jul 2021 19:43:32 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 16 Jul 2021 19:43:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 16 Jul 2021 19:43:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jul 2021 19:43:33 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:58ab47519297212468320b23b8100fc1b2b96e8d342040806ae509a778a0a07a`  
		Last Modified: Tue, 15 Jun 2021 21:46:03 GMT  
		Size: 2.7 MB (2709626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb8dc96e2a4b7f90ae2dbfca981fe199966b64e3426ca1f742499d46ad1aa357`  
		Last Modified: Sat, 26 Jun 2021 02:21:19 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8c3184374687ff476a2df3cb0a583c7cdf8b474d986b52f6946494cc09d0ec`  
		Last Modified: Fri, 16 Jul 2021 19:45:56 GMT  
		Size: 5.9 MB (5853671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0876de74f4d496ea89b2dd94ab42ac10a89c126a7ae41afdcb95663aa770cb84`  
		Last Modified: Fri, 16 Jul 2021 19:45:55 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1522372a935e1c998f7f3a339befd16649484ce1e3b7c4ce73c9adb76c05b8a`  
		Last Modified: Fri, 16 Jul 2021 19:45:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0-alpine` - linux; 386

```console
$ docker pull haproxy@sha256:ea37cb563ee1ddfb904d4f87b9389f975b601cd52f584360e300b25c93347035
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.5 MB (8530862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:727c3bb8573eb3227f79b2217f013f902249c59106f6998d491880e706139bcc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 21:38:30 GMT
ADD file:3b0fe1454491bb05e218b090fd461f2fd39546aa4a53eb3f953ee8eae149ac57 in / 
# Tue, 15 Jun 2021 21:38:30 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 01:39:05 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 16 Jul 2021 19:43:03 GMT
ENV HAPROXY_VERSION=2.0.23
# Fri, 16 Jul 2021 19:43:03 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.23.tar.gz
# Fri, 16 Jul 2021 19:43:03 GMT
ENV HAPROXY_SHA256=5ddc04e9040a07c647fa4b68fc9da6ec36063d56e12824b356e770dcf677c87a
# Fri, 16 Jul 2021 19:44:01 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 16 Jul 2021 19:44:01 GMT
STOPSIGNAL SIGUSR1
# Fri, 16 Jul 2021 19:44:01 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 16 Jul 2021 19:44:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 16 Jul 2021 19:44:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jul 2021 19:44:02 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:be21df321efb39c5daf3151073ebff7688e15ea6cd5158878bc9559a5db76ac6`  
		Last Modified: Tue, 15 Jun 2021 21:39:16 GMT  
		Size: 2.8 MB (2820718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc6fe536c8e50a97873c166db7d3b669842dec91d85ce73433028b3b198a1c4`  
		Last Modified: Sat, 26 Jun 2021 01:49:46 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b9dd4148547520495a2a60126d6c014a51405e99a34774a7ef989e1e3cb425`  
		Last Modified: Fri, 16 Jul 2021 19:46:32 GMT  
		Size: 5.7 MB (5708379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f673c2889d2a2ff0b3e7700c1737b7b5ef99db9a98ba63e0bf25b515842613e`  
		Last Modified: Fri, 16 Jul 2021 19:46:31 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7fbd961173b99ad9352281a5d38a477c40487328a5577afba22cf6653b4bcad`  
		Last Modified: Fri, 16 Jul 2021 19:46:31 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0-alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:1ddeb53e4407134e03b90f17a12d723d79f4ca3cf90a87ee780135a1eaca952c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.9 MB (8876305 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec7952d62ab78b1304020f3ed42b4e24eb7ee4bb049cf83494e87b39f7319e4c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:27:00 GMT
ADD file:0075aad7a94f0496483442bb2d9fdaa13e9c23087b90638d014b4bc263aa3861 in / 
# Tue, 15 Jun 2021 22:27:03 GMT
CMD ["/bin/sh"]
# Fri, 16 Jul 2021 20:17:57 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 16 Jul 2021 20:33:51 GMT
ENV HAPROXY_VERSION=2.0.23
# Fri, 16 Jul 2021 20:34:00 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.23.tar.gz
# Fri, 16 Jul 2021 20:34:07 GMT
ENV HAPROXY_SHA256=5ddc04e9040a07c647fa4b68fc9da6ec36063d56e12824b356e770dcf677c87a
# Thu, 22 Jul 2021 03:25:45 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 22 Jul 2021 03:25:47 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 03:25:51 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 03:26:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Jul 2021 03:26:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 03:26:10 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:baf144cfb66ebe9df1969f3b90f1c448beff98edc84de1ccb5d6346195a070d4`  
		Last Modified: Tue, 15 Jun 2021 22:27:38 GMT  
		Size: 2.8 MB (2810478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e907663c9428bbbb731a221721c606bad29e54dac6f0dda85d6aa3175a725e`  
		Last Modified: Thu, 22 Jul 2021 03:40:16 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58c65248e94b1a16d74ea6c2e8f9e9fb0200b29496d3f629fceb9d16c3b8aa70`  
		Last Modified: Thu, 22 Jul 2021 03:42:20 GMT  
		Size: 6.1 MB (6064058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0107d6abeeaed80b469419a01bd3f90ac390d59d41b97fba3c729b47121912b6`  
		Last Modified: Thu, 22 Jul 2021 03:42:18 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20bf1a2eda94523ba1152a2692ab73cdbb1e962a05178ed92ccacaac57a1b86`  
		Last Modified: Thu, 22 Jul 2021 03:42:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0-alpine` - linux; s390x

```console
$ docker pull haproxy@sha256:293442e60508fc935ff391348a5996d64d6eeda811861ef39184f61e5b817aed
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.4 MB (8381609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e1c50e6367e0814cb0b7d2a9f4ce26225facb71c39faa887f22019cf419cfa4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:54:24 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 20:56:58 GMT
ENV HAPROXY_VERSION=2.0.22
# Wed, 14 Apr 2021 20:56:58 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.22.tar.gz
# Wed, 14 Apr 2021 20:56:58 GMT
ENV HAPROXY_SHA256=5e1dccf30a3ad782d1e3298cc4e4955b168e4aa06cad4e3ea1c0334cdc0f966d
# Wed, 14 Apr 2021 20:57:33 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 20:57:33 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 20:57:33 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:57:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 20:57:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:57:35 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267275aba58470c82626189a59be76cd169bd245568e2f2545ed1ee64ff8a8ff`  
		Last Modified: Wed, 14 Apr 2021 20:59:06 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5baa4dad803c789741ebc1f7cb61771b5c89417dcac880e1dc0f0eddb342ded`  
		Last Modified: Wed, 14 Apr 2021 20:59:38 GMT  
		Size: 5.8 MB (5777204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b272d803c3aad18ee76c50db0627de49c115d046c0acafc910571f0ea8e08578`  
		Last Modified: Wed, 14 Apr 2021 20:59:37 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c1eb67bc4c1cfcab424bfc0385b8c9c97507568646d815a5511c42c82b4250a`  
		Last Modified: Wed, 14 Apr 2021 20:59:37 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.0.23`

```console
$ docker pull haproxy@sha256:138702b49465b4c9888f54a809d22331230b9dbcaf0627d0423a702c3cf9760c
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

### `haproxy:2.0.23` - linux; amd64

```console
$ docker pull haproxy@sha256:e23a2254dbea4fce44679c7017a8b2d09f08665c6fc21b0c81d08e86c4cbcb5f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.8 MB (35809252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04015a55056dc92dcbe712fa83cbb1b5d6c99ceb07b6b8dccc82cf445db0d268`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 06:19:17 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 16 Jul 2021 20:22:01 GMT
ENV HAPROXY_VERSION=2.0.23
# Fri, 16 Jul 2021 20:22:01 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.23.tar.gz
# Fri, 16 Jul 2021 20:22:01 GMT
ENV HAPROXY_SHA256=5ddc04e9040a07c647fa4b68fc9da6ec36063d56e12824b356e770dcf677c87a
# Fri, 16 Jul 2021 20:22:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 16 Jul 2021 20:22:54 GMT
STOPSIGNAL SIGUSR1
# Fri, 16 Jul 2021 20:22:55 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 16 Jul 2021 20:22:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 16 Jul 2021 20:22:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jul 2021 20:22:56 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91332cb81883405a321c1a2d2144bdd0aef8d1c69f90fdf0cf219982161b6e6e`  
		Last Modified: Wed, 23 Jun 2021 06:29:07 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a3a75bd4f980d88055f8d6dc5e659eae8aa1d65d1cf09499c3ea3f6dfd0c4f`  
		Last Modified: Fri, 16 Jul 2021 20:25:14 GMT  
		Size: 8.7 MB (8661448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4c86e186785e009b76f53d8371fde694020334f0c7fcee94d2c621f2d80bc6b`  
		Last Modified: Fri, 16 Jul 2021 20:25:12 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715c25c22c1e52db6636c84e959e8dda5d6b95fd721cb4a8e003db69770b10bb`  
		Last Modified: Fri, 16 Jul 2021 20:25:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0.23` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:1ea758cc14b6f3dfe45650e197d8df22ae573ab3c41e56c3cd122716402b804d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.1 MB (33069410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f93df7025ee4e7be230bf75b5e4e30836f420519916695321a5344c3641023e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 22 Jun 2021 23:50:09 GMT
ADD file:78d4ced31112d85490c684f350aceeebfc72a804262c7ad3e033257e3894f5c4 in / 
# Tue, 22 Jun 2021 23:50:11 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:15:11 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 16 Jul 2021 19:50:26 GMT
ENV HAPROXY_VERSION=2.0.23
# Fri, 16 Jul 2021 19:50:26 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.23.tar.gz
# Fri, 16 Jul 2021 19:50:27 GMT
ENV HAPROXY_SHA256=5ddc04e9040a07c647fa4b68fc9da6ec36063d56e12824b356e770dcf677c87a
# Fri, 16 Jul 2021 19:51:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 16 Jul 2021 19:51:16 GMT
STOPSIGNAL SIGUSR1
# Fri, 16 Jul 2021 19:51:17 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 16 Jul 2021 19:51:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 16 Jul 2021 19:51:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jul 2021 19:51:19 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:532d6df30af5174ac6e1b379c32b8f464d44651ac060376a560c4a76a87704a7`  
		Last Modified: Wed, 23 Jun 2021 00:01:46 GMT  
		Size: 24.9 MB (24878945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48649e3d7de4cd80d3a9a34c725a2935be904ff90e99ea6c8e4bb6e1e7a4eeb7`  
		Last Modified: Wed, 23 Jun 2021 05:24:11 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de179a73ab38812fe744f4984790e412ec57ce2acce04638ffa2a41ed258e0c3`  
		Last Modified: Fri, 16 Jul 2021 19:53:32 GMT  
		Size: 8.2 MB (8188519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eed6b8b10dcb7503a4037f31b3e3c20dbe705c3c2655f9161805cf08db301f3`  
		Last Modified: Fri, 16 Jul 2021 19:53:27 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c8fa2481a0e1635ffa5e396654295801b17a6d6a5be125ff3334ce358731ac5`  
		Last Modified: Fri, 16 Jul 2021 19:53:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0.23` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:c1040c9ac9c6cd38d8b5e76a57da4913ddf903bf9716f948391413cf12e7319a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.9 MB (30861541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b04744c0c97785732765b8c9a92ca8b89b83d9a69478e097b9e3c706fdf1ba2d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:31 GMT
ADD file:8d200a3bbe985ff355343675c5555852f27550a9e367969df6bc98034efb8fd4 in / 
# Wed, 23 Jun 2021 00:20:31 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:21:41 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 16 Jul 2021 20:38:05 GMT
ENV HAPROXY_VERSION=2.0.23
# Fri, 16 Jul 2021 20:38:05 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.23.tar.gz
# Fri, 16 Jul 2021 20:38:06 GMT
ENV HAPROXY_SHA256=5ddc04e9040a07c647fa4b68fc9da6ec36063d56e12824b356e770dcf677c87a
# Fri, 16 Jul 2021 20:38:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 16 Jul 2021 20:38:51 GMT
STOPSIGNAL SIGUSR1
# Fri, 16 Jul 2021 20:38:52 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 16 Jul 2021 20:38:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 16 Jul 2021 20:38:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jul 2021 20:38:54 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:8452be1adf00f91570fe21a8e61aaf4c12e014daf67d7de65d984f4e8ecca2f1`  
		Last Modified: Wed, 23 Jun 2021 00:31:49 GMT  
		Size: 22.7 MB (22746055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed1c9c92d0076fd4bf40503e3f47102509a5b99d182f4dd9e81e64d0a7e0b8a`  
		Last Modified: Wed, 23 Jun 2021 05:35:48 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a4707ad32ba231e4366e36f1a859edd24952c7e77c200d1737dbe917e32a670`  
		Last Modified: Fri, 16 Jul 2021 20:43:38 GMT  
		Size: 8.1 MB (8113539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aeb934403d774d328050209d2fa7157e7cd0f483fe1ddfaf86630910df0718c`  
		Last Modified: Fri, 16 Jul 2021 20:43:33 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9cec3dc0c28d8cbdb7b25acd084e80b1f1c70c80685d1e921d943171897f959`  
		Last Modified: Fri, 16 Jul 2021 20:43:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0.23` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:92a27f5848362f34e6b4074caa860fddce95d22fe63bc9e32ce5c79345d4eb12
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.4 MB (34439104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3aa1e7b28a2822eccb53903de5dce966be08997b4d8c562d7a2c70e1cbd04fb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:40 GMT
ADD file:beee00b59da720f68e12e2ba2a8134207c80c777ddb4ceb03c71e3e4c3f51c93 in / 
# Tue, 22 Jun 2021 23:49:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 03:19:31 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 16 Jul 2021 19:42:05 GMT
ENV HAPROXY_VERSION=2.0.23
# Fri, 16 Jul 2021 19:42:05 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.23.tar.gz
# Fri, 16 Jul 2021 19:42:05 GMT
ENV HAPROXY_SHA256=5ddc04e9040a07c647fa4b68fc9da6ec36063d56e12824b356e770dcf677c87a
# Fri, 16 Jul 2021 19:42:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 16 Jul 2021 19:42:40 GMT
STOPSIGNAL SIGUSR1
# Fri, 16 Jul 2021 19:42:41 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 16 Jul 2021 19:42:42 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 16 Jul 2021 19:42:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jul 2021 19:42:42 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:448f6bf000e31217a7c202c659b03b7f8ac8d3ae6b03ef7a2f8339be2f00ff4a`  
		Last Modified: Tue, 22 Jun 2021 23:55:25 GMT  
		Size: 25.9 MB (25914993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b05ad81dc8a7d67656235988f0e5fb72c374c7d8df44c105b91d712e06c4ac`  
		Last Modified: Wed, 23 Jun 2021 03:26:16 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27571973ed676b6b80333392ed3bff443d02940d7391eb5305a2ca15aa7f7171`  
		Last Modified: Fri, 16 Jul 2021 19:45:44 GMT  
		Size: 8.5 MB (8522161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b9e3742d5e38bce45625e755934c9c25c143447d6b53c253b2519619918435`  
		Last Modified: Fri, 16 Jul 2021 19:45:42 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d3a947db69556f61b2d10db26e579d74665e585ea7d17d73b1a612b3542aa8`  
		Last Modified: Fri, 16 Jul 2021 19:45:42 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0.23` - linux; 386

```console
$ docker pull haproxy@sha256:95e4d43371492ccc71318f3bbf365ad878b3f9996bdda95045e573fd255734a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36299325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2de994a6f5c25434fea01095e252592edac58522cda4982717fd89566cc61946`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 22 Jun 2021 23:39:35 GMT
ADD file:48f656ac6733911048b3de850490438d0233b3badc11861fca62062d4edfaf40 in / 
# Tue, 22 Jun 2021 23:39:35 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:23:13 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 16 Jul 2021 19:42:02 GMT
ENV HAPROXY_VERSION=2.0.23
# Fri, 16 Jul 2021 19:42:02 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.23.tar.gz
# Fri, 16 Jul 2021 19:42:02 GMT
ENV HAPROXY_SHA256=5ddc04e9040a07c647fa4b68fc9da6ec36063d56e12824b356e770dcf677c87a
# Fri, 16 Jul 2021 19:42:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 16 Jul 2021 19:42:51 GMT
STOPSIGNAL SIGUSR1
# Fri, 16 Jul 2021 19:42:51 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 16 Jul 2021 19:42:52 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 16 Jul 2021 19:42:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jul 2021 19:42:52 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:33af2dcb865e65d53cdeb843b67a0ef62151fa32df292293e7c6b0eb728ac5ac`  
		Last Modified: Tue, 22 Jun 2021 23:46:23 GMT  
		Size: 27.8 MB (27797411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a6e4d42b23996eb7d8a1baa85ee19828c2667fd4a2dca6eb1040b266680e9f`  
		Last Modified: Wed, 23 Jun 2021 00:32:00 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c10787c75f23a36f58130786923d1b9c7d2be2b9c2f0c1a29441585915839f`  
		Last Modified: Fri, 16 Jul 2021 19:46:20 GMT  
		Size: 8.5 MB (8499965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d89c48ad14be00161088c14311a315bd124c1827a6fd335ae59c01a6c50169`  
		Last Modified: Fri, 16 Jul 2021 19:46:18 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79347bc64811a94a1f9ab15200d7e967f6a6c727baa14e067be5327432664a4f`  
		Last Modified: Fri, 16 Jul 2021 19:46:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0.23` - linux; mips64le

```console
$ docker pull haproxy@sha256:a7e464070f23af3cebfb2f0c59a05afbd6fc188899ad57b81e21fc6d41aed554
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (33980886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12e019131fc52eab8cb173b369886c8d17e0c0e45f64271e60e0034e7d1c9164`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 22 Jul 2021 00:09:45 GMT
ADD file:1f77b9001c4977ba733be674fc5eb4b85130f1dea8a7b39d545b70f9c107695f in / 
# Thu, 22 Jul 2021 00:09:46 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:07:49 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 22 Jul 2021 01:18:18 GMT
ENV HAPROXY_VERSION=2.0.23
# Thu, 22 Jul 2021 01:18:18 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.23.tar.gz
# Thu, 22 Jul 2021 01:18:18 GMT
ENV HAPROXY_SHA256=5ddc04e9040a07c647fa4b68fc9da6ec36063d56e12824b356e770dcf677c87a
# Thu, 22 Jul 2021 01:20:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 22 Jul 2021 01:20:27 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 01:20:28 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 01:20:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Jul 2021 01:20:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 01:20:30 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:99ee621d0b0485e9de65aa19604aa2453d19ea7fc86b22c5b77c1bab74e3cb42`  
		Last Modified: Thu, 22 Jul 2021 00:16:11 GMT  
		Size: 25.8 MB (25812771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f444627794f98947a9df95ec5d19b2a1cd6c151ed438982b1dc0b89f5eaf19e`  
		Last Modified: Thu, 22 Jul 2021 01:24:39 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f3fbdf3d24084b506b77df980ed801fd6591161d93020ae86b0ac1a61ef51f0`  
		Last Modified: Thu, 22 Jul 2021 01:25:57 GMT  
		Size: 8.2 MB (8166166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99bf2632263ce35635f645c39391e1e69eeaf0060511034d7208473afae08e46`  
		Last Modified: Thu, 22 Jul 2021 01:25:51 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ddaa89cefd98b83df09b7ba1939792e7086ab48488f57c5a10f6f36623034a2`  
		Last Modified: Thu, 22 Jul 2021 01:25:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0.23` - linux; ppc64le

```console
$ docker pull haproxy@sha256:4f3791fd7a97745942e986039df47ad7253611c3cfcbc2058e985a9dfc488683
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39530637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d25faf283d1d4f4d134d17d01081d2e0962225dc772f73e1f131d8521afa03ff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 22 Jul 2021 00:19:04 GMT
ADD file:3a6bd6ce3eff98b88a13de5d0f26cff0b026f876674204dbad6f84fafcf145b1 in / 
# Thu, 22 Jul 2021 00:19:13 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 02:52:46 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 22 Jul 2021 03:19:53 GMT
ENV HAPROXY_VERSION=2.0.23
# Thu, 22 Jul 2021 03:20:00 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.23.tar.gz
# Thu, 22 Jul 2021 03:20:02 GMT
ENV HAPROXY_SHA256=5ddc04e9040a07c647fa4b68fc9da6ec36063d56e12824b356e770dcf677c87a
# Thu, 22 Jul 2021 03:24:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 22 Jul 2021 03:24:19 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 03:24:22 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 03:24:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Jul 2021 03:24:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 03:24:42 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:1130517d52da84a09f9465006bddab5e49afd398860890eab6274fd0bff32371`  
		Last Modified: Thu, 22 Jul 2021 00:27:49 GMT  
		Size: 30.6 MB (30553709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251bf3fe1d4bbe9c27e393cd8ddc550b56cec90eb916bf9bec24d657c9f6556f`  
		Last Modified: Thu, 22 Jul 2021 03:40:01 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c55c238bc1907043b37b9d8cb6291f274fa835260ca9cac932d3d874bd8b7b0`  
		Last Modified: Thu, 22 Jul 2021 03:42:07 GMT  
		Size: 9.0 MB (8974978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbde6ae5ee13fdc489d2f1bd57efb16e74502018edf256b8a96701350bcc3a66`  
		Last Modified: Thu, 22 Jul 2021 03:42:06 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:954fbe9c0656b0b9294f95c8c9b345dd787fecfcb7c68c95c7ea6d954450cb37`  
		Last Modified: Thu, 22 Jul 2021 03:42:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0.23` - linux; s390x

```console
$ docker pull haproxy@sha256:916e33a3d363209003f80014e34e500d5c59578f595c3a341cab79ecb8c42619
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (34024632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98a02cae6f0544ced632fbd992d3b5c4c2d70b26efa9ef284a8fff5136b3fc53`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 22 Jul 2021 00:42:45 GMT
ADD file:1ab999eb6f80d8ce91ce3a173e23fd2710f2779117bba29037eaa82aadcbf6ed in / 
# Thu, 22 Jul 2021 00:42:48 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:30:19 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 22 Jul 2021 01:35:55 GMT
ENV HAPROXY_VERSION=2.0.23
# Thu, 22 Jul 2021 01:35:55 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.23.tar.gz
# Thu, 22 Jul 2021 01:35:56 GMT
ENV HAPROXY_SHA256=5ddc04e9040a07c647fa4b68fc9da6ec36063d56e12824b356e770dcf677c87a
# Thu, 22 Jul 2021 01:36:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 22 Jul 2021 01:36:36 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 01:36:37 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 01:36:38 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Jul 2021 01:36:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 01:36:38 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:7a50fdd85ff244c1465e71c51354d055e3df0b90ff5faad28cc22d9ecde9daf3`  
		Last Modified: Thu, 22 Jul 2021 00:48:13 GMT  
		Size: 25.8 MB (25760761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05fb34d1ed21b67502665114a7ae60445472fc7bafa620bbf6c79b7df85a01d4`  
		Last Modified: Thu, 22 Jul 2021 01:39:54 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bab0b3e4d539350140e6dd3ea43e7cef0280ff75d00866201b6634ccf26c698e`  
		Last Modified: Thu, 22 Jul 2021 01:40:39 GMT  
		Size: 8.3 MB (8261922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb12d95dcae6f2a60a850c017c8df27d6cb67de4a641154af2d805c9730ee2ca`  
		Last Modified: Thu, 22 Jul 2021 01:40:38 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f9933e89a89dc17bd9122153d663c16017e600e89b9335e33d7ec68048fe189`  
		Last Modified: Thu, 22 Jul 2021 01:40:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.0.23-alpine`

```console
$ docker pull haproxy@sha256:e335b39ce4dc8a137cda53b859f817022e9f954c8107534d38b641746de32632
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `haproxy:2.0.23-alpine` - linux; amd64

```console
$ docker pull haproxy@sha256:657d634a900142d3a96c90bccbb68bf1ee0d5069d9de3ede94441fe3ee7b1446
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8670230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7215f9d9dac129b8f0c78a04814c97f31872ab1daa5759035503900699d5cc73`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 02:48:50 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 16 Jul 2021 20:23:01 GMT
ENV HAPROXY_VERSION=2.0.23
# Fri, 16 Jul 2021 20:23:01 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.23.tar.gz
# Fri, 16 Jul 2021 20:23:01 GMT
ENV HAPROXY_SHA256=5ddc04e9040a07c647fa4b68fc9da6ec36063d56e12824b356e770dcf677c87a
# Fri, 16 Jul 2021 20:23:54 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 16 Jul 2021 20:23:55 GMT
STOPSIGNAL SIGUSR1
# Fri, 16 Jul 2021 20:23:55 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 16 Jul 2021 20:23:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 16 Jul 2021 20:23:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jul 2021 20:23:56 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7834d945b9e597e693f56fb0f9847718c1732b738a2f4956ab2c1b66c289d90`  
		Last Modified: Sat, 26 Jun 2021 02:56:43 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf810fd8955797371ff4970318e4052e9909d569596a1ff0a105d243c48b88da`  
		Last Modified: Fri, 16 Jul 2021 20:25:25 GMT  
		Size: 5.9 MB (5856986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73eecfee78d7d1e2487332b5a2ce41103f0d341f85212cc9846964e4ccf8742d`  
		Last Modified: Fri, 16 Jul 2021 20:25:24 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d0c6db4f430ca2862389ecdb9f7284085b7d6ac045c94b30f1a33e81e591a63`  
		Last Modified: Fri, 16 Jul 2021 20:25:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0.23-alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:13057810b2adfa48c3f605260c004b456dc99cecccefefcd9500d03c98ddb505
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8327525 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46f6b2b809d02bf3208c1d92f4389ec4b3e4ce054da8aed4ad9871e3163902d9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:26 GMT
ADD file:c80bc2b093cbc0fc466582ef21cbed377de9fa874aedbf320079525ddacd1200 in / 
# Tue, 15 Jun 2021 22:57:26 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 02:02:51 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 16 Jul 2021 19:52:33 GMT
ENV HAPROXY_VERSION=2.0.23
# Fri, 16 Jul 2021 19:52:33 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.23.tar.gz
# Fri, 16 Jul 2021 19:52:33 GMT
ENV HAPROXY_SHA256=5ddc04e9040a07c647fa4b68fc9da6ec36063d56e12824b356e770dcf677c87a
# Fri, 16 Jul 2021 19:52:56 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 16 Jul 2021 19:52:57 GMT
STOPSIGNAL SIGUSR1
# Fri, 16 Jul 2021 19:52:57 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 16 Jul 2021 19:52:59 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 16 Jul 2021 19:52:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jul 2021 19:53:00 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:b4c9a0924271af3466de27804af26420eb58da1466e7eaaba127d178b380fea3`  
		Last Modified: Tue, 15 Jun 2021 22:58:47 GMT  
		Size: 2.6 MB (2624382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85fa2947d9cc2655af4fd4aa21641629e791bcaf309a7095db77d309ddd05dfa`  
		Last Modified: Sat, 26 Jun 2021 02:08:45 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9756c72b35754f6a91e5f930a9d42bb57863c3ed5c753ab23a197c3f7de2a667`  
		Last Modified: Fri, 16 Jul 2021 19:55:05 GMT  
		Size: 5.7 MB (5701377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2992efc609d9957220262aec7662fbaa3207913556ad6c2a70a34521f172f9f`  
		Last Modified: Fri, 16 Jul 2021 19:55:02 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dcc04e669898be9be46cb1aa718ac715c114ad288d15c344d0208af3a4b26b5`  
		Last Modified: Fri, 16 Jul 2021 19:55:02 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0.23-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:4027076637468b8e8412e5b3eaea7c08e177ec7c704ca362de863199b729e040
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8108123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad0d25c1c58b9ab434d7c216f535a5901591bfff7e4de3938f31c806b98a18fd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:05 GMT
ADD file:416a8b507abdc6bdcb22997a4be0a4170796c3f9f77e315b2dbff2b0a212bc68 in / 
# Tue, 15 Jun 2021 23:15:06 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 05:27:42 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 16 Jul 2021 20:39:11 GMT
ENV HAPROXY_VERSION=2.0.23
# Fri, 16 Jul 2021 20:39:11 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.23.tar.gz
# Fri, 16 Jul 2021 20:39:12 GMT
ENV HAPROXY_SHA256=5ddc04e9040a07c647fa4b68fc9da6ec36063d56e12824b356e770dcf677c87a
# Fri, 16 Jul 2021 20:39:33 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 16 Jul 2021 20:39:34 GMT
STOPSIGNAL SIGUSR1
# Fri, 16 Jul 2021 20:39:34 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 16 Jul 2021 20:39:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 16 Jul 2021 20:39:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jul 2021 20:39:37 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:136482bf81d1fa351b424ebb8c7e34d15f2c5ed3fc0b66b544b8312bda3d52d9`  
		Last Modified: Tue, 15 Jun 2021 23:16:40 GMT  
		Size: 2.4 MB (2427917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5464af225bd487370319e7125fb2769222c5c7371d1be737936169d2e5b01c`  
		Last Modified: Sat, 26 Jun 2021 05:35:56 GMT  
		Size: 1.2 KB (1196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c492ba23364ced5d240104278dc33640247764256605ff8f1b547099a187dcc`  
		Last Modified: Fri, 16 Jul 2021 20:43:53 GMT  
		Size: 5.7 MB (5678440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e32e313e881b9a57a54a5fdb9c0003ce9f18ce93c6fcc4c301afc8d82f891ef7`  
		Last Modified: Fri, 16 Jul 2021 20:43:50 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c355fced946247b83b3d173c997dc1f5de85918ed61785fb3de4102a8d1158b`  
		Last Modified: Fri, 16 Jul 2021 20:43:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0.23-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:68fcca71ebfc1caa49f7a51bbb49863d85511a0af6e15635bbf13fa136b95cb7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8565065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52ea6d4fcb48cc14cada74f76e1732a8f44bae8dc2f50c6486acabc57cc627de`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 21:44:56 GMT
ADD file:6797caacbfe41bfe44000b39ed017016c6fcc492b3d6557cdaba88536df6c876 in / 
# Tue, 15 Jun 2021 21:44:56 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 02:13:15 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 16 Jul 2021 19:42:49 GMT
ENV HAPROXY_VERSION=2.0.23
# Fri, 16 Jul 2021 19:42:49 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.23.tar.gz
# Fri, 16 Jul 2021 19:42:49 GMT
ENV HAPROXY_SHA256=5ddc04e9040a07c647fa4b68fc9da6ec36063d56e12824b356e770dcf677c87a
# Fri, 16 Jul 2021 19:43:31 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 16 Jul 2021 19:43:31 GMT
STOPSIGNAL SIGUSR1
# Fri, 16 Jul 2021 19:43:32 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 16 Jul 2021 19:43:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 16 Jul 2021 19:43:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jul 2021 19:43:33 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:58ab47519297212468320b23b8100fc1b2b96e8d342040806ae509a778a0a07a`  
		Last Modified: Tue, 15 Jun 2021 21:46:03 GMT  
		Size: 2.7 MB (2709626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb8dc96e2a4b7f90ae2dbfca981fe199966b64e3426ca1f742499d46ad1aa357`  
		Last Modified: Sat, 26 Jun 2021 02:21:19 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8c3184374687ff476a2df3cb0a583c7cdf8b474d986b52f6946494cc09d0ec`  
		Last Modified: Fri, 16 Jul 2021 19:45:56 GMT  
		Size: 5.9 MB (5853671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0876de74f4d496ea89b2dd94ab42ac10a89c126a7ae41afdcb95663aa770cb84`  
		Last Modified: Fri, 16 Jul 2021 19:45:55 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1522372a935e1c998f7f3a339befd16649484ce1e3b7c4ce73c9adb76c05b8a`  
		Last Modified: Fri, 16 Jul 2021 19:45:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0.23-alpine` - linux; 386

```console
$ docker pull haproxy@sha256:ea37cb563ee1ddfb904d4f87b9389f975b601cd52f584360e300b25c93347035
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.5 MB (8530862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:727c3bb8573eb3227f79b2217f013f902249c59106f6998d491880e706139bcc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 21:38:30 GMT
ADD file:3b0fe1454491bb05e218b090fd461f2fd39546aa4a53eb3f953ee8eae149ac57 in / 
# Tue, 15 Jun 2021 21:38:30 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 01:39:05 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 16 Jul 2021 19:43:03 GMT
ENV HAPROXY_VERSION=2.0.23
# Fri, 16 Jul 2021 19:43:03 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.23.tar.gz
# Fri, 16 Jul 2021 19:43:03 GMT
ENV HAPROXY_SHA256=5ddc04e9040a07c647fa4b68fc9da6ec36063d56e12824b356e770dcf677c87a
# Fri, 16 Jul 2021 19:44:01 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 16 Jul 2021 19:44:01 GMT
STOPSIGNAL SIGUSR1
# Fri, 16 Jul 2021 19:44:01 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 16 Jul 2021 19:44:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 16 Jul 2021 19:44:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jul 2021 19:44:02 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:be21df321efb39c5daf3151073ebff7688e15ea6cd5158878bc9559a5db76ac6`  
		Last Modified: Tue, 15 Jun 2021 21:39:16 GMT  
		Size: 2.8 MB (2820718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc6fe536c8e50a97873c166db7d3b669842dec91d85ce73433028b3b198a1c4`  
		Last Modified: Sat, 26 Jun 2021 01:49:46 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b9dd4148547520495a2a60126d6c014a51405e99a34774a7ef989e1e3cb425`  
		Last Modified: Fri, 16 Jul 2021 19:46:32 GMT  
		Size: 5.7 MB (5708379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f673c2889d2a2ff0b3e7700c1737b7b5ef99db9a98ba63e0bf25b515842613e`  
		Last Modified: Fri, 16 Jul 2021 19:46:31 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7fbd961173b99ad9352281a5d38a477c40487328a5577afba22cf6653b4bcad`  
		Last Modified: Fri, 16 Jul 2021 19:46:31 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0.23-alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:1ddeb53e4407134e03b90f17a12d723d79f4ca3cf90a87ee780135a1eaca952c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.9 MB (8876305 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec7952d62ab78b1304020f3ed42b4e24eb7ee4bb049cf83494e87b39f7319e4c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:27:00 GMT
ADD file:0075aad7a94f0496483442bb2d9fdaa13e9c23087b90638d014b4bc263aa3861 in / 
# Tue, 15 Jun 2021 22:27:03 GMT
CMD ["/bin/sh"]
# Fri, 16 Jul 2021 20:17:57 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 16 Jul 2021 20:33:51 GMT
ENV HAPROXY_VERSION=2.0.23
# Fri, 16 Jul 2021 20:34:00 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.23.tar.gz
# Fri, 16 Jul 2021 20:34:07 GMT
ENV HAPROXY_SHA256=5ddc04e9040a07c647fa4b68fc9da6ec36063d56e12824b356e770dcf677c87a
# Thu, 22 Jul 2021 03:25:45 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 22 Jul 2021 03:25:47 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 03:25:51 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 03:26:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Jul 2021 03:26:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 03:26:10 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:baf144cfb66ebe9df1969f3b90f1c448beff98edc84de1ccb5d6346195a070d4`  
		Last Modified: Tue, 15 Jun 2021 22:27:38 GMT  
		Size: 2.8 MB (2810478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e907663c9428bbbb731a221721c606bad29e54dac6f0dda85d6aa3175a725e`  
		Last Modified: Thu, 22 Jul 2021 03:40:16 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58c65248e94b1a16d74ea6c2e8f9e9fb0200b29496d3f629fceb9d16c3b8aa70`  
		Last Modified: Thu, 22 Jul 2021 03:42:20 GMT  
		Size: 6.1 MB (6064058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0107d6abeeaed80b469419a01bd3f90ac390d59d41b97fba3c729b47121912b6`  
		Last Modified: Thu, 22 Jul 2021 03:42:18 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20bf1a2eda94523ba1152a2692ab73cdbb1e962a05178ed92ccacaac57a1b86`  
		Last Modified: Thu, 22 Jul 2021 03:42:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.2`

```console
$ docker pull haproxy@sha256:fb767f85cab72c631ce4ba85016ef9278f8ca32e9dd5b61450c72a9fc5ec467b
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

### `haproxy:2.2` - linux; amd64

```console
$ docker pull haproxy@sha256:5d801584f803733c0b0d72889af06cc8df1ff4426bd8bcc13597398051dcbfa3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.4 MB (36424023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a64ca9212401f70f933ec02a71f4b83938e0ffc7f8a5c273a3d7bcdfeb2cb9d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 06:19:17 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 16 Jul 2021 20:20:01 GMT
ENV HAPROXY_VERSION=2.2.15
# Fri, 16 Jul 2021 20:20:01 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.15.tar.gz
# Fri, 16 Jul 2021 20:20:01 GMT
ENV HAPROXY_SHA256=48cd0e1cb5de889657cd080fe66cc2ada8198cfece55d63f3a0c011553384cd9
# Fri, 16 Jul 2021 20:20:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 16 Jul 2021 20:20:50 GMT
STOPSIGNAL SIGUSR1
# Fri, 16 Jul 2021 20:20:51 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 16 Jul 2021 20:20:52 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 16 Jul 2021 20:20:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jul 2021 20:20:52 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91332cb81883405a321c1a2d2144bdd0aef8d1c69f90fdf0cf219982161b6e6e`  
		Last Modified: Wed, 23 Jun 2021 06:29:07 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:130f668a56e23dbe0b4ae9299f34cefd8defa2c85bb310d1d9ed60a43753e16b`  
		Last Modified: Fri, 16 Jul 2021 20:24:51 GMT  
		Size: 9.3 MB (9276221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b27c1a4ce34e49a4f78089202069a370cabad72e98f76329afb491a886f9ae34`  
		Last Modified: Fri, 16 Jul 2021 20:24:49 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:852f34ad7c2e203f7ef014ce8ce5b87f38a2909ab12e73cf06f408146bb52a8e`  
		Last Modified: Fri, 16 Jul 2021 20:24:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:520e6e4e449b22c0af424e32f5192f0641cf577bb27e5531685ce5ff3d309913
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33823615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e114961b20a94b2d848b075e25f352b829f6418c0351b461e1ddd49c007192bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 22 Jun 2021 23:50:09 GMT
ADD file:78d4ced31112d85490c684f350aceeebfc72a804262c7ad3e033257e3894f5c4 in / 
# Tue, 22 Jun 2021 23:50:11 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:15:11 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 16 Jul 2021 19:49:08 GMT
ENV HAPROXY_VERSION=2.2.15
# Fri, 16 Jul 2021 19:49:08 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.15.tar.gz
# Fri, 16 Jul 2021 19:49:08 GMT
ENV HAPROXY_SHA256=48cd0e1cb5de889657cd080fe66cc2ada8198cfece55d63f3a0c011553384cd9
# Fri, 16 Jul 2021 19:50:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 16 Jul 2021 19:50:04 GMT
STOPSIGNAL SIGUSR1
# Fri, 16 Jul 2021 19:50:04 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 16 Jul 2021 19:50:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 16 Jul 2021 19:50:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jul 2021 19:50:07 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:532d6df30af5174ac6e1b379c32b8f464d44651ac060376a560c4a76a87704a7`  
		Last Modified: Wed, 23 Jun 2021 00:01:46 GMT  
		Size: 24.9 MB (24878945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48649e3d7de4cd80d3a9a34c725a2935be904ff90e99ea6c8e4bb6e1e7a4eeb7`  
		Last Modified: Wed, 23 Jun 2021 05:24:11 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1cfc69ddcf12a6a2cba97c24d59d814cc3a672b0f3e8d67f53a89406d1e9b02`  
		Last Modified: Fri, 16 Jul 2021 19:53:15 GMT  
		Size: 8.9 MB (8942721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e63b1158d9eeabee3a103177b27c1fa14deec6ec2c8208f38176bab74854be`  
		Last Modified: Fri, 16 Jul 2021 19:53:09 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:572b41c83b25a00c34858adb3f1d7457221cc3dbf90866415ca06e17639a5f50`  
		Last Modified: Fri, 16 Jul 2021 19:53:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:92840e403a4c0a8d986c4457183cd425dc6b7fdbf839f39ebdb247d450e3c265
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.5 MB (31470907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4106be21b86cd5c091da93021a632474404535440ceb4d9b95001b44067371e0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:31 GMT
ADD file:8d200a3bbe985ff355343675c5555852f27550a9e367969df6bc98034efb8fd4 in / 
# Wed, 23 Jun 2021 00:20:31 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:21:41 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 16 Jul 2021 20:36:16 GMT
ENV HAPROXY_VERSION=2.2.15
# Fri, 16 Jul 2021 20:36:17 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.15.tar.gz
# Fri, 16 Jul 2021 20:36:17 GMT
ENV HAPROXY_SHA256=48cd0e1cb5de889657cd080fe66cc2ada8198cfece55d63f3a0c011553384cd9
# Fri, 16 Jul 2021 20:37:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 16 Jul 2021 20:37:06 GMT
STOPSIGNAL SIGUSR1
# Fri, 16 Jul 2021 20:37:07 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 16 Jul 2021 20:37:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 16 Jul 2021 20:37:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jul 2021 20:37:09 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:8452be1adf00f91570fe21a8e61aaf4c12e014daf67d7de65d984f4e8ecca2f1`  
		Last Modified: Wed, 23 Jun 2021 00:31:49 GMT  
		Size: 22.7 MB (22746055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed1c9c92d0076fd4bf40503e3f47102509a5b99d182f4dd9e81e64d0a7e0b8a`  
		Last Modified: Wed, 23 Jun 2021 05:35:48 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b99c2809fb4747d352b784da5afeae2d6b932abb2fa832665119567775e29c46`  
		Last Modified: Fri, 16 Jul 2021 20:43:05 GMT  
		Size: 8.7 MB (8722902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c39132d4b90bd76d5f757c0ac430258bb37957a426b441d6cceeeb3d4a3ceda2`  
		Last Modified: Fri, 16 Jul 2021 20:43:00 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2fed208dfc50b2b0242d33e6b607a7e850cc60f14de5e92959e3e2c7e96d631`  
		Last Modified: Fri, 16 Jul 2021 20:43:00 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:59489d1d5628853f1b78f579ca503b9a45f880ebe7d71a0844cc2d38fdec5e9c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.0 MB (35049312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f453c9eea8ff002138c9a63b430ed68618aa3b75c28b323e1de9eb4eadfdc467`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:40 GMT
ADD file:beee00b59da720f68e12e2ba2a8134207c80c777ddb4ceb03c71e3e4c3f51c93 in / 
# Tue, 22 Jun 2021 23:49:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 03:19:31 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 16 Jul 2021 19:40:21 GMT
ENV HAPROXY_VERSION=2.2.15
# Fri, 16 Jul 2021 19:40:22 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.15.tar.gz
# Fri, 16 Jul 2021 19:40:22 GMT
ENV HAPROXY_SHA256=48cd0e1cb5de889657cd080fe66cc2ada8198cfece55d63f3a0c011553384cd9
# Fri, 16 Jul 2021 19:41:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 16 Jul 2021 19:41:00 GMT
STOPSIGNAL SIGUSR1
# Fri, 16 Jul 2021 19:41:00 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 16 Jul 2021 19:41:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 16 Jul 2021 19:41:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jul 2021 19:41:02 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:448f6bf000e31217a7c202c659b03b7f8ac8d3ae6b03ef7a2f8339be2f00ff4a`  
		Last Modified: Tue, 22 Jun 2021 23:55:25 GMT  
		Size: 25.9 MB (25914993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b05ad81dc8a7d67656235988f0e5fb72c374c7d8df44c105b91d712e06c4ac`  
		Last Modified: Wed, 23 Jun 2021 03:26:16 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49d0bf2dc021b5945dea30811ea0d37f7fb5afd010c7a7b359dac92df51f67f5`  
		Last Modified: Fri, 16 Jul 2021 19:45:19 GMT  
		Size: 9.1 MB (9132367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2009e0bf94a6df8c8ec4f7f4ccaaf47ce596eea8a79276d21a2f62d46c154994`  
		Last Modified: Fri, 16 Jul 2021 19:45:17 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:775e922f9020d150a4f5e43756cd8550095ad55f01d05c52761643b336ee7a4e`  
		Last Modified: Fri, 16 Jul 2021 19:45:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2` - linux; 386

```console
$ docker pull haproxy@sha256:a5445ba6fd37b20b7f9bd3b414921260401aa8a7623e00f747e2c76befded1d0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (37020424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9011886094855355a7c3c0f2493109f13417b5dc0ce9554cd73d8c6deb0111d4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 22 Jun 2021 23:39:35 GMT
ADD file:48f656ac6733911048b3de850490438d0233b3badc11861fca62062d4edfaf40 in / 
# Tue, 22 Jun 2021 23:39:35 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:23:13 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 16 Jul 2021 19:39:47 GMT
ENV HAPROXY_VERSION=2.2.15
# Fri, 16 Jul 2021 19:39:47 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.15.tar.gz
# Fri, 16 Jul 2021 19:39:47 GMT
ENV HAPROXY_SHA256=48cd0e1cb5de889657cd080fe66cc2ada8198cfece55d63f3a0c011553384cd9
# Fri, 16 Jul 2021 19:40:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 16 Jul 2021 19:40:42 GMT
STOPSIGNAL SIGUSR1
# Fri, 16 Jul 2021 19:40:42 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 16 Jul 2021 19:40:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 16 Jul 2021 19:40:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jul 2021 19:40:43 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:33af2dcb865e65d53cdeb843b67a0ef62151fa32df292293e7c6b0eb728ac5ac`  
		Last Modified: Tue, 22 Jun 2021 23:46:23 GMT  
		Size: 27.8 MB (27797411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a6e4d42b23996eb7d8a1baa85ee19828c2667fd4a2dca6eb1040b266680e9f`  
		Last Modified: Wed, 23 Jun 2021 00:32:00 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c91c7c9f9bce06eef7b2967290b1744349eac18c2e4c762540e73c77905a42c`  
		Last Modified: Fri, 16 Jul 2021 19:45:54 GMT  
		Size: 9.2 MB (9221064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63168d04187be322165c283ad32ef35a0c49b8cb6d27ab882d713b60dd69cc37`  
		Last Modified: Fri, 16 Jul 2021 19:45:51 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e4b284deab5ad5e747b812cf07395824c8538e241628ab46c363ed80abd86d3`  
		Last Modified: Fri, 16 Jul 2021 19:45:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2` - linux; mips64le

```console
$ docker pull haproxy@sha256:1cbfbde1093616ae6a05dcc4506cd4e1b87306fdf50691b054635d8f549599fa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34716599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:720c70507d5b559ce8704eb736f0ecf4d7b13bd3edcb506a708de6ef2945c270`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 22 Jul 2021 00:09:45 GMT
ADD file:1f77b9001c4977ba733be674fc5eb4b85130f1dea8a7b39d545b70f9c107695f in / 
# Thu, 22 Jul 2021 00:09:46 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:07:49 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 22 Jul 2021 01:15:37 GMT
ENV HAPROXY_VERSION=2.2.15
# Thu, 22 Jul 2021 01:15:37 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.15.tar.gz
# Thu, 22 Jul 2021 01:15:37 GMT
ENV HAPROXY_SHA256=48cd0e1cb5de889657cd080fe66cc2ada8198cfece55d63f3a0c011553384cd9
# Thu, 22 Jul 2021 01:17:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 22 Jul 2021 01:17:58 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 01:17:59 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 01:18:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Jul 2021 01:18:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 01:18:01 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:99ee621d0b0485e9de65aa19604aa2453d19ea7fc86b22c5b77c1bab74e3cb42`  
		Last Modified: Thu, 22 Jul 2021 00:16:11 GMT  
		Size: 25.8 MB (25812771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f444627794f98947a9df95ec5d19b2a1cd6c151ed438982b1dc0b89f5eaf19e`  
		Last Modified: Thu, 22 Jul 2021 01:24:39 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5458fd4453a41d027193836695559ee97bc19973370e591a8d8d1805e0c0e9cf`  
		Last Modified: Thu, 22 Jul 2021 01:25:41 GMT  
		Size: 8.9 MB (8901878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df0cce5a1dbc0531cf273fa968579a29cb688c3ef7a6bafea7b7588d9b3b6d2`  
		Last Modified: Thu, 22 Jul 2021 01:25:34 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2547e77a536680a51595cca012d7eb80a5b8d1574fb2233fb475f286e3fda38b`  
		Last Modified: Thu, 22 Jul 2021 01:25:37 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2` - linux; ppc64le

```console
$ docker pull haproxy@sha256:87cb7d5e34b5b865eb81a06905f7a1c3bb129f903081823edb48f3b1c29e359c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.4 MB (40365004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0473612005f06a26a21a7fa145678740d9199c8bd2f29448b760583b99c0954a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 22 Jul 2021 00:19:04 GMT
ADD file:3a6bd6ce3eff98b88a13de5d0f26cff0b026f876674204dbad6f84fafcf145b1 in / 
# Thu, 22 Jul 2021 00:19:13 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 02:52:46 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 22 Jul 2021 03:12:54 GMT
ENV HAPROXY_VERSION=2.2.15
# Thu, 22 Jul 2021 03:12:59 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.15.tar.gz
# Thu, 22 Jul 2021 03:13:03 GMT
ENV HAPROXY_SHA256=48cd0e1cb5de889657cd080fe66cc2ada8198cfece55d63f3a0c011553384cd9
# Thu, 22 Jul 2021 03:17:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 22 Jul 2021 03:17:48 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 03:17:50 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 03:18:07 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Jul 2021 03:18:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 03:18:14 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:1130517d52da84a09f9465006bddab5e49afd398860890eab6274fd0bff32371`  
		Last Modified: Thu, 22 Jul 2021 00:27:49 GMT  
		Size: 30.6 MB (30553709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251bf3fe1d4bbe9c27e393cd8ddc550b56cec90eb916bf9bec24d657c9f6556f`  
		Last Modified: Thu, 22 Jul 2021 03:40:01 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3653c9fa6bff431075a219ada0b2e255d8184581dc36063186815333f06de05`  
		Last Modified: Thu, 22 Jul 2021 03:41:41 GMT  
		Size: 9.8 MB (9809348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d95bdff7e3e2155ee289913825f422d5a4c3460de68fdbad75e1072323ce9c66`  
		Last Modified: Thu, 22 Jul 2021 03:41:39 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f711c12d7a95ec8b0ae6a7c59b5ee56b909f4571ba29baee7e64cec1e7df557d`  
		Last Modified: Thu, 22 Jul 2021 03:41:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2` - linux; s390x

```console
$ docker pull haproxy@sha256:f86e1c1f59f055af9f1cce5c97307502a3043a8c5547b18c04bf4cc6dc2400f7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34803423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60fb0d78497b02b7bc534b0a76fe5d6f3626f4a16ade59391d8ae825d25f49f1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 22 Jul 2021 00:42:45 GMT
ADD file:1ab999eb6f80d8ce91ce3a173e23fd2710f2779117bba29037eaa82aadcbf6ed in / 
# Thu, 22 Jul 2021 00:42:48 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:30:19 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 22 Jul 2021 01:34:25 GMT
ENV HAPROXY_VERSION=2.2.15
# Thu, 22 Jul 2021 01:34:25 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.15.tar.gz
# Thu, 22 Jul 2021 01:34:25 GMT
ENV HAPROXY_SHA256=48cd0e1cb5de889657cd080fe66cc2ada8198cfece55d63f3a0c011553384cd9
# Thu, 22 Jul 2021 01:35:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 22 Jul 2021 01:35:09 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 01:35:10 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 01:35:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Jul 2021 01:35:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 01:35:11 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:7a50fdd85ff244c1465e71c51354d055e3df0b90ff5faad28cc22d9ecde9daf3`  
		Last Modified: Thu, 22 Jul 2021 00:48:13 GMT  
		Size: 25.8 MB (25760761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05fb34d1ed21b67502665114a7ae60445472fc7bafa620bbf6c79b7df85a01d4`  
		Last Modified: Thu, 22 Jul 2021 01:39:54 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b15e5cf4cb4ed8d7994364c1330f8753dab6faffc8dd0236c41b901e63981554`  
		Last Modified: Thu, 22 Jul 2021 01:40:27 GMT  
		Size: 9.0 MB (9040712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:351a8c9835e3f604cd5db18b86cbc27e55d125813cc0bd87ef73801be8a1f465`  
		Last Modified: Thu, 22 Jul 2021 01:40:26 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cce3640d5c727c8b5ca61886c76b8c770912983132051dd077649f3451510f2`  
		Last Modified: Thu, 22 Jul 2021 01:40:26 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.2-alpine`

```console
$ docker pull haproxy@sha256:52be0979286c0e151ba26e4214bbc0223a5a28af24cec60a7c4a455a1f39b900
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `haproxy:2.2-alpine` - linux; amd64

```console
$ docker pull haproxy@sha256:d5079998fb1e5885ae0ec36c8d696df8ab8d94503cedce7b3b848420d02f73eb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.2 MB (9183607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1978a4f77a6bb5a8d5d70b0682e8887bcdddad0b632d78fd1f5bef2afb64c619`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 02:48:50 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 16 Jul 2021 20:21:01 GMT
ENV HAPROXY_VERSION=2.2.15
# Fri, 16 Jul 2021 20:21:01 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.15.tar.gz
# Fri, 16 Jul 2021 20:21:01 GMT
ENV HAPROXY_SHA256=48cd0e1cb5de889657cd080fe66cc2ada8198cfece55d63f3a0c011553384cd9
# Fri, 16 Jul 2021 20:21:53 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 16 Jul 2021 20:21:53 GMT
STOPSIGNAL SIGUSR1
# Fri, 16 Jul 2021 20:21:54 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 16 Jul 2021 20:21:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 16 Jul 2021 20:21:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jul 2021 20:21:55 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7834d945b9e597e693f56fb0f9847718c1732b738a2f4956ab2c1b66c289d90`  
		Last Modified: Sat, 26 Jun 2021 02:56:43 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4503b62662ebb03c72eef87d5e386f25c1f6bf50b26e363a5d79304aada5e21`  
		Last Modified: Fri, 16 Jul 2021 20:25:02 GMT  
		Size: 6.4 MB (6370364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f14e978219962603947faf4154e4b3aef9242dc22050cbed2d8a5fd11faaca`  
		Last Modified: Fri, 16 Jul 2021 20:25:01 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b29b2882ec593a19430c38619e2e746b6f94bb28c4efdf3dcf9e01cef1a8c5f`  
		Last Modified: Fri, 16 Jul 2021 20:25:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2-alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:c2f46d1b746154bb7f2154ba8040baa8d97049756080123c3f1e10d34ca72dac
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.9 MB (8894324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17cc292ea9ff3bd0e3b2679306110d4be2027b95b66d3c4964ea410bb5af3b57`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:26 GMT
ADD file:c80bc2b093cbc0fc466582ef21cbed377de9fa874aedbf320079525ddacd1200 in / 
# Tue, 15 Jun 2021 22:57:26 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 02:02:51 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 16 Jul 2021 19:51:50 GMT
ENV HAPROXY_VERSION=2.2.15
# Fri, 16 Jul 2021 19:51:50 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.15.tar.gz
# Fri, 16 Jul 2021 19:51:51 GMT
ENV HAPROXY_SHA256=48cd0e1cb5de889657cd080fe66cc2ada8198cfece55d63f3a0c011553384cd9
# Fri, 16 Jul 2021 19:52:19 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 16 Jul 2021 19:52:19 GMT
STOPSIGNAL SIGUSR1
# Fri, 16 Jul 2021 19:52:20 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 16 Jul 2021 19:52:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 16 Jul 2021 19:52:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jul 2021 19:52:22 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:b4c9a0924271af3466de27804af26420eb58da1466e7eaaba127d178b380fea3`  
		Last Modified: Tue, 15 Jun 2021 22:58:47 GMT  
		Size: 2.6 MB (2624382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85fa2947d9cc2655af4fd4aa21641629e791bcaf309a7095db77d309ddd05dfa`  
		Last Modified: Sat, 26 Jun 2021 02:08:45 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd622ad240a50ac5cea62cec763266261c4a7e7381e905683ac71f0c1aa5d77`  
		Last Modified: Fri, 16 Jul 2021 19:54:50 GMT  
		Size: 6.3 MB (6268178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac0a5e3bef02be4409d1fdb918db30ff37d5ee7d605b9f501e6a21c08f65e7c8`  
		Last Modified: Fri, 16 Jul 2021 19:54:46 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20d041211cf66df3bca589f8baf656200aa3f4e34ef0a48506b8d050d7886433`  
		Last Modified: Fri, 16 Jul 2021 19:54:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:2161bacbb0ff8f69ca9b3407d4a3c03d5604b4e5d1e1a6dcf51dcd3ff8854c3d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8598879 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a233535dd638821a95741fb8ea17f0b70c1576d0340d16dd4e5da1c5b5f2e828`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:05 GMT
ADD file:416a8b507abdc6bdcb22997a4be0a4170796c3f9f77e315b2dbff2b0a212bc68 in / 
# Tue, 15 Jun 2021 23:15:06 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 05:27:42 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 16 Jul 2021 20:37:23 GMT
ENV HAPROXY_VERSION=2.2.15
# Fri, 16 Jul 2021 20:37:23 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.15.tar.gz
# Fri, 16 Jul 2021 20:37:24 GMT
ENV HAPROXY_SHA256=48cd0e1cb5de889657cd080fe66cc2ada8198cfece55d63f3a0c011553384cd9
# Fri, 16 Jul 2021 20:37:49 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 16 Jul 2021 20:37:50 GMT
STOPSIGNAL SIGUSR1
# Fri, 16 Jul 2021 20:37:50 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 16 Jul 2021 20:37:52 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 16 Jul 2021 20:37:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jul 2021 20:37:53 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:136482bf81d1fa351b424ebb8c7e34d15f2c5ed3fc0b66b544b8312bda3d52d9`  
		Last Modified: Tue, 15 Jun 2021 23:16:40 GMT  
		Size: 2.4 MB (2427917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5464af225bd487370319e7125fb2769222c5c7371d1be737936169d2e5b01c`  
		Last Modified: Sat, 26 Jun 2021 05:35:56 GMT  
		Size: 1.2 KB (1196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed027d2048a3392220a7959453fb02a221f21a71faeae4bdc6bb900bb8dc6c7a`  
		Last Modified: Fri, 16 Jul 2021 20:43:21 GMT  
		Size: 6.2 MB (6169197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de1a2718e85f9ad030af5bb6578a28e574813d1f5aebf51194a87039a7dcc0b5`  
		Last Modified: Fri, 16 Jul 2021 20:43:17 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa186376fca912c014c7abd185e349ab2f56cad26b384c1b0cf7267a1f8d2199`  
		Last Modified: Fri, 16 Jul 2021 20:43:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:9e50b1981ce6323ef61d29566d08b8b4c041bceaf60aac4efde11fae69b54b6f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.1 MB (9100357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f782ea25f9d3e282dc40dbca1555bfa22cdb3f34e4aea852dd1c2d56b2aa77b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 21:44:56 GMT
ADD file:6797caacbfe41bfe44000b39ed017016c6fcc492b3d6557cdaba88536df6c876 in / 
# Tue, 15 Jun 2021 21:44:56 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 02:13:15 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 16 Jul 2021 19:41:13 GMT
ENV HAPROXY_VERSION=2.2.15
# Fri, 16 Jul 2021 19:41:13 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.15.tar.gz
# Fri, 16 Jul 2021 19:41:14 GMT
ENV HAPROXY_SHA256=48cd0e1cb5de889657cd080fe66cc2ada8198cfece55d63f3a0c011553384cd9
# Fri, 16 Jul 2021 19:41:58 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 16 Jul 2021 19:41:58 GMT
STOPSIGNAL SIGUSR1
# Fri, 16 Jul 2021 19:41:59 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 16 Jul 2021 19:41:59 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 16 Jul 2021 19:42:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jul 2021 19:42:00 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:58ab47519297212468320b23b8100fc1b2b96e8d342040806ae509a778a0a07a`  
		Last Modified: Tue, 15 Jun 2021 21:46:03 GMT  
		Size: 2.7 MB (2709626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb8dc96e2a4b7f90ae2dbfca981fe199966b64e3426ca1f742499d46ad1aa357`  
		Last Modified: Sat, 26 Jun 2021 02:21:19 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3633c11f8825cccf4db110e4621f2ad4e5c895799a8a49a4bf810ba919dfa478`  
		Last Modified: Fri, 16 Jul 2021 19:45:31 GMT  
		Size: 6.4 MB (6388965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c877b8aa2303fa413c5d69497fa7fafeceda383b83a55d8580c58a9b922efb1`  
		Last Modified: Fri, 16 Jul 2021 19:45:30 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d71fcd03f304168ee1c375d2b03ca13ba4b6025c18e02f42e99431b5ec1fc77`  
		Last Modified: Fri, 16 Jul 2021 19:45:30 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2-alpine` - linux; 386

```console
$ docker pull haproxy@sha256:d89cde92e122ae28fc245c341c5e9dbe15dd19aa68f0242b13a911c28013455f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9048078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1456760fc9bbb3df68355f6ff18837db53daa2d2340f9dfab219d72ee07b15cb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 21:38:30 GMT
ADD file:3b0fe1454491bb05e218b090fd461f2fd39546aa4a53eb3f953ee8eae149ac57 in / 
# Tue, 15 Jun 2021 21:38:30 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 01:39:05 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 16 Jul 2021 19:40:49 GMT
ENV HAPROXY_VERSION=2.2.15
# Fri, 16 Jul 2021 19:40:49 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.15.tar.gz
# Fri, 16 Jul 2021 19:40:49 GMT
ENV HAPROXY_SHA256=48cd0e1cb5de889657cd080fe66cc2ada8198cfece55d63f3a0c011553384cd9
# Fri, 16 Jul 2021 19:41:49 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 16 Jul 2021 19:41:49 GMT
STOPSIGNAL SIGUSR1
# Fri, 16 Jul 2021 19:41:49 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 16 Jul 2021 19:41:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 16 Jul 2021 19:41:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jul 2021 19:41:51 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:be21df321efb39c5daf3151073ebff7688e15ea6cd5158878bc9559a5db76ac6`  
		Last Modified: Tue, 15 Jun 2021 21:39:16 GMT  
		Size: 2.8 MB (2820718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc6fe536c8e50a97873c166db7d3b669842dec91d85ce73433028b3b198a1c4`  
		Last Modified: Sat, 26 Jun 2021 01:49:46 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9928b291dd1da6088fd487934595dbe2e599d5413769e858d6405ad7bf4265e`  
		Last Modified: Fri, 16 Jul 2021 19:46:07 GMT  
		Size: 6.2 MB (6225597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d290d72d744b2245d5c6a0b64f0503fb71e9ac292b02e02969d40d2e2c0a3807`  
		Last Modified: Fri, 16 Jul 2021 19:46:06 GMT  
		Size: 447.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e51c7579310e066ebf25d53928150d39ea84e3ca35c08d386bc238dd1f585bdd`  
		Last Modified: Fri, 16 Jul 2021 19:46:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2-alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:a12fba28fbf006ed034ee0fc7eb0ab26e79a36a99815fd47bc83b8d518fa78d5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9519701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcdfad7039b75be3278562e46e07712e13524244d8a7bef3c63f541e9d82c697`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:27:00 GMT
ADD file:0075aad7a94f0496483442bb2d9fdaa13e9c23087b90638d014b4bc263aa3861 in / 
# Tue, 15 Jun 2021 22:27:03 GMT
CMD ["/bin/sh"]
# Fri, 16 Jul 2021 20:17:57 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 16 Jul 2021 20:27:19 GMT
ENV HAPROXY_VERSION=2.2.15
# Fri, 16 Jul 2021 20:27:22 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.15.tar.gz
# Fri, 16 Jul 2021 20:27:27 GMT
ENV HAPROXY_SHA256=48cd0e1cb5de889657cd080fe66cc2ada8198cfece55d63f3a0c011553384cd9
# Thu, 22 Jul 2021 03:19:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 22 Jul 2021 03:19:18 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 03:19:20 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 03:19:28 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Jul 2021 03:19:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 03:19:39 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:baf144cfb66ebe9df1969f3b90f1c448beff98edc84de1ccb5d6346195a070d4`  
		Last Modified: Tue, 15 Jun 2021 22:27:38 GMT  
		Size: 2.8 MB (2810478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e907663c9428bbbb731a221721c606bad29e54dac6f0dda85d6aa3175a725e`  
		Last Modified: Thu, 22 Jul 2021 03:40:16 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0ffd2888ce89fabb79d101f0f75f1945b0d91d47dd02d1d75bd8bbd85fb3df5`  
		Last Modified: Thu, 22 Jul 2021 03:41:54 GMT  
		Size: 6.7 MB (6707455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50458b4a7a19297ded472eef7e0d0bbb73924ccd421a614293161b85001de8b6`  
		Last Modified: Thu, 22 Jul 2021 03:41:53 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45bc5148f462cfd0d09265d96af1502308d438ba9e02dc9d2a49a8498bc797e9`  
		Last Modified: Thu, 22 Jul 2021 03:41:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2-alpine` - linux; s390x

```console
$ docker pull haproxy@sha256:46c26b096b2727e54bd284ce787acdf250105eef2499a26ad3c781ee07ddea65
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.9 MB (8944856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b011e7b2da4973daf7d6c3188e86cb22d4bde3bbfb56281369bc18ac0b7ad66`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:54:24 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 29 Apr 2021 17:43:14 GMT
ENV HAPROXY_VERSION=2.2.14
# Thu, 29 Apr 2021 17:43:14 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Thu, 29 Apr 2021 17:43:14 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Thu, 29 Apr 2021 17:43:57 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 29 Apr 2021 17:43:58 GMT
STOPSIGNAL SIGUSR1
# Thu, 29 Apr 2021 17:43:58 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 29 Apr 2021 17:43:59 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 29 Apr 2021 17:44:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Apr 2021 17:44:01 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267275aba58470c82626189a59be76cd169bd245568e2f2545ed1ee64ff8a8ff`  
		Last Modified: Wed, 14 Apr 2021 20:59:06 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53bd90fedbb3ad8d7ce19548b2051961aba93878bb770199538eb7d77b84c615`  
		Last Modified: Thu, 29 Apr 2021 17:45:16 GMT  
		Size: 6.3 MB (6340449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b7746ababb0b63330117e707635f5d6f4bb1d0a1641718dc1c4c49af72d0f0`  
		Last Modified: Thu, 29 Apr 2021 17:45:16 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03b76e05f6e27ece4bdcb064a2e1f70ce99db1fd371bdb31de6f2a4ad604fd2f`  
		Last Modified: Thu, 29 Apr 2021 17:45:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.2.15`

```console
$ docker pull haproxy@sha256:fb767f85cab72c631ce4ba85016ef9278f8ca32e9dd5b61450c72a9fc5ec467b
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

### `haproxy:2.2.15` - linux; amd64

```console
$ docker pull haproxy@sha256:5d801584f803733c0b0d72889af06cc8df1ff4426bd8bcc13597398051dcbfa3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.4 MB (36424023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a64ca9212401f70f933ec02a71f4b83938e0ffc7f8a5c273a3d7bcdfeb2cb9d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 06:19:17 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 16 Jul 2021 20:20:01 GMT
ENV HAPROXY_VERSION=2.2.15
# Fri, 16 Jul 2021 20:20:01 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.15.tar.gz
# Fri, 16 Jul 2021 20:20:01 GMT
ENV HAPROXY_SHA256=48cd0e1cb5de889657cd080fe66cc2ada8198cfece55d63f3a0c011553384cd9
# Fri, 16 Jul 2021 20:20:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 16 Jul 2021 20:20:50 GMT
STOPSIGNAL SIGUSR1
# Fri, 16 Jul 2021 20:20:51 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 16 Jul 2021 20:20:52 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 16 Jul 2021 20:20:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jul 2021 20:20:52 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91332cb81883405a321c1a2d2144bdd0aef8d1c69f90fdf0cf219982161b6e6e`  
		Last Modified: Wed, 23 Jun 2021 06:29:07 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:130f668a56e23dbe0b4ae9299f34cefd8defa2c85bb310d1d9ed60a43753e16b`  
		Last Modified: Fri, 16 Jul 2021 20:24:51 GMT  
		Size: 9.3 MB (9276221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b27c1a4ce34e49a4f78089202069a370cabad72e98f76329afb491a886f9ae34`  
		Last Modified: Fri, 16 Jul 2021 20:24:49 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:852f34ad7c2e203f7ef014ce8ce5b87f38a2909ab12e73cf06f408146bb52a8e`  
		Last Modified: Fri, 16 Jul 2021 20:24:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.15` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:520e6e4e449b22c0af424e32f5192f0641cf577bb27e5531685ce5ff3d309913
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33823615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e114961b20a94b2d848b075e25f352b829f6418c0351b461e1ddd49c007192bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 22 Jun 2021 23:50:09 GMT
ADD file:78d4ced31112d85490c684f350aceeebfc72a804262c7ad3e033257e3894f5c4 in / 
# Tue, 22 Jun 2021 23:50:11 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:15:11 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 16 Jul 2021 19:49:08 GMT
ENV HAPROXY_VERSION=2.2.15
# Fri, 16 Jul 2021 19:49:08 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.15.tar.gz
# Fri, 16 Jul 2021 19:49:08 GMT
ENV HAPROXY_SHA256=48cd0e1cb5de889657cd080fe66cc2ada8198cfece55d63f3a0c011553384cd9
# Fri, 16 Jul 2021 19:50:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 16 Jul 2021 19:50:04 GMT
STOPSIGNAL SIGUSR1
# Fri, 16 Jul 2021 19:50:04 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 16 Jul 2021 19:50:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 16 Jul 2021 19:50:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jul 2021 19:50:07 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:532d6df30af5174ac6e1b379c32b8f464d44651ac060376a560c4a76a87704a7`  
		Last Modified: Wed, 23 Jun 2021 00:01:46 GMT  
		Size: 24.9 MB (24878945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48649e3d7de4cd80d3a9a34c725a2935be904ff90e99ea6c8e4bb6e1e7a4eeb7`  
		Last Modified: Wed, 23 Jun 2021 05:24:11 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1cfc69ddcf12a6a2cba97c24d59d814cc3a672b0f3e8d67f53a89406d1e9b02`  
		Last Modified: Fri, 16 Jul 2021 19:53:15 GMT  
		Size: 8.9 MB (8942721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e63b1158d9eeabee3a103177b27c1fa14deec6ec2c8208f38176bab74854be`  
		Last Modified: Fri, 16 Jul 2021 19:53:09 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:572b41c83b25a00c34858adb3f1d7457221cc3dbf90866415ca06e17639a5f50`  
		Last Modified: Fri, 16 Jul 2021 19:53:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.15` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:92840e403a4c0a8d986c4457183cd425dc6b7fdbf839f39ebdb247d450e3c265
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.5 MB (31470907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4106be21b86cd5c091da93021a632474404535440ceb4d9b95001b44067371e0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:31 GMT
ADD file:8d200a3bbe985ff355343675c5555852f27550a9e367969df6bc98034efb8fd4 in / 
# Wed, 23 Jun 2021 00:20:31 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:21:41 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 16 Jul 2021 20:36:16 GMT
ENV HAPROXY_VERSION=2.2.15
# Fri, 16 Jul 2021 20:36:17 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.15.tar.gz
# Fri, 16 Jul 2021 20:36:17 GMT
ENV HAPROXY_SHA256=48cd0e1cb5de889657cd080fe66cc2ada8198cfece55d63f3a0c011553384cd9
# Fri, 16 Jul 2021 20:37:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 16 Jul 2021 20:37:06 GMT
STOPSIGNAL SIGUSR1
# Fri, 16 Jul 2021 20:37:07 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 16 Jul 2021 20:37:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 16 Jul 2021 20:37:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jul 2021 20:37:09 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:8452be1adf00f91570fe21a8e61aaf4c12e014daf67d7de65d984f4e8ecca2f1`  
		Last Modified: Wed, 23 Jun 2021 00:31:49 GMT  
		Size: 22.7 MB (22746055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed1c9c92d0076fd4bf40503e3f47102509a5b99d182f4dd9e81e64d0a7e0b8a`  
		Last Modified: Wed, 23 Jun 2021 05:35:48 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b99c2809fb4747d352b784da5afeae2d6b932abb2fa832665119567775e29c46`  
		Last Modified: Fri, 16 Jul 2021 20:43:05 GMT  
		Size: 8.7 MB (8722902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c39132d4b90bd76d5f757c0ac430258bb37957a426b441d6cceeeb3d4a3ceda2`  
		Last Modified: Fri, 16 Jul 2021 20:43:00 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2fed208dfc50b2b0242d33e6b607a7e850cc60f14de5e92959e3e2c7e96d631`  
		Last Modified: Fri, 16 Jul 2021 20:43:00 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.15` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:59489d1d5628853f1b78f579ca503b9a45f880ebe7d71a0844cc2d38fdec5e9c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.0 MB (35049312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f453c9eea8ff002138c9a63b430ed68618aa3b75c28b323e1de9eb4eadfdc467`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:40 GMT
ADD file:beee00b59da720f68e12e2ba2a8134207c80c777ddb4ceb03c71e3e4c3f51c93 in / 
# Tue, 22 Jun 2021 23:49:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 03:19:31 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 16 Jul 2021 19:40:21 GMT
ENV HAPROXY_VERSION=2.2.15
# Fri, 16 Jul 2021 19:40:22 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.15.tar.gz
# Fri, 16 Jul 2021 19:40:22 GMT
ENV HAPROXY_SHA256=48cd0e1cb5de889657cd080fe66cc2ada8198cfece55d63f3a0c011553384cd9
# Fri, 16 Jul 2021 19:41:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 16 Jul 2021 19:41:00 GMT
STOPSIGNAL SIGUSR1
# Fri, 16 Jul 2021 19:41:00 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 16 Jul 2021 19:41:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 16 Jul 2021 19:41:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jul 2021 19:41:02 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:448f6bf000e31217a7c202c659b03b7f8ac8d3ae6b03ef7a2f8339be2f00ff4a`  
		Last Modified: Tue, 22 Jun 2021 23:55:25 GMT  
		Size: 25.9 MB (25914993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b05ad81dc8a7d67656235988f0e5fb72c374c7d8df44c105b91d712e06c4ac`  
		Last Modified: Wed, 23 Jun 2021 03:26:16 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49d0bf2dc021b5945dea30811ea0d37f7fb5afd010c7a7b359dac92df51f67f5`  
		Last Modified: Fri, 16 Jul 2021 19:45:19 GMT  
		Size: 9.1 MB (9132367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2009e0bf94a6df8c8ec4f7f4ccaaf47ce596eea8a79276d21a2f62d46c154994`  
		Last Modified: Fri, 16 Jul 2021 19:45:17 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:775e922f9020d150a4f5e43756cd8550095ad55f01d05c52761643b336ee7a4e`  
		Last Modified: Fri, 16 Jul 2021 19:45:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.15` - linux; 386

```console
$ docker pull haproxy@sha256:a5445ba6fd37b20b7f9bd3b414921260401aa8a7623e00f747e2c76befded1d0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (37020424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9011886094855355a7c3c0f2493109f13417b5dc0ce9554cd73d8c6deb0111d4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 22 Jun 2021 23:39:35 GMT
ADD file:48f656ac6733911048b3de850490438d0233b3badc11861fca62062d4edfaf40 in / 
# Tue, 22 Jun 2021 23:39:35 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:23:13 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 16 Jul 2021 19:39:47 GMT
ENV HAPROXY_VERSION=2.2.15
# Fri, 16 Jul 2021 19:39:47 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.15.tar.gz
# Fri, 16 Jul 2021 19:39:47 GMT
ENV HAPROXY_SHA256=48cd0e1cb5de889657cd080fe66cc2ada8198cfece55d63f3a0c011553384cd9
# Fri, 16 Jul 2021 19:40:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 16 Jul 2021 19:40:42 GMT
STOPSIGNAL SIGUSR1
# Fri, 16 Jul 2021 19:40:42 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 16 Jul 2021 19:40:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 16 Jul 2021 19:40:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jul 2021 19:40:43 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:33af2dcb865e65d53cdeb843b67a0ef62151fa32df292293e7c6b0eb728ac5ac`  
		Last Modified: Tue, 22 Jun 2021 23:46:23 GMT  
		Size: 27.8 MB (27797411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a6e4d42b23996eb7d8a1baa85ee19828c2667fd4a2dca6eb1040b266680e9f`  
		Last Modified: Wed, 23 Jun 2021 00:32:00 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c91c7c9f9bce06eef7b2967290b1744349eac18c2e4c762540e73c77905a42c`  
		Last Modified: Fri, 16 Jul 2021 19:45:54 GMT  
		Size: 9.2 MB (9221064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63168d04187be322165c283ad32ef35a0c49b8cb6d27ab882d713b60dd69cc37`  
		Last Modified: Fri, 16 Jul 2021 19:45:51 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e4b284deab5ad5e747b812cf07395824c8538e241628ab46c363ed80abd86d3`  
		Last Modified: Fri, 16 Jul 2021 19:45:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.15` - linux; mips64le

```console
$ docker pull haproxy@sha256:1cbfbde1093616ae6a05dcc4506cd4e1b87306fdf50691b054635d8f549599fa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34716599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:720c70507d5b559ce8704eb736f0ecf4d7b13bd3edcb506a708de6ef2945c270`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 22 Jul 2021 00:09:45 GMT
ADD file:1f77b9001c4977ba733be674fc5eb4b85130f1dea8a7b39d545b70f9c107695f in / 
# Thu, 22 Jul 2021 00:09:46 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:07:49 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 22 Jul 2021 01:15:37 GMT
ENV HAPROXY_VERSION=2.2.15
# Thu, 22 Jul 2021 01:15:37 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.15.tar.gz
# Thu, 22 Jul 2021 01:15:37 GMT
ENV HAPROXY_SHA256=48cd0e1cb5de889657cd080fe66cc2ada8198cfece55d63f3a0c011553384cd9
# Thu, 22 Jul 2021 01:17:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 22 Jul 2021 01:17:58 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 01:17:59 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 01:18:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Jul 2021 01:18:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 01:18:01 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:99ee621d0b0485e9de65aa19604aa2453d19ea7fc86b22c5b77c1bab74e3cb42`  
		Last Modified: Thu, 22 Jul 2021 00:16:11 GMT  
		Size: 25.8 MB (25812771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f444627794f98947a9df95ec5d19b2a1cd6c151ed438982b1dc0b89f5eaf19e`  
		Last Modified: Thu, 22 Jul 2021 01:24:39 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5458fd4453a41d027193836695559ee97bc19973370e591a8d8d1805e0c0e9cf`  
		Last Modified: Thu, 22 Jul 2021 01:25:41 GMT  
		Size: 8.9 MB (8901878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df0cce5a1dbc0531cf273fa968579a29cb688c3ef7a6bafea7b7588d9b3b6d2`  
		Last Modified: Thu, 22 Jul 2021 01:25:34 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2547e77a536680a51595cca012d7eb80a5b8d1574fb2233fb475f286e3fda38b`  
		Last Modified: Thu, 22 Jul 2021 01:25:37 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.15` - linux; ppc64le

```console
$ docker pull haproxy@sha256:87cb7d5e34b5b865eb81a06905f7a1c3bb129f903081823edb48f3b1c29e359c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.4 MB (40365004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0473612005f06a26a21a7fa145678740d9199c8bd2f29448b760583b99c0954a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 22 Jul 2021 00:19:04 GMT
ADD file:3a6bd6ce3eff98b88a13de5d0f26cff0b026f876674204dbad6f84fafcf145b1 in / 
# Thu, 22 Jul 2021 00:19:13 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 02:52:46 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 22 Jul 2021 03:12:54 GMT
ENV HAPROXY_VERSION=2.2.15
# Thu, 22 Jul 2021 03:12:59 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.15.tar.gz
# Thu, 22 Jul 2021 03:13:03 GMT
ENV HAPROXY_SHA256=48cd0e1cb5de889657cd080fe66cc2ada8198cfece55d63f3a0c011553384cd9
# Thu, 22 Jul 2021 03:17:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 22 Jul 2021 03:17:48 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 03:17:50 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 03:18:07 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Jul 2021 03:18:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 03:18:14 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:1130517d52da84a09f9465006bddab5e49afd398860890eab6274fd0bff32371`  
		Last Modified: Thu, 22 Jul 2021 00:27:49 GMT  
		Size: 30.6 MB (30553709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251bf3fe1d4bbe9c27e393cd8ddc550b56cec90eb916bf9bec24d657c9f6556f`  
		Last Modified: Thu, 22 Jul 2021 03:40:01 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3653c9fa6bff431075a219ada0b2e255d8184581dc36063186815333f06de05`  
		Last Modified: Thu, 22 Jul 2021 03:41:41 GMT  
		Size: 9.8 MB (9809348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d95bdff7e3e2155ee289913825f422d5a4c3460de68fdbad75e1072323ce9c66`  
		Last Modified: Thu, 22 Jul 2021 03:41:39 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f711c12d7a95ec8b0ae6a7c59b5ee56b909f4571ba29baee7e64cec1e7df557d`  
		Last Modified: Thu, 22 Jul 2021 03:41:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.15` - linux; s390x

```console
$ docker pull haproxy@sha256:f86e1c1f59f055af9f1cce5c97307502a3043a8c5547b18c04bf4cc6dc2400f7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34803423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60fb0d78497b02b7bc534b0a76fe5d6f3626f4a16ade59391d8ae825d25f49f1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 22 Jul 2021 00:42:45 GMT
ADD file:1ab999eb6f80d8ce91ce3a173e23fd2710f2779117bba29037eaa82aadcbf6ed in / 
# Thu, 22 Jul 2021 00:42:48 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:30:19 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 22 Jul 2021 01:34:25 GMT
ENV HAPROXY_VERSION=2.2.15
# Thu, 22 Jul 2021 01:34:25 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.15.tar.gz
# Thu, 22 Jul 2021 01:34:25 GMT
ENV HAPROXY_SHA256=48cd0e1cb5de889657cd080fe66cc2ada8198cfece55d63f3a0c011553384cd9
# Thu, 22 Jul 2021 01:35:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 22 Jul 2021 01:35:09 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 01:35:10 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 01:35:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Jul 2021 01:35:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 01:35:11 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:7a50fdd85ff244c1465e71c51354d055e3df0b90ff5faad28cc22d9ecde9daf3`  
		Last Modified: Thu, 22 Jul 2021 00:48:13 GMT  
		Size: 25.8 MB (25760761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05fb34d1ed21b67502665114a7ae60445472fc7bafa620bbf6c79b7df85a01d4`  
		Last Modified: Thu, 22 Jul 2021 01:39:54 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b15e5cf4cb4ed8d7994364c1330f8753dab6faffc8dd0236c41b901e63981554`  
		Last Modified: Thu, 22 Jul 2021 01:40:27 GMT  
		Size: 9.0 MB (9040712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:351a8c9835e3f604cd5db18b86cbc27e55d125813cc0bd87ef73801be8a1f465`  
		Last Modified: Thu, 22 Jul 2021 01:40:26 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cce3640d5c727c8b5ca61886c76b8c770912983132051dd077649f3451510f2`  
		Last Modified: Thu, 22 Jul 2021 01:40:26 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.2.15-alpine`

```console
$ docker pull haproxy@sha256:ee856b7e6b61c677144ec9ab7d3122cf1a5af154915e8b63aa793ac35afb340c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `haproxy:2.2.15-alpine` - linux; amd64

```console
$ docker pull haproxy@sha256:d5079998fb1e5885ae0ec36c8d696df8ab8d94503cedce7b3b848420d02f73eb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.2 MB (9183607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1978a4f77a6bb5a8d5d70b0682e8887bcdddad0b632d78fd1f5bef2afb64c619`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 02:48:50 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 16 Jul 2021 20:21:01 GMT
ENV HAPROXY_VERSION=2.2.15
# Fri, 16 Jul 2021 20:21:01 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.15.tar.gz
# Fri, 16 Jul 2021 20:21:01 GMT
ENV HAPROXY_SHA256=48cd0e1cb5de889657cd080fe66cc2ada8198cfece55d63f3a0c011553384cd9
# Fri, 16 Jul 2021 20:21:53 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 16 Jul 2021 20:21:53 GMT
STOPSIGNAL SIGUSR1
# Fri, 16 Jul 2021 20:21:54 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 16 Jul 2021 20:21:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 16 Jul 2021 20:21:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jul 2021 20:21:55 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7834d945b9e597e693f56fb0f9847718c1732b738a2f4956ab2c1b66c289d90`  
		Last Modified: Sat, 26 Jun 2021 02:56:43 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4503b62662ebb03c72eef87d5e386f25c1f6bf50b26e363a5d79304aada5e21`  
		Last Modified: Fri, 16 Jul 2021 20:25:02 GMT  
		Size: 6.4 MB (6370364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f14e978219962603947faf4154e4b3aef9242dc22050cbed2d8a5fd11faaca`  
		Last Modified: Fri, 16 Jul 2021 20:25:01 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b29b2882ec593a19430c38619e2e746b6f94bb28c4efdf3dcf9e01cef1a8c5f`  
		Last Modified: Fri, 16 Jul 2021 20:25:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.15-alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:c2f46d1b746154bb7f2154ba8040baa8d97049756080123c3f1e10d34ca72dac
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.9 MB (8894324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17cc292ea9ff3bd0e3b2679306110d4be2027b95b66d3c4964ea410bb5af3b57`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:26 GMT
ADD file:c80bc2b093cbc0fc466582ef21cbed377de9fa874aedbf320079525ddacd1200 in / 
# Tue, 15 Jun 2021 22:57:26 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 02:02:51 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 16 Jul 2021 19:51:50 GMT
ENV HAPROXY_VERSION=2.2.15
# Fri, 16 Jul 2021 19:51:50 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.15.tar.gz
# Fri, 16 Jul 2021 19:51:51 GMT
ENV HAPROXY_SHA256=48cd0e1cb5de889657cd080fe66cc2ada8198cfece55d63f3a0c011553384cd9
# Fri, 16 Jul 2021 19:52:19 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 16 Jul 2021 19:52:19 GMT
STOPSIGNAL SIGUSR1
# Fri, 16 Jul 2021 19:52:20 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 16 Jul 2021 19:52:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 16 Jul 2021 19:52:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jul 2021 19:52:22 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:b4c9a0924271af3466de27804af26420eb58da1466e7eaaba127d178b380fea3`  
		Last Modified: Tue, 15 Jun 2021 22:58:47 GMT  
		Size: 2.6 MB (2624382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85fa2947d9cc2655af4fd4aa21641629e791bcaf309a7095db77d309ddd05dfa`  
		Last Modified: Sat, 26 Jun 2021 02:08:45 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd622ad240a50ac5cea62cec763266261c4a7e7381e905683ac71f0c1aa5d77`  
		Last Modified: Fri, 16 Jul 2021 19:54:50 GMT  
		Size: 6.3 MB (6268178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac0a5e3bef02be4409d1fdb918db30ff37d5ee7d605b9f501e6a21c08f65e7c8`  
		Last Modified: Fri, 16 Jul 2021 19:54:46 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20d041211cf66df3bca589f8baf656200aa3f4e34ef0a48506b8d050d7886433`  
		Last Modified: Fri, 16 Jul 2021 19:54:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.15-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:2161bacbb0ff8f69ca9b3407d4a3c03d5604b4e5d1e1a6dcf51dcd3ff8854c3d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8598879 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a233535dd638821a95741fb8ea17f0b70c1576d0340d16dd4e5da1c5b5f2e828`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:05 GMT
ADD file:416a8b507abdc6bdcb22997a4be0a4170796c3f9f77e315b2dbff2b0a212bc68 in / 
# Tue, 15 Jun 2021 23:15:06 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 05:27:42 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 16 Jul 2021 20:37:23 GMT
ENV HAPROXY_VERSION=2.2.15
# Fri, 16 Jul 2021 20:37:23 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.15.tar.gz
# Fri, 16 Jul 2021 20:37:24 GMT
ENV HAPROXY_SHA256=48cd0e1cb5de889657cd080fe66cc2ada8198cfece55d63f3a0c011553384cd9
# Fri, 16 Jul 2021 20:37:49 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 16 Jul 2021 20:37:50 GMT
STOPSIGNAL SIGUSR1
# Fri, 16 Jul 2021 20:37:50 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 16 Jul 2021 20:37:52 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 16 Jul 2021 20:37:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jul 2021 20:37:53 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:136482bf81d1fa351b424ebb8c7e34d15f2c5ed3fc0b66b544b8312bda3d52d9`  
		Last Modified: Tue, 15 Jun 2021 23:16:40 GMT  
		Size: 2.4 MB (2427917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5464af225bd487370319e7125fb2769222c5c7371d1be737936169d2e5b01c`  
		Last Modified: Sat, 26 Jun 2021 05:35:56 GMT  
		Size: 1.2 KB (1196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed027d2048a3392220a7959453fb02a221f21a71faeae4bdc6bb900bb8dc6c7a`  
		Last Modified: Fri, 16 Jul 2021 20:43:21 GMT  
		Size: 6.2 MB (6169197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de1a2718e85f9ad030af5bb6578a28e574813d1f5aebf51194a87039a7dcc0b5`  
		Last Modified: Fri, 16 Jul 2021 20:43:17 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa186376fca912c014c7abd185e349ab2f56cad26b384c1b0cf7267a1f8d2199`  
		Last Modified: Fri, 16 Jul 2021 20:43:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.15-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:9e50b1981ce6323ef61d29566d08b8b4c041bceaf60aac4efde11fae69b54b6f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.1 MB (9100357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f782ea25f9d3e282dc40dbca1555bfa22cdb3f34e4aea852dd1c2d56b2aa77b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 21:44:56 GMT
ADD file:6797caacbfe41bfe44000b39ed017016c6fcc492b3d6557cdaba88536df6c876 in / 
# Tue, 15 Jun 2021 21:44:56 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 02:13:15 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 16 Jul 2021 19:41:13 GMT
ENV HAPROXY_VERSION=2.2.15
# Fri, 16 Jul 2021 19:41:13 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.15.tar.gz
# Fri, 16 Jul 2021 19:41:14 GMT
ENV HAPROXY_SHA256=48cd0e1cb5de889657cd080fe66cc2ada8198cfece55d63f3a0c011553384cd9
# Fri, 16 Jul 2021 19:41:58 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 16 Jul 2021 19:41:58 GMT
STOPSIGNAL SIGUSR1
# Fri, 16 Jul 2021 19:41:59 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 16 Jul 2021 19:41:59 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 16 Jul 2021 19:42:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jul 2021 19:42:00 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:58ab47519297212468320b23b8100fc1b2b96e8d342040806ae509a778a0a07a`  
		Last Modified: Tue, 15 Jun 2021 21:46:03 GMT  
		Size: 2.7 MB (2709626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb8dc96e2a4b7f90ae2dbfca981fe199966b64e3426ca1f742499d46ad1aa357`  
		Last Modified: Sat, 26 Jun 2021 02:21:19 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3633c11f8825cccf4db110e4621f2ad4e5c895799a8a49a4bf810ba919dfa478`  
		Last Modified: Fri, 16 Jul 2021 19:45:31 GMT  
		Size: 6.4 MB (6388965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c877b8aa2303fa413c5d69497fa7fafeceda383b83a55d8580c58a9b922efb1`  
		Last Modified: Fri, 16 Jul 2021 19:45:30 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d71fcd03f304168ee1c375d2b03ca13ba4b6025c18e02f42e99431b5ec1fc77`  
		Last Modified: Fri, 16 Jul 2021 19:45:30 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.15-alpine` - linux; 386

```console
$ docker pull haproxy@sha256:d89cde92e122ae28fc245c341c5e9dbe15dd19aa68f0242b13a911c28013455f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9048078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1456760fc9bbb3df68355f6ff18837db53daa2d2340f9dfab219d72ee07b15cb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 21:38:30 GMT
ADD file:3b0fe1454491bb05e218b090fd461f2fd39546aa4a53eb3f953ee8eae149ac57 in / 
# Tue, 15 Jun 2021 21:38:30 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 01:39:05 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 16 Jul 2021 19:40:49 GMT
ENV HAPROXY_VERSION=2.2.15
# Fri, 16 Jul 2021 19:40:49 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.15.tar.gz
# Fri, 16 Jul 2021 19:40:49 GMT
ENV HAPROXY_SHA256=48cd0e1cb5de889657cd080fe66cc2ada8198cfece55d63f3a0c011553384cd9
# Fri, 16 Jul 2021 19:41:49 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 16 Jul 2021 19:41:49 GMT
STOPSIGNAL SIGUSR1
# Fri, 16 Jul 2021 19:41:49 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 16 Jul 2021 19:41:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 16 Jul 2021 19:41:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jul 2021 19:41:51 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:be21df321efb39c5daf3151073ebff7688e15ea6cd5158878bc9559a5db76ac6`  
		Last Modified: Tue, 15 Jun 2021 21:39:16 GMT  
		Size: 2.8 MB (2820718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc6fe536c8e50a97873c166db7d3b669842dec91d85ce73433028b3b198a1c4`  
		Last Modified: Sat, 26 Jun 2021 01:49:46 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9928b291dd1da6088fd487934595dbe2e599d5413769e858d6405ad7bf4265e`  
		Last Modified: Fri, 16 Jul 2021 19:46:07 GMT  
		Size: 6.2 MB (6225597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d290d72d744b2245d5c6a0b64f0503fb71e9ac292b02e02969d40d2e2c0a3807`  
		Last Modified: Fri, 16 Jul 2021 19:46:06 GMT  
		Size: 447.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e51c7579310e066ebf25d53928150d39ea84e3ca35c08d386bc238dd1f585bdd`  
		Last Modified: Fri, 16 Jul 2021 19:46:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.15-alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:a12fba28fbf006ed034ee0fc7eb0ab26e79a36a99815fd47bc83b8d518fa78d5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9519701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcdfad7039b75be3278562e46e07712e13524244d8a7bef3c63f541e9d82c697`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:27:00 GMT
ADD file:0075aad7a94f0496483442bb2d9fdaa13e9c23087b90638d014b4bc263aa3861 in / 
# Tue, 15 Jun 2021 22:27:03 GMT
CMD ["/bin/sh"]
# Fri, 16 Jul 2021 20:17:57 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 16 Jul 2021 20:27:19 GMT
ENV HAPROXY_VERSION=2.2.15
# Fri, 16 Jul 2021 20:27:22 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.15.tar.gz
# Fri, 16 Jul 2021 20:27:27 GMT
ENV HAPROXY_SHA256=48cd0e1cb5de889657cd080fe66cc2ada8198cfece55d63f3a0c011553384cd9
# Thu, 22 Jul 2021 03:19:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 22 Jul 2021 03:19:18 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 03:19:20 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 03:19:28 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Jul 2021 03:19:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 03:19:39 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:baf144cfb66ebe9df1969f3b90f1c448beff98edc84de1ccb5d6346195a070d4`  
		Last Modified: Tue, 15 Jun 2021 22:27:38 GMT  
		Size: 2.8 MB (2810478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e907663c9428bbbb731a221721c606bad29e54dac6f0dda85d6aa3175a725e`  
		Last Modified: Thu, 22 Jul 2021 03:40:16 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0ffd2888ce89fabb79d101f0f75f1945b0d91d47dd02d1d75bd8bbd85fb3df5`  
		Last Modified: Thu, 22 Jul 2021 03:41:54 GMT  
		Size: 6.7 MB (6707455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50458b4a7a19297ded472eef7e0d0bbb73924ccd421a614293161b85001de8b6`  
		Last Modified: Thu, 22 Jul 2021 03:41:53 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45bc5148f462cfd0d09265d96af1502308d438ba9e02dc9d2a49a8498bc797e9`  
		Last Modified: Thu, 22 Jul 2021 03:41:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.3`

```console
$ docker pull haproxy@sha256:45498d849dd25e32583e0dc49f95c7532238bf25bc4a20a510c1f8439f41e760
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

### `haproxy:2.3` - linux; amd64

```console
$ docker pull haproxy@sha256:68cb03467313a5987f561036fd65e56b3456abceaffb415f16d491085cefa030
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.7 MB (36740622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2284eda222175dceb42433967cda6b39a3d66ae6fec3b819e737811efe6654e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 06:19:17 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 18:35:22 GMT
ENV HAPROXY_VERSION=2.3.12
# Thu, 08 Jul 2021 18:35:22 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.12.tar.gz
# Thu, 08 Jul 2021 18:35:22 GMT
ENV HAPROXY_SHA256=684670d71ffe1ab3f0bfd1be0e55ea9d932732081dd01858b9e351c1a909be3e
# Thu, 08 Jul 2021 18:36:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 08 Jul 2021 18:36:09 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 18:36:09 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 18:36:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 08 Jul 2021 18:36:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 18:36:10 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91332cb81883405a321c1a2d2144bdd0aef8d1c69f90fdf0cf219982161b6e6e`  
		Last Modified: Wed, 23 Jun 2021 06:29:07 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:422cd51572ac35441fa1391d3af4c32782b34e4e0a1f2e4385866af7527fda84`  
		Last Modified: Thu, 08 Jul 2021 18:38:53 GMT  
		Size: 9.6 MB (9592819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e3e85d243f82e23dd5cae540e7c1efde44f005cb9197bf86508d4cc0ca1ab0`  
		Last Modified: Thu, 08 Jul 2021 18:38:51 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d29c924bfb1c6ae4fe5dc24480de3a357adddd7b860250fe2cfcc0d4ce4fa29`  
		Last Modified: Thu, 08 Jul 2021 18:38:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:e86977cfb95dc7493065ff747fe5f88d68f131c5132d204b8ab134f572f8a6ba
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34085775 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1167453fdc9a90b7493a480f833be2ca9ff6b593ea34105c24a0d7a81ac0954`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 22 Jun 2021 23:50:09 GMT
ADD file:78d4ced31112d85490c684f350aceeebfc72a804262c7ad3e033257e3894f5c4 in / 
# Tue, 22 Jun 2021 23:50:11 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:15:11 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 18:59:24 GMT
ENV HAPROXY_VERSION=2.3.12
# Thu, 08 Jul 2021 18:59:25 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.12.tar.gz
# Thu, 08 Jul 2021 18:59:25 GMT
ENV HAPROXY_SHA256=684670d71ffe1ab3f0bfd1be0e55ea9d932732081dd01858b9e351c1a909be3e
# Thu, 08 Jul 2021 19:00:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 08 Jul 2021 19:00:17 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 19:00:17 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 19:00:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 08 Jul 2021 19:00:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 19:00:20 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:532d6df30af5174ac6e1b379c32b8f464d44651ac060376a560c4a76a87704a7`  
		Last Modified: Wed, 23 Jun 2021 00:01:46 GMT  
		Size: 24.9 MB (24878945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48649e3d7de4cd80d3a9a34c725a2935be904ff90e99ea6c8e4bb6e1e7a4eeb7`  
		Last Modified: Wed, 23 Jun 2021 05:24:11 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44e953f92e8b96c10711100856bb7df45e1cf3924244fbe2891b355332345a8b`  
		Last Modified: Thu, 08 Jul 2021 19:02:47 GMT  
		Size: 9.2 MB (9204881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358e52b423b27743d958defdbda6e97f2f0b2a6d13821072dbfc57d239ec63dd`  
		Last Modified: Thu, 08 Jul 2021 19:02:42 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7e14c3f304ab1b81faaad28bb67adf906eedc4885879a2cc7454c8a685ce6f2`  
		Last Modified: Thu, 08 Jul 2021 19:02:42 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:47e7fb65c4b26ae61b23635731c517cbb4c3248cac8b96c8fd5f9b57e33c2c12
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31814170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10c416ce9bbf39065ddd3c2c836636ea04ad2be3131069a37af83ff690af222b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:31 GMT
ADD file:8d200a3bbe985ff355343675c5555852f27550a9e367969df6bc98034efb8fd4 in / 
# Wed, 23 Jun 2021 00:20:31 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:21:41 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 21:30:38 GMT
ENV HAPROXY_VERSION=2.3.12
# Thu, 08 Jul 2021 21:30:38 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.12.tar.gz
# Thu, 08 Jul 2021 21:30:39 GMT
ENV HAPROXY_SHA256=684670d71ffe1ab3f0bfd1be0e55ea9d932732081dd01858b9e351c1a909be3e
# Thu, 08 Jul 2021 21:31:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 08 Jul 2021 21:31:29 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 21:31:29 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 21:31:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 08 Jul 2021 21:31:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 21:31:32 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:8452be1adf00f91570fe21a8e61aaf4c12e014daf67d7de65d984f4e8ecca2f1`  
		Last Modified: Wed, 23 Jun 2021 00:31:49 GMT  
		Size: 22.7 MB (22746055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed1c9c92d0076fd4bf40503e3f47102509a5b99d182f4dd9e81e64d0a7e0b8a`  
		Last Modified: Wed, 23 Jun 2021 05:35:48 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e29791717c1ac2f1b357af6dbe4f820ba1f1335cdcd9da5ae1c892b3702150d`  
		Last Modified: Thu, 08 Jul 2021 21:36:48 GMT  
		Size: 9.1 MB (9066165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4baa85e5af16db5705bcf431bf70b3865e7fb08a35145a6ed4acf33c761c05b`  
		Last Modified: Thu, 08 Jul 2021 21:36:42 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6ec7c40aa4680570686ad7e5049c62b9814f57379ee205ab5b6a71a50027fe`  
		Last Modified: Thu, 08 Jul 2021 21:36:42 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:8f63e361162ffbeb4ac24e1d0e7fc174859a68a9b52434a2452fc819105cc389
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.4 MB (35397233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2eb091ce61f587502b8be5aa71950e7b4450909d98b07424c5ef1f72810018d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:40 GMT
ADD file:beee00b59da720f68e12e2ba2a8134207c80c777ddb4ceb03c71e3e4c3f51c93 in / 
# Tue, 22 Jun 2021 23:49:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 03:19:31 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 19:03:40 GMT
ENV HAPROXY_VERSION=2.3.12
# Thu, 08 Jul 2021 19:03:40 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.12.tar.gz
# Thu, 08 Jul 2021 19:03:40 GMT
ENV HAPROXY_SHA256=684670d71ffe1ab3f0bfd1be0e55ea9d932732081dd01858b9e351c1a909be3e
# Thu, 08 Jul 2021 19:04:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 08 Jul 2021 19:04:22 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 19:04:23 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 19:04:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 08 Jul 2021 19:04:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 19:04:24 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:448f6bf000e31217a7c202c659b03b7f8ac8d3ae6b03ef7a2f8339be2f00ff4a`  
		Last Modified: Tue, 22 Jun 2021 23:55:25 GMT  
		Size: 25.9 MB (25914993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b05ad81dc8a7d67656235988f0e5fb72c374c7d8df44c105b91d712e06c4ac`  
		Last Modified: Wed, 23 Jun 2021 03:26:16 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e124a9856fc99b850f30e5708fb5baccaaa125fae7f2ef5fa5fe4aeaeed13a10`  
		Last Modified: Thu, 08 Jul 2021 19:07:50 GMT  
		Size: 9.5 MB (9480290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9562e4ee7013d30f2a1bc452f925385a02ffa68ee218c4aaada41cd24535e7f`  
		Last Modified: Thu, 08 Jul 2021 19:07:48 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb6ab6d24e5ea6e754e17ece166baf577af85bf4f46da4c0d7842dd4d093350`  
		Last Modified: Thu, 08 Jul 2021 19:07:48 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3` - linux; 386

```console
$ docker pull haproxy@sha256:d7939f77b7c5ef6fe1dceecfd485fef8530b07d1d98df64f8b841fceaed24b63
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37254715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64eb514ee8458d97c56b3982c304bb0fecfb48084ca6b92016cb4c1d6fb5099e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 22 Jun 2021 23:39:35 GMT
ADD file:48f656ac6733911048b3de850490438d0233b3badc11861fca62062d4edfaf40 in / 
# Tue, 22 Jun 2021 23:39:35 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:23:13 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 19:04:35 GMT
ENV HAPROXY_VERSION=2.3.12
# Thu, 08 Jul 2021 19:04:35 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.12.tar.gz
# Thu, 08 Jul 2021 19:04:36 GMT
ENV HAPROXY_SHA256=684670d71ffe1ab3f0bfd1be0e55ea9d932732081dd01858b9e351c1a909be3e
# Thu, 08 Jul 2021 19:05:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 08 Jul 2021 19:05:30 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 19:05:31 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 19:05:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 08 Jul 2021 19:05:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 19:05:32 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:33af2dcb865e65d53cdeb843b67a0ef62151fa32df292293e7c6b0eb728ac5ac`  
		Last Modified: Tue, 22 Jun 2021 23:46:23 GMT  
		Size: 27.8 MB (27797411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a6e4d42b23996eb7d8a1baa85ee19828c2667fd4a2dca6eb1040b266680e9f`  
		Last Modified: Wed, 23 Jun 2021 00:32:00 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37efc86b2e00e507c6d44d17c8a28fbaa2a2cb20540f2c55876f1e6a5d7bdb34`  
		Last Modified: Thu, 08 Jul 2021 19:09:22 GMT  
		Size: 9.5 MB (9455355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86483d8a5986ce2af7872d23e6cf6b4d8ba973bae21385e9c1038b8633823140`  
		Last Modified: Thu, 08 Jul 2021 19:09:20 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324f5e4c45b8bbc90738f03a0fa65575a6f6d2a463de53e087088da1ed237c54`  
		Last Modified: Thu, 08 Jul 2021 19:09:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3` - linux; mips64le

```console
$ docker pull haproxy@sha256:1eda3903211c50314ffe719bf10801c97799020a6f8ddbb268a9958392b96afc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.0 MB (34984503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec569212873529dd3ea1aa0b631406786a12a1f440b80be0242ff67b910df5af`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 22 Jul 2021 00:09:45 GMT
ADD file:1f77b9001c4977ba733be674fc5eb4b85130f1dea8a7b39d545b70f9c107695f in / 
# Thu, 22 Jul 2021 00:09:46 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:07:49 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 22 Jul 2021 01:13:10 GMT
ENV HAPROXY_VERSION=2.3.12
# Thu, 22 Jul 2021 01:13:11 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.12.tar.gz
# Thu, 22 Jul 2021 01:13:11 GMT
ENV HAPROXY_SHA256=684670d71ffe1ab3f0bfd1be0e55ea9d932732081dd01858b9e351c1a909be3e
# Thu, 22 Jul 2021 01:15:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 22 Jul 2021 01:15:30 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 01:15:30 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 01:15:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Jul 2021 01:15:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 01:15:32 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:99ee621d0b0485e9de65aa19604aa2453d19ea7fc86b22c5b77c1bab74e3cb42`  
		Last Modified: Thu, 22 Jul 2021 00:16:11 GMT  
		Size: 25.8 MB (25812771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f444627794f98947a9df95ec5d19b2a1cd6c151ed438982b1dc0b89f5eaf19e`  
		Last Modified: Thu, 22 Jul 2021 01:24:39 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ae90db1e8f355c3b216e7a237c0c0b9b3e5a9417dadcdee7c7472d6252e8279`  
		Last Modified: Thu, 22 Jul 2021 01:25:24 GMT  
		Size: 9.2 MB (9169782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf07251517cbd0fe2633f9c6635f9d32859ea99c32e0c89095556afadd189b45`  
		Last Modified: Thu, 22 Jul 2021 01:25:18 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e71af1c1859745da6b45e4d845faee2c227f6723f2ca4fb65b4e149d72c3ab8`  
		Last Modified: Thu, 22 Jul 2021 01:25:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3` - linux; ppc64le

```console
$ docker pull haproxy@sha256:ed27885da66642999f672d9c5db094925c69276b0eee3ee4d14fa00b60095a6a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40638007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f488fac7200212ad62bd2e4a7c020ce3022d3f7a3b51a759950f4ee331509537`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 22 Jul 2021 00:19:04 GMT
ADD file:3a6bd6ce3eff98b88a13de5d0f26cff0b026f876674204dbad6f84fafcf145b1 in / 
# Thu, 22 Jul 2021 00:19:13 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 02:52:46 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 22 Jul 2021 03:05:30 GMT
ENV HAPROXY_VERSION=2.3.12
# Thu, 22 Jul 2021 03:05:36 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.12.tar.gz
# Thu, 22 Jul 2021 03:05:41 GMT
ENV HAPROXY_SHA256=684670d71ffe1ab3f0bfd1be0e55ea9d932732081dd01858b9e351c1a909be3e
# Thu, 22 Jul 2021 03:10:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 22 Jul 2021 03:10:42 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 03:10:45 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 03:10:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Jul 2021 03:11:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 03:11:09 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:1130517d52da84a09f9465006bddab5e49afd398860890eab6274fd0bff32371`  
		Last Modified: Thu, 22 Jul 2021 00:27:49 GMT  
		Size: 30.6 MB (30553709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251bf3fe1d4bbe9c27e393cd8ddc550b56cec90eb916bf9bec24d657c9f6556f`  
		Last Modified: Thu, 22 Jul 2021 03:40:01 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f76e52cf75d1e0f11ee8c12da9ae491ad953f7b1c029f4ae5321046a3fe36ffe`  
		Last Modified: Thu, 22 Jul 2021 03:41:14 GMT  
		Size: 10.1 MB (10082353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a89b07577129d3e0e985055fc6b1aaa202edecfe70b41374df5b69dcf62bdffd`  
		Last Modified: Thu, 22 Jul 2021 03:41:12 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea6ca41ec8e1799b7ea68480f97ea49e6982e1818babccea975295279242b90`  
		Last Modified: Thu, 22 Jul 2021 03:41:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3` - linux; s390x

```console
$ docker pull haproxy@sha256:cfc9f870a64c4d9af6d5907b431d3d0b5c91db3c2c9e0a230d0c1ff1db8707ac
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35091164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0905fb4f4929e66c54e7f59a933e17ad2f0514f320874e9808375b773a2c3aec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 22 Jul 2021 00:42:45 GMT
ADD file:1ab999eb6f80d8ce91ce3a173e23fd2710f2779117bba29037eaa82aadcbf6ed in / 
# Thu, 22 Jul 2021 00:42:48 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:30:19 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 22 Jul 2021 01:33:02 GMT
ENV HAPROXY_VERSION=2.3.12
# Thu, 22 Jul 2021 01:33:03 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.12.tar.gz
# Thu, 22 Jul 2021 01:33:03 GMT
ENV HAPROXY_SHA256=684670d71ffe1ab3f0bfd1be0e55ea9d932732081dd01858b9e351c1a909be3e
# Thu, 22 Jul 2021 01:33:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 22 Jul 2021 01:33:43 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 01:33:43 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 01:33:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Jul 2021 01:33:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 01:33:45 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:7a50fdd85ff244c1465e71c51354d055e3df0b90ff5faad28cc22d9ecde9daf3`  
		Last Modified: Thu, 22 Jul 2021 00:48:13 GMT  
		Size: 25.8 MB (25760761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05fb34d1ed21b67502665114a7ae60445472fc7bafa620bbf6c79b7df85a01d4`  
		Last Modified: Thu, 22 Jul 2021 01:39:54 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f186c5b9325a025e10eb09c2a960452fb9a23e281015aa36758ac1e6e789360d`  
		Last Modified: Thu, 22 Jul 2021 01:40:18 GMT  
		Size: 9.3 MB (9328455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dacc4ee1b6b54c40402ba28cff0c1524afa0a9b35652093dc49d0daf91b0d17b`  
		Last Modified: Thu, 22 Jul 2021 01:40:17 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde7a6d82d80dde0d3298b8d9318983ab15d95e844197c47a0e021fa550fc739`  
		Last Modified: Thu, 22 Jul 2021 01:40:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.3-alpine`

```console
$ docker pull haproxy@sha256:e73d0f8f178f0844e1f9c1cb41d698674a0b397ce4c2e8938409048c397ef5d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `haproxy:2.3-alpine` - linux; amd64

```console
$ docker pull haproxy@sha256:139bd6b31d2137e1ae7854ac79c4fdf86218da658584cc57e10300f9fe4388f2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9502461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ed504bfb421c4c6bced9b1e5d37c8b9586501626bd94d66975ecd76bba5b4eb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 02:48:50 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 18:36:22 GMT
ENV HAPROXY_VERSION=2.3.12
# Thu, 08 Jul 2021 18:36:22 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.12.tar.gz
# Thu, 08 Jul 2021 18:36:22 GMT
ENV HAPROXY_SHA256=684670d71ffe1ab3f0bfd1be0e55ea9d932732081dd01858b9e351c1a909be3e
# Thu, 08 Jul 2021 18:37:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 08 Jul 2021 18:37:15 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 18:37:16 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 18:37:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 08 Jul 2021 18:37:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 18:37:17 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7834d945b9e597e693f56fb0f9847718c1732b738a2f4956ab2c1b66c289d90`  
		Last Modified: Sat, 26 Jun 2021 02:56:43 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bde4c23b6a12e07b03235202edde2b22cd6056191579930c9b5e2423c6169c0`  
		Last Modified: Thu, 08 Jul 2021 18:39:04 GMT  
		Size: 6.7 MB (6689221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a159a5ad1f5aa7e876850c413d5177cd91e30b9921dadf7c794cd63203617ff5`  
		Last Modified: Thu, 08 Jul 2021 18:39:02 GMT  
		Size: 447.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dc77dcbd1fb5c06cce39d05e264b0d3784ea463bad1201596d0279a39210653`  
		Last Modified: Thu, 08 Jul 2021 18:39:02 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3-alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:528b6a86af209e4e57fcc3d1068a754b097ca7db526885a2a3af2ac8c522c702
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.2 MB (9238914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d903fa39287b915771659e02df1e6eb57fd4e5038def5d079fffc172582f0f3c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:26 GMT
ADD file:c80bc2b093cbc0fc466582ef21cbed377de9fa874aedbf320079525ddacd1200 in / 
# Tue, 15 Jun 2021 22:57:26 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 02:02:51 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 19:08:28 GMT
ENV HAPROXY_VERSION=2.3.12
# Thu, 08 Jul 2021 19:08:28 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.12.tar.gz
# Thu, 08 Jul 2021 19:08:29 GMT
ENV HAPROXY_SHA256=684670d71ffe1ab3f0bfd1be0e55ea9d932732081dd01858b9e351c1a909be3e
# Thu, 08 Jul 2021 19:08:55 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 08 Jul 2021 19:08:55 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 19:08:56 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 19:08:57 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 08 Jul 2021 19:08:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 19:08:58 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:b4c9a0924271af3466de27804af26420eb58da1466e7eaaba127d178b380fea3`  
		Last Modified: Tue, 15 Jun 2021 22:58:47 GMT  
		Size: 2.6 MB (2624382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85fa2947d9cc2655af4fd4aa21641629e791bcaf309a7095db77d309ddd05dfa`  
		Last Modified: Sat, 26 Jun 2021 02:08:45 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ebafa2c1c2a2a178662adfeb6404a20f4d7d6b0f15fd1dfe06780f9763fdb5`  
		Last Modified: Thu, 08 Jul 2021 19:11:26 GMT  
		Size: 6.6 MB (6612764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d79d3a60be51f185501824d40e726ea744a7886f06d46d0af8c38064598b793b`  
		Last Modified: Thu, 08 Jul 2021 19:11:21 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c6e4b94a2d124e63e0975574ec4d855cdb27a44cfe005edf2bdfcf9cbb46d4a`  
		Last Modified: Thu, 08 Jul 2021 19:11:21 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:c6bee7a2156e5aa328f86686945429fe44a83dcfa6a1e0026e2c2ceb8cf23b4a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.9 MB (8939198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2a1fead38b60d97ee0d89f31009b123ad573c9818938780ac564b2398381f2c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:05 GMT
ADD file:416a8b507abdc6bdcb22997a4be0a4170796c3f9f77e315b2dbff2b0a212bc68 in / 
# Tue, 15 Jun 2021 23:15:06 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 05:27:42 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 21:31:44 GMT
ENV HAPROXY_VERSION=2.3.12
# Thu, 08 Jul 2021 21:31:45 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.12.tar.gz
# Thu, 08 Jul 2021 21:31:45 GMT
ENV HAPROXY_SHA256=684670d71ffe1ab3f0bfd1be0e55ea9d932732081dd01858b9e351c1a909be3e
# Thu, 08 Jul 2021 21:32:11 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 08 Jul 2021 21:32:11 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 21:32:12 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 21:32:14 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 08 Jul 2021 21:32:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 21:32:14 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:136482bf81d1fa351b424ebb8c7e34d15f2c5ed3fc0b66b544b8312bda3d52d9`  
		Last Modified: Tue, 15 Jun 2021 23:16:40 GMT  
		Size: 2.4 MB (2427917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5464af225bd487370319e7125fb2769222c5c7371d1be737936169d2e5b01c`  
		Last Modified: Sat, 26 Jun 2021 05:35:56 GMT  
		Size: 1.2 KB (1196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e101eaa240968a0b1dc69dc1781b7243c4767d7f2974b68b31bcad82dc4e41a5`  
		Last Modified: Thu, 08 Jul 2021 21:37:04 GMT  
		Size: 6.5 MB (6509513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:952d669a4a2b908243b212ef3a03f745db60ca164b86923aa3119f31120f2bb1`  
		Last Modified: Thu, 08 Jul 2021 21:36:59 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:206b57e75e9c72c96f79dba44cb8d88cf41dc41c53e29393648012c7f8794179`  
		Last Modified: Thu, 08 Jul 2021 21:36:59 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:bdddad96e0dcee3f6d26e8d608c8c9dab9c4e4112a15534de812e9eaeaa37b6e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9423882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b85f37a7bc4a1cfa1e8d634c5654956b82640feb78c5cd27cd71029b00cdc62`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 21:44:56 GMT
ADD file:6797caacbfe41bfe44000b39ed017016c6fcc492b3d6557cdaba88536df6c876 in / 
# Tue, 15 Jun 2021 21:44:56 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 02:13:15 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 19:04:31 GMT
ENV HAPROXY_VERSION=2.3.12
# Thu, 08 Jul 2021 19:04:32 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.12.tar.gz
# Thu, 08 Jul 2021 19:04:32 GMT
ENV HAPROXY_SHA256=684670d71ffe1ab3f0bfd1be0e55ea9d932732081dd01858b9e351c1a909be3e
# Thu, 08 Jul 2021 19:05:17 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 08 Jul 2021 19:05:17 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 19:05:17 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 19:05:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 08 Jul 2021 19:05:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 19:05:18 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:58ab47519297212468320b23b8100fc1b2b96e8d342040806ae509a778a0a07a`  
		Last Modified: Tue, 15 Jun 2021 21:46:03 GMT  
		Size: 2.7 MB (2709626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb8dc96e2a4b7f90ae2dbfca981fe199966b64e3426ca1f742499d46ad1aa357`  
		Last Modified: Sat, 26 Jun 2021 02:21:19 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08349c2a8842ea189edf883d942e7fb370a090a02afc4fe538fbe2854e2e4a3a`  
		Last Modified: Thu, 08 Jul 2021 19:08:03 GMT  
		Size: 6.7 MB (6712490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d9b75df55dfc9233984444070416de967601aef766b59b9cd991fd9ddc51f6`  
		Last Modified: Thu, 08 Jul 2021 19:08:01 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1026e4b45765f53b4736f68cb63f67d150185fb95bcd3b69b45f0767726ee85a`  
		Last Modified: Thu, 08 Jul 2021 19:08:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3-alpine` - linux; 386

```console
$ docker pull haproxy@sha256:d70bf9a3aa05a06cc82d51cf2d6f545537b115649124650caef84b6e8eb824dd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9379406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c741bad0b30f51eb5d7a209145c2b1031c9b92e0efe77a83898cc18df44d3228`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 21:38:30 GMT
ADD file:3b0fe1454491bb05e218b090fd461f2fd39546aa4a53eb3f953ee8eae149ac57 in / 
# Tue, 15 Jun 2021 21:38:30 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 01:39:05 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 19:05:38 GMT
ENV HAPROXY_VERSION=2.3.12
# Thu, 08 Jul 2021 19:05:38 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.12.tar.gz
# Thu, 08 Jul 2021 19:05:38 GMT
ENV HAPROXY_SHA256=684670d71ffe1ab3f0bfd1be0e55ea9d932732081dd01858b9e351c1a909be3e
# Thu, 08 Jul 2021 19:06:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 08 Jul 2021 19:06:43 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 19:06:44 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 19:06:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 08 Jul 2021 19:06:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 19:06:45 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:be21df321efb39c5daf3151073ebff7688e15ea6cd5158878bc9559a5db76ac6`  
		Last Modified: Tue, 15 Jun 2021 21:39:16 GMT  
		Size: 2.8 MB (2820718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc6fe536c8e50a97873c166db7d3b669842dec91d85ce73433028b3b198a1c4`  
		Last Modified: Sat, 26 Jun 2021 01:49:46 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f1db007c417f267ab0d29cbddfedc24ac2c97f03e36050e3ba3ae75762fe82d`  
		Last Modified: Thu, 08 Jul 2021 19:09:35 GMT  
		Size: 6.6 MB (6556921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05dcba06e39fe66f5f431b378324191f1a8d349b1ad03fbc8f2070f2e3c931a4`  
		Last Modified: Thu, 08 Jul 2021 19:09:33 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49184c0500278ba2af56c16b80d0717741e606a00bd70b0dd10ab822156e5206`  
		Last Modified: Thu, 08 Jul 2021 19:09:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3-alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:3595f780d567d526bcc5384a0974c1a82d06e11424112acb6d7fced16219ba1a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9858364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a45467e080dc275cdbd86aea3113497b239f8022cc43bf2ba163712ea8db5b6f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:27:00 GMT
ADD file:0075aad7a94f0496483442bb2d9fdaa13e9c23087b90638d014b4bc263aa3861 in / 
# Tue, 15 Jun 2021 22:27:03 GMT
CMD ["/bin/sh"]
# Fri, 16 Jul 2021 20:17:57 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 16 Jul 2021 20:21:16 GMT
ENV HAPROXY_VERSION=2.3.12
# Fri, 16 Jul 2021 20:21:19 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.12.tar.gz
# Fri, 16 Jul 2021 20:21:25 GMT
ENV HAPROXY_SHA256=684670d71ffe1ab3f0bfd1be0e55ea9d932732081dd01858b9e351c1a909be3e
# Thu, 22 Jul 2021 03:12:05 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 22 Jul 2021 03:12:12 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 03:12:15 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 03:12:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Jul 2021 03:12:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 03:12:39 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:baf144cfb66ebe9df1969f3b90f1c448beff98edc84de1ccb5d6346195a070d4`  
		Last Modified: Tue, 15 Jun 2021 22:27:38 GMT  
		Size: 2.8 MB (2810478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e907663c9428bbbb731a221721c606bad29e54dac6f0dda85d6aa3175a725e`  
		Last Modified: Thu, 22 Jul 2021 03:40:16 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0008e4d1138d3cc9a9b5870cccefa199a25ed8006dc5dca6270cb1a7888e0d3c`  
		Last Modified: Thu, 22 Jul 2021 03:41:27 GMT  
		Size: 7.0 MB (7046114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f798460f1147e4b49ead0f482ca43ceede007cb949f979322a687b184e8ad5e`  
		Last Modified: Thu, 22 Jul 2021 03:41:26 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5caa03e44179cf876a689b69c698cd0f3bdf49f41a9ee874ce3f954d440f8bb`  
		Last Modified: Thu, 22 Jul 2021 03:41:26 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3-alpine` - linux; s390x

```console
$ docker pull haproxy@sha256:d8002e556915178004debf14488aa6b7e820edbbc4e51471336ba90925a46971
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9259665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d35ad497512239f4a077e815769908cf9d12f272fb7d41abae65c31d78fd5e02`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:54:24 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 23 Apr 2021 20:43:09 GMT
ENV HAPROXY_VERSION=2.3.10
# Fri, 23 Apr 2021 20:43:10 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Fri, 23 Apr 2021 20:43:11 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Fri, 23 Apr 2021 20:43:57 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 23 Apr 2021 20:43:58 GMT
STOPSIGNAL SIGUSR1
# Fri, 23 Apr 2021 20:43:58 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 23 Apr 2021 20:43:59 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 20:43:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 20:43:59 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267275aba58470c82626189a59be76cd169bd245568e2f2545ed1ee64ff8a8ff`  
		Last Modified: Wed, 14 Apr 2021 20:59:06 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aac9cf42616b874dc26fc410c1d0b7ddd5b5acdc32829cab01df78d6a831e01`  
		Last Modified: Fri, 23 Apr 2021 20:45:18 GMT  
		Size: 6.7 MB (6655259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13309a7e4b19e568f7683f6a8dbc48ce6d73e5f6e8ee693c8bd979a4a5774956`  
		Last Modified: Fri, 23 Apr 2021 20:45:17 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59770393e0a5b1867600ef163090de4e39b9733dcaea56ae6d84ebce64f759f`  
		Last Modified: Fri, 23 Apr 2021 20:45:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.3.12`

```console
$ docker pull haproxy@sha256:45498d849dd25e32583e0dc49f95c7532238bf25bc4a20a510c1f8439f41e760
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

### `haproxy:2.3.12` - linux; amd64

```console
$ docker pull haproxy@sha256:68cb03467313a5987f561036fd65e56b3456abceaffb415f16d491085cefa030
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.7 MB (36740622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2284eda222175dceb42433967cda6b39a3d66ae6fec3b819e737811efe6654e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 06:19:17 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 18:35:22 GMT
ENV HAPROXY_VERSION=2.3.12
# Thu, 08 Jul 2021 18:35:22 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.12.tar.gz
# Thu, 08 Jul 2021 18:35:22 GMT
ENV HAPROXY_SHA256=684670d71ffe1ab3f0bfd1be0e55ea9d932732081dd01858b9e351c1a909be3e
# Thu, 08 Jul 2021 18:36:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 08 Jul 2021 18:36:09 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 18:36:09 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 18:36:10 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 08 Jul 2021 18:36:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 18:36:10 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91332cb81883405a321c1a2d2144bdd0aef8d1c69f90fdf0cf219982161b6e6e`  
		Last Modified: Wed, 23 Jun 2021 06:29:07 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:422cd51572ac35441fa1391d3af4c32782b34e4e0a1f2e4385866af7527fda84`  
		Last Modified: Thu, 08 Jul 2021 18:38:53 GMT  
		Size: 9.6 MB (9592819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e3e85d243f82e23dd5cae540e7c1efde44f005cb9197bf86508d4cc0ca1ab0`  
		Last Modified: Thu, 08 Jul 2021 18:38:51 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d29c924bfb1c6ae4fe5dc24480de3a357adddd7b860250fe2cfcc0d4ce4fa29`  
		Last Modified: Thu, 08 Jul 2021 18:38:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.12` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:e86977cfb95dc7493065ff747fe5f88d68f131c5132d204b8ab134f572f8a6ba
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34085775 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1167453fdc9a90b7493a480f833be2ca9ff6b593ea34105c24a0d7a81ac0954`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 22 Jun 2021 23:50:09 GMT
ADD file:78d4ced31112d85490c684f350aceeebfc72a804262c7ad3e033257e3894f5c4 in / 
# Tue, 22 Jun 2021 23:50:11 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:15:11 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 18:59:24 GMT
ENV HAPROXY_VERSION=2.3.12
# Thu, 08 Jul 2021 18:59:25 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.12.tar.gz
# Thu, 08 Jul 2021 18:59:25 GMT
ENV HAPROXY_SHA256=684670d71ffe1ab3f0bfd1be0e55ea9d932732081dd01858b9e351c1a909be3e
# Thu, 08 Jul 2021 19:00:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 08 Jul 2021 19:00:17 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 19:00:17 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 19:00:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 08 Jul 2021 19:00:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 19:00:20 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:532d6df30af5174ac6e1b379c32b8f464d44651ac060376a560c4a76a87704a7`  
		Last Modified: Wed, 23 Jun 2021 00:01:46 GMT  
		Size: 24.9 MB (24878945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48649e3d7de4cd80d3a9a34c725a2935be904ff90e99ea6c8e4bb6e1e7a4eeb7`  
		Last Modified: Wed, 23 Jun 2021 05:24:11 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44e953f92e8b96c10711100856bb7df45e1cf3924244fbe2891b355332345a8b`  
		Last Modified: Thu, 08 Jul 2021 19:02:47 GMT  
		Size: 9.2 MB (9204881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358e52b423b27743d958defdbda6e97f2f0b2a6d13821072dbfc57d239ec63dd`  
		Last Modified: Thu, 08 Jul 2021 19:02:42 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7e14c3f304ab1b81faaad28bb67adf906eedc4885879a2cc7454c8a685ce6f2`  
		Last Modified: Thu, 08 Jul 2021 19:02:42 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.12` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:47e7fb65c4b26ae61b23635731c517cbb4c3248cac8b96c8fd5f9b57e33c2c12
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31814170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10c416ce9bbf39065ddd3c2c836636ea04ad2be3131069a37af83ff690af222b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:31 GMT
ADD file:8d200a3bbe985ff355343675c5555852f27550a9e367969df6bc98034efb8fd4 in / 
# Wed, 23 Jun 2021 00:20:31 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:21:41 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 21:30:38 GMT
ENV HAPROXY_VERSION=2.3.12
# Thu, 08 Jul 2021 21:30:38 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.12.tar.gz
# Thu, 08 Jul 2021 21:30:39 GMT
ENV HAPROXY_SHA256=684670d71ffe1ab3f0bfd1be0e55ea9d932732081dd01858b9e351c1a909be3e
# Thu, 08 Jul 2021 21:31:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 08 Jul 2021 21:31:29 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 21:31:29 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 21:31:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 08 Jul 2021 21:31:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 21:31:32 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:8452be1adf00f91570fe21a8e61aaf4c12e014daf67d7de65d984f4e8ecca2f1`  
		Last Modified: Wed, 23 Jun 2021 00:31:49 GMT  
		Size: 22.7 MB (22746055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed1c9c92d0076fd4bf40503e3f47102509a5b99d182f4dd9e81e64d0a7e0b8a`  
		Last Modified: Wed, 23 Jun 2021 05:35:48 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e29791717c1ac2f1b357af6dbe4f820ba1f1335cdcd9da5ae1c892b3702150d`  
		Last Modified: Thu, 08 Jul 2021 21:36:48 GMT  
		Size: 9.1 MB (9066165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4baa85e5af16db5705bcf431bf70b3865e7fb08a35145a6ed4acf33c761c05b`  
		Last Modified: Thu, 08 Jul 2021 21:36:42 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6ec7c40aa4680570686ad7e5049c62b9814f57379ee205ab5b6a71a50027fe`  
		Last Modified: Thu, 08 Jul 2021 21:36:42 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.12` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:8f63e361162ffbeb4ac24e1d0e7fc174859a68a9b52434a2452fc819105cc389
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.4 MB (35397233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2eb091ce61f587502b8be5aa71950e7b4450909d98b07424c5ef1f72810018d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:40 GMT
ADD file:beee00b59da720f68e12e2ba2a8134207c80c777ddb4ceb03c71e3e4c3f51c93 in / 
# Tue, 22 Jun 2021 23:49:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 03:19:31 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 19:03:40 GMT
ENV HAPROXY_VERSION=2.3.12
# Thu, 08 Jul 2021 19:03:40 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.12.tar.gz
# Thu, 08 Jul 2021 19:03:40 GMT
ENV HAPROXY_SHA256=684670d71ffe1ab3f0bfd1be0e55ea9d932732081dd01858b9e351c1a909be3e
# Thu, 08 Jul 2021 19:04:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 08 Jul 2021 19:04:22 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 19:04:23 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 19:04:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 08 Jul 2021 19:04:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 19:04:24 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:448f6bf000e31217a7c202c659b03b7f8ac8d3ae6b03ef7a2f8339be2f00ff4a`  
		Last Modified: Tue, 22 Jun 2021 23:55:25 GMT  
		Size: 25.9 MB (25914993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b05ad81dc8a7d67656235988f0e5fb72c374c7d8df44c105b91d712e06c4ac`  
		Last Modified: Wed, 23 Jun 2021 03:26:16 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e124a9856fc99b850f30e5708fb5baccaaa125fae7f2ef5fa5fe4aeaeed13a10`  
		Last Modified: Thu, 08 Jul 2021 19:07:50 GMT  
		Size: 9.5 MB (9480290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9562e4ee7013d30f2a1bc452f925385a02ffa68ee218c4aaada41cd24535e7f`  
		Last Modified: Thu, 08 Jul 2021 19:07:48 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb6ab6d24e5ea6e754e17ece166baf577af85bf4f46da4c0d7842dd4d093350`  
		Last Modified: Thu, 08 Jul 2021 19:07:48 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.12` - linux; 386

```console
$ docker pull haproxy@sha256:d7939f77b7c5ef6fe1dceecfd485fef8530b07d1d98df64f8b841fceaed24b63
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37254715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64eb514ee8458d97c56b3982c304bb0fecfb48084ca6b92016cb4c1d6fb5099e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 22 Jun 2021 23:39:35 GMT
ADD file:48f656ac6733911048b3de850490438d0233b3badc11861fca62062d4edfaf40 in / 
# Tue, 22 Jun 2021 23:39:35 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:23:13 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 19:04:35 GMT
ENV HAPROXY_VERSION=2.3.12
# Thu, 08 Jul 2021 19:04:35 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.12.tar.gz
# Thu, 08 Jul 2021 19:04:36 GMT
ENV HAPROXY_SHA256=684670d71ffe1ab3f0bfd1be0e55ea9d932732081dd01858b9e351c1a909be3e
# Thu, 08 Jul 2021 19:05:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 08 Jul 2021 19:05:30 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 19:05:31 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 19:05:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 08 Jul 2021 19:05:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 19:05:32 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:33af2dcb865e65d53cdeb843b67a0ef62151fa32df292293e7c6b0eb728ac5ac`  
		Last Modified: Tue, 22 Jun 2021 23:46:23 GMT  
		Size: 27.8 MB (27797411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a6e4d42b23996eb7d8a1baa85ee19828c2667fd4a2dca6eb1040b266680e9f`  
		Last Modified: Wed, 23 Jun 2021 00:32:00 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37efc86b2e00e507c6d44d17c8a28fbaa2a2cb20540f2c55876f1e6a5d7bdb34`  
		Last Modified: Thu, 08 Jul 2021 19:09:22 GMT  
		Size: 9.5 MB (9455355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86483d8a5986ce2af7872d23e6cf6b4d8ba973bae21385e9c1038b8633823140`  
		Last Modified: Thu, 08 Jul 2021 19:09:20 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324f5e4c45b8bbc90738f03a0fa65575a6f6d2a463de53e087088da1ed237c54`  
		Last Modified: Thu, 08 Jul 2021 19:09:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.12` - linux; mips64le

```console
$ docker pull haproxy@sha256:1eda3903211c50314ffe719bf10801c97799020a6f8ddbb268a9958392b96afc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.0 MB (34984503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec569212873529dd3ea1aa0b631406786a12a1f440b80be0242ff67b910df5af`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 22 Jul 2021 00:09:45 GMT
ADD file:1f77b9001c4977ba733be674fc5eb4b85130f1dea8a7b39d545b70f9c107695f in / 
# Thu, 22 Jul 2021 00:09:46 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:07:49 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 22 Jul 2021 01:13:10 GMT
ENV HAPROXY_VERSION=2.3.12
# Thu, 22 Jul 2021 01:13:11 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.12.tar.gz
# Thu, 22 Jul 2021 01:13:11 GMT
ENV HAPROXY_SHA256=684670d71ffe1ab3f0bfd1be0e55ea9d932732081dd01858b9e351c1a909be3e
# Thu, 22 Jul 2021 01:15:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 22 Jul 2021 01:15:30 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 01:15:30 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 01:15:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Jul 2021 01:15:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 01:15:32 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:99ee621d0b0485e9de65aa19604aa2453d19ea7fc86b22c5b77c1bab74e3cb42`  
		Last Modified: Thu, 22 Jul 2021 00:16:11 GMT  
		Size: 25.8 MB (25812771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f444627794f98947a9df95ec5d19b2a1cd6c151ed438982b1dc0b89f5eaf19e`  
		Last Modified: Thu, 22 Jul 2021 01:24:39 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ae90db1e8f355c3b216e7a237c0c0b9b3e5a9417dadcdee7c7472d6252e8279`  
		Last Modified: Thu, 22 Jul 2021 01:25:24 GMT  
		Size: 9.2 MB (9169782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf07251517cbd0fe2633f9c6635f9d32859ea99c32e0c89095556afadd189b45`  
		Last Modified: Thu, 22 Jul 2021 01:25:18 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e71af1c1859745da6b45e4d845faee2c227f6723f2ca4fb65b4e149d72c3ab8`  
		Last Modified: Thu, 22 Jul 2021 01:25:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.12` - linux; ppc64le

```console
$ docker pull haproxy@sha256:ed27885da66642999f672d9c5db094925c69276b0eee3ee4d14fa00b60095a6a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40638007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f488fac7200212ad62bd2e4a7c020ce3022d3f7a3b51a759950f4ee331509537`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 22 Jul 2021 00:19:04 GMT
ADD file:3a6bd6ce3eff98b88a13de5d0f26cff0b026f876674204dbad6f84fafcf145b1 in / 
# Thu, 22 Jul 2021 00:19:13 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 02:52:46 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 22 Jul 2021 03:05:30 GMT
ENV HAPROXY_VERSION=2.3.12
# Thu, 22 Jul 2021 03:05:36 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.12.tar.gz
# Thu, 22 Jul 2021 03:05:41 GMT
ENV HAPROXY_SHA256=684670d71ffe1ab3f0bfd1be0e55ea9d932732081dd01858b9e351c1a909be3e
# Thu, 22 Jul 2021 03:10:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 22 Jul 2021 03:10:42 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 03:10:45 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 03:10:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Jul 2021 03:11:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 03:11:09 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:1130517d52da84a09f9465006bddab5e49afd398860890eab6274fd0bff32371`  
		Last Modified: Thu, 22 Jul 2021 00:27:49 GMT  
		Size: 30.6 MB (30553709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251bf3fe1d4bbe9c27e393cd8ddc550b56cec90eb916bf9bec24d657c9f6556f`  
		Last Modified: Thu, 22 Jul 2021 03:40:01 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f76e52cf75d1e0f11ee8c12da9ae491ad953f7b1c029f4ae5321046a3fe36ffe`  
		Last Modified: Thu, 22 Jul 2021 03:41:14 GMT  
		Size: 10.1 MB (10082353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a89b07577129d3e0e985055fc6b1aaa202edecfe70b41374df5b69dcf62bdffd`  
		Last Modified: Thu, 22 Jul 2021 03:41:12 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea6ca41ec8e1799b7ea68480f97ea49e6982e1818babccea975295279242b90`  
		Last Modified: Thu, 22 Jul 2021 03:41:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.12` - linux; s390x

```console
$ docker pull haproxy@sha256:cfc9f870a64c4d9af6d5907b431d3d0b5c91db3c2c9e0a230d0c1ff1db8707ac
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35091164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0905fb4f4929e66c54e7f59a933e17ad2f0514f320874e9808375b773a2c3aec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 22 Jul 2021 00:42:45 GMT
ADD file:1ab999eb6f80d8ce91ce3a173e23fd2710f2779117bba29037eaa82aadcbf6ed in / 
# Thu, 22 Jul 2021 00:42:48 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:30:19 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 22 Jul 2021 01:33:02 GMT
ENV HAPROXY_VERSION=2.3.12
# Thu, 22 Jul 2021 01:33:03 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.12.tar.gz
# Thu, 22 Jul 2021 01:33:03 GMT
ENV HAPROXY_SHA256=684670d71ffe1ab3f0bfd1be0e55ea9d932732081dd01858b9e351c1a909be3e
# Thu, 22 Jul 2021 01:33:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 22 Jul 2021 01:33:43 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 01:33:43 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 01:33:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Jul 2021 01:33:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 01:33:45 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:7a50fdd85ff244c1465e71c51354d055e3df0b90ff5faad28cc22d9ecde9daf3`  
		Last Modified: Thu, 22 Jul 2021 00:48:13 GMT  
		Size: 25.8 MB (25760761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05fb34d1ed21b67502665114a7ae60445472fc7bafa620bbf6c79b7df85a01d4`  
		Last Modified: Thu, 22 Jul 2021 01:39:54 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f186c5b9325a025e10eb09c2a960452fb9a23e281015aa36758ac1e6e789360d`  
		Last Modified: Thu, 22 Jul 2021 01:40:18 GMT  
		Size: 9.3 MB (9328455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dacc4ee1b6b54c40402ba28cff0c1524afa0a9b35652093dc49d0daf91b0d17b`  
		Last Modified: Thu, 22 Jul 2021 01:40:17 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde7a6d82d80dde0d3298b8d9318983ab15d95e844197c47a0e021fa550fc739`  
		Last Modified: Thu, 22 Jul 2021 01:40:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.3.12-alpine`

```console
$ docker pull haproxy@sha256:fbd45002c6eca233454085a5671221c44800a766a05d56e92cc1d132bb8c5e7c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `haproxy:2.3.12-alpine` - linux; amd64

```console
$ docker pull haproxy@sha256:139bd6b31d2137e1ae7854ac79c4fdf86218da658584cc57e10300f9fe4388f2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9502461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ed504bfb421c4c6bced9b1e5d37c8b9586501626bd94d66975ecd76bba5b4eb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 02:48:50 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 18:36:22 GMT
ENV HAPROXY_VERSION=2.3.12
# Thu, 08 Jul 2021 18:36:22 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.12.tar.gz
# Thu, 08 Jul 2021 18:36:22 GMT
ENV HAPROXY_SHA256=684670d71ffe1ab3f0bfd1be0e55ea9d932732081dd01858b9e351c1a909be3e
# Thu, 08 Jul 2021 18:37:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 08 Jul 2021 18:37:15 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 18:37:16 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 18:37:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 08 Jul 2021 18:37:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 18:37:17 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7834d945b9e597e693f56fb0f9847718c1732b738a2f4956ab2c1b66c289d90`  
		Last Modified: Sat, 26 Jun 2021 02:56:43 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bde4c23b6a12e07b03235202edde2b22cd6056191579930c9b5e2423c6169c0`  
		Last Modified: Thu, 08 Jul 2021 18:39:04 GMT  
		Size: 6.7 MB (6689221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a159a5ad1f5aa7e876850c413d5177cd91e30b9921dadf7c794cd63203617ff5`  
		Last Modified: Thu, 08 Jul 2021 18:39:02 GMT  
		Size: 447.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dc77dcbd1fb5c06cce39d05e264b0d3784ea463bad1201596d0279a39210653`  
		Last Modified: Thu, 08 Jul 2021 18:39:02 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.12-alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:528b6a86af209e4e57fcc3d1068a754b097ca7db526885a2a3af2ac8c522c702
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.2 MB (9238914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d903fa39287b915771659e02df1e6eb57fd4e5038def5d079fffc172582f0f3c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:26 GMT
ADD file:c80bc2b093cbc0fc466582ef21cbed377de9fa874aedbf320079525ddacd1200 in / 
# Tue, 15 Jun 2021 22:57:26 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 02:02:51 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 19:08:28 GMT
ENV HAPROXY_VERSION=2.3.12
# Thu, 08 Jul 2021 19:08:28 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.12.tar.gz
# Thu, 08 Jul 2021 19:08:29 GMT
ENV HAPROXY_SHA256=684670d71ffe1ab3f0bfd1be0e55ea9d932732081dd01858b9e351c1a909be3e
# Thu, 08 Jul 2021 19:08:55 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 08 Jul 2021 19:08:55 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 19:08:56 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 19:08:57 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 08 Jul 2021 19:08:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 19:08:58 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:b4c9a0924271af3466de27804af26420eb58da1466e7eaaba127d178b380fea3`  
		Last Modified: Tue, 15 Jun 2021 22:58:47 GMT  
		Size: 2.6 MB (2624382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85fa2947d9cc2655af4fd4aa21641629e791bcaf309a7095db77d309ddd05dfa`  
		Last Modified: Sat, 26 Jun 2021 02:08:45 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ebafa2c1c2a2a178662adfeb6404a20f4d7d6b0f15fd1dfe06780f9763fdb5`  
		Last Modified: Thu, 08 Jul 2021 19:11:26 GMT  
		Size: 6.6 MB (6612764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d79d3a60be51f185501824d40e726ea744a7886f06d46d0af8c38064598b793b`  
		Last Modified: Thu, 08 Jul 2021 19:11:21 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c6e4b94a2d124e63e0975574ec4d855cdb27a44cfe005edf2bdfcf9cbb46d4a`  
		Last Modified: Thu, 08 Jul 2021 19:11:21 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.12-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:c6bee7a2156e5aa328f86686945429fe44a83dcfa6a1e0026e2c2ceb8cf23b4a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.9 MB (8939198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2a1fead38b60d97ee0d89f31009b123ad573c9818938780ac564b2398381f2c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:05 GMT
ADD file:416a8b507abdc6bdcb22997a4be0a4170796c3f9f77e315b2dbff2b0a212bc68 in / 
# Tue, 15 Jun 2021 23:15:06 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 05:27:42 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 21:31:44 GMT
ENV HAPROXY_VERSION=2.3.12
# Thu, 08 Jul 2021 21:31:45 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.12.tar.gz
# Thu, 08 Jul 2021 21:31:45 GMT
ENV HAPROXY_SHA256=684670d71ffe1ab3f0bfd1be0e55ea9d932732081dd01858b9e351c1a909be3e
# Thu, 08 Jul 2021 21:32:11 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 08 Jul 2021 21:32:11 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 21:32:12 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 21:32:14 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 08 Jul 2021 21:32:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 21:32:14 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:136482bf81d1fa351b424ebb8c7e34d15f2c5ed3fc0b66b544b8312bda3d52d9`  
		Last Modified: Tue, 15 Jun 2021 23:16:40 GMT  
		Size: 2.4 MB (2427917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5464af225bd487370319e7125fb2769222c5c7371d1be737936169d2e5b01c`  
		Last Modified: Sat, 26 Jun 2021 05:35:56 GMT  
		Size: 1.2 KB (1196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e101eaa240968a0b1dc69dc1781b7243c4767d7f2974b68b31bcad82dc4e41a5`  
		Last Modified: Thu, 08 Jul 2021 21:37:04 GMT  
		Size: 6.5 MB (6509513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:952d669a4a2b908243b212ef3a03f745db60ca164b86923aa3119f31120f2bb1`  
		Last Modified: Thu, 08 Jul 2021 21:36:59 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:206b57e75e9c72c96f79dba44cb8d88cf41dc41c53e29393648012c7f8794179`  
		Last Modified: Thu, 08 Jul 2021 21:36:59 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.12-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:bdddad96e0dcee3f6d26e8d608c8c9dab9c4e4112a15534de812e9eaeaa37b6e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9423882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b85f37a7bc4a1cfa1e8d634c5654956b82640feb78c5cd27cd71029b00cdc62`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 21:44:56 GMT
ADD file:6797caacbfe41bfe44000b39ed017016c6fcc492b3d6557cdaba88536df6c876 in / 
# Tue, 15 Jun 2021 21:44:56 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 02:13:15 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 19:04:31 GMT
ENV HAPROXY_VERSION=2.3.12
# Thu, 08 Jul 2021 19:04:32 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.12.tar.gz
# Thu, 08 Jul 2021 19:04:32 GMT
ENV HAPROXY_SHA256=684670d71ffe1ab3f0bfd1be0e55ea9d932732081dd01858b9e351c1a909be3e
# Thu, 08 Jul 2021 19:05:17 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 08 Jul 2021 19:05:17 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 19:05:17 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 19:05:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 08 Jul 2021 19:05:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 19:05:18 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:58ab47519297212468320b23b8100fc1b2b96e8d342040806ae509a778a0a07a`  
		Last Modified: Tue, 15 Jun 2021 21:46:03 GMT  
		Size: 2.7 MB (2709626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb8dc96e2a4b7f90ae2dbfca981fe199966b64e3426ca1f742499d46ad1aa357`  
		Last Modified: Sat, 26 Jun 2021 02:21:19 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08349c2a8842ea189edf883d942e7fb370a090a02afc4fe538fbe2854e2e4a3a`  
		Last Modified: Thu, 08 Jul 2021 19:08:03 GMT  
		Size: 6.7 MB (6712490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d9b75df55dfc9233984444070416de967601aef766b59b9cd991fd9ddc51f6`  
		Last Modified: Thu, 08 Jul 2021 19:08:01 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1026e4b45765f53b4736f68cb63f67d150185fb95bcd3b69b45f0767726ee85a`  
		Last Modified: Thu, 08 Jul 2021 19:08:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.12-alpine` - linux; 386

```console
$ docker pull haproxy@sha256:d70bf9a3aa05a06cc82d51cf2d6f545537b115649124650caef84b6e8eb824dd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9379406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c741bad0b30f51eb5d7a209145c2b1031c9b92e0efe77a83898cc18df44d3228`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 21:38:30 GMT
ADD file:3b0fe1454491bb05e218b090fd461f2fd39546aa4a53eb3f953ee8eae149ac57 in / 
# Tue, 15 Jun 2021 21:38:30 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 01:39:05 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 19:05:38 GMT
ENV HAPROXY_VERSION=2.3.12
# Thu, 08 Jul 2021 19:05:38 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.12.tar.gz
# Thu, 08 Jul 2021 19:05:38 GMT
ENV HAPROXY_SHA256=684670d71ffe1ab3f0bfd1be0e55ea9d932732081dd01858b9e351c1a909be3e
# Thu, 08 Jul 2021 19:06:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 08 Jul 2021 19:06:43 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 19:06:44 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 19:06:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 08 Jul 2021 19:06:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 19:06:45 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:be21df321efb39c5daf3151073ebff7688e15ea6cd5158878bc9559a5db76ac6`  
		Last Modified: Tue, 15 Jun 2021 21:39:16 GMT  
		Size: 2.8 MB (2820718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc6fe536c8e50a97873c166db7d3b669842dec91d85ce73433028b3b198a1c4`  
		Last Modified: Sat, 26 Jun 2021 01:49:46 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f1db007c417f267ab0d29cbddfedc24ac2c97f03e36050e3ba3ae75762fe82d`  
		Last Modified: Thu, 08 Jul 2021 19:09:35 GMT  
		Size: 6.6 MB (6556921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05dcba06e39fe66f5f431b378324191f1a8d349b1ad03fbc8f2070f2e3c931a4`  
		Last Modified: Thu, 08 Jul 2021 19:09:33 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49184c0500278ba2af56c16b80d0717741e606a00bd70b0dd10ab822156e5206`  
		Last Modified: Thu, 08 Jul 2021 19:09:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.12-alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:3595f780d567d526bcc5384a0974c1a82d06e11424112acb6d7fced16219ba1a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9858364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a45467e080dc275cdbd86aea3113497b239f8022cc43bf2ba163712ea8db5b6f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:27:00 GMT
ADD file:0075aad7a94f0496483442bb2d9fdaa13e9c23087b90638d014b4bc263aa3861 in / 
# Tue, 15 Jun 2021 22:27:03 GMT
CMD ["/bin/sh"]
# Fri, 16 Jul 2021 20:17:57 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 16 Jul 2021 20:21:16 GMT
ENV HAPROXY_VERSION=2.3.12
# Fri, 16 Jul 2021 20:21:19 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.12.tar.gz
# Fri, 16 Jul 2021 20:21:25 GMT
ENV HAPROXY_SHA256=684670d71ffe1ab3f0bfd1be0e55ea9d932732081dd01858b9e351c1a909be3e
# Thu, 22 Jul 2021 03:12:05 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 22 Jul 2021 03:12:12 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 03:12:15 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 03:12:25 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 22 Jul 2021 03:12:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 03:12:39 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:baf144cfb66ebe9df1969f3b90f1c448beff98edc84de1ccb5d6346195a070d4`  
		Last Modified: Tue, 15 Jun 2021 22:27:38 GMT  
		Size: 2.8 MB (2810478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e907663c9428bbbb731a221721c606bad29e54dac6f0dda85d6aa3175a725e`  
		Last Modified: Thu, 22 Jul 2021 03:40:16 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0008e4d1138d3cc9a9b5870cccefa199a25ed8006dc5dca6270cb1a7888e0d3c`  
		Last Modified: Thu, 22 Jul 2021 03:41:27 GMT  
		Size: 7.0 MB (7046114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f798460f1147e4b49ead0f482ca43ceede007cb949f979322a687b184e8ad5e`  
		Last Modified: Thu, 22 Jul 2021 03:41:26 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5caa03e44179cf876a689b69c698cd0f3bdf49f41a9ee874ce3f954d440f8bb`  
		Last Modified: Thu, 22 Jul 2021 03:41:26 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.4`

```console
$ docker pull haproxy@sha256:0b604e2d9b0366e304d89393dd42651698bbbc2d588b65155b6aabaf4995ba00
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

### `haproxy:2.4` - linux; amd64

```console
$ docker pull haproxy@sha256:52aa1ec7d5d0b74f20d4e5c03c8f7561ead3db8931e0b733d6007b397a2d3880
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37295916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d784089a656dab7a82fd06ce515c7a5f2865055cc3d9422c8795a07300428f07`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 06:19:17 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 18:33:10 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 08 Jul 2021 18:33:10 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 08 Jul 2021 18:33:10 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 08 Jul 2021 18:34:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 08 Jul 2021 18:34:02 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 18:34:02 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 18:34:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 18:34:03 GMT
USER haproxy
# Thu, 08 Jul 2021 18:34:03 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91332cb81883405a321c1a2d2144bdd0aef8d1c69f90fdf0cf219982161b6e6e`  
		Last Modified: Wed, 23 Jun 2021 06:29:07 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6373e07bfb885e35a6bd53edfdc9040601b27fc0961fe6129588015b2096db20`  
		Last Modified: Thu, 08 Jul 2021 18:38:19 GMT  
		Size: 10.1 MB (10148233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a5b51f2be69ce74243979e96aaae4a74e55466e342bcd0bb697a2b1e62d59b`  
		Last Modified: Thu, 08 Jul 2021 18:38:18 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:2f24bc20c43df5eb2b7e5ffc0e95674782b29896f65a1226bc2adff0b3d68e0a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34665575 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed1196ca984d9efa3ec3c4f779f012f0662a9586517f0c0e041612416ff4fbc8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 22 Jun 2021 23:50:09 GMT
ADD file:78d4ced31112d85490c684f350aceeebfc72a804262c7ad3e033257e3894f5c4 in / 
# Tue, 22 Jun 2021 23:50:11 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:15:11 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 18:58:15 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 08 Jul 2021 18:58:16 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 08 Jul 2021 18:58:16 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 08 Jul 2021 18:59:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 08 Jul 2021 18:59:09 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 18:59:10 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 18:59:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 18:59:10 GMT
USER haproxy
# Thu, 08 Jul 2021 18:59:11 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:532d6df30af5174ac6e1b379c32b8f464d44651ac060376a560c4a76a87704a7`  
		Last Modified: Wed, 23 Jun 2021 00:01:46 GMT  
		Size: 24.9 MB (24878945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48649e3d7de4cd80d3a9a34c725a2935be904ff90e99ea6c8e4bb6e1e7a4eeb7`  
		Last Modified: Wed, 23 Jun 2021 05:24:11 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ee3e06cb1904b6bc00db8565860713531b542e6ef7389f534e96705484113d`  
		Last Modified: Thu, 08 Jul 2021 19:02:21 GMT  
		Size: 9.8 MB (9784805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b6869880a0636c536ab6434a503f73fbe4faa5d871d3ae25f498d9995adc0f3`  
		Last Modified: Thu, 08 Jul 2021 19:02:15 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:7b6339c2dff4e7a1d7bbb7c72bc74cf2072bf95ff20841bd1c3392db483209b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.4 MB (32372088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9405b9497ca1234f5dd526dab824511329f7053f2f2b6766f2a64e2c9734d7bb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:31 GMT
ADD file:8d200a3bbe985ff355343675c5555852f27550a9e367969df6bc98034efb8fd4 in / 
# Wed, 23 Jun 2021 00:20:31 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:21:41 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 21:28:35 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 08 Jul 2021 21:28:36 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 08 Jul 2021 21:28:37 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 08 Jul 2021 21:29:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 08 Jul 2021 21:29:24 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 21:29:25 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 21:29:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 21:29:26 GMT
USER haproxy
# Thu, 08 Jul 2021 21:29:26 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:8452be1adf00f91570fe21a8e61aaf4c12e014daf67d7de65d984f4e8ecca2f1`  
		Last Modified: Wed, 23 Jun 2021 00:31:49 GMT  
		Size: 22.7 MB (22746055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed1c9c92d0076fd4bf40503e3f47102509a5b99d182f4dd9e81e64d0a7e0b8a`  
		Last Modified: Wed, 23 Jun 2021 05:35:48 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b090e05bfe544bc62f527dcf70dd8799d4180499bcedf6d5a8ffa14c7a75b31d`  
		Last Modified: Thu, 08 Jul 2021 21:35:57 GMT  
		Size: 9.6 MB (9624206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9cdb9eefea684230e2e659f2753469d8df08683a747d1a8d95dc6da0954cb60`  
		Last Modified: Thu, 08 Jul 2021 21:35:52 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:ecddae360d89e478a3ca8575fe6902f41f5bce6d136ffa9d002979696533aed9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35942280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b004550c7f1e6363193435537a32221dc4e6ce0bb68cea61b3c97378b6362064`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:40 GMT
ADD file:beee00b59da720f68e12e2ba2a8134207c80c777ddb4ceb03c71e3e4c3f51c93 in / 
# Tue, 22 Jun 2021 23:49:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 03:19:31 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 19:01:35 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 08 Jul 2021 19:01:35 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 08 Jul 2021 19:01:35 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 08 Jul 2021 19:02:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 08 Jul 2021 19:02:18 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 19:02:18 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 19:02:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 19:02:18 GMT
USER haproxy
# Thu, 08 Jul 2021 19:02:18 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:448f6bf000e31217a7c202c659b03b7f8ac8d3ae6b03ef7a2f8339be2f00ff4a`  
		Last Modified: Tue, 22 Jun 2021 23:55:25 GMT  
		Size: 25.9 MB (25914993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b05ad81dc8a7d67656235988f0e5fb72c374c7d8df44c105b91d712e06c4ac`  
		Last Modified: Wed, 23 Jun 2021 03:26:16 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076876a81ee03b4e5250b7a31318f330ccf4ea3eeef84cecafdc1a92b4803062`  
		Last Modified: Thu, 08 Jul 2021 19:07:11 GMT  
		Size: 10.0 MB (10025457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:277cf44e1cd25ac34ef95ef8bc0084be15c5d80b5fd94d6b8ba385807423dce0`  
		Last Modified: Thu, 08 Jul 2021 19:07:08 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4` - linux; 386

```console
$ docker pull haproxy@sha256:ef1c5085a09fe3d0028e256643a9453a2b853f34cf360c895fdc418095a9525a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.8 MB (37792502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87c94a82fd63b1e3cbd90c3cca2b24076d38dcdfd88fc0b5f9367719bd84cbdd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 22 Jun 2021 23:39:35 GMT
ADD file:48f656ac6733911048b3de850490438d0233b3badc11861fca62062d4edfaf40 in / 
# Tue, 22 Jun 2021 23:39:35 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:23:13 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 19:01:56 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 08 Jul 2021 19:01:56 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 08 Jul 2021 19:01:56 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 08 Jul 2021 19:02:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 08 Jul 2021 19:02:57 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 19:02:57 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 19:02:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 19:02:58 GMT
USER haproxy
# Thu, 08 Jul 2021 19:02:58 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:33af2dcb865e65d53cdeb843b67a0ef62151fa32df292293e7c6b0eb728ac5ac`  
		Last Modified: Tue, 22 Jun 2021 23:46:23 GMT  
		Size: 27.8 MB (27797411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a6e4d42b23996eb7d8a1baa85ee19828c2667fd4a2dca6eb1040b266680e9f`  
		Last Modified: Wed, 23 Jun 2021 00:32:00 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c640aece6fea8db01bc9744204c373af3285d4d3b15911631fdc1508b30fe28f`  
		Last Modified: Thu, 08 Jul 2021 19:08:39 GMT  
		Size: 10.0 MB (9993262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e1e627dabfcf736ac7f517f394391e6eeb0fa52347a5f92cee7310d00c35fac`  
		Last Modified: Thu, 08 Jul 2021 19:08:38 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4` - linux; mips64le

```console
$ docker pull haproxy@sha256:0831d16085b3616dd56baae5d2b16911f5df76ff3643f6ed0cc9206bcdd1b0ef
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.6 MB (35582649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a67c72bc16cd3442d99818a1691f620bb8fba803aa322938bf1f76185d160ae9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 22 Jul 2021 00:09:45 GMT
ADD file:1f77b9001c4977ba733be674fc5eb4b85130f1dea8a7b39d545b70f9c107695f in / 
# Thu, 22 Jul 2021 00:09:46 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:07:49 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 22 Jul 2021 01:10:29 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 22 Jul 2021 01:10:29 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 22 Jul 2021 01:10:30 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 22 Jul 2021 01:12:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 22 Jul 2021 01:12:58 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 01:12:58 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 01:12:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 01:12:59 GMT
USER haproxy
# Thu, 22 Jul 2021 01:12:59 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:99ee621d0b0485e9de65aa19604aa2453d19ea7fc86b22c5b77c1bab74e3cb42`  
		Last Modified: Thu, 22 Jul 2021 00:16:11 GMT  
		Size: 25.8 MB (25812771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f444627794f98947a9df95ec5d19b2a1cd6c151ed438982b1dc0b89f5eaf19e`  
		Last Modified: Thu, 22 Jul 2021 01:24:39 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529ec01a3a5cb58c3aa92432192c7025a9df5ac852a7e1606269d172da56dd54`  
		Last Modified: Thu, 22 Jul 2021 01:25:03 GMT  
		Size: 9.8 MB (9768048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0dc46dbff91be84b369de7651cd4d1d725a03b3d65bfef0a41478894b38fe2`  
		Last Modified: Thu, 22 Jul 2021 01:24:56 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4` - linux; ppc64le

```console
$ docker pull haproxy@sha256:0265c0700be024578a661ef439408b91cfa73fef6b763a58ddad4d78fdbc51db
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.2 MB (41213069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae16a408d428d4d0a7ed8262d6b984676689a578932f9ff1a168c726b85fb6e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 22 Jul 2021 00:19:04 GMT
ADD file:3a6bd6ce3eff98b88a13de5d0f26cff0b026f876674204dbad6f84fafcf145b1 in / 
# Thu, 22 Jul 2021 00:19:13 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 02:52:46 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 22 Jul 2021 02:59:40 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 22 Jul 2021 02:59:52 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 22 Jul 2021 03:00:03 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 22 Jul 2021 03:03:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 22 Jul 2021 03:03:39 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 03:03:41 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 03:03:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 03:03:48 GMT
USER haproxy
# Thu, 22 Jul 2021 03:03:52 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:1130517d52da84a09f9465006bddab5e49afd398860890eab6274fd0bff32371`  
		Last Modified: Thu, 22 Jul 2021 00:27:49 GMT  
		Size: 30.6 MB (30553709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251bf3fe1d4bbe9c27e393cd8ddc550b56cec90eb916bf9bec24d657c9f6556f`  
		Last Modified: Thu, 22 Jul 2021 03:40:01 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f4b7133364510c1fc0f847a528a441235df0500c39d8318c3557708a9ea74fa`  
		Last Modified: Thu, 22 Jul 2021 03:40:33 GMT  
		Size: 10.7 MB (10657533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1244f9b6844b16203e11b9ed8754bed5a0289f1a3b6bd59d295e18b9fca91bc`  
		Last Modified: Thu, 22 Jul 2021 03:40:30 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4` - linux; s390x

```console
$ docker pull haproxy@sha256:2f711e846e54ca0e3063a51b841c4291dc0a07925552f9feab60e56ceeb54a8b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.6 MB (35587765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:123ac19f2aeb23d953a63211cc6c840f267890f19ee5a8db61abaed33280a5b5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 22 Jul 2021 00:42:45 GMT
ADD file:1ab999eb6f80d8ce91ce3a173e23fd2710f2779117bba29037eaa82aadcbf6ed in / 
# Thu, 22 Jul 2021 00:42:48 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:30:19 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 22 Jul 2021 01:31:40 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 22 Jul 2021 01:31:40 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 22 Jul 2021 01:31:40 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 22 Jul 2021 01:32:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 22 Jul 2021 01:32:21 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 01:32:21 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 01:32:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 01:32:22 GMT
USER haproxy
# Thu, 22 Jul 2021 01:32:22 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:7a50fdd85ff244c1465e71c51354d055e3df0b90ff5faad28cc22d9ecde9daf3`  
		Last Modified: Thu, 22 Jul 2021 00:48:13 GMT  
		Size: 25.8 MB (25760761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05fb34d1ed21b67502665114a7ae60445472fc7bafa620bbf6c79b7df85a01d4`  
		Last Modified: Thu, 22 Jul 2021 01:39:54 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509cd29cce72fe3b56df141c72bd9ac7c85aafc2da6d1596ec7e29ef8e10db0f`  
		Last Modified: Thu, 22 Jul 2021 01:40:05 GMT  
		Size: 9.8 MB (9825173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b04c9d12d457a528c260ddcaaecc8d44f66fb72fb0a54770d3011ba16f8433`  
		Last Modified: Thu, 22 Jul 2021 01:40:04 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.4-alpine`

```console
$ docker pull haproxy@sha256:278afc7563fcb5d498201d0093f9c700e659628677604bc15a82e3abba175799
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `haproxy:2.4-alpine` - linux; amd64

```console
$ docker pull haproxy@sha256:8819f159761cf992682ccb1267ab52e4b086a332e2baed24df18ff51bf49bd6a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.1 MB (10128308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7a37d8a7b2f124598b023e74621914426f81ab8b4f8e01d74cfbee1dd62ef0f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 02:48:50 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 18:34:10 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 08 Jul 2021 18:34:10 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 08 Jul 2021 18:34:10 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 08 Jul 2021 18:35:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 08 Jul 2021 18:35:12 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 18:35:12 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 18:35:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 18:35:13 GMT
USER haproxy
# Thu, 08 Jul 2021 18:35:13 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7834d945b9e597e693f56fb0f9847718c1732b738a2f4956ab2c1b66c289d90`  
		Last Modified: Sat, 26 Jun 2021 02:56:43 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddff1cb6bb6da9a692c61843d46abe17a215c726bb13d570212777a87398a3d9`  
		Last Modified: Thu, 08 Jul 2021 18:38:36 GMT  
		Size: 7.3 MB (7315186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee55c5b3ebb2b318c44f2635d4eea44eadfd079d55d0b8c5a6918b8aa9d5b1dc`  
		Last Modified: Thu, 08 Jul 2021 18:38:34 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:b79f0c78bc069755084556b3bd897a39780d24fe70b909b7c119d53f9a6bbc01
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9912733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05e37a7293c9eccbd033a7a1a38aa77387373ba82f719cbcc400dec92a69aad3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:26 GMT
ADD file:c80bc2b093cbc0fc466582ef21cbed377de9fa874aedbf320079525ddacd1200 in / 
# Tue, 15 Jun 2021 22:57:26 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 02:02:51 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 19:07:43 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 08 Jul 2021 19:07:44 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 08 Jul 2021 19:07:44 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 08 Jul 2021 19:08:13 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 08 Jul 2021 19:08:13 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 19:08:14 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 19:08:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 19:08:15 GMT
USER haproxy
# Thu, 08 Jul 2021 19:08:15 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:b4c9a0924271af3466de27804af26420eb58da1466e7eaaba127d178b380fea3`  
		Last Modified: Tue, 15 Jun 2021 22:58:47 GMT  
		Size: 2.6 MB (2624382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85fa2947d9cc2655af4fd4aa21641629e791bcaf309a7095db77d309ddd05dfa`  
		Last Modified: Sat, 26 Jun 2021 02:08:45 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a9ab1152df106ecaf9c67a2a14b91a15581a3b86248b43604172b704b71167`  
		Last Modified: Thu, 08 Jul 2021 19:11:00 GMT  
		Size: 7.3 MB (7286705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc34702136897eee4ca8c94845af335a66311b8b8a57a5f1c40292b913ef9f72`  
		Last Modified: Thu, 08 Jul 2021 19:10:56 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:b318934bc8973f8f73ad46a1c4f1c097899f57cdba1f6bff40285760584a684c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9631368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c900ed3b5e7e8ae25ede6582344b41bf064d26e831bdf4bfd385861422503a3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:05 GMT
ADD file:416a8b507abdc6bdcb22997a4be0a4170796c3f9f77e315b2dbff2b0a212bc68 in / 
# Tue, 15 Jun 2021 23:15:06 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 05:27:42 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 21:29:41 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 08 Jul 2021 21:29:42 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 08 Jul 2021 21:29:42 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 08 Jul 2021 21:30:19 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 08 Jul 2021 21:30:20 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 21:30:21 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 21:30:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 21:30:22 GMT
USER haproxy
# Thu, 08 Jul 2021 21:30:22 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:136482bf81d1fa351b424ebb8c7e34d15f2c5ed3fc0b66b544b8312bda3d52d9`  
		Last Modified: Tue, 15 Jun 2021 23:16:40 GMT  
		Size: 2.4 MB (2427917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5464af225bd487370319e7125fb2769222c5c7371d1be737936169d2e5b01c`  
		Last Modified: Sat, 26 Jun 2021 05:35:56 GMT  
		Size: 1.2 KB (1196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f903498f8e23244ca6430d647dd5515930d69394f19d017d07930d288ca6580`  
		Last Modified: Thu, 08 Jul 2021 21:36:22 GMT  
		Size: 7.2 MB (7201807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a0d8812e6df331ba2d781cc1fc08c2e4ddad2bb05b762b0eb737308a1205d5`  
		Last Modified: Thu, 08 Jul 2021 21:36:18 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:c17729aebb94fdae2758381c550a8866ce8856237ce1892a6fba9d0cdadd7c5b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.1 MB (10133906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b500e8260787f1a0bcdc19f790686cd272d751cdd28f848f01eb2f054c700341`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 21:44:56 GMT
ADD file:6797caacbfe41bfe44000b39ed017016c6fcc492b3d6557cdaba88536df6c876 in / 
# Tue, 15 Jun 2021 21:44:56 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 02:13:15 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 19:02:27 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 08 Jul 2021 19:02:27 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 08 Jul 2021 19:02:27 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 08 Jul 2021 19:03:26 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 08 Jul 2021 19:03:26 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 19:03:27 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 19:03:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 19:03:27 GMT
USER haproxy
# Thu, 08 Jul 2021 19:03:27 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:58ab47519297212468320b23b8100fc1b2b96e8d342040806ae509a778a0a07a`  
		Last Modified: Tue, 15 Jun 2021 21:46:03 GMT  
		Size: 2.7 MB (2709626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb8dc96e2a4b7f90ae2dbfca981fe199966b64e3426ca1f742499d46ad1aa357`  
		Last Modified: Sat, 26 Jun 2021 02:21:19 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b367d065849fc1a609fb169119e94047ed3a2b475932bb292bff5b6cc45a1f`  
		Last Modified: Thu, 08 Jul 2021 19:07:30 GMT  
		Size: 7.4 MB (7422635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60cf6675a5a8e39f65c07f8553ab269ab83f947cbfa20da77e6da66ca033969e`  
		Last Modified: Thu, 08 Jul 2021 19:07:28 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-alpine` - linux; 386

```console
$ docker pull haproxy@sha256:01a8472d10c0512c1950dad3ae7472f99767eeaa8f0bbbb3aa53813d35961ab0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (9998434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e50005241013c0fb9d14f539c88cbf5dd3ebfec6c0498014c4a70a002cbe3d48`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 21:38:30 GMT
ADD file:3b0fe1454491bb05e218b090fd461f2fd39546aa4a53eb3f953ee8eae149ac57 in / 
# Tue, 15 Jun 2021 21:38:30 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 01:39:05 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 19:03:09 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 08 Jul 2021 19:03:09 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 08 Jul 2021 19:03:09 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 08 Jul 2021 19:04:25 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 08 Jul 2021 19:04:25 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 19:04:25 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 19:04:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 19:04:26 GMT
USER haproxy
# Thu, 08 Jul 2021 19:04:26 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:be21df321efb39c5daf3151073ebff7688e15ea6cd5158878bc9559a5db76ac6`  
		Last Modified: Tue, 15 Jun 2021 21:39:16 GMT  
		Size: 2.8 MB (2820718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc6fe536c8e50a97873c166db7d3b669842dec91d85ce73433028b3b198a1c4`  
		Last Modified: Sat, 26 Jun 2021 01:49:46 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:832c00757ee7003ebca753eff8d4c6af86ebcf09efecec8e1171e550c8fc816f`  
		Last Modified: Thu, 08 Jul 2021 19:08:59 GMT  
		Size: 7.2 MB (7176071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85e6578d15134f65f8b977b9e7c9322e6281b3c765978ce760142c0bac7197ad`  
		Last Modified: Thu, 08 Jul 2021 19:08:57 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:8371490329ce959d92d6d6bca900a6702869e800fbd8c4a80438da13efa8b696
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.6 MB (10556641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5510c2e0b44e02d587dd27e62dd07ef69cc51b3e43f00927403e3c29eb34cfc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:27:00 GMT
ADD file:0075aad7a94f0496483442bb2d9fdaa13e9c23087b90638d014b4bc263aa3861 in / 
# Tue, 15 Jun 2021 22:27:03 GMT
CMD ["/bin/sh"]
# Fri, 16 Jul 2021 20:17:57 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 16 Jul 2021 20:19:42 GMT
ENV HAPROXY_VERSION=2.4.2
# Fri, 16 Jul 2021 20:19:48 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Fri, 16 Jul 2021 20:19:51 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 22 Jul 2021 03:04:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 22 Jul 2021 03:04:47 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 03:04:50 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 03:04:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 03:04:59 GMT
USER haproxy
# Thu, 22 Jul 2021 03:05:04 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:baf144cfb66ebe9df1969f3b90f1c448beff98edc84de1ccb5d6346195a070d4`  
		Last Modified: Tue, 15 Jun 2021 22:27:38 GMT  
		Size: 2.8 MB (2810478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e907663c9428bbbb731a221721c606bad29e54dac6f0dda85d6aa3175a725e`  
		Last Modified: Thu, 22 Jul 2021 03:40:16 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25fed8e719bd522b435fea4d6999c2ecffeb38e8288458cea40c3ecfa9131656`  
		Last Modified: Thu, 22 Jul 2021 03:40:53 GMT  
		Size: 7.7 MB (7744514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c45ecd590d1194b07f22c1e98348800abd5fdc2592d5c85e8fd5413acc1f29`  
		Last Modified: Thu, 22 Jul 2021 03:40:50 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-alpine` - linux; s390x

```console
$ docker pull haproxy@sha256:67c77b2f75cda356f4462fa8c7cfe05d80b220bb7e3ddff6782557ca308381e0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9899025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8353b377710bdcc56a8dd1fcdf4213b83d4378a795634015c8ec0817188591f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:54:24 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:45:22 GMT
ENV HAPROXY_VERSION=2.4.0
# Fri, 14 May 2021 19:45:23 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Fri, 14 May 2021 19:45:23 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Fri, 14 May 2021 19:46:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 14 May 2021 19:46:14 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:46:14 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:46:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:46:15 GMT
USER haproxy
# Fri, 14 May 2021 19:46:15 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267275aba58470c82626189a59be76cd169bd245568e2f2545ed1ee64ff8a8ff`  
		Last Modified: Wed, 14 Apr 2021 20:59:06 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1af9bde57dd624c224ba02793a7568cd9f00874c978ff5ab4d6bc0c32fdb81f`  
		Last Modified: Fri, 14 May 2021 19:48:00 GMT  
		Size: 7.3 MB (7294741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68dd09d54ba9406459ae1956173c0df96676de52e5a01f9392966e3493acae68`  
		Last Modified: Fri, 14 May 2021 19:47:59 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.4.2`

```console
$ docker pull haproxy@sha256:0b604e2d9b0366e304d89393dd42651698bbbc2d588b65155b6aabaf4995ba00
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

### `haproxy:2.4.2` - linux; amd64

```console
$ docker pull haproxy@sha256:52aa1ec7d5d0b74f20d4e5c03c8f7561ead3db8931e0b733d6007b397a2d3880
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37295916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d784089a656dab7a82fd06ce515c7a5f2865055cc3d9422c8795a07300428f07`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 06:19:17 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 18:33:10 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 08 Jul 2021 18:33:10 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 08 Jul 2021 18:33:10 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 08 Jul 2021 18:34:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 08 Jul 2021 18:34:02 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 18:34:02 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 18:34:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 18:34:03 GMT
USER haproxy
# Thu, 08 Jul 2021 18:34:03 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91332cb81883405a321c1a2d2144bdd0aef8d1c69f90fdf0cf219982161b6e6e`  
		Last Modified: Wed, 23 Jun 2021 06:29:07 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6373e07bfb885e35a6bd53edfdc9040601b27fc0961fe6129588015b2096db20`  
		Last Modified: Thu, 08 Jul 2021 18:38:19 GMT  
		Size: 10.1 MB (10148233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a5b51f2be69ce74243979e96aaae4a74e55466e342bcd0bb697a2b1e62d59b`  
		Last Modified: Thu, 08 Jul 2021 18:38:18 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4.2` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:2f24bc20c43df5eb2b7e5ffc0e95674782b29896f65a1226bc2adff0b3d68e0a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34665575 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed1196ca984d9efa3ec3c4f779f012f0662a9586517f0c0e041612416ff4fbc8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 22 Jun 2021 23:50:09 GMT
ADD file:78d4ced31112d85490c684f350aceeebfc72a804262c7ad3e033257e3894f5c4 in / 
# Tue, 22 Jun 2021 23:50:11 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:15:11 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 18:58:15 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 08 Jul 2021 18:58:16 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 08 Jul 2021 18:58:16 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 08 Jul 2021 18:59:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 08 Jul 2021 18:59:09 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 18:59:10 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 18:59:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 18:59:10 GMT
USER haproxy
# Thu, 08 Jul 2021 18:59:11 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:532d6df30af5174ac6e1b379c32b8f464d44651ac060376a560c4a76a87704a7`  
		Last Modified: Wed, 23 Jun 2021 00:01:46 GMT  
		Size: 24.9 MB (24878945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48649e3d7de4cd80d3a9a34c725a2935be904ff90e99ea6c8e4bb6e1e7a4eeb7`  
		Last Modified: Wed, 23 Jun 2021 05:24:11 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ee3e06cb1904b6bc00db8565860713531b542e6ef7389f534e96705484113d`  
		Last Modified: Thu, 08 Jul 2021 19:02:21 GMT  
		Size: 9.8 MB (9784805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b6869880a0636c536ab6434a503f73fbe4faa5d871d3ae25f498d9995adc0f3`  
		Last Modified: Thu, 08 Jul 2021 19:02:15 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4.2` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:7b6339c2dff4e7a1d7bbb7c72bc74cf2072bf95ff20841bd1c3392db483209b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.4 MB (32372088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9405b9497ca1234f5dd526dab824511329f7053f2f2b6766f2a64e2c9734d7bb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:31 GMT
ADD file:8d200a3bbe985ff355343675c5555852f27550a9e367969df6bc98034efb8fd4 in / 
# Wed, 23 Jun 2021 00:20:31 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:21:41 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 21:28:35 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 08 Jul 2021 21:28:36 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 08 Jul 2021 21:28:37 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 08 Jul 2021 21:29:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 08 Jul 2021 21:29:24 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 21:29:25 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 21:29:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 21:29:26 GMT
USER haproxy
# Thu, 08 Jul 2021 21:29:26 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:8452be1adf00f91570fe21a8e61aaf4c12e014daf67d7de65d984f4e8ecca2f1`  
		Last Modified: Wed, 23 Jun 2021 00:31:49 GMT  
		Size: 22.7 MB (22746055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed1c9c92d0076fd4bf40503e3f47102509a5b99d182f4dd9e81e64d0a7e0b8a`  
		Last Modified: Wed, 23 Jun 2021 05:35:48 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b090e05bfe544bc62f527dcf70dd8799d4180499bcedf6d5a8ffa14c7a75b31d`  
		Last Modified: Thu, 08 Jul 2021 21:35:57 GMT  
		Size: 9.6 MB (9624206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9cdb9eefea684230e2e659f2753469d8df08683a747d1a8d95dc6da0954cb60`  
		Last Modified: Thu, 08 Jul 2021 21:35:52 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4.2` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:ecddae360d89e478a3ca8575fe6902f41f5bce6d136ffa9d002979696533aed9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35942280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b004550c7f1e6363193435537a32221dc4e6ce0bb68cea61b3c97378b6362064`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:40 GMT
ADD file:beee00b59da720f68e12e2ba2a8134207c80c777ddb4ceb03c71e3e4c3f51c93 in / 
# Tue, 22 Jun 2021 23:49:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 03:19:31 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 19:01:35 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 08 Jul 2021 19:01:35 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 08 Jul 2021 19:01:35 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 08 Jul 2021 19:02:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 08 Jul 2021 19:02:18 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 19:02:18 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 19:02:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 19:02:18 GMT
USER haproxy
# Thu, 08 Jul 2021 19:02:18 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:448f6bf000e31217a7c202c659b03b7f8ac8d3ae6b03ef7a2f8339be2f00ff4a`  
		Last Modified: Tue, 22 Jun 2021 23:55:25 GMT  
		Size: 25.9 MB (25914993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b05ad81dc8a7d67656235988f0e5fb72c374c7d8df44c105b91d712e06c4ac`  
		Last Modified: Wed, 23 Jun 2021 03:26:16 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076876a81ee03b4e5250b7a31318f330ccf4ea3eeef84cecafdc1a92b4803062`  
		Last Modified: Thu, 08 Jul 2021 19:07:11 GMT  
		Size: 10.0 MB (10025457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:277cf44e1cd25ac34ef95ef8bc0084be15c5d80b5fd94d6b8ba385807423dce0`  
		Last Modified: Thu, 08 Jul 2021 19:07:08 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4.2` - linux; 386

```console
$ docker pull haproxy@sha256:ef1c5085a09fe3d0028e256643a9453a2b853f34cf360c895fdc418095a9525a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.8 MB (37792502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87c94a82fd63b1e3cbd90c3cca2b24076d38dcdfd88fc0b5f9367719bd84cbdd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 22 Jun 2021 23:39:35 GMT
ADD file:48f656ac6733911048b3de850490438d0233b3badc11861fca62062d4edfaf40 in / 
# Tue, 22 Jun 2021 23:39:35 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:23:13 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 19:01:56 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 08 Jul 2021 19:01:56 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 08 Jul 2021 19:01:56 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 08 Jul 2021 19:02:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 08 Jul 2021 19:02:57 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 19:02:57 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 19:02:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 19:02:58 GMT
USER haproxy
# Thu, 08 Jul 2021 19:02:58 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:33af2dcb865e65d53cdeb843b67a0ef62151fa32df292293e7c6b0eb728ac5ac`  
		Last Modified: Tue, 22 Jun 2021 23:46:23 GMT  
		Size: 27.8 MB (27797411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a6e4d42b23996eb7d8a1baa85ee19828c2667fd4a2dca6eb1040b266680e9f`  
		Last Modified: Wed, 23 Jun 2021 00:32:00 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c640aece6fea8db01bc9744204c373af3285d4d3b15911631fdc1508b30fe28f`  
		Last Modified: Thu, 08 Jul 2021 19:08:39 GMT  
		Size: 10.0 MB (9993262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e1e627dabfcf736ac7f517f394391e6eeb0fa52347a5f92cee7310d00c35fac`  
		Last Modified: Thu, 08 Jul 2021 19:08:38 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4.2` - linux; mips64le

```console
$ docker pull haproxy@sha256:0831d16085b3616dd56baae5d2b16911f5df76ff3643f6ed0cc9206bcdd1b0ef
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.6 MB (35582649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a67c72bc16cd3442d99818a1691f620bb8fba803aa322938bf1f76185d160ae9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 22 Jul 2021 00:09:45 GMT
ADD file:1f77b9001c4977ba733be674fc5eb4b85130f1dea8a7b39d545b70f9c107695f in / 
# Thu, 22 Jul 2021 00:09:46 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:07:49 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 22 Jul 2021 01:10:29 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 22 Jul 2021 01:10:29 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 22 Jul 2021 01:10:30 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 22 Jul 2021 01:12:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 22 Jul 2021 01:12:58 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 01:12:58 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 01:12:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 01:12:59 GMT
USER haproxy
# Thu, 22 Jul 2021 01:12:59 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:99ee621d0b0485e9de65aa19604aa2453d19ea7fc86b22c5b77c1bab74e3cb42`  
		Last Modified: Thu, 22 Jul 2021 00:16:11 GMT  
		Size: 25.8 MB (25812771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f444627794f98947a9df95ec5d19b2a1cd6c151ed438982b1dc0b89f5eaf19e`  
		Last Modified: Thu, 22 Jul 2021 01:24:39 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529ec01a3a5cb58c3aa92432192c7025a9df5ac852a7e1606269d172da56dd54`  
		Last Modified: Thu, 22 Jul 2021 01:25:03 GMT  
		Size: 9.8 MB (9768048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0dc46dbff91be84b369de7651cd4d1d725a03b3d65bfef0a41478894b38fe2`  
		Last Modified: Thu, 22 Jul 2021 01:24:56 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4.2` - linux; ppc64le

```console
$ docker pull haproxy@sha256:0265c0700be024578a661ef439408b91cfa73fef6b763a58ddad4d78fdbc51db
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.2 MB (41213069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae16a408d428d4d0a7ed8262d6b984676689a578932f9ff1a168c726b85fb6e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 22 Jul 2021 00:19:04 GMT
ADD file:3a6bd6ce3eff98b88a13de5d0f26cff0b026f876674204dbad6f84fafcf145b1 in / 
# Thu, 22 Jul 2021 00:19:13 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 02:52:46 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 22 Jul 2021 02:59:40 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 22 Jul 2021 02:59:52 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 22 Jul 2021 03:00:03 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 22 Jul 2021 03:03:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 22 Jul 2021 03:03:39 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 03:03:41 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 03:03:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 03:03:48 GMT
USER haproxy
# Thu, 22 Jul 2021 03:03:52 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:1130517d52da84a09f9465006bddab5e49afd398860890eab6274fd0bff32371`  
		Last Modified: Thu, 22 Jul 2021 00:27:49 GMT  
		Size: 30.6 MB (30553709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251bf3fe1d4bbe9c27e393cd8ddc550b56cec90eb916bf9bec24d657c9f6556f`  
		Last Modified: Thu, 22 Jul 2021 03:40:01 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f4b7133364510c1fc0f847a528a441235df0500c39d8318c3557708a9ea74fa`  
		Last Modified: Thu, 22 Jul 2021 03:40:33 GMT  
		Size: 10.7 MB (10657533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1244f9b6844b16203e11b9ed8754bed5a0289f1a3b6bd59d295e18b9fca91bc`  
		Last Modified: Thu, 22 Jul 2021 03:40:30 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4.2` - linux; s390x

```console
$ docker pull haproxy@sha256:2f711e846e54ca0e3063a51b841c4291dc0a07925552f9feab60e56ceeb54a8b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.6 MB (35587765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:123ac19f2aeb23d953a63211cc6c840f267890f19ee5a8db61abaed33280a5b5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 22 Jul 2021 00:42:45 GMT
ADD file:1ab999eb6f80d8ce91ce3a173e23fd2710f2779117bba29037eaa82aadcbf6ed in / 
# Thu, 22 Jul 2021 00:42:48 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:30:19 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 22 Jul 2021 01:31:40 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 22 Jul 2021 01:31:40 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 22 Jul 2021 01:31:40 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 22 Jul 2021 01:32:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 22 Jul 2021 01:32:21 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 01:32:21 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 01:32:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 01:32:22 GMT
USER haproxy
# Thu, 22 Jul 2021 01:32:22 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:7a50fdd85ff244c1465e71c51354d055e3df0b90ff5faad28cc22d9ecde9daf3`  
		Last Modified: Thu, 22 Jul 2021 00:48:13 GMT  
		Size: 25.8 MB (25760761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05fb34d1ed21b67502665114a7ae60445472fc7bafa620bbf6c79b7df85a01d4`  
		Last Modified: Thu, 22 Jul 2021 01:39:54 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509cd29cce72fe3b56df141c72bd9ac7c85aafc2da6d1596ec7e29ef8e10db0f`  
		Last Modified: Thu, 22 Jul 2021 01:40:05 GMT  
		Size: 9.8 MB (9825173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b04c9d12d457a528c260ddcaaecc8d44f66fb72fb0a54770d3011ba16f8433`  
		Last Modified: Thu, 22 Jul 2021 01:40:04 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.4.2-alpine`

```console
$ docker pull haproxy@sha256:734a112b00322962f3f962b4557771db09b855d48a8e8b015d958cd7eb5a2052
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `haproxy:2.4.2-alpine` - linux; amd64

```console
$ docker pull haproxy@sha256:8819f159761cf992682ccb1267ab52e4b086a332e2baed24df18ff51bf49bd6a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.1 MB (10128308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7a37d8a7b2f124598b023e74621914426f81ab8b4f8e01d74cfbee1dd62ef0f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 02:48:50 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 18:34:10 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 08 Jul 2021 18:34:10 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 08 Jul 2021 18:34:10 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 08 Jul 2021 18:35:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 08 Jul 2021 18:35:12 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 18:35:12 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 18:35:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 18:35:13 GMT
USER haproxy
# Thu, 08 Jul 2021 18:35:13 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7834d945b9e597e693f56fb0f9847718c1732b738a2f4956ab2c1b66c289d90`  
		Last Modified: Sat, 26 Jun 2021 02:56:43 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddff1cb6bb6da9a692c61843d46abe17a215c726bb13d570212777a87398a3d9`  
		Last Modified: Thu, 08 Jul 2021 18:38:36 GMT  
		Size: 7.3 MB (7315186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee55c5b3ebb2b318c44f2635d4eea44eadfd079d55d0b8c5a6918b8aa9d5b1dc`  
		Last Modified: Thu, 08 Jul 2021 18:38:34 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4.2-alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:b79f0c78bc069755084556b3bd897a39780d24fe70b909b7c119d53f9a6bbc01
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9912733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05e37a7293c9eccbd033a7a1a38aa77387373ba82f719cbcc400dec92a69aad3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:26 GMT
ADD file:c80bc2b093cbc0fc466582ef21cbed377de9fa874aedbf320079525ddacd1200 in / 
# Tue, 15 Jun 2021 22:57:26 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 02:02:51 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 19:07:43 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 08 Jul 2021 19:07:44 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 08 Jul 2021 19:07:44 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 08 Jul 2021 19:08:13 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 08 Jul 2021 19:08:13 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 19:08:14 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 19:08:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 19:08:15 GMT
USER haproxy
# Thu, 08 Jul 2021 19:08:15 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:b4c9a0924271af3466de27804af26420eb58da1466e7eaaba127d178b380fea3`  
		Last Modified: Tue, 15 Jun 2021 22:58:47 GMT  
		Size: 2.6 MB (2624382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85fa2947d9cc2655af4fd4aa21641629e791bcaf309a7095db77d309ddd05dfa`  
		Last Modified: Sat, 26 Jun 2021 02:08:45 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a9ab1152df106ecaf9c67a2a14b91a15581a3b86248b43604172b704b71167`  
		Last Modified: Thu, 08 Jul 2021 19:11:00 GMT  
		Size: 7.3 MB (7286705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc34702136897eee4ca8c94845af335a66311b8b8a57a5f1c40292b913ef9f72`  
		Last Modified: Thu, 08 Jul 2021 19:10:56 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4.2-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:b318934bc8973f8f73ad46a1c4f1c097899f57cdba1f6bff40285760584a684c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9631368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c900ed3b5e7e8ae25ede6582344b41bf064d26e831bdf4bfd385861422503a3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:05 GMT
ADD file:416a8b507abdc6bdcb22997a4be0a4170796c3f9f77e315b2dbff2b0a212bc68 in / 
# Tue, 15 Jun 2021 23:15:06 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 05:27:42 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 21:29:41 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 08 Jul 2021 21:29:42 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 08 Jul 2021 21:29:42 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 08 Jul 2021 21:30:19 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 08 Jul 2021 21:30:20 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 21:30:21 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 21:30:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 21:30:22 GMT
USER haproxy
# Thu, 08 Jul 2021 21:30:22 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:136482bf81d1fa351b424ebb8c7e34d15f2c5ed3fc0b66b544b8312bda3d52d9`  
		Last Modified: Tue, 15 Jun 2021 23:16:40 GMT  
		Size: 2.4 MB (2427917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5464af225bd487370319e7125fb2769222c5c7371d1be737936169d2e5b01c`  
		Last Modified: Sat, 26 Jun 2021 05:35:56 GMT  
		Size: 1.2 KB (1196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f903498f8e23244ca6430d647dd5515930d69394f19d017d07930d288ca6580`  
		Last Modified: Thu, 08 Jul 2021 21:36:22 GMT  
		Size: 7.2 MB (7201807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a0d8812e6df331ba2d781cc1fc08c2e4ddad2bb05b762b0eb737308a1205d5`  
		Last Modified: Thu, 08 Jul 2021 21:36:18 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4.2-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:c17729aebb94fdae2758381c550a8866ce8856237ce1892a6fba9d0cdadd7c5b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.1 MB (10133906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b500e8260787f1a0bcdc19f790686cd272d751cdd28f848f01eb2f054c700341`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 21:44:56 GMT
ADD file:6797caacbfe41bfe44000b39ed017016c6fcc492b3d6557cdaba88536df6c876 in / 
# Tue, 15 Jun 2021 21:44:56 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 02:13:15 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 19:02:27 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 08 Jul 2021 19:02:27 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 08 Jul 2021 19:02:27 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 08 Jul 2021 19:03:26 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 08 Jul 2021 19:03:26 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 19:03:27 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 19:03:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 19:03:27 GMT
USER haproxy
# Thu, 08 Jul 2021 19:03:27 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:58ab47519297212468320b23b8100fc1b2b96e8d342040806ae509a778a0a07a`  
		Last Modified: Tue, 15 Jun 2021 21:46:03 GMT  
		Size: 2.7 MB (2709626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb8dc96e2a4b7f90ae2dbfca981fe199966b64e3426ca1f742499d46ad1aa357`  
		Last Modified: Sat, 26 Jun 2021 02:21:19 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b367d065849fc1a609fb169119e94047ed3a2b475932bb292bff5b6cc45a1f`  
		Last Modified: Thu, 08 Jul 2021 19:07:30 GMT  
		Size: 7.4 MB (7422635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60cf6675a5a8e39f65c07f8553ab269ab83f947cbfa20da77e6da66ca033969e`  
		Last Modified: Thu, 08 Jul 2021 19:07:28 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4.2-alpine` - linux; 386

```console
$ docker pull haproxy@sha256:01a8472d10c0512c1950dad3ae7472f99767eeaa8f0bbbb3aa53813d35961ab0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (9998434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e50005241013c0fb9d14f539c88cbf5dd3ebfec6c0498014c4a70a002cbe3d48`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 21:38:30 GMT
ADD file:3b0fe1454491bb05e218b090fd461f2fd39546aa4a53eb3f953ee8eae149ac57 in / 
# Tue, 15 Jun 2021 21:38:30 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 01:39:05 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 19:03:09 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 08 Jul 2021 19:03:09 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 08 Jul 2021 19:03:09 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 08 Jul 2021 19:04:25 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 08 Jul 2021 19:04:25 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 19:04:25 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 19:04:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 19:04:26 GMT
USER haproxy
# Thu, 08 Jul 2021 19:04:26 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:be21df321efb39c5daf3151073ebff7688e15ea6cd5158878bc9559a5db76ac6`  
		Last Modified: Tue, 15 Jun 2021 21:39:16 GMT  
		Size: 2.8 MB (2820718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc6fe536c8e50a97873c166db7d3b669842dec91d85ce73433028b3b198a1c4`  
		Last Modified: Sat, 26 Jun 2021 01:49:46 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:832c00757ee7003ebca753eff8d4c6af86ebcf09efecec8e1171e550c8fc816f`  
		Last Modified: Thu, 08 Jul 2021 19:08:59 GMT  
		Size: 7.2 MB (7176071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85e6578d15134f65f8b977b9e7c9322e6281b3c765978ce760142c0bac7197ad`  
		Last Modified: Thu, 08 Jul 2021 19:08:57 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4.2-alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:8371490329ce959d92d6d6bca900a6702869e800fbd8c4a80438da13efa8b696
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.6 MB (10556641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5510c2e0b44e02d587dd27e62dd07ef69cc51b3e43f00927403e3c29eb34cfc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:27:00 GMT
ADD file:0075aad7a94f0496483442bb2d9fdaa13e9c23087b90638d014b4bc263aa3861 in / 
# Tue, 15 Jun 2021 22:27:03 GMT
CMD ["/bin/sh"]
# Fri, 16 Jul 2021 20:17:57 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 16 Jul 2021 20:19:42 GMT
ENV HAPROXY_VERSION=2.4.2
# Fri, 16 Jul 2021 20:19:48 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Fri, 16 Jul 2021 20:19:51 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 22 Jul 2021 03:04:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 22 Jul 2021 03:04:47 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 03:04:50 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 03:04:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 03:04:59 GMT
USER haproxy
# Thu, 22 Jul 2021 03:05:04 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:baf144cfb66ebe9df1969f3b90f1c448beff98edc84de1ccb5d6346195a070d4`  
		Last Modified: Tue, 15 Jun 2021 22:27:38 GMT  
		Size: 2.8 MB (2810478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e907663c9428bbbb731a221721c606bad29e54dac6f0dda85d6aa3175a725e`  
		Last Modified: Thu, 22 Jul 2021 03:40:16 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25fed8e719bd522b435fea4d6999c2ecffeb38e8288458cea40c3ecfa9131656`  
		Last Modified: Thu, 22 Jul 2021 03:40:53 GMT  
		Size: 7.7 MB (7744514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c45ecd590d1194b07f22c1e98348800abd5fdc2592d5c85e8fd5413acc1f29`  
		Last Modified: Thu, 22 Jul 2021 03:40:50 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.5-dev`

```console
$ docker pull haproxy@sha256:e91459e8fdcd49eb36c36312781f08ad8f5d8aa26c9c81489e57131cdb948258
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

### `haproxy:2.5-dev` - linux; amd64

```console
$ docker pull haproxy@sha256:bf0fc40d8665de6369ad6c517a55e63b7dc93dcd8d0ccc9f76bfbef5ae90b2c9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37412571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5c05bfc15437ed9d95f3f1454f1b65a7636063fe682bb157415b7f411b2a01a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 06:19:17 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 19 Jul 2021 20:19:58 GMT
ENV HAPROXY_VERSION=2.5-dev2
# Mon, 19 Jul 2021 20:19:58 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev2.tar.gz
# Mon, 19 Jul 2021 20:19:58 GMT
ENV HAPROXY_SHA256=34c2eee806f68bc892888c32477d9732e4610faf250d09aee6bea2d4f9fa5777
# Mon, 19 Jul 2021 20:20:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Mon, 19 Jul 2021 20:20:50 GMT
STOPSIGNAL SIGUSR1
# Mon, 19 Jul 2021 20:20:50 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 19 Jul 2021 20:20:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 19 Jul 2021 20:20:50 GMT
USER haproxy
# Mon, 19 Jul 2021 20:20:50 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91332cb81883405a321c1a2d2144bdd0aef8d1c69f90fdf0cf219982161b6e6e`  
		Last Modified: Wed, 23 Jun 2021 06:29:07 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66c209dcfe8f165048f6a9ae26c8ba09d7963402cfb278b38acf0dc6f3c5fa61`  
		Last Modified: Mon, 19 Jul 2021 20:23:15 GMT  
		Size: 10.3 MB (10264889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb9ed68b2620e2504c164fa92cb4a72b7aa2d68d349fa9ff3fc8cc0028834c6a`  
		Last Modified: Mon, 19 Jul 2021 20:23:13 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.5-dev` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:e55ab72555e1b8050393e2600ce9b582e1af1fa166ae106ec7b5cb4cea018643
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34779822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b24f5bd2e94969579e7bb676335ad4d7861d74fb8f834d6bdfd3df1d4c28c07f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 22 Jun 2021 23:50:09 GMT
ADD file:78d4ced31112d85490c684f350aceeebfc72a804262c7ad3e033257e3894f5c4 in / 
# Tue, 22 Jun 2021 23:50:11 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:15:11 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 19 Jul 2021 20:48:40 GMT
ENV HAPROXY_VERSION=2.5-dev2
# Mon, 19 Jul 2021 20:48:40 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev2.tar.gz
# Mon, 19 Jul 2021 20:48:41 GMT
ENV HAPROXY_SHA256=34c2eee806f68bc892888c32477d9732e4610faf250d09aee6bea2d4f9fa5777
# Mon, 19 Jul 2021 20:49:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Mon, 19 Jul 2021 20:49:33 GMT
STOPSIGNAL SIGUSR1
# Mon, 19 Jul 2021 20:49:34 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 19 Jul 2021 20:49:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 19 Jul 2021 20:49:35 GMT
USER haproxy
# Mon, 19 Jul 2021 20:49:36 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:532d6df30af5174ac6e1b379c32b8f464d44651ac060376a560c4a76a87704a7`  
		Last Modified: Wed, 23 Jun 2021 00:01:46 GMT  
		Size: 24.9 MB (24878945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48649e3d7de4cd80d3a9a34c725a2935be904ff90e99ea6c8e4bb6e1e7a4eeb7`  
		Last Modified: Wed, 23 Jun 2021 05:24:11 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0545e5132500350dc06ff151f05a2b7680b52828137ee41c7b816e10960c9596`  
		Last Modified: Mon, 19 Jul 2021 20:51:54 GMT  
		Size: 9.9 MB (9899051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af15fadccb57ba9f1e3e73f8ce1efdb6b60991b89b28390bd8b4886a2be782a8`  
		Last Modified: Mon, 19 Jul 2021 20:51:48 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.5-dev` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:17798523b8a7fe6c57f41d9eb14164d12ba7e84119bef0c27e41001bc903307e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.5 MB (32483310 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf3130e0248707a35c6e17746378b8889d5b212a53a5d7a967242c723b9983f5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:31 GMT
ADD file:8d200a3bbe985ff355343675c5555852f27550a9e367969df6bc98034efb8fd4 in / 
# Wed, 23 Jun 2021 00:20:31 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:21:41 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 19 Jul 2021 22:04:03 GMT
ENV HAPROXY_VERSION=2.5-dev2
# Mon, 19 Jul 2021 22:04:04 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev2.tar.gz
# Mon, 19 Jul 2021 22:04:04 GMT
ENV HAPROXY_SHA256=34c2eee806f68bc892888c32477d9732e4610faf250d09aee6bea2d4f9fa5777
# Mon, 19 Jul 2021 22:04:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Mon, 19 Jul 2021 22:04:52 GMT
STOPSIGNAL SIGUSR1
# Mon, 19 Jul 2021 22:04:52 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 19 Jul 2021 22:04:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 19 Jul 2021 22:04:53 GMT
USER haproxy
# Mon, 19 Jul 2021 22:04:54 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:8452be1adf00f91570fe21a8e61aaf4c12e014daf67d7de65d984f4e8ecca2f1`  
		Last Modified: Wed, 23 Jun 2021 00:31:49 GMT  
		Size: 22.7 MB (22746055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed1c9c92d0076fd4bf40503e3f47102509a5b99d182f4dd9e81e64d0a7e0b8a`  
		Last Modified: Wed, 23 Jun 2021 05:35:48 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e72d6a2939c6224b929df392236d82db340d3ba4ef4859ba2bea8b644ea47f22`  
		Last Modified: Mon, 19 Jul 2021 22:10:00 GMT  
		Size: 9.7 MB (9735426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a3e35f24f2e37079d3df25f32d2a042796e085fafba9d57faf8a9268ef47221`  
		Last Modified: Mon, 19 Jul 2021 22:09:54 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.5-dev` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:faa3bcdbe67a498ca404a917d19e2bda3e676bac667b934502ebb729db656a5d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.1 MB (36061996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c6c9ea4f56923bcc1914103a9c435a7bd3f26b885ffa62079579094afc28476`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:40 GMT
ADD file:beee00b59da720f68e12e2ba2a8134207c80c777ddb4ceb03c71e3e4c3f51c93 in / 
# Tue, 22 Jun 2021 23:49:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 03:19:31 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 19 Jul 2021 20:39:57 GMT
ENV HAPROXY_VERSION=2.5-dev2
# Mon, 19 Jul 2021 20:39:57 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev2.tar.gz
# Mon, 19 Jul 2021 20:39:58 GMT
ENV HAPROXY_SHA256=34c2eee806f68bc892888c32477d9732e4610faf250d09aee6bea2d4f9fa5777
# Mon, 19 Jul 2021 20:40:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Mon, 19 Jul 2021 20:40:40 GMT
STOPSIGNAL SIGUSR1
# Mon, 19 Jul 2021 20:40:40 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 19 Jul 2021 20:40:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 19 Jul 2021 20:40:41 GMT
USER haproxy
# Mon, 19 Jul 2021 20:40:41 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:448f6bf000e31217a7c202c659b03b7f8ac8d3ae6b03ef7a2f8339be2f00ff4a`  
		Last Modified: Tue, 22 Jun 2021 23:55:25 GMT  
		Size: 25.9 MB (25914993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b05ad81dc8a7d67656235988f0e5fb72c374c7d8df44c105b91d712e06c4ac`  
		Last Modified: Wed, 23 Jun 2021 03:26:16 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b51a038984cd049eaaa5a2e8b13fadc6e46fc5d6dbda0a3f3de3908442fe701`  
		Last Modified: Mon, 19 Jul 2021 20:44:04 GMT  
		Size: 10.1 MB (10145173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:865e8fa76c1bd5e14eacaa3cf6350d2728ab2066aaa43ece4f0939e9aaef5657`  
		Last Modified: Mon, 19 Jul 2021 20:44:02 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.5-dev` - linux; 386

```console
$ docker pull haproxy@sha256:1a840103d609689559fb1a8e00f25fae4fdb4a6db7704c517a12f2e8d54d5d7e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.9 MB (37903685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2920f2bc63a6d5cfde69881c748e26e057d5289d5aadfc4058a6b76e46df1934`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 22 Jun 2021 23:39:35 GMT
ADD file:48f656ac6733911048b3de850490438d0233b3badc11861fca62062d4edfaf40 in / 
# Tue, 22 Jun 2021 23:39:35 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:23:13 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 19 Jul 2021 20:38:36 GMT
ENV HAPROXY_VERSION=2.5-dev2
# Mon, 19 Jul 2021 20:38:36 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev2.tar.gz
# Mon, 19 Jul 2021 20:38:37 GMT
ENV HAPROXY_SHA256=34c2eee806f68bc892888c32477d9732e4610faf250d09aee6bea2d4f9fa5777
# Mon, 19 Jul 2021 20:39:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Mon, 19 Jul 2021 20:39:32 GMT
STOPSIGNAL SIGUSR1
# Mon, 19 Jul 2021 20:39:33 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 19 Jul 2021 20:39:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 19 Jul 2021 20:39:33 GMT
USER haproxy
# Mon, 19 Jul 2021 20:39:33 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:33af2dcb865e65d53cdeb843b67a0ef62151fa32df292293e7c6b0eb728ac5ac`  
		Last Modified: Tue, 22 Jun 2021 23:46:23 GMT  
		Size: 27.8 MB (27797411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a6e4d42b23996eb7d8a1baa85ee19828c2667fd4a2dca6eb1040b266680e9f`  
		Last Modified: Wed, 23 Jun 2021 00:32:00 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33cc48c758b0c469549ce417d46a3225b3778676962833651ccee76618641a9`  
		Last Modified: Mon, 19 Jul 2021 20:43:11 GMT  
		Size: 10.1 MB (10104446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963183e2fdff3997e532fd330fce8f8cbb1741fb6c7f0c1368442e54954b524d`  
		Last Modified: Mon, 19 Jul 2021 20:43:09 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.5-dev` - linux; mips64le

```console
$ docker pull haproxy@sha256:587e6f1b6708a5fb8e509527c48e8d6ad0b6d7a93510e21ac3a41c9663cd9bd0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.7 MB (35705393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf89984299bd1584db6f29a5a5be0c953c9ddd447ec4052f00565e0490282c1d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 22 Jul 2021 00:09:45 GMT
ADD file:1f77b9001c4977ba733be674fc5eb4b85130f1dea8a7b39d545b70f9c107695f in / 
# Thu, 22 Jul 2021 00:09:46 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:07:49 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 22 Jul 2021 01:07:49 GMT
ENV HAPROXY_VERSION=2.5-dev2
# Thu, 22 Jul 2021 01:07:50 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev2.tar.gz
# Thu, 22 Jul 2021 01:07:50 GMT
ENV HAPROXY_SHA256=34c2eee806f68bc892888c32477d9732e4610faf250d09aee6bea2d4f9fa5777
# Thu, 22 Jul 2021 01:10:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 22 Jul 2021 01:10:20 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 01:10:20 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 01:10:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 01:10:21 GMT
USER haproxy
# Thu, 22 Jul 2021 01:10:21 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:99ee621d0b0485e9de65aa19604aa2453d19ea7fc86b22c5b77c1bab74e3cb42`  
		Last Modified: Thu, 22 Jul 2021 00:16:11 GMT  
		Size: 25.8 MB (25812771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f444627794f98947a9df95ec5d19b2a1cd6c151ed438982b1dc0b89f5eaf19e`  
		Last Modified: Thu, 22 Jul 2021 01:24:39 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af78d65613ad4c895f5faa33e45a488e3c5b80b6bbfb909e596c3b45aa03f4d2`  
		Last Modified: Thu, 22 Jul 2021 01:24:46 GMT  
		Size: 9.9 MB (9890792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f4c8fcc371badbebc85cd184033e4e971729e2250cc3ff7eb7fdafdf3e5b8c7`  
		Last Modified: Thu, 22 Jul 2021 01:24:39 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.5-dev` - linux; ppc64le

```console
$ docker pull haproxy@sha256:9628eda260937df3053662bc6ef5021a73288121a4b5ad42fda517548f4ac104
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41337072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fee84aa56c5f735d2ddd9e9ee05aead0629cecc842c1e75988b66fe4556e159f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 22 Jul 2021 00:19:04 GMT
ADD file:3a6bd6ce3eff98b88a13de5d0f26cff0b026f876674204dbad6f84fafcf145b1 in / 
# Thu, 22 Jul 2021 00:19:13 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 02:52:46 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 22 Jul 2021 02:52:48 GMT
ENV HAPROXY_VERSION=2.5-dev2
# Thu, 22 Jul 2021 02:52:51 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev2.tar.gz
# Thu, 22 Jul 2021 02:52:54 GMT
ENV HAPROXY_SHA256=34c2eee806f68bc892888c32477d9732e4610faf250d09aee6bea2d4f9fa5777
# Thu, 22 Jul 2021 02:57:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 22 Jul 2021 02:57:32 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 02:57:35 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 02:57:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 02:57:49 GMT
USER haproxy
# Thu, 22 Jul 2021 02:57:55 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:1130517d52da84a09f9465006bddab5e49afd398860890eab6274fd0bff32371`  
		Last Modified: Thu, 22 Jul 2021 00:27:49 GMT  
		Size: 30.6 MB (30553709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251bf3fe1d4bbe9c27e393cd8ddc550b56cec90eb916bf9bec24d657c9f6556f`  
		Last Modified: Thu, 22 Jul 2021 03:40:01 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e541a77e80948d994e130c58cab9eeca18dfa8926bbae633afa238f254ead6db`  
		Last Modified: Thu, 22 Jul 2021 03:40:04 GMT  
		Size: 10.8 MB (10781535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e6bee79099d0dac33ae4ae8ae713b806048f5a75b60da7eb38dd73f12afe5a3`  
		Last Modified: Thu, 22 Jul 2021 03:40:01 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.5-dev` - linux; s390x

```console
$ docker pull haproxy@sha256:209e9fea2a0a2e89d75e9807ce2054c069b29411bddb4aadd6e3b0ef0a76eae4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.7 MB (35709317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5de350c41ba70768387f48e0bfc020047d1811390312bfde9bdfc7c876f92af`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 22 Jul 2021 00:42:45 GMT
ADD file:1ab999eb6f80d8ce91ce3a173e23fd2710f2779117bba29037eaa82aadcbf6ed in / 
# Thu, 22 Jul 2021 00:42:48 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:30:19 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 22 Jul 2021 01:30:19 GMT
ENV HAPROXY_VERSION=2.5-dev2
# Thu, 22 Jul 2021 01:30:20 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev2.tar.gz
# Thu, 22 Jul 2021 01:30:20 GMT
ENV HAPROXY_SHA256=34c2eee806f68bc892888c32477d9732e4610faf250d09aee6bea2d4f9fa5777
# Thu, 22 Jul 2021 01:30:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 22 Jul 2021 01:31:00 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 01:31:00 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 01:31:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 01:31:01 GMT
USER haproxy
# Thu, 22 Jul 2021 01:31:01 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:7a50fdd85ff244c1465e71c51354d055e3df0b90ff5faad28cc22d9ecde9daf3`  
		Last Modified: Thu, 22 Jul 2021 00:48:13 GMT  
		Size: 25.8 MB (25760761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05fb34d1ed21b67502665114a7ae60445472fc7bafa620bbf6c79b7df85a01d4`  
		Last Modified: Thu, 22 Jul 2021 01:39:54 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa91183bd1605686e9b95641fbb9536985642c023164d3ac759fe2212041ac28`  
		Last Modified: Thu, 22 Jul 2021 01:39:55 GMT  
		Size: 9.9 MB (9946726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92689905b44b2a82e92bd2442ba6ed05aca6bbed461837a4b9063c933c934d9f`  
		Last Modified: Thu, 22 Jul 2021 01:39:54 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.5-dev-alpine`

```console
$ docker pull haproxy@sha256:433f7d381db23fbae0e71c7e1765a2d20cbf34b8ed4c94f241eedaa7c846437e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `haproxy:2.5-dev-alpine` - linux; amd64

```console
$ docker pull haproxy@sha256:285c441480b9472edac38f7f3a8c9bc944d5ae741e5315880f9e786449b307a9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.2 MB (10247274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e44b5d3cc93e51de6ca73abbe4c9af56e6ae9271a5733c3b75e7cbd36ef9d7a8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 02:48:50 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 19 Jul 2021 20:20:58 GMT
ENV HAPROXY_VERSION=2.5-dev2
# Mon, 19 Jul 2021 20:20:58 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev2.tar.gz
# Mon, 19 Jul 2021 20:20:58 GMT
ENV HAPROXY_SHA256=34c2eee806f68bc892888c32477d9732e4610faf250d09aee6bea2d4f9fa5777
# Mon, 19 Jul 2021 20:21:59 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Mon, 19 Jul 2021 20:21:59 GMT
STOPSIGNAL SIGUSR1
# Mon, 19 Jul 2021 20:21:59 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 19 Jul 2021 20:21:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 19 Jul 2021 20:22:00 GMT
USER haproxy
# Mon, 19 Jul 2021 20:22:00 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7834d945b9e597e693f56fb0f9847718c1732b738a2f4956ab2c1b66c289d90`  
		Last Modified: Sat, 26 Jun 2021 02:56:43 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9748714368d19c518c7cea20a72f82aef224e9a83a35c47b9a30703ff07338e8`  
		Last Modified: Mon, 19 Jul 2021 20:23:26 GMT  
		Size: 7.4 MB (7434154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e3d039a8ccce39b26a30411867661c2ba7fafce288b2fc89b8cecbbf9fc2fc0`  
		Last Modified: Mon, 19 Jul 2021 20:23:25 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.5-dev-alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:6e51da9ec54287f9f9386c3cac05f9414f0d5ee05e187019839df93d4bd70af6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (10016132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c09290cc5a02b7585e7f99af07b3aab045e09ea91f90547938dd41404673d8d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:26 GMT
ADD file:c80bc2b093cbc0fc466582ef21cbed377de9fa874aedbf320079525ddacd1200 in / 
# Tue, 15 Jun 2021 22:57:26 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 02:02:51 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 19 Jul 2021 20:51:14 GMT
ENV HAPROXY_VERSION=2.5-dev2
# Mon, 19 Jul 2021 20:51:14 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev2.tar.gz
# Mon, 19 Jul 2021 20:51:15 GMT
ENV HAPROXY_SHA256=34c2eee806f68bc892888c32477d9732e4610faf250d09aee6bea2d4f9fa5777
# Mon, 19 Jul 2021 20:51:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Mon, 19 Jul 2021 20:51:43 GMT
STOPSIGNAL SIGUSR1
# Mon, 19 Jul 2021 20:51:43 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 19 Jul 2021 20:51:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 19 Jul 2021 20:51:44 GMT
USER haproxy
# Mon, 19 Jul 2021 20:51:45 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:b4c9a0924271af3466de27804af26420eb58da1466e7eaaba127d178b380fea3`  
		Last Modified: Tue, 15 Jun 2021 22:58:47 GMT  
		Size: 2.6 MB (2624382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85fa2947d9cc2655af4fd4aa21641629e791bcaf309a7095db77d309ddd05dfa`  
		Last Modified: Sat, 26 Jun 2021 02:08:45 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:528eaf13fb9650e1aa29c9c7237489fef17436ffdbf3210810247d274b44828c`  
		Last Modified: Mon, 19 Jul 2021 20:54:02 GMT  
		Size: 7.4 MB (7390108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ddc7abd5e0eac09889562b8699def80aa605077352ba82f7536c86660aab96f`  
		Last Modified: Mon, 19 Jul 2021 20:53:56 GMT  
		Size: 447.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.5-dev-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:d29ea3244794cb62bbc4da76c9bac7470708ad183c56b6f44bbd7cef3721c7b5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9748891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8eba494332ee1b97e98472b42473451c05c08b637207985c69357b0e7a9d0579`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:05 GMT
ADD file:416a8b507abdc6bdcb22997a4be0a4170796c3f9f77e315b2dbff2b0a212bc68 in / 
# Tue, 15 Jun 2021 23:15:06 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 05:27:42 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 19 Jul 2021 22:05:09 GMT
ENV HAPROXY_VERSION=2.5-dev2
# Mon, 19 Jul 2021 22:05:10 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev2.tar.gz
# Mon, 19 Jul 2021 22:05:10 GMT
ENV HAPROXY_SHA256=34c2eee806f68bc892888c32477d9732e4610faf250d09aee6bea2d4f9fa5777
# Mon, 19 Jul 2021 22:05:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Mon, 19 Jul 2021 22:05:38 GMT
STOPSIGNAL SIGUSR1
# Mon, 19 Jul 2021 22:05:38 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 19 Jul 2021 22:05:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 19 Jul 2021 22:05:39 GMT
USER haproxy
# Mon, 19 Jul 2021 22:05:40 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:136482bf81d1fa351b424ebb8c7e34d15f2c5ed3fc0b66b544b8312bda3d52d9`  
		Last Modified: Tue, 15 Jun 2021 23:16:40 GMT  
		Size: 2.4 MB (2427917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5464af225bd487370319e7125fb2769222c5c7371d1be737936169d2e5b01c`  
		Last Modified: Sat, 26 Jun 2021 05:35:56 GMT  
		Size: 1.2 KB (1196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fb6f783f6a974eec5cbb8fe40b15d5094d8b1706951bf89b672c96c1c24890c`  
		Last Modified: Mon, 19 Jul 2021 22:10:18 GMT  
		Size: 7.3 MB (7319329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5173583e05b8ea8863c18c69d9e5724d17659387960267599d9f148330e8767`  
		Last Modified: Mon, 19 Jul 2021 22:10:13 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.5-dev-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:b103722ad8547adf72c6abf584808f5965dc9624f27f22bb153335f3e6a42e9a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.3 MB (10253414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfacf2b0908da0a4fb1ad07166604ac80689fff3b49d44f8c27595fd96a2dc0b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 21:44:56 GMT
ADD file:6797caacbfe41bfe44000b39ed017016c6fcc492b3d6557cdaba88536df6c876 in / 
# Tue, 15 Jun 2021 21:44:56 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 02:13:15 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 19 Jul 2021 20:40:49 GMT
ENV HAPROXY_VERSION=2.5-dev2
# Mon, 19 Jul 2021 20:40:49 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev2.tar.gz
# Mon, 19 Jul 2021 20:40:49 GMT
ENV HAPROXY_SHA256=34c2eee806f68bc892888c32477d9732e4610faf250d09aee6bea2d4f9fa5777
# Mon, 19 Jul 2021 20:41:49 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Mon, 19 Jul 2021 20:41:49 GMT
STOPSIGNAL SIGUSR1
# Mon, 19 Jul 2021 20:41:50 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 19 Jul 2021 20:41:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 19 Jul 2021 20:41:50 GMT
USER haproxy
# Mon, 19 Jul 2021 20:41:50 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:58ab47519297212468320b23b8100fc1b2b96e8d342040806ae509a778a0a07a`  
		Last Modified: Tue, 15 Jun 2021 21:46:03 GMT  
		Size: 2.7 MB (2709626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb8dc96e2a4b7f90ae2dbfca981fe199966b64e3426ca1f742499d46ad1aa357`  
		Last Modified: Sat, 26 Jun 2021 02:21:19 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:067b9aa25fba74d6c9e77ed1a9c3d3157ba07893b06e5f97cf0b91afe570585c`  
		Last Modified: Mon, 19 Jul 2021 20:44:17 GMT  
		Size: 7.5 MB (7542146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052aefb4611ad99c43a5abd99e6a593db80fed0ff3f12e5fe57f2f659ac76fca`  
		Last Modified: Mon, 19 Jul 2021 20:44:15 GMT  
		Size: 445.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.5-dev-alpine` - linux; 386

```console
$ docker pull haproxy@sha256:6e2d016d57b800c954ac40a0ad7dab22a6f686a8ea4d2cd11c801a2df1f4aa6a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.1 MB (10103291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2dd830195af5cbec860580475781babb20937ac58423f82d963b5ef656201edb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 21:38:30 GMT
ADD file:3b0fe1454491bb05e218b090fd461f2fd39546aa4a53eb3f953ee8eae149ac57 in / 
# Tue, 15 Jun 2021 21:38:30 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 01:39:05 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 19 Jul 2021 20:39:39 GMT
ENV HAPROXY_VERSION=2.5-dev2
# Mon, 19 Jul 2021 20:39:39 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev2.tar.gz
# Mon, 19 Jul 2021 20:39:39 GMT
ENV HAPROXY_SHA256=34c2eee806f68bc892888c32477d9732e4610faf250d09aee6bea2d4f9fa5777
# Mon, 19 Jul 2021 20:40:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Mon, 19 Jul 2021 20:40:48 GMT
STOPSIGNAL SIGUSR1
# Mon, 19 Jul 2021 20:40:49 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 19 Jul 2021 20:40:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 19 Jul 2021 20:40:49 GMT
USER haproxy
# Mon, 19 Jul 2021 20:40:49 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:be21df321efb39c5daf3151073ebff7688e15ea6cd5158878bc9559a5db76ac6`  
		Last Modified: Tue, 15 Jun 2021 21:39:16 GMT  
		Size: 2.8 MB (2820718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc6fe536c8e50a97873c166db7d3b669842dec91d85ce73433028b3b198a1c4`  
		Last Modified: Sat, 26 Jun 2021 01:49:46 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:796ca18efd1209b0147e4fffea36abda4cd7b4773541f996ab699d77c61b86c0`  
		Last Modified: Mon, 19 Jul 2021 20:43:24 GMT  
		Size: 7.3 MB (7280930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e2759026673ac7b4c18d0e5e7aa4dd1e85392b04cdbc8bdc29af8ad9775753`  
		Last Modified: Mon, 19 Jul 2021 20:43:22 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.5-dev-alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:c93e04b42d7ebf4111a9cbd90d38e8bef5438ad008714e231354ac5e06aefca8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.7 MB (10676989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ed0aa53dd5cbf72232a21725e8a69f46645c5dbd7eb06555d196a5698fd9458`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:27:00 GMT
ADD file:0075aad7a94f0496483442bb2d9fdaa13e9c23087b90638d014b4bc263aa3861 in / 
# Tue, 15 Jun 2021 22:27:03 GMT
CMD ["/bin/sh"]
# Fri, 16 Jul 2021 20:17:57 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 19 Jul 2021 20:22:41 GMT
ENV HAPROXY_VERSION=2.5-dev2
# Mon, 19 Jul 2021 20:22:48 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev2.tar.gz
# Mon, 19 Jul 2021 20:22:54 GMT
ENV HAPROXY_SHA256=34c2eee806f68bc892888c32477d9732e4610faf250d09aee6bea2d4f9fa5777
# Thu, 22 Jul 2021 02:58:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 22 Jul 2021 02:58:57 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 02:58:59 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 02:59:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 02:59:08 GMT
USER haproxy
# Thu, 22 Jul 2021 02:59:17 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:baf144cfb66ebe9df1969f3b90f1c448beff98edc84de1ccb5d6346195a070d4`  
		Last Modified: Tue, 15 Jun 2021 22:27:38 GMT  
		Size: 2.8 MB (2810478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e907663c9428bbbb731a221721c606bad29e54dac6f0dda85d6aa3175a725e`  
		Last Modified: Thu, 22 Jul 2021 03:40:16 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45e3511671e77d8086d4858c635cd3bc9d363b6933ccd46baf12a3b10fdedfa5`  
		Last Modified: Thu, 22 Jul 2021 03:40:17 GMT  
		Size: 7.9 MB (7864861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:796b651947f6e02a1e51f0a2b0bfbe212a8d3886fbed5e7ad77ccdc97bb117e0`  
		Last Modified: Thu, 22 Jul 2021 03:40:16 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.5-dev-alpine` - linux; s390x

```console
$ docker pull haproxy@sha256:e72417786e6b2cd712168a5e7f30765f0d43c08862b357d56a5d89b9d6c8d552
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9899016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89f7571e36d5cd7a81877a3a147bc540bab5011e63a020b3cbaa0d239961cc4a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:54:24 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:42:56 GMT
ENV HAPROXY_VERSION=2.5-dev0
# Fri, 14 May 2021 19:42:57 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev0.tar.gz
# Fri, 14 May 2021 19:42:57 GMT
ENV HAPROXY_SHA256=6ee45b5047649b2df3fd48f6659860e8845d970bd4e0c1764490a54c3047bd23
# Fri, 14 May 2021 19:43:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 14 May 2021 19:43:53 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:43:53 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:43:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:43:54 GMT
USER haproxy
# Fri, 14 May 2021 19:43:55 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267275aba58470c82626189a59be76cd169bd245568e2f2545ed1ee64ff8a8ff`  
		Last Modified: Wed, 14 Apr 2021 20:59:06 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b79e3a1c3d9c059731828093ca4846dfff4ba8ad68671e62fa5d5df56590563`  
		Last Modified: Fri, 14 May 2021 19:47:45 GMT  
		Size: 7.3 MB (7294732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9093b846e5e13ecfca4b82d2d45fd7bdc1c0d026e4fbc93faf64e9d450f9b485`  
		Last Modified: Fri, 14 May 2021 19:47:43 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.5-dev2`

```console
$ docker pull haproxy@sha256:e91459e8fdcd49eb36c36312781f08ad8f5d8aa26c9c81489e57131cdb948258
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

### `haproxy:2.5-dev2` - linux; amd64

```console
$ docker pull haproxy@sha256:bf0fc40d8665de6369ad6c517a55e63b7dc93dcd8d0ccc9f76bfbef5ae90b2c9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37412571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5c05bfc15437ed9d95f3f1454f1b65a7636063fe682bb157415b7f411b2a01a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 06:19:17 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 19 Jul 2021 20:19:58 GMT
ENV HAPROXY_VERSION=2.5-dev2
# Mon, 19 Jul 2021 20:19:58 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev2.tar.gz
# Mon, 19 Jul 2021 20:19:58 GMT
ENV HAPROXY_SHA256=34c2eee806f68bc892888c32477d9732e4610faf250d09aee6bea2d4f9fa5777
# Mon, 19 Jul 2021 20:20:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Mon, 19 Jul 2021 20:20:50 GMT
STOPSIGNAL SIGUSR1
# Mon, 19 Jul 2021 20:20:50 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 19 Jul 2021 20:20:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 19 Jul 2021 20:20:50 GMT
USER haproxy
# Mon, 19 Jul 2021 20:20:50 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91332cb81883405a321c1a2d2144bdd0aef8d1c69f90fdf0cf219982161b6e6e`  
		Last Modified: Wed, 23 Jun 2021 06:29:07 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66c209dcfe8f165048f6a9ae26c8ba09d7963402cfb278b38acf0dc6f3c5fa61`  
		Last Modified: Mon, 19 Jul 2021 20:23:15 GMT  
		Size: 10.3 MB (10264889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb9ed68b2620e2504c164fa92cb4a72b7aa2d68d349fa9ff3fc8cc0028834c6a`  
		Last Modified: Mon, 19 Jul 2021 20:23:13 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.5-dev2` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:e55ab72555e1b8050393e2600ce9b582e1af1fa166ae106ec7b5cb4cea018643
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34779822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b24f5bd2e94969579e7bb676335ad4d7861d74fb8f834d6bdfd3df1d4c28c07f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 22 Jun 2021 23:50:09 GMT
ADD file:78d4ced31112d85490c684f350aceeebfc72a804262c7ad3e033257e3894f5c4 in / 
# Tue, 22 Jun 2021 23:50:11 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:15:11 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 19 Jul 2021 20:48:40 GMT
ENV HAPROXY_VERSION=2.5-dev2
# Mon, 19 Jul 2021 20:48:40 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev2.tar.gz
# Mon, 19 Jul 2021 20:48:41 GMT
ENV HAPROXY_SHA256=34c2eee806f68bc892888c32477d9732e4610faf250d09aee6bea2d4f9fa5777
# Mon, 19 Jul 2021 20:49:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Mon, 19 Jul 2021 20:49:33 GMT
STOPSIGNAL SIGUSR1
# Mon, 19 Jul 2021 20:49:34 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 19 Jul 2021 20:49:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 19 Jul 2021 20:49:35 GMT
USER haproxy
# Mon, 19 Jul 2021 20:49:36 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:532d6df30af5174ac6e1b379c32b8f464d44651ac060376a560c4a76a87704a7`  
		Last Modified: Wed, 23 Jun 2021 00:01:46 GMT  
		Size: 24.9 MB (24878945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48649e3d7de4cd80d3a9a34c725a2935be904ff90e99ea6c8e4bb6e1e7a4eeb7`  
		Last Modified: Wed, 23 Jun 2021 05:24:11 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0545e5132500350dc06ff151f05a2b7680b52828137ee41c7b816e10960c9596`  
		Last Modified: Mon, 19 Jul 2021 20:51:54 GMT  
		Size: 9.9 MB (9899051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af15fadccb57ba9f1e3e73f8ce1efdb6b60991b89b28390bd8b4886a2be782a8`  
		Last Modified: Mon, 19 Jul 2021 20:51:48 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.5-dev2` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:17798523b8a7fe6c57f41d9eb14164d12ba7e84119bef0c27e41001bc903307e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.5 MB (32483310 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf3130e0248707a35c6e17746378b8889d5b212a53a5d7a967242c723b9983f5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:31 GMT
ADD file:8d200a3bbe985ff355343675c5555852f27550a9e367969df6bc98034efb8fd4 in / 
# Wed, 23 Jun 2021 00:20:31 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:21:41 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 19 Jul 2021 22:04:03 GMT
ENV HAPROXY_VERSION=2.5-dev2
# Mon, 19 Jul 2021 22:04:04 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev2.tar.gz
# Mon, 19 Jul 2021 22:04:04 GMT
ENV HAPROXY_SHA256=34c2eee806f68bc892888c32477d9732e4610faf250d09aee6bea2d4f9fa5777
# Mon, 19 Jul 2021 22:04:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Mon, 19 Jul 2021 22:04:52 GMT
STOPSIGNAL SIGUSR1
# Mon, 19 Jul 2021 22:04:52 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 19 Jul 2021 22:04:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 19 Jul 2021 22:04:53 GMT
USER haproxy
# Mon, 19 Jul 2021 22:04:54 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:8452be1adf00f91570fe21a8e61aaf4c12e014daf67d7de65d984f4e8ecca2f1`  
		Last Modified: Wed, 23 Jun 2021 00:31:49 GMT  
		Size: 22.7 MB (22746055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed1c9c92d0076fd4bf40503e3f47102509a5b99d182f4dd9e81e64d0a7e0b8a`  
		Last Modified: Wed, 23 Jun 2021 05:35:48 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e72d6a2939c6224b929df392236d82db340d3ba4ef4859ba2bea8b644ea47f22`  
		Last Modified: Mon, 19 Jul 2021 22:10:00 GMT  
		Size: 9.7 MB (9735426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a3e35f24f2e37079d3df25f32d2a042796e085fafba9d57faf8a9268ef47221`  
		Last Modified: Mon, 19 Jul 2021 22:09:54 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.5-dev2` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:faa3bcdbe67a498ca404a917d19e2bda3e676bac667b934502ebb729db656a5d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.1 MB (36061996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c6c9ea4f56923bcc1914103a9c435a7bd3f26b885ffa62079579094afc28476`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:40 GMT
ADD file:beee00b59da720f68e12e2ba2a8134207c80c777ddb4ceb03c71e3e4c3f51c93 in / 
# Tue, 22 Jun 2021 23:49:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 03:19:31 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 19 Jul 2021 20:39:57 GMT
ENV HAPROXY_VERSION=2.5-dev2
# Mon, 19 Jul 2021 20:39:57 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev2.tar.gz
# Mon, 19 Jul 2021 20:39:58 GMT
ENV HAPROXY_SHA256=34c2eee806f68bc892888c32477d9732e4610faf250d09aee6bea2d4f9fa5777
# Mon, 19 Jul 2021 20:40:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Mon, 19 Jul 2021 20:40:40 GMT
STOPSIGNAL SIGUSR1
# Mon, 19 Jul 2021 20:40:40 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 19 Jul 2021 20:40:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 19 Jul 2021 20:40:41 GMT
USER haproxy
# Mon, 19 Jul 2021 20:40:41 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:448f6bf000e31217a7c202c659b03b7f8ac8d3ae6b03ef7a2f8339be2f00ff4a`  
		Last Modified: Tue, 22 Jun 2021 23:55:25 GMT  
		Size: 25.9 MB (25914993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b05ad81dc8a7d67656235988f0e5fb72c374c7d8df44c105b91d712e06c4ac`  
		Last Modified: Wed, 23 Jun 2021 03:26:16 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b51a038984cd049eaaa5a2e8b13fadc6e46fc5d6dbda0a3f3de3908442fe701`  
		Last Modified: Mon, 19 Jul 2021 20:44:04 GMT  
		Size: 10.1 MB (10145173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:865e8fa76c1bd5e14eacaa3cf6350d2728ab2066aaa43ece4f0939e9aaef5657`  
		Last Modified: Mon, 19 Jul 2021 20:44:02 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.5-dev2` - linux; 386

```console
$ docker pull haproxy@sha256:1a840103d609689559fb1a8e00f25fae4fdb4a6db7704c517a12f2e8d54d5d7e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.9 MB (37903685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2920f2bc63a6d5cfde69881c748e26e057d5289d5aadfc4058a6b76e46df1934`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 22 Jun 2021 23:39:35 GMT
ADD file:48f656ac6733911048b3de850490438d0233b3badc11861fca62062d4edfaf40 in / 
# Tue, 22 Jun 2021 23:39:35 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:23:13 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 19 Jul 2021 20:38:36 GMT
ENV HAPROXY_VERSION=2.5-dev2
# Mon, 19 Jul 2021 20:38:36 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev2.tar.gz
# Mon, 19 Jul 2021 20:38:37 GMT
ENV HAPROXY_SHA256=34c2eee806f68bc892888c32477d9732e4610faf250d09aee6bea2d4f9fa5777
# Mon, 19 Jul 2021 20:39:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Mon, 19 Jul 2021 20:39:32 GMT
STOPSIGNAL SIGUSR1
# Mon, 19 Jul 2021 20:39:33 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 19 Jul 2021 20:39:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 19 Jul 2021 20:39:33 GMT
USER haproxy
# Mon, 19 Jul 2021 20:39:33 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:33af2dcb865e65d53cdeb843b67a0ef62151fa32df292293e7c6b0eb728ac5ac`  
		Last Modified: Tue, 22 Jun 2021 23:46:23 GMT  
		Size: 27.8 MB (27797411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a6e4d42b23996eb7d8a1baa85ee19828c2667fd4a2dca6eb1040b266680e9f`  
		Last Modified: Wed, 23 Jun 2021 00:32:00 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33cc48c758b0c469549ce417d46a3225b3778676962833651ccee76618641a9`  
		Last Modified: Mon, 19 Jul 2021 20:43:11 GMT  
		Size: 10.1 MB (10104446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963183e2fdff3997e532fd330fce8f8cbb1741fb6c7f0c1368442e54954b524d`  
		Last Modified: Mon, 19 Jul 2021 20:43:09 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.5-dev2` - linux; mips64le

```console
$ docker pull haproxy@sha256:587e6f1b6708a5fb8e509527c48e8d6ad0b6d7a93510e21ac3a41c9663cd9bd0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.7 MB (35705393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf89984299bd1584db6f29a5a5be0c953c9ddd447ec4052f00565e0490282c1d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 22 Jul 2021 00:09:45 GMT
ADD file:1f77b9001c4977ba733be674fc5eb4b85130f1dea8a7b39d545b70f9c107695f in / 
# Thu, 22 Jul 2021 00:09:46 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:07:49 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 22 Jul 2021 01:07:49 GMT
ENV HAPROXY_VERSION=2.5-dev2
# Thu, 22 Jul 2021 01:07:50 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev2.tar.gz
# Thu, 22 Jul 2021 01:07:50 GMT
ENV HAPROXY_SHA256=34c2eee806f68bc892888c32477d9732e4610faf250d09aee6bea2d4f9fa5777
# Thu, 22 Jul 2021 01:10:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 22 Jul 2021 01:10:20 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 01:10:20 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 01:10:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 01:10:21 GMT
USER haproxy
# Thu, 22 Jul 2021 01:10:21 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:99ee621d0b0485e9de65aa19604aa2453d19ea7fc86b22c5b77c1bab74e3cb42`  
		Last Modified: Thu, 22 Jul 2021 00:16:11 GMT  
		Size: 25.8 MB (25812771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f444627794f98947a9df95ec5d19b2a1cd6c151ed438982b1dc0b89f5eaf19e`  
		Last Modified: Thu, 22 Jul 2021 01:24:39 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af78d65613ad4c895f5faa33e45a488e3c5b80b6bbfb909e596c3b45aa03f4d2`  
		Last Modified: Thu, 22 Jul 2021 01:24:46 GMT  
		Size: 9.9 MB (9890792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f4c8fcc371badbebc85cd184033e4e971729e2250cc3ff7eb7fdafdf3e5b8c7`  
		Last Modified: Thu, 22 Jul 2021 01:24:39 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.5-dev2` - linux; ppc64le

```console
$ docker pull haproxy@sha256:9628eda260937df3053662bc6ef5021a73288121a4b5ad42fda517548f4ac104
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41337072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fee84aa56c5f735d2ddd9e9ee05aead0629cecc842c1e75988b66fe4556e159f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 22 Jul 2021 00:19:04 GMT
ADD file:3a6bd6ce3eff98b88a13de5d0f26cff0b026f876674204dbad6f84fafcf145b1 in / 
# Thu, 22 Jul 2021 00:19:13 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 02:52:46 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 22 Jul 2021 02:52:48 GMT
ENV HAPROXY_VERSION=2.5-dev2
# Thu, 22 Jul 2021 02:52:51 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev2.tar.gz
# Thu, 22 Jul 2021 02:52:54 GMT
ENV HAPROXY_SHA256=34c2eee806f68bc892888c32477d9732e4610faf250d09aee6bea2d4f9fa5777
# Thu, 22 Jul 2021 02:57:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 22 Jul 2021 02:57:32 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 02:57:35 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 02:57:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 02:57:49 GMT
USER haproxy
# Thu, 22 Jul 2021 02:57:55 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:1130517d52da84a09f9465006bddab5e49afd398860890eab6274fd0bff32371`  
		Last Modified: Thu, 22 Jul 2021 00:27:49 GMT  
		Size: 30.6 MB (30553709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251bf3fe1d4bbe9c27e393cd8ddc550b56cec90eb916bf9bec24d657c9f6556f`  
		Last Modified: Thu, 22 Jul 2021 03:40:01 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e541a77e80948d994e130c58cab9eeca18dfa8926bbae633afa238f254ead6db`  
		Last Modified: Thu, 22 Jul 2021 03:40:04 GMT  
		Size: 10.8 MB (10781535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e6bee79099d0dac33ae4ae8ae713b806048f5a75b60da7eb38dd73f12afe5a3`  
		Last Modified: Thu, 22 Jul 2021 03:40:01 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.5-dev2` - linux; s390x

```console
$ docker pull haproxy@sha256:209e9fea2a0a2e89d75e9807ce2054c069b29411bddb4aadd6e3b0ef0a76eae4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.7 MB (35709317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5de350c41ba70768387f48e0bfc020047d1811390312bfde9bdfc7c876f92af`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 22 Jul 2021 00:42:45 GMT
ADD file:1ab999eb6f80d8ce91ce3a173e23fd2710f2779117bba29037eaa82aadcbf6ed in / 
# Thu, 22 Jul 2021 00:42:48 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:30:19 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 22 Jul 2021 01:30:19 GMT
ENV HAPROXY_VERSION=2.5-dev2
# Thu, 22 Jul 2021 01:30:20 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev2.tar.gz
# Thu, 22 Jul 2021 01:30:20 GMT
ENV HAPROXY_SHA256=34c2eee806f68bc892888c32477d9732e4610faf250d09aee6bea2d4f9fa5777
# Thu, 22 Jul 2021 01:30:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 22 Jul 2021 01:31:00 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 01:31:00 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 01:31:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 01:31:01 GMT
USER haproxy
# Thu, 22 Jul 2021 01:31:01 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:7a50fdd85ff244c1465e71c51354d055e3df0b90ff5faad28cc22d9ecde9daf3`  
		Last Modified: Thu, 22 Jul 2021 00:48:13 GMT  
		Size: 25.8 MB (25760761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05fb34d1ed21b67502665114a7ae60445472fc7bafa620bbf6c79b7df85a01d4`  
		Last Modified: Thu, 22 Jul 2021 01:39:54 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa91183bd1605686e9b95641fbb9536985642c023164d3ac759fe2212041ac28`  
		Last Modified: Thu, 22 Jul 2021 01:39:55 GMT  
		Size: 9.9 MB (9946726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92689905b44b2a82e92bd2442ba6ed05aca6bbed461837a4b9063c933c934d9f`  
		Last Modified: Thu, 22 Jul 2021 01:39:54 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.5-dev2-alpine`

```console
$ docker pull haproxy@sha256:60e0dd5228ebd2cf57dba638fa7f91f9062c4c00cd3cdb7c1791fcb07bdb123f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `haproxy:2.5-dev2-alpine` - linux; amd64

```console
$ docker pull haproxy@sha256:285c441480b9472edac38f7f3a8c9bc944d5ae741e5315880f9e786449b307a9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.2 MB (10247274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e44b5d3cc93e51de6ca73abbe4c9af56e6ae9271a5733c3b75e7cbd36ef9d7a8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 02:48:50 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 19 Jul 2021 20:20:58 GMT
ENV HAPROXY_VERSION=2.5-dev2
# Mon, 19 Jul 2021 20:20:58 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev2.tar.gz
# Mon, 19 Jul 2021 20:20:58 GMT
ENV HAPROXY_SHA256=34c2eee806f68bc892888c32477d9732e4610faf250d09aee6bea2d4f9fa5777
# Mon, 19 Jul 2021 20:21:59 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Mon, 19 Jul 2021 20:21:59 GMT
STOPSIGNAL SIGUSR1
# Mon, 19 Jul 2021 20:21:59 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 19 Jul 2021 20:21:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 19 Jul 2021 20:22:00 GMT
USER haproxy
# Mon, 19 Jul 2021 20:22:00 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7834d945b9e597e693f56fb0f9847718c1732b738a2f4956ab2c1b66c289d90`  
		Last Modified: Sat, 26 Jun 2021 02:56:43 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9748714368d19c518c7cea20a72f82aef224e9a83a35c47b9a30703ff07338e8`  
		Last Modified: Mon, 19 Jul 2021 20:23:26 GMT  
		Size: 7.4 MB (7434154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e3d039a8ccce39b26a30411867661c2ba7fafce288b2fc89b8cecbbf9fc2fc0`  
		Last Modified: Mon, 19 Jul 2021 20:23:25 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.5-dev2-alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:6e51da9ec54287f9f9386c3cac05f9414f0d5ee05e187019839df93d4bd70af6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (10016132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c09290cc5a02b7585e7f99af07b3aab045e09ea91f90547938dd41404673d8d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:26 GMT
ADD file:c80bc2b093cbc0fc466582ef21cbed377de9fa874aedbf320079525ddacd1200 in / 
# Tue, 15 Jun 2021 22:57:26 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 02:02:51 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 19 Jul 2021 20:51:14 GMT
ENV HAPROXY_VERSION=2.5-dev2
# Mon, 19 Jul 2021 20:51:14 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev2.tar.gz
# Mon, 19 Jul 2021 20:51:15 GMT
ENV HAPROXY_SHA256=34c2eee806f68bc892888c32477d9732e4610faf250d09aee6bea2d4f9fa5777
# Mon, 19 Jul 2021 20:51:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Mon, 19 Jul 2021 20:51:43 GMT
STOPSIGNAL SIGUSR1
# Mon, 19 Jul 2021 20:51:43 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 19 Jul 2021 20:51:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 19 Jul 2021 20:51:44 GMT
USER haproxy
# Mon, 19 Jul 2021 20:51:45 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:b4c9a0924271af3466de27804af26420eb58da1466e7eaaba127d178b380fea3`  
		Last Modified: Tue, 15 Jun 2021 22:58:47 GMT  
		Size: 2.6 MB (2624382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85fa2947d9cc2655af4fd4aa21641629e791bcaf309a7095db77d309ddd05dfa`  
		Last Modified: Sat, 26 Jun 2021 02:08:45 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:528eaf13fb9650e1aa29c9c7237489fef17436ffdbf3210810247d274b44828c`  
		Last Modified: Mon, 19 Jul 2021 20:54:02 GMT  
		Size: 7.4 MB (7390108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ddc7abd5e0eac09889562b8699def80aa605077352ba82f7536c86660aab96f`  
		Last Modified: Mon, 19 Jul 2021 20:53:56 GMT  
		Size: 447.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.5-dev2-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:d29ea3244794cb62bbc4da76c9bac7470708ad183c56b6f44bbd7cef3721c7b5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9748891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8eba494332ee1b97e98472b42473451c05c08b637207985c69357b0e7a9d0579`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:05 GMT
ADD file:416a8b507abdc6bdcb22997a4be0a4170796c3f9f77e315b2dbff2b0a212bc68 in / 
# Tue, 15 Jun 2021 23:15:06 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 05:27:42 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 19 Jul 2021 22:05:09 GMT
ENV HAPROXY_VERSION=2.5-dev2
# Mon, 19 Jul 2021 22:05:10 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev2.tar.gz
# Mon, 19 Jul 2021 22:05:10 GMT
ENV HAPROXY_SHA256=34c2eee806f68bc892888c32477d9732e4610faf250d09aee6bea2d4f9fa5777
# Mon, 19 Jul 2021 22:05:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Mon, 19 Jul 2021 22:05:38 GMT
STOPSIGNAL SIGUSR1
# Mon, 19 Jul 2021 22:05:38 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 19 Jul 2021 22:05:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 19 Jul 2021 22:05:39 GMT
USER haproxy
# Mon, 19 Jul 2021 22:05:40 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:136482bf81d1fa351b424ebb8c7e34d15f2c5ed3fc0b66b544b8312bda3d52d9`  
		Last Modified: Tue, 15 Jun 2021 23:16:40 GMT  
		Size: 2.4 MB (2427917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5464af225bd487370319e7125fb2769222c5c7371d1be737936169d2e5b01c`  
		Last Modified: Sat, 26 Jun 2021 05:35:56 GMT  
		Size: 1.2 KB (1196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fb6f783f6a974eec5cbb8fe40b15d5094d8b1706951bf89b672c96c1c24890c`  
		Last Modified: Mon, 19 Jul 2021 22:10:18 GMT  
		Size: 7.3 MB (7319329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5173583e05b8ea8863c18c69d9e5724d17659387960267599d9f148330e8767`  
		Last Modified: Mon, 19 Jul 2021 22:10:13 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.5-dev2-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:b103722ad8547adf72c6abf584808f5965dc9624f27f22bb153335f3e6a42e9a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.3 MB (10253414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfacf2b0908da0a4fb1ad07166604ac80689fff3b49d44f8c27595fd96a2dc0b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 21:44:56 GMT
ADD file:6797caacbfe41bfe44000b39ed017016c6fcc492b3d6557cdaba88536df6c876 in / 
# Tue, 15 Jun 2021 21:44:56 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 02:13:15 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 19 Jul 2021 20:40:49 GMT
ENV HAPROXY_VERSION=2.5-dev2
# Mon, 19 Jul 2021 20:40:49 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev2.tar.gz
# Mon, 19 Jul 2021 20:40:49 GMT
ENV HAPROXY_SHA256=34c2eee806f68bc892888c32477d9732e4610faf250d09aee6bea2d4f9fa5777
# Mon, 19 Jul 2021 20:41:49 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Mon, 19 Jul 2021 20:41:49 GMT
STOPSIGNAL SIGUSR1
# Mon, 19 Jul 2021 20:41:50 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 19 Jul 2021 20:41:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 19 Jul 2021 20:41:50 GMT
USER haproxy
# Mon, 19 Jul 2021 20:41:50 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:58ab47519297212468320b23b8100fc1b2b96e8d342040806ae509a778a0a07a`  
		Last Modified: Tue, 15 Jun 2021 21:46:03 GMT  
		Size: 2.7 MB (2709626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb8dc96e2a4b7f90ae2dbfca981fe199966b64e3426ca1f742499d46ad1aa357`  
		Last Modified: Sat, 26 Jun 2021 02:21:19 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:067b9aa25fba74d6c9e77ed1a9c3d3157ba07893b06e5f97cf0b91afe570585c`  
		Last Modified: Mon, 19 Jul 2021 20:44:17 GMT  
		Size: 7.5 MB (7542146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052aefb4611ad99c43a5abd99e6a593db80fed0ff3f12e5fe57f2f659ac76fca`  
		Last Modified: Mon, 19 Jul 2021 20:44:15 GMT  
		Size: 445.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.5-dev2-alpine` - linux; 386

```console
$ docker pull haproxy@sha256:6e2d016d57b800c954ac40a0ad7dab22a6f686a8ea4d2cd11c801a2df1f4aa6a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.1 MB (10103291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2dd830195af5cbec860580475781babb20937ac58423f82d963b5ef656201edb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 21:38:30 GMT
ADD file:3b0fe1454491bb05e218b090fd461f2fd39546aa4a53eb3f953ee8eae149ac57 in / 
# Tue, 15 Jun 2021 21:38:30 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 01:39:05 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 19 Jul 2021 20:39:39 GMT
ENV HAPROXY_VERSION=2.5-dev2
# Mon, 19 Jul 2021 20:39:39 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev2.tar.gz
# Mon, 19 Jul 2021 20:39:39 GMT
ENV HAPROXY_SHA256=34c2eee806f68bc892888c32477d9732e4610faf250d09aee6bea2d4f9fa5777
# Mon, 19 Jul 2021 20:40:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Mon, 19 Jul 2021 20:40:48 GMT
STOPSIGNAL SIGUSR1
# Mon, 19 Jul 2021 20:40:49 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 19 Jul 2021 20:40:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 19 Jul 2021 20:40:49 GMT
USER haproxy
# Mon, 19 Jul 2021 20:40:49 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:be21df321efb39c5daf3151073ebff7688e15ea6cd5158878bc9559a5db76ac6`  
		Last Modified: Tue, 15 Jun 2021 21:39:16 GMT  
		Size: 2.8 MB (2820718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc6fe536c8e50a97873c166db7d3b669842dec91d85ce73433028b3b198a1c4`  
		Last Modified: Sat, 26 Jun 2021 01:49:46 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:796ca18efd1209b0147e4fffea36abda4cd7b4773541f996ab699d77c61b86c0`  
		Last Modified: Mon, 19 Jul 2021 20:43:24 GMT  
		Size: 7.3 MB (7280930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e2759026673ac7b4c18d0e5e7aa4dd1e85392b04cdbc8bdc29af8ad9775753`  
		Last Modified: Mon, 19 Jul 2021 20:43:22 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.5-dev2-alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:c93e04b42d7ebf4111a9cbd90d38e8bef5438ad008714e231354ac5e06aefca8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.7 MB (10676989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ed0aa53dd5cbf72232a21725e8a69f46645c5dbd7eb06555d196a5698fd9458`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:27:00 GMT
ADD file:0075aad7a94f0496483442bb2d9fdaa13e9c23087b90638d014b4bc263aa3861 in / 
# Tue, 15 Jun 2021 22:27:03 GMT
CMD ["/bin/sh"]
# Fri, 16 Jul 2021 20:17:57 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 19 Jul 2021 20:22:41 GMT
ENV HAPROXY_VERSION=2.5-dev2
# Mon, 19 Jul 2021 20:22:48 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev2.tar.gz
# Mon, 19 Jul 2021 20:22:54 GMT
ENV HAPROXY_SHA256=34c2eee806f68bc892888c32477d9732e4610faf250d09aee6bea2d4f9fa5777
# Thu, 22 Jul 2021 02:58:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 22 Jul 2021 02:58:57 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 02:58:59 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 02:59:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 02:59:08 GMT
USER haproxy
# Thu, 22 Jul 2021 02:59:17 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:baf144cfb66ebe9df1969f3b90f1c448beff98edc84de1ccb5d6346195a070d4`  
		Last Modified: Tue, 15 Jun 2021 22:27:38 GMT  
		Size: 2.8 MB (2810478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e907663c9428bbbb731a221721c606bad29e54dac6f0dda85d6aa3175a725e`  
		Last Modified: Thu, 22 Jul 2021 03:40:16 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45e3511671e77d8086d4858c635cd3bc9d363b6933ccd46baf12a3b10fdedfa5`  
		Last Modified: Thu, 22 Jul 2021 03:40:17 GMT  
		Size: 7.9 MB (7864861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:796b651947f6e02a1e51f0a2b0bfbe212a8d3886fbed5e7ad77ccdc97bb117e0`  
		Last Modified: Thu, 22 Jul 2021 03:40:16 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:alpine`

```console
$ docker pull haproxy@sha256:278afc7563fcb5d498201d0093f9c700e659628677604bc15a82e3abba175799
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `haproxy:alpine` - linux; amd64

```console
$ docker pull haproxy@sha256:8819f159761cf992682ccb1267ab52e4b086a332e2baed24df18ff51bf49bd6a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.1 MB (10128308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7a37d8a7b2f124598b023e74621914426f81ab8b4f8e01d74cfbee1dd62ef0f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 02:48:50 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 18:34:10 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 08 Jul 2021 18:34:10 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 08 Jul 2021 18:34:10 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 08 Jul 2021 18:35:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 08 Jul 2021 18:35:12 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 18:35:12 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 18:35:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 18:35:13 GMT
USER haproxy
# Thu, 08 Jul 2021 18:35:13 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7834d945b9e597e693f56fb0f9847718c1732b738a2f4956ab2c1b66c289d90`  
		Last Modified: Sat, 26 Jun 2021 02:56:43 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddff1cb6bb6da9a692c61843d46abe17a215c726bb13d570212777a87398a3d9`  
		Last Modified: Thu, 08 Jul 2021 18:38:36 GMT  
		Size: 7.3 MB (7315186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee55c5b3ebb2b318c44f2635d4eea44eadfd079d55d0b8c5a6918b8aa9d5b1dc`  
		Last Modified: Thu, 08 Jul 2021 18:38:34 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:b79f0c78bc069755084556b3bd897a39780d24fe70b909b7c119d53f9a6bbc01
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9912733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05e37a7293c9eccbd033a7a1a38aa77387373ba82f719cbcc400dec92a69aad3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:26 GMT
ADD file:c80bc2b093cbc0fc466582ef21cbed377de9fa874aedbf320079525ddacd1200 in / 
# Tue, 15 Jun 2021 22:57:26 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 02:02:51 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 19:07:43 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 08 Jul 2021 19:07:44 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 08 Jul 2021 19:07:44 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 08 Jul 2021 19:08:13 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 08 Jul 2021 19:08:13 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 19:08:14 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 19:08:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 19:08:15 GMT
USER haproxy
# Thu, 08 Jul 2021 19:08:15 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:b4c9a0924271af3466de27804af26420eb58da1466e7eaaba127d178b380fea3`  
		Last Modified: Tue, 15 Jun 2021 22:58:47 GMT  
		Size: 2.6 MB (2624382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85fa2947d9cc2655af4fd4aa21641629e791bcaf309a7095db77d309ddd05dfa`  
		Last Modified: Sat, 26 Jun 2021 02:08:45 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a9ab1152df106ecaf9c67a2a14b91a15581a3b86248b43604172b704b71167`  
		Last Modified: Thu, 08 Jul 2021 19:11:00 GMT  
		Size: 7.3 MB (7286705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc34702136897eee4ca8c94845af335a66311b8b8a57a5f1c40292b913ef9f72`  
		Last Modified: Thu, 08 Jul 2021 19:10:56 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:b318934bc8973f8f73ad46a1c4f1c097899f57cdba1f6bff40285760584a684c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9631368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c900ed3b5e7e8ae25ede6582344b41bf064d26e831bdf4bfd385861422503a3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:05 GMT
ADD file:416a8b507abdc6bdcb22997a4be0a4170796c3f9f77e315b2dbff2b0a212bc68 in / 
# Tue, 15 Jun 2021 23:15:06 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 05:27:42 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 21:29:41 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 08 Jul 2021 21:29:42 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 08 Jul 2021 21:29:42 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 08 Jul 2021 21:30:19 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 08 Jul 2021 21:30:20 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 21:30:21 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 21:30:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 21:30:22 GMT
USER haproxy
# Thu, 08 Jul 2021 21:30:22 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:136482bf81d1fa351b424ebb8c7e34d15f2c5ed3fc0b66b544b8312bda3d52d9`  
		Last Modified: Tue, 15 Jun 2021 23:16:40 GMT  
		Size: 2.4 MB (2427917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5464af225bd487370319e7125fb2769222c5c7371d1be737936169d2e5b01c`  
		Last Modified: Sat, 26 Jun 2021 05:35:56 GMT  
		Size: 1.2 KB (1196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f903498f8e23244ca6430d647dd5515930d69394f19d017d07930d288ca6580`  
		Last Modified: Thu, 08 Jul 2021 21:36:22 GMT  
		Size: 7.2 MB (7201807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a0d8812e6df331ba2d781cc1fc08c2e4ddad2bb05b762b0eb737308a1205d5`  
		Last Modified: Thu, 08 Jul 2021 21:36:18 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:c17729aebb94fdae2758381c550a8866ce8856237ce1892a6fba9d0cdadd7c5b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.1 MB (10133906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b500e8260787f1a0bcdc19f790686cd272d751cdd28f848f01eb2f054c700341`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 21:44:56 GMT
ADD file:6797caacbfe41bfe44000b39ed017016c6fcc492b3d6557cdaba88536df6c876 in / 
# Tue, 15 Jun 2021 21:44:56 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 02:13:15 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 19:02:27 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 08 Jul 2021 19:02:27 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 08 Jul 2021 19:02:27 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 08 Jul 2021 19:03:26 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 08 Jul 2021 19:03:26 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 19:03:27 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 19:03:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 19:03:27 GMT
USER haproxy
# Thu, 08 Jul 2021 19:03:27 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:58ab47519297212468320b23b8100fc1b2b96e8d342040806ae509a778a0a07a`  
		Last Modified: Tue, 15 Jun 2021 21:46:03 GMT  
		Size: 2.7 MB (2709626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb8dc96e2a4b7f90ae2dbfca981fe199966b64e3426ca1f742499d46ad1aa357`  
		Last Modified: Sat, 26 Jun 2021 02:21:19 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b367d065849fc1a609fb169119e94047ed3a2b475932bb292bff5b6cc45a1f`  
		Last Modified: Thu, 08 Jul 2021 19:07:30 GMT  
		Size: 7.4 MB (7422635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60cf6675a5a8e39f65c07f8553ab269ab83f947cbfa20da77e6da66ca033969e`  
		Last Modified: Thu, 08 Jul 2021 19:07:28 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:alpine` - linux; 386

```console
$ docker pull haproxy@sha256:01a8472d10c0512c1950dad3ae7472f99767eeaa8f0bbbb3aa53813d35961ab0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (9998434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e50005241013c0fb9d14f539c88cbf5dd3ebfec6c0498014c4a70a002cbe3d48`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 21:38:30 GMT
ADD file:3b0fe1454491bb05e218b090fd461f2fd39546aa4a53eb3f953ee8eae149ac57 in / 
# Tue, 15 Jun 2021 21:38:30 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 01:39:05 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 19:03:09 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 08 Jul 2021 19:03:09 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 08 Jul 2021 19:03:09 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 08 Jul 2021 19:04:25 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 08 Jul 2021 19:04:25 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 19:04:25 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 19:04:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 19:04:26 GMT
USER haproxy
# Thu, 08 Jul 2021 19:04:26 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:be21df321efb39c5daf3151073ebff7688e15ea6cd5158878bc9559a5db76ac6`  
		Last Modified: Tue, 15 Jun 2021 21:39:16 GMT  
		Size: 2.8 MB (2820718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc6fe536c8e50a97873c166db7d3b669842dec91d85ce73433028b3b198a1c4`  
		Last Modified: Sat, 26 Jun 2021 01:49:46 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:832c00757ee7003ebca753eff8d4c6af86ebcf09efecec8e1171e550c8fc816f`  
		Last Modified: Thu, 08 Jul 2021 19:08:59 GMT  
		Size: 7.2 MB (7176071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85e6578d15134f65f8b977b9e7c9322e6281b3c765978ce760142c0bac7197ad`  
		Last Modified: Thu, 08 Jul 2021 19:08:57 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:8371490329ce959d92d6d6bca900a6702869e800fbd8c4a80438da13efa8b696
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.6 MB (10556641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5510c2e0b44e02d587dd27e62dd07ef69cc51b3e43f00927403e3c29eb34cfc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:27:00 GMT
ADD file:0075aad7a94f0496483442bb2d9fdaa13e9c23087b90638d014b4bc263aa3861 in / 
# Tue, 15 Jun 2021 22:27:03 GMT
CMD ["/bin/sh"]
# Fri, 16 Jul 2021 20:17:57 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 16 Jul 2021 20:19:42 GMT
ENV HAPROXY_VERSION=2.4.2
# Fri, 16 Jul 2021 20:19:48 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Fri, 16 Jul 2021 20:19:51 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 22 Jul 2021 03:04:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 22 Jul 2021 03:04:47 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 03:04:50 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 03:04:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 03:04:59 GMT
USER haproxy
# Thu, 22 Jul 2021 03:05:04 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:baf144cfb66ebe9df1969f3b90f1c448beff98edc84de1ccb5d6346195a070d4`  
		Last Modified: Tue, 15 Jun 2021 22:27:38 GMT  
		Size: 2.8 MB (2810478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e907663c9428bbbb731a221721c606bad29e54dac6f0dda85d6aa3175a725e`  
		Last Modified: Thu, 22 Jul 2021 03:40:16 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25fed8e719bd522b435fea4d6999c2ecffeb38e8288458cea40c3ecfa9131656`  
		Last Modified: Thu, 22 Jul 2021 03:40:53 GMT  
		Size: 7.7 MB (7744514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c45ecd590d1194b07f22c1e98348800abd5fdc2592d5c85e8fd5413acc1f29`  
		Last Modified: Thu, 22 Jul 2021 03:40:50 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:alpine` - linux; s390x

```console
$ docker pull haproxy@sha256:67c77b2f75cda356f4462fa8c7cfe05d80b220bb7e3ddff6782557ca308381e0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9899025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8353b377710bdcc56a8dd1fcdf4213b83d4378a795634015c8ec0817188591f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:54:24 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:45:22 GMT
ENV HAPROXY_VERSION=2.4.0
# Fri, 14 May 2021 19:45:23 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Fri, 14 May 2021 19:45:23 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Fri, 14 May 2021 19:46:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 14 May 2021 19:46:14 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:46:14 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:46:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:46:15 GMT
USER haproxy
# Fri, 14 May 2021 19:46:15 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267275aba58470c82626189a59be76cd169bd245568e2f2545ed1ee64ff8a8ff`  
		Last Modified: Wed, 14 Apr 2021 20:59:06 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1af9bde57dd624c224ba02793a7568cd9f00874c978ff5ab4d6bc0c32fdb81f`  
		Last Modified: Fri, 14 May 2021 19:48:00 GMT  
		Size: 7.3 MB (7294741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68dd09d54ba9406459ae1956173c0df96676de52e5a01f9392966e3493acae68`  
		Last Modified: Fri, 14 May 2021 19:47:59 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:latest`

```console
$ docker pull haproxy@sha256:0b604e2d9b0366e304d89393dd42651698bbbc2d588b65155b6aabaf4995ba00
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

### `haproxy:latest` - linux; amd64

```console
$ docker pull haproxy@sha256:52aa1ec7d5d0b74f20d4e5c03c8f7561ead3db8931e0b733d6007b397a2d3880
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37295916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d784089a656dab7a82fd06ce515c7a5f2865055cc3d9422c8795a07300428f07`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 06:19:17 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 18:33:10 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 08 Jul 2021 18:33:10 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 08 Jul 2021 18:33:10 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 08 Jul 2021 18:34:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 08 Jul 2021 18:34:02 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 18:34:02 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 18:34:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 18:34:03 GMT
USER haproxy
# Thu, 08 Jul 2021 18:34:03 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91332cb81883405a321c1a2d2144bdd0aef8d1c69f90fdf0cf219982161b6e6e`  
		Last Modified: Wed, 23 Jun 2021 06:29:07 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6373e07bfb885e35a6bd53edfdc9040601b27fc0961fe6129588015b2096db20`  
		Last Modified: Thu, 08 Jul 2021 18:38:19 GMT  
		Size: 10.1 MB (10148233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a5b51f2be69ce74243979e96aaae4a74e55466e342bcd0bb697a2b1e62d59b`  
		Last Modified: Thu, 08 Jul 2021 18:38:18 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:latest` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:2f24bc20c43df5eb2b7e5ffc0e95674782b29896f65a1226bc2adff0b3d68e0a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34665575 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed1196ca984d9efa3ec3c4f779f012f0662a9586517f0c0e041612416ff4fbc8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 22 Jun 2021 23:50:09 GMT
ADD file:78d4ced31112d85490c684f350aceeebfc72a804262c7ad3e033257e3894f5c4 in / 
# Tue, 22 Jun 2021 23:50:11 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:15:11 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 18:58:15 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 08 Jul 2021 18:58:16 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 08 Jul 2021 18:58:16 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 08 Jul 2021 18:59:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 08 Jul 2021 18:59:09 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 18:59:10 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 18:59:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 18:59:10 GMT
USER haproxy
# Thu, 08 Jul 2021 18:59:11 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:532d6df30af5174ac6e1b379c32b8f464d44651ac060376a560c4a76a87704a7`  
		Last Modified: Wed, 23 Jun 2021 00:01:46 GMT  
		Size: 24.9 MB (24878945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48649e3d7de4cd80d3a9a34c725a2935be904ff90e99ea6c8e4bb6e1e7a4eeb7`  
		Last Modified: Wed, 23 Jun 2021 05:24:11 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ee3e06cb1904b6bc00db8565860713531b542e6ef7389f534e96705484113d`  
		Last Modified: Thu, 08 Jul 2021 19:02:21 GMT  
		Size: 9.8 MB (9784805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b6869880a0636c536ab6434a503f73fbe4faa5d871d3ae25f498d9995adc0f3`  
		Last Modified: Thu, 08 Jul 2021 19:02:15 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:latest` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:7b6339c2dff4e7a1d7bbb7c72bc74cf2072bf95ff20841bd1c3392db483209b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.4 MB (32372088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9405b9497ca1234f5dd526dab824511329f7053f2f2b6766f2a64e2c9734d7bb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:31 GMT
ADD file:8d200a3bbe985ff355343675c5555852f27550a9e367969df6bc98034efb8fd4 in / 
# Wed, 23 Jun 2021 00:20:31 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:21:41 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 21:28:35 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 08 Jul 2021 21:28:36 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 08 Jul 2021 21:28:37 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 08 Jul 2021 21:29:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 08 Jul 2021 21:29:24 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 21:29:25 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 21:29:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 21:29:26 GMT
USER haproxy
# Thu, 08 Jul 2021 21:29:26 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:8452be1adf00f91570fe21a8e61aaf4c12e014daf67d7de65d984f4e8ecca2f1`  
		Last Modified: Wed, 23 Jun 2021 00:31:49 GMT  
		Size: 22.7 MB (22746055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed1c9c92d0076fd4bf40503e3f47102509a5b99d182f4dd9e81e64d0a7e0b8a`  
		Last Modified: Wed, 23 Jun 2021 05:35:48 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b090e05bfe544bc62f527dcf70dd8799d4180499bcedf6d5a8ffa14c7a75b31d`  
		Last Modified: Thu, 08 Jul 2021 21:35:57 GMT  
		Size: 9.6 MB (9624206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9cdb9eefea684230e2e659f2753469d8df08683a747d1a8d95dc6da0954cb60`  
		Last Modified: Thu, 08 Jul 2021 21:35:52 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:latest` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:ecddae360d89e478a3ca8575fe6902f41f5bce6d136ffa9d002979696533aed9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35942280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b004550c7f1e6363193435537a32221dc4e6ce0bb68cea61b3c97378b6362064`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:40 GMT
ADD file:beee00b59da720f68e12e2ba2a8134207c80c777ddb4ceb03c71e3e4c3f51c93 in / 
# Tue, 22 Jun 2021 23:49:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 03:19:31 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 19:01:35 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 08 Jul 2021 19:01:35 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 08 Jul 2021 19:01:35 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 08 Jul 2021 19:02:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 08 Jul 2021 19:02:18 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 19:02:18 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 19:02:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 19:02:18 GMT
USER haproxy
# Thu, 08 Jul 2021 19:02:18 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:448f6bf000e31217a7c202c659b03b7f8ac8d3ae6b03ef7a2f8339be2f00ff4a`  
		Last Modified: Tue, 22 Jun 2021 23:55:25 GMT  
		Size: 25.9 MB (25914993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b05ad81dc8a7d67656235988f0e5fb72c374c7d8df44c105b91d712e06c4ac`  
		Last Modified: Wed, 23 Jun 2021 03:26:16 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076876a81ee03b4e5250b7a31318f330ccf4ea3eeef84cecafdc1a92b4803062`  
		Last Modified: Thu, 08 Jul 2021 19:07:11 GMT  
		Size: 10.0 MB (10025457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:277cf44e1cd25ac34ef95ef8bc0084be15c5d80b5fd94d6b8ba385807423dce0`  
		Last Modified: Thu, 08 Jul 2021 19:07:08 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:latest` - linux; 386

```console
$ docker pull haproxy@sha256:ef1c5085a09fe3d0028e256643a9453a2b853f34cf360c895fdc418095a9525a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.8 MB (37792502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87c94a82fd63b1e3cbd90c3cca2b24076d38dcdfd88fc0b5f9367719bd84cbdd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 22 Jun 2021 23:39:35 GMT
ADD file:48f656ac6733911048b3de850490438d0233b3badc11861fca62062d4edfaf40 in / 
# Tue, 22 Jun 2021 23:39:35 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:23:13 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 19:01:56 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 08 Jul 2021 19:01:56 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 08 Jul 2021 19:01:56 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 08 Jul 2021 19:02:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 08 Jul 2021 19:02:57 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 19:02:57 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 19:02:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 19:02:58 GMT
USER haproxy
# Thu, 08 Jul 2021 19:02:58 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:33af2dcb865e65d53cdeb843b67a0ef62151fa32df292293e7c6b0eb728ac5ac`  
		Last Modified: Tue, 22 Jun 2021 23:46:23 GMT  
		Size: 27.8 MB (27797411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a6e4d42b23996eb7d8a1baa85ee19828c2667fd4a2dca6eb1040b266680e9f`  
		Last Modified: Wed, 23 Jun 2021 00:32:00 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c640aece6fea8db01bc9744204c373af3285d4d3b15911631fdc1508b30fe28f`  
		Last Modified: Thu, 08 Jul 2021 19:08:39 GMT  
		Size: 10.0 MB (9993262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e1e627dabfcf736ac7f517f394391e6eeb0fa52347a5f92cee7310d00c35fac`  
		Last Modified: Thu, 08 Jul 2021 19:08:38 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:latest` - linux; mips64le

```console
$ docker pull haproxy@sha256:0831d16085b3616dd56baae5d2b16911f5df76ff3643f6ed0cc9206bcdd1b0ef
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.6 MB (35582649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a67c72bc16cd3442d99818a1691f620bb8fba803aa322938bf1f76185d160ae9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 22 Jul 2021 00:09:45 GMT
ADD file:1f77b9001c4977ba733be674fc5eb4b85130f1dea8a7b39d545b70f9c107695f in / 
# Thu, 22 Jul 2021 00:09:46 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:07:49 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 22 Jul 2021 01:10:29 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 22 Jul 2021 01:10:29 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 22 Jul 2021 01:10:30 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 22 Jul 2021 01:12:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 22 Jul 2021 01:12:58 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 01:12:58 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 01:12:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 01:12:59 GMT
USER haproxy
# Thu, 22 Jul 2021 01:12:59 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:99ee621d0b0485e9de65aa19604aa2453d19ea7fc86b22c5b77c1bab74e3cb42`  
		Last Modified: Thu, 22 Jul 2021 00:16:11 GMT  
		Size: 25.8 MB (25812771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f444627794f98947a9df95ec5d19b2a1cd6c151ed438982b1dc0b89f5eaf19e`  
		Last Modified: Thu, 22 Jul 2021 01:24:39 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529ec01a3a5cb58c3aa92432192c7025a9df5ac852a7e1606269d172da56dd54`  
		Last Modified: Thu, 22 Jul 2021 01:25:03 GMT  
		Size: 9.8 MB (9768048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0dc46dbff91be84b369de7651cd4d1d725a03b3d65bfef0a41478894b38fe2`  
		Last Modified: Thu, 22 Jul 2021 01:24:56 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:latest` - linux; ppc64le

```console
$ docker pull haproxy@sha256:0265c0700be024578a661ef439408b91cfa73fef6b763a58ddad4d78fdbc51db
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.2 MB (41213069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae16a408d428d4d0a7ed8262d6b984676689a578932f9ff1a168c726b85fb6e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 22 Jul 2021 00:19:04 GMT
ADD file:3a6bd6ce3eff98b88a13de5d0f26cff0b026f876674204dbad6f84fafcf145b1 in / 
# Thu, 22 Jul 2021 00:19:13 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 02:52:46 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 22 Jul 2021 02:59:40 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 22 Jul 2021 02:59:52 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 22 Jul 2021 03:00:03 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 22 Jul 2021 03:03:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 22 Jul 2021 03:03:39 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 03:03:41 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 03:03:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 03:03:48 GMT
USER haproxy
# Thu, 22 Jul 2021 03:03:52 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:1130517d52da84a09f9465006bddab5e49afd398860890eab6274fd0bff32371`  
		Last Modified: Thu, 22 Jul 2021 00:27:49 GMT  
		Size: 30.6 MB (30553709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251bf3fe1d4bbe9c27e393cd8ddc550b56cec90eb916bf9bec24d657c9f6556f`  
		Last Modified: Thu, 22 Jul 2021 03:40:01 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f4b7133364510c1fc0f847a528a441235df0500c39d8318c3557708a9ea74fa`  
		Last Modified: Thu, 22 Jul 2021 03:40:33 GMT  
		Size: 10.7 MB (10657533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1244f9b6844b16203e11b9ed8754bed5a0289f1a3b6bd59d295e18b9fca91bc`  
		Last Modified: Thu, 22 Jul 2021 03:40:30 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:latest` - linux; s390x

```console
$ docker pull haproxy@sha256:2f711e846e54ca0e3063a51b841c4291dc0a07925552f9feab60e56ceeb54a8b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.6 MB (35587765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:123ac19f2aeb23d953a63211cc6c840f267890f19ee5a8db61abaed33280a5b5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 22 Jul 2021 00:42:45 GMT
ADD file:1ab999eb6f80d8ce91ce3a173e23fd2710f2779117bba29037eaa82aadcbf6ed in / 
# Thu, 22 Jul 2021 00:42:48 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:30:19 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 22 Jul 2021 01:31:40 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 22 Jul 2021 01:31:40 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 22 Jul 2021 01:31:40 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 22 Jul 2021 01:32:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 22 Jul 2021 01:32:21 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 01:32:21 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 01:32:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 01:32:22 GMT
USER haproxy
# Thu, 22 Jul 2021 01:32:22 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:7a50fdd85ff244c1465e71c51354d055e3df0b90ff5faad28cc22d9ecde9daf3`  
		Last Modified: Thu, 22 Jul 2021 00:48:13 GMT  
		Size: 25.8 MB (25760761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05fb34d1ed21b67502665114a7ae60445472fc7bafa620bbf6c79b7df85a01d4`  
		Last Modified: Thu, 22 Jul 2021 01:39:54 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509cd29cce72fe3b56df141c72bd9ac7c85aafc2da6d1596ec7e29ef8e10db0f`  
		Last Modified: Thu, 22 Jul 2021 01:40:05 GMT  
		Size: 9.8 MB (9825173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b04c9d12d457a528c260ddcaaecc8d44f66fb72fb0a54770d3011ba16f8433`  
		Last Modified: Thu, 22 Jul 2021 01:40:04 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:lts`

```console
$ docker pull haproxy@sha256:0b604e2d9b0366e304d89393dd42651698bbbc2d588b65155b6aabaf4995ba00
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

### `haproxy:lts` - linux; amd64

```console
$ docker pull haproxy@sha256:52aa1ec7d5d0b74f20d4e5c03c8f7561ead3db8931e0b733d6007b397a2d3880
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37295916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d784089a656dab7a82fd06ce515c7a5f2865055cc3d9422c8795a07300428f07`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 06:19:17 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 18:33:10 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 08 Jul 2021 18:33:10 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 08 Jul 2021 18:33:10 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 08 Jul 2021 18:34:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 08 Jul 2021 18:34:02 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 18:34:02 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 18:34:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 18:34:03 GMT
USER haproxy
# Thu, 08 Jul 2021 18:34:03 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91332cb81883405a321c1a2d2144bdd0aef8d1c69f90fdf0cf219982161b6e6e`  
		Last Modified: Wed, 23 Jun 2021 06:29:07 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6373e07bfb885e35a6bd53edfdc9040601b27fc0961fe6129588015b2096db20`  
		Last Modified: Thu, 08 Jul 2021 18:38:19 GMT  
		Size: 10.1 MB (10148233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a5b51f2be69ce74243979e96aaae4a74e55466e342bcd0bb697a2b1e62d59b`  
		Last Modified: Thu, 08 Jul 2021 18:38:18 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:2f24bc20c43df5eb2b7e5ffc0e95674782b29896f65a1226bc2adff0b3d68e0a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34665575 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed1196ca984d9efa3ec3c4f779f012f0662a9586517f0c0e041612416ff4fbc8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 22 Jun 2021 23:50:09 GMT
ADD file:78d4ced31112d85490c684f350aceeebfc72a804262c7ad3e033257e3894f5c4 in / 
# Tue, 22 Jun 2021 23:50:11 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:15:11 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 18:58:15 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 08 Jul 2021 18:58:16 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 08 Jul 2021 18:58:16 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 08 Jul 2021 18:59:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 08 Jul 2021 18:59:09 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 18:59:10 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 18:59:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 18:59:10 GMT
USER haproxy
# Thu, 08 Jul 2021 18:59:11 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:532d6df30af5174ac6e1b379c32b8f464d44651ac060376a560c4a76a87704a7`  
		Last Modified: Wed, 23 Jun 2021 00:01:46 GMT  
		Size: 24.9 MB (24878945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48649e3d7de4cd80d3a9a34c725a2935be904ff90e99ea6c8e4bb6e1e7a4eeb7`  
		Last Modified: Wed, 23 Jun 2021 05:24:11 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ee3e06cb1904b6bc00db8565860713531b542e6ef7389f534e96705484113d`  
		Last Modified: Thu, 08 Jul 2021 19:02:21 GMT  
		Size: 9.8 MB (9784805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b6869880a0636c536ab6434a503f73fbe4faa5d871d3ae25f498d9995adc0f3`  
		Last Modified: Thu, 08 Jul 2021 19:02:15 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:7b6339c2dff4e7a1d7bbb7c72bc74cf2072bf95ff20841bd1c3392db483209b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.4 MB (32372088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9405b9497ca1234f5dd526dab824511329f7053f2f2b6766f2a64e2c9734d7bb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:31 GMT
ADD file:8d200a3bbe985ff355343675c5555852f27550a9e367969df6bc98034efb8fd4 in / 
# Wed, 23 Jun 2021 00:20:31 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:21:41 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 21:28:35 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 08 Jul 2021 21:28:36 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 08 Jul 2021 21:28:37 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 08 Jul 2021 21:29:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 08 Jul 2021 21:29:24 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 21:29:25 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 21:29:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 21:29:26 GMT
USER haproxy
# Thu, 08 Jul 2021 21:29:26 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:8452be1adf00f91570fe21a8e61aaf4c12e014daf67d7de65d984f4e8ecca2f1`  
		Last Modified: Wed, 23 Jun 2021 00:31:49 GMT  
		Size: 22.7 MB (22746055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed1c9c92d0076fd4bf40503e3f47102509a5b99d182f4dd9e81e64d0a7e0b8a`  
		Last Modified: Wed, 23 Jun 2021 05:35:48 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b090e05bfe544bc62f527dcf70dd8799d4180499bcedf6d5a8ffa14c7a75b31d`  
		Last Modified: Thu, 08 Jul 2021 21:35:57 GMT  
		Size: 9.6 MB (9624206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9cdb9eefea684230e2e659f2753469d8df08683a747d1a8d95dc6da0954cb60`  
		Last Modified: Thu, 08 Jul 2021 21:35:52 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:ecddae360d89e478a3ca8575fe6902f41f5bce6d136ffa9d002979696533aed9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35942280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b004550c7f1e6363193435537a32221dc4e6ce0bb68cea61b3c97378b6362064`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:40 GMT
ADD file:beee00b59da720f68e12e2ba2a8134207c80c777ddb4ceb03c71e3e4c3f51c93 in / 
# Tue, 22 Jun 2021 23:49:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 03:19:31 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 19:01:35 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 08 Jul 2021 19:01:35 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 08 Jul 2021 19:01:35 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 08 Jul 2021 19:02:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 08 Jul 2021 19:02:18 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 19:02:18 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 19:02:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 19:02:18 GMT
USER haproxy
# Thu, 08 Jul 2021 19:02:18 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:448f6bf000e31217a7c202c659b03b7f8ac8d3ae6b03ef7a2f8339be2f00ff4a`  
		Last Modified: Tue, 22 Jun 2021 23:55:25 GMT  
		Size: 25.9 MB (25914993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b05ad81dc8a7d67656235988f0e5fb72c374c7d8df44c105b91d712e06c4ac`  
		Last Modified: Wed, 23 Jun 2021 03:26:16 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076876a81ee03b4e5250b7a31318f330ccf4ea3eeef84cecafdc1a92b4803062`  
		Last Modified: Thu, 08 Jul 2021 19:07:11 GMT  
		Size: 10.0 MB (10025457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:277cf44e1cd25ac34ef95ef8bc0084be15c5d80b5fd94d6b8ba385807423dce0`  
		Last Modified: Thu, 08 Jul 2021 19:07:08 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; 386

```console
$ docker pull haproxy@sha256:ef1c5085a09fe3d0028e256643a9453a2b853f34cf360c895fdc418095a9525a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.8 MB (37792502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87c94a82fd63b1e3cbd90c3cca2b24076d38dcdfd88fc0b5f9367719bd84cbdd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 22 Jun 2021 23:39:35 GMT
ADD file:48f656ac6733911048b3de850490438d0233b3badc11861fca62062d4edfaf40 in / 
# Tue, 22 Jun 2021 23:39:35 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:23:13 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 19:01:56 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 08 Jul 2021 19:01:56 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 08 Jul 2021 19:01:56 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 08 Jul 2021 19:02:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 08 Jul 2021 19:02:57 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 19:02:57 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 19:02:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 19:02:58 GMT
USER haproxy
# Thu, 08 Jul 2021 19:02:58 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:33af2dcb865e65d53cdeb843b67a0ef62151fa32df292293e7c6b0eb728ac5ac`  
		Last Modified: Tue, 22 Jun 2021 23:46:23 GMT  
		Size: 27.8 MB (27797411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a6e4d42b23996eb7d8a1baa85ee19828c2667fd4a2dca6eb1040b266680e9f`  
		Last Modified: Wed, 23 Jun 2021 00:32:00 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c640aece6fea8db01bc9744204c373af3285d4d3b15911631fdc1508b30fe28f`  
		Last Modified: Thu, 08 Jul 2021 19:08:39 GMT  
		Size: 10.0 MB (9993262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e1e627dabfcf736ac7f517f394391e6eeb0fa52347a5f92cee7310d00c35fac`  
		Last Modified: Thu, 08 Jul 2021 19:08:38 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; mips64le

```console
$ docker pull haproxy@sha256:0831d16085b3616dd56baae5d2b16911f5df76ff3643f6ed0cc9206bcdd1b0ef
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.6 MB (35582649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a67c72bc16cd3442d99818a1691f620bb8fba803aa322938bf1f76185d160ae9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 22 Jul 2021 00:09:45 GMT
ADD file:1f77b9001c4977ba733be674fc5eb4b85130f1dea8a7b39d545b70f9c107695f in / 
# Thu, 22 Jul 2021 00:09:46 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:07:49 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 22 Jul 2021 01:10:29 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 22 Jul 2021 01:10:29 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 22 Jul 2021 01:10:30 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 22 Jul 2021 01:12:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 22 Jul 2021 01:12:58 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 01:12:58 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 01:12:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 01:12:59 GMT
USER haproxy
# Thu, 22 Jul 2021 01:12:59 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:99ee621d0b0485e9de65aa19604aa2453d19ea7fc86b22c5b77c1bab74e3cb42`  
		Last Modified: Thu, 22 Jul 2021 00:16:11 GMT  
		Size: 25.8 MB (25812771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f444627794f98947a9df95ec5d19b2a1cd6c151ed438982b1dc0b89f5eaf19e`  
		Last Modified: Thu, 22 Jul 2021 01:24:39 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529ec01a3a5cb58c3aa92432192c7025a9df5ac852a7e1606269d172da56dd54`  
		Last Modified: Thu, 22 Jul 2021 01:25:03 GMT  
		Size: 9.8 MB (9768048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0dc46dbff91be84b369de7651cd4d1d725a03b3d65bfef0a41478894b38fe2`  
		Last Modified: Thu, 22 Jul 2021 01:24:56 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; ppc64le

```console
$ docker pull haproxy@sha256:0265c0700be024578a661ef439408b91cfa73fef6b763a58ddad4d78fdbc51db
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.2 MB (41213069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae16a408d428d4d0a7ed8262d6b984676689a578932f9ff1a168c726b85fb6e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 22 Jul 2021 00:19:04 GMT
ADD file:3a6bd6ce3eff98b88a13de5d0f26cff0b026f876674204dbad6f84fafcf145b1 in / 
# Thu, 22 Jul 2021 00:19:13 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 02:52:46 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 22 Jul 2021 02:59:40 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 22 Jul 2021 02:59:52 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 22 Jul 2021 03:00:03 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 22 Jul 2021 03:03:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 22 Jul 2021 03:03:39 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 03:03:41 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 03:03:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 03:03:48 GMT
USER haproxy
# Thu, 22 Jul 2021 03:03:52 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:1130517d52da84a09f9465006bddab5e49afd398860890eab6274fd0bff32371`  
		Last Modified: Thu, 22 Jul 2021 00:27:49 GMT  
		Size: 30.6 MB (30553709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251bf3fe1d4bbe9c27e393cd8ddc550b56cec90eb916bf9bec24d657c9f6556f`  
		Last Modified: Thu, 22 Jul 2021 03:40:01 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f4b7133364510c1fc0f847a528a441235df0500c39d8318c3557708a9ea74fa`  
		Last Modified: Thu, 22 Jul 2021 03:40:33 GMT  
		Size: 10.7 MB (10657533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1244f9b6844b16203e11b9ed8754bed5a0289f1a3b6bd59d295e18b9fca91bc`  
		Last Modified: Thu, 22 Jul 2021 03:40:30 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; s390x

```console
$ docker pull haproxy@sha256:2f711e846e54ca0e3063a51b841c4291dc0a07925552f9feab60e56ceeb54a8b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.6 MB (35587765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:123ac19f2aeb23d953a63211cc6c840f267890f19ee5a8db61abaed33280a5b5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 22 Jul 2021 00:42:45 GMT
ADD file:1ab999eb6f80d8ce91ce3a173e23fd2710f2779117bba29037eaa82aadcbf6ed in / 
# Thu, 22 Jul 2021 00:42:48 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:30:19 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 22 Jul 2021 01:31:40 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 22 Jul 2021 01:31:40 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 22 Jul 2021 01:31:40 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 22 Jul 2021 01:32:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 22 Jul 2021 01:32:21 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 01:32:21 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 01:32:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 01:32:22 GMT
USER haproxy
# Thu, 22 Jul 2021 01:32:22 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:7a50fdd85ff244c1465e71c51354d055e3df0b90ff5faad28cc22d9ecde9daf3`  
		Last Modified: Thu, 22 Jul 2021 00:48:13 GMT  
		Size: 25.8 MB (25760761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05fb34d1ed21b67502665114a7ae60445472fc7bafa620bbf6c79b7df85a01d4`  
		Last Modified: Thu, 22 Jul 2021 01:39:54 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509cd29cce72fe3b56df141c72bd9ac7c85aafc2da6d1596ec7e29ef8e10db0f`  
		Last Modified: Thu, 22 Jul 2021 01:40:05 GMT  
		Size: 9.8 MB (9825173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b04c9d12d457a528c260ddcaaecc8d44f66fb72fb0a54770d3011ba16f8433`  
		Last Modified: Thu, 22 Jul 2021 01:40:04 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:lts-alpine`

```console
$ docker pull haproxy@sha256:278afc7563fcb5d498201d0093f9c700e659628677604bc15a82e3abba175799
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `haproxy:lts-alpine` - linux; amd64

```console
$ docker pull haproxy@sha256:8819f159761cf992682ccb1267ab52e4b086a332e2baed24df18ff51bf49bd6a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.1 MB (10128308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7a37d8a7b2f124598b023e74621914426f81ab8b4f8e01d74cfbee1dd62ef0f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 02:48:50 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 18:34:10 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 08 Jul 2021 18:34:10 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 08 Jul 2021 18:34:10 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 08 Jul 2021 18:35:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 08 Jul 2021 18:35:12 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 18:35:12 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 18:35:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 18:35:13 GMT
USER haproxy
# Thu, 08 Jul 2021 18:35:13 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7834d945b9e597e693f56fb0f9847718c1732b738a2f4956ab2c1b66c289d90`  
		Last Modified: Sat, 26 Jun 2021 02:56:43 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddff1cb6bb6da9a692c61843d46abe17a215c726bb13d570212777a87398a3d9`  
		Last Modified: Thu, 08 Jul 2021 18:38:36 GMT  
		Size: 7.3 MB (7315186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee55c5b3ebb2b318c44f2635d4eea44eadfd079d55d0b8c5a6918b8aa9d5b1dc`  
		Last Modified: Thu, 08 Jul 2021 18:38:34 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts-alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:b79f0c78bc069755084556b3bd897a39780d24fe70b909b7c119d53f9a6bbc01
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9912733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05e37a7293c9eccbd033a7a1a38aa77387373ba82f719cbcc400dec92a69aad3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:26 GMT
ADD file:c80bc2b093cbc0fc466582ef21cbed377de9fa874aedbf320079525ddacd1200 in / 
# Tue, 15 Jun 2021 22:57:26 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 02:02:51 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 19:07:43 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 08 Jul 2021 19:07:44 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 08 Jul 2021 19:07:44 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 08 Jul 2021 19:08:13 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 08 Jul 2021 19:08:13 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 19:08:14 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 19:08:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 19:08:15 GMT
USER haproxy
# Thu, 08 Jul 2021 19:08:15 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:b4c9a0924271af3466de27804af26420eb58da1466e7eaaba127d178b380fea3`  
		Last Modified: Tue, 15 Jun 2021 22:58:47 GMT  
		Size: 2.6 MB (2624382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85fa2947d9cc2655af4fd4aa21641629e791bcaf309a7095db77d309ddd05dfa`  
		Last Modified: Sat, 26 Jun 2021 02:08:45 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a9ab1152df106ecaf9c67a2a14b91a15581a3b86248b43604172b704b71167`  
		Last Modified: Thu, 08 Jul 2021 19:11:00 GMT  
		Size: 7.3 MB (7286705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc34702136897eee4ca8c94845af335a66311b8b8a57a5f1c40292b913ef9f72`  
		Last Modified: Thu, 08 Jul 2021 19:10:56 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:b318934bc8973f8f73ad46a1c4f1c097899f57cdba1f6bff40285760584a684c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9631368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c900ed3b5e7e8ae25ede6582344b41bf064d26e831bdf4bfd385861422503a3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:05 GMT
ADD file:416a8b507abdc6bdcb22997a4be0a4170796c3f9f77e315b2dbff2b0a212bc68 in / 
# Tue, 15 Jun 2021 23:15:06 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 05:27:42 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 21:29:41 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 08 Jul 2021 21:29:42 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 08 Jul 2021 21:29:42 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 08 Jul 2021 21:30:19 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 08 Jul 2021 21:30:20 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 21:30:21 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 21:30:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 21:30:22 GMT
USER haproxy
# Thu, 08 Jul 2021 21:30:22 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:136482bf81d1fa351b424ebb8c7e34d15f2c5ed3fc0b66b544b8312bda3d52d9`  
		Last Modified: Tue, 15 Jun 2021 23:16:40 GMT  
		Size: 2.4 MB (2427917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5464af225bd487370319e7125fb2769222c5c7371d1be737936169d2e5b01c`  
		Last Modified: Sat, 26 Jun 2021 05:35:56 GMT  
		Size: 1.2 KB (1196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f903498f8e23244ca6430d647dd5515930d69394f19d017d07930d288ca6580`  
		Last Modified: Thu, 08 Jul 2021 21:36:22 GMT  
		Size: 7.2 MB (7201807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a0d8812e6df331ba2d781cc1fc08c2e4ddad2bb05b762b0eb737308a1205d5`  
		Last Modified: Thu, 08 Jul 2021 21:36:18 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:c17729aebb94fdae2758381c550a8866ce8856237ce1892a6fba9d0cdadd7c5b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.1 MB (10133906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b500e8260787f1a0bcdc19f790686cd272d751cdd28f848f01eb2f054c700341`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 21:44:56 GMT
ADD file:6797caacbfe41bfe44000b39ed017016c6fcc492b3d6557cdaba88536df6c876 in / 
# Tue, 15 Jun 2021 21:44:56 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 02:13:15 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 19:02:27 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 08 Jul 2021 19:02:27 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 08 Jul 2021 19:02:27 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 08 Jul 2021 19:03:26 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 08 Jul 2021 19:03:26 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 19:03:27 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 19:03:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 19:03:27 GMT
USER haproxy
# Thu, 08 Jul 2021 19:03:27 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:58ab47519297212468320b23b8100fc1b2b96e8d342040806ae509a778a0a07a`  
		Last Modified: Tue, 15 Jun 2021 21:46:03 GMT  
		Size: 2.7 MB (2709626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb8dc96e2a4b7f90ae2dbfca981fe199966b64e3426ca1f742499d46ad1aa357`  
		Last Modified: Sat, 26 Jun 2021 02:21:19 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b367d065849fc1a609fb169119e94047ed3a2b475932bb292bff5b6cc45a1f`  
		Last Modified: Thu, 08 Jul 2021 19:07:30 GMT  
		Size: 7.4 MB (7422635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60cf6675a5a8e39f65c07f8553ab269ab83f947cbfa20da77e6da66ca033969e`  
		Last Modified: Thu, 08 Jul 2021 19:07:28 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts-alpine` - linux; 386

```console
$ docker pull haproxy@sha256:01a8472d10c0512c1950dad3ae7472f99767eeaa8f0bbbb3aa53813d35961ab0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (9998434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e50005241013c0fb9d14f539c88cbf5dd3ebfec6c0498014c4a70a002cbe3d48`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 21:38:30 GMT
ADD file:3b0fe1454491bb05e218b090fd461f2fd39546aa4a53eb3f953ee8eae149ac57 in / 
# Tue, 15 Jun 2021 21:38:30 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 01:39:05 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 19:03:09 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 08 Jul 2021 19:03:09 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 08 Jul 2021 19:03:09 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 08 Jul 2021 19:04:25 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 08 Jul 2021 19:04:25 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 19:04:25 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 19:04:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 19:04:26 GMT
USER haproxy
# Thu, 08 Jul 2021 19:04:26 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:be21df321efb39c5daf3151073ebff7688e15ea6cd5158878bc9559a5db76ac6`  
		Last Modified: Tue, 15 Jun 2021 21:39:16 GMT  
		Size: 2.8 MB (2820718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc6fe536c8e50a97873c166db7d3b669842dec91d85ce73433028b3b198a1c4`  
		Last Modified: Sat, 26 Jun 2021 01:49:46 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:832c00757ee7003ebca753eff8d4c6af86ebcf09efecec8e1171e550c8fc816f`  
		Last Modified: Thu, 08 Jul 2021 19:08:59 GMT  
		Size: 7.2 MB (7176071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85e6578d15134f65f8b977b9e7c9322e6281b3c765978ce760142c0bac7197ad`  
		Last Modified: Thu, 08 Jul 2021 19:08:57 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts-alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:8371490329ce959d92d6d6bca900a6702869e800fbd8c4a80438da13efa8b696
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.6 MB (10556641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5510c2e0b44e02d587dd27e62dd07ef69cc51b3e43f00927403e3c29eb34cfc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:27:00 GMT
ADD file:0075aad7a94f0496483442bb2d9fdaa13e9c23087b90638d014b4bc263aa3861 in / 
# Tue, 15 Jun 2021 22:27:03 GMT
CMD ["/bin/sh"]
# Fri, 16 Jul 2021 20:17:57 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 16 Jul 2021 20:19:42 GMT
ENV HAPROXY_VERSION=2.4.2
# Fri, 16 Jul 2021 20:19:48 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Fri, 16 Jul 2021 20:19:51 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 22 Jul 2021 03:04:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 22 Jul 2021 03:04:47 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 03:04:50 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 03:04:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 03:04:59 GMT
USER haproxy
# Thu, 22 Jul 2021 03:05:04 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:baf144cfb66ebe9df1969f3b90f1c448beff98edc84de1ccb5d6346195a070d4`  
		Last Modified: Tue, 15 Jun 2021 22:27:38 GMT  
		Size: 2.8 MB (2810478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e907663c9428bbbb731a221721c606bad29e54dac6f0dda85d6aa3175a725e`  
		Last Modified: Thu, 22 Jul 2021 03:40:16 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25fed8e719bd522b435fea4d6999c2ecffeb38e8288458cea40c3ecfa9131656`  
		Last Modified: Thu, 22 Jul 2021 03:40:53 GMT  
		Size: 7.7 MB (7744514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c45ecd590d1194b07f22c1e98348800abd5fdc2592d5c85e8fd5413acc1f29`  
		Last Modified: Thu, 22 Jul 2021 03:40:50 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts-alpine` - linux; s390x

```console
$ docker pull haproxy@sha256:67c77b2f75cda356f4462fa8c7cfe05d80b220bb7e3ddff6782557ca308381e0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9899025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8353b377710bdcc56a8dd1fcdf4213b83d4378a795634015c8ec0817188591f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:54:24 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:45:22 GMT
ENV HAPROXY_VERSION=2.4.0
# Fri, 14 May 2021 19:45:23 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Fri, 14 May 2021 19:45:23 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Fri, 14 May 2021 19:46:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 14 May 2021 19:46:14 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:46:14 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:46:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:46:15 GMT
USER haproxy
# Fri, 14 May 2021 19:46:15 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267275aba58470c82626189a59be76cd169bd245568e2f2545ed1ee64ff8a8ff`  
		Last Modified: Wed, 14 Apr 2021 20:59:06 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1af9bde57dd624c224ba02793a7568cd9f00874c978ff5ab4d6bc0c32fdb81f`  
		Last Modified: Fri, 14 May 2021 19:48:00 GMT  
		Size: 7.3 MB (7294741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68dd09d54ba9406459ae1956173c0df96676de52e5a01f9392966e3493acae68`  
		Last Modified: Fri, 14 May 2021 19:47:59 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
