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
-	[`haproxy:2.0.22`](#haproxy2022)
-	[`haproxy:2.0.22-alpine`](#haproxy2022-alpine)
-	[`haproxy:2.2`](#haproxy22)
-	[`haproxy:2.2-alpine`](#haproxy22-alpine)
-	[`haproxy:2.2.14`](#haproxy2214)
-	[`haproxy:2.2.14-alpine`](#haproxy2214-alpine)
-	[`haproxy:2.3`](#haproxy23)
-	[`haproxy:2.3-alpine`](#haproxy23-alpine)
-	[`haproxy:2.3.10`](#haproxy2310)
-	[`haproxy:2.3.10-alpine`](#haproxy2310-alpine)
-	[`haproxy:2.4-dev`](#haproxy24-dev)
-	[`haproxy:2.4-dev-alpine`](#haproxy24-dev-alpine)
-	[`haproxy:2.4-dev18`](#haproxy24-dev18)
-	[`haproxy:2.4-dev18-alpine`](#haproxy24-dev18-alpine)
-	[`haproxy:alpine`](#haproxyalpine)
-	[`haproxy:latest`](#haproxylatest)
-	[`haproxy:lts`](#haproxylts)
-	[`haproxy:lts-alpine`](#haproxylts-alpine)

## `haproxy:1.7`

```console
$ docker pull haproxy@sha256:86765641239369793563fc94431094fb03155fa1bd4a62c629e8f66f20354203
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

### `haproxy:1.7` - linux; amd64

```console
$ docker pull haproxy@sha256:9485dcd2d4423b92e2d0c601f047b96457bd16aca9f39187202b9947423bdfa7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.5 MB (32534800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3be5a7d35fe52f0890dbf6ac5cd34328096cb4e1d7684fa967224712b37f44f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:29:42 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 06:36:18 GMT
ENV HAPROXY_VERSION=1.7.14
# Sat, 10 Apr 2021 06:36:18 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Sat, 10 Apr 2021 06:36:18 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Sat, 10 Apr 2021 06:37:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 06:37:12 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 06:37:13 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Sat, 10 Apr 2021 06:37:15 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 06:37:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 06:37:16 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7abf58d954de379f38a19e07330116ba6b11f21007bc7b7507d233e5b0aa3fe0`  
		Last Modified: Sat, 10 Apr 2021 06:38:07 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71b4d12088d66d0b010097d7ccdf29d852983431b12fd54bfb27ef76f28d772d`  
		Last Modified: Sat, 10 Apr 2021 06:39:20 GMT  
		Size: 5.4 MB (5393454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3708361d286bf7ea0f198c6ba458905ef44ba431e6015b505899b9d4d15c1ce`  
		Last Modified: Sat, 10 Apr 2021 06:39:19 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a619b7e443cfa8041c2c9b85bd675b0cf4aced43ba03a121044294e7b9c070f`  
		Last Modified: Sat, 10 Apr 2021 06:39:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:f06241b916c44402f5e50ccbc8d631f2f107393c5f255074aa054d45a684b673
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.9 MB (29895450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36d3d59f5f1f9a9f1ef78b13ccabb67daccf0b24446f88bf75ea88640662d136`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:51:31 GMT
ADD file:926533a23a69aa2481a9122b667bb6300a347154eea366c9e679a230aa7f373a in / 
# Sat, 10 Apr 2021 00:51:34 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 02:24:17 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 02:34:41 GMT
ENV HAPROXY_VERSION=1.7.14
# Sat, 10 Apr 2021 02:34:44 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Sat, 10 Apr 2021 02:34:48 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Sat, 10 Apr 2021 02:35:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 02:36:01 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 02:36:07 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Sat, 10 Apr 2021 02:36:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 02:36:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 02:36:26 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:33d77752597b664d047cc829e58a223d6fb077b61f69ca0462fcfb9b78d5f69b`  
		Last Modified: Sat, 10 Apr 2021 00:59:22 GMT  
		Size: 24.9 MB (24873199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c107a5973e1ce17cb311e2bf8a0d841875ca9f02219922ca12a9203602b5ce`  
		Last Modified: Sat, 10 Apr 2021 02:36:55 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81a91c28d6dd3e14fce15c11fca2be426efd5d0582469b80bb108d04e8fbbe7b`  
		Last Modified: Sat, 10 Apr 2021 02:37:42 GMT  
		Size: 5.0 MB (5020278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b042298e0abddeb2579b6902b25a6f7add0bb10eaa676c8678180a93f63721`  
		Last Modified: Sat, 10 Apr 2021 02:37:41 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf7a056727806508eccdb522b8db9a445156c0ec24ee14276cde5eee53d478b`  
		Last Modified: Sat, 10 Apr 2021 02:37:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:b0b6fc253ad59ff074e6d9f9f05849b0a8d415ccf5ab8bfc6cc784fb3633d280
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.6 MB (27634002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5291a5a95e002009e8ccd80ddeea8c9e1d92709b69155765f029e2f4a54690ca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:59:45 GMT
ADD file:3fbd246a2de82566bcaaf62e3e0bf57175a7ad46b4156366a110661b31eab240 in / 
# Sat, 10 Apr 2021 00:59:47 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 08:58:51 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 09:04:10 GMT
ENV HAPROXY_VERSION=1.7.14
# Sat, 10 Apr 2021 09:04:11 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Sat, 10 Apr 2021 09:04:11 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Sat, 10 Apr 2021 09:04:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 09:04:48 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 09:04:49 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Sat, 10 Apr 2021 09:04:51 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 09:04:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 09:04:52 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:8c6bea184b33030fb923c3c09d634b73235dec3fe2d411db9fd22bda669f2c37`  
		Last Modified: Sat, 10 Apr 2021 01:07:51 GMT  
		Size: 22.7 MB (22739801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5be95d3afdef3cc4c8a37695b513cf41e6cf6ffeecd9ce2426d38cb245a0b52`  
		Last Modified: Sat, 10 Apr 2021 09:05:25 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb8ab14dd1beb0c93a00b06aadd01d3fb77474e66b58564726a449b950b70db4`  
		Last Modified: Sat, 10 Apr 2021 09:06:20 GMT  
		Size: 4.9 MB (4892231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d098795434c94de9c66d34e1bca584e022e1f5bd5af3d84ddcb791c47f82bb`  
		Last Modified: Sat, 10 Apr 2021 09:06:19 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04bfde9a4621e14b08e187449ae3dda95c998963564063e9ab8d8365f1c3bc88`  
		Last Modified: Sat, 10 Apr 2021 09:06:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:95d5098892c699ea75bbe15ace7f3210dfa6db41c593284b22b7165d1ed5c35c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31187715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd1e1128cc650bf8352ae830322c84ddec8fda039ce75baf8f1dc515699ba8c3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:41:25 GMT
ADD file:b24da7eb23eeae04e00d0e45da29a89fe8f992e8dcf4ba482afb907b8015b7bf in / 
# Sat, 10 Apr 2021 00:41:28 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:13:29 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 01:19:52 GMT
ENV HAPROXY_VERSION=1.7.14
# Sat, 10 Apr 2021 01:19:53 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Sat, 10 Apr 2021 01:19:55 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Sat, 10 Apr 2021 01:20:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 01:20:43 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 01:20:43 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Sat, 10 Apr 2021 01:20:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 01:20:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 01:20:47 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:15cb40b9c4df1a06940dc2a154c3be46844241235c1a091afa70da0ee2dc811a`  
		Last Modified: Sat, 10 Apr 2021 00:47:53 GMT  
		Size: 25.9 MB (25904582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48cb832c3e00ffed789c3f464caa612fe4996ba4683f72f8cf214d1437268efe`  
		Last Modified: Sat, 10 Apr 2021 01:21:27 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ebf48ef9ec5574efcb786f08ce3e5b52e32cd9834a232b19a8593b3aaaa08c7`  
		Last Modified: Sat, 10 Apr 2021 01:22:21 GMT  
		Size: 5.3 MB (5281159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0768d0b6af82665897144eb3fd5910ee55aa6582abc1d7861b80697b3b23a18`  
		Last Modified: Sat, 10 Apr 2021 01:22:20 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901558bac4fe36e25c875021ad726eda7f74bbaed863c618b921bc606466cab1`  
		Last Modified: Sat, 10 Apr 2021 01:22:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7` - linux; 386

```console
$ docker pull haproxy@sha256:9bc5ffa3cddfb4bb907f138684d1a8447ecffd036e334a9c3f76cd7d071468e5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.1 MB (33115032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f75e795c5681951cf4b3d5ca9c47b5bc811f4f216d344f8279f8909f557d474`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:39:42 GMT
ADD file:8885d4d13678543780bb04ba14b621179665f7951d5b261036a7092df9b376e7 in / 
# Sat, 10 Apr 2021 00:39:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 03:48:12 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 03:56:14 GMT
ENV HAPROXY_VERSION=1.7.14
# Sat, 10 Apr 2021 03:56:14 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Sat, 10 Apr 2021 03:56:15 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Sat, 10 Apr 2021 03:57:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 03:57:12 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 03:57:13 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Sat, 10 Apr 2021 03:57:14 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 03:57:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 03:57:15 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:7cc57a8772e5e479618650dfa70f315b474d3f205d04bde7f602f469c1928d84`  
		Last Modified: Sat, 10 Apr 2021 00:46:07 GMT  
		Size: 27.8 MB (27788987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d92d68a52363235dcdfb59fa81e5ef1a4561c958501e4f28d6b79e86f8b8501`  
		Last Modified: Sat, 10 Apr 2021 03:59:08 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:629908cb93e866d44e3508c38cbc066756feadc5348273d3d64bf9102ab28f2a`  
		Last Modified: Sat, 10 Apr 2021 04:01:00 GMT  
		Size: 5.3 MB (5324076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5537909f96855611b54beef42d7ff791fc263dd0f684024ce806243adf6e37c0`  
		Last Modified: Sat, 10 Apr 2021 04:00:58 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9100d54ae5d2cc0b8489fa2575401edf65b8d33d89442caa682ea43e79b1e80f`  
		Last Modified: Sat, 10 Apr 2021 04:00:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7` - linux; mips64le

```console
$ docker pull haproxy@sha256:a61f4b6f4d7d92713ae98a11473848ce2b32c2bb5fd903886030d606743d4c6e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.8 MB (30836184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10a09dc9d28c1a946bbcfb047bcabdb758a1fbe3c195e1be75bde071942fe267`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:09:40 GMT
ADD file:0c93801c4a3719dfd4c047d7f2f4d52bf463eba2ab875da1dc54dcc832aae20b in / 
# Sat, 10 Apr 2021 01:09:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:39:36 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 01:51:47 GMT
ENV HAPROXY_VERSION=1.7.14
# Sat, 10 Apr 2021 01:51:47 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Sat, 10 Apr 2021 01:51:47 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Sat, 10 Apr 2021 01:53:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 01:53:14 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 01:53:14 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Sat, 10 Apr 2021 01:53:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 01:53:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 01:53:16 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:09ea659ba566d9c3c62493e5ae0b964f1eee4fcf35aabc91c5c34ca1ad686541`  
		Last Modified: Sat, 10 Apr 2021 01:16:07 GMT  
		Size: 25.8 MB (25806410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10fa5ae1be1fc686c91c15f24ebaaa72d7c4f64321c8ead8386f2f4f9d1a6705`  
		Last Modified: Sat, 10 Apr 2021 01:53:41 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9757bab144db1fb0996ab850993e2de8d8c30f21a1f2fa8e11cc984bfa6f80f3`  
		Last Modified: Sat, 10 Apr 2021 01:55:14 GMT  
		Size: 5.0 MB (5027800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39556ccdc324eabb8b9bd09f741be110bfe117f772a613c7dec675eb3f56ec77`  
		Last Modified: Sat, 10 Apr 2021 01:55:07 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb5414398847953189a815e20fd3b61944bd827c7dacce9b99b2d47775130a2`  
		Last Modified: Sat, 10 Apr 2021 01:55:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7` - linux; ppc64le

```console
$ docker pull haproxy@sha256:4bab382a46428053e37eddb8d06b88c81528dfd3efac87b9461a689dc34961f0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36258558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42d662ebb2842077bf6dbe8a8d2621f65d6d3572add1e50cc95743cd3a2ce1e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:26:49 GMT
ADD file:ab87d4854aa8628ce8f4e603c0496499f6f28c3d2525ace782c7369691dafc8c in / 
# Sat, 10 Apr 2021 01:26:56 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 04:45:12 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 05:06:20 GMT
ENV HAPROXY_VERSION=1.7.14
# Sat, 10 Apr 2021 05:06:25 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Sat, 10 Apr 2021 05:06:30 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Sat, 10 Apr 2021 05:08:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 05:08:59 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 05:09:00 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Sat, 10 Apr 2021 05:09:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 05:09:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 05:09:16 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:3e1e599482ca47095f85e429b346b76375aa85015ddcca050e85c2a8b1fdda9c`  
		Last Modified: Sat, 10 Apr 2021 01:33:57 GMT  
		Size: 30.5 MB (30545933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ee41bdc57145d3cb6e9f5fa23eed213567ae52835c7cff5fd57fe17b52f5ec`  
		Last Modified: Sat, 10 Apr 2021 05:09:50 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a71cf39f4df29687ac3b57f39c0fefb91f7898604c6fdb3aa89d548afc02c94`  
		Last Modified: Sat, 10 Apr 2021 05:11:02 GMT  
		Size: 5.7 MB (5710642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea5d73bbd5d3066055cacfd83b3730fb8abf3ae966708fe6b233ad535e52fbf`  
		Last Modified: Sat, 10 Apr 2021 05:11:03 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03372ab2f2d2acf89f5046a84b066fb237f83e5fe47075e6380063fa262e3c84`  
		Last Modified: Sat, 10 Apr 2021 05:11:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7` - linux; s390x

```console
$ docker pull haproxy@sha256:5f5f42af0448c88201e26120de1317a85e7f62eefa46fcd819a65c6307490c4e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.9 MB (30884842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2da0f740ecc4c945e2a957512245be48400b38d47d56fe425badefd75949d82c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:42:23 GMT
ADD file:dbe2182f8699f2a6011413ea01862e6c0e85853d922dffd72a28d994d23c79bc in / 
# Sat, 10 Apr 2021 00:42:25 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:38:04 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 01:41:37 GMT
ENV HAPROXY_VERSION=1.7.14
# Sat, 10 Apr 2021 01:41:37 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Sat, 10 Apr 2021 01:41:37 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Sat, 10 Apr 2021 01:41:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 01:41:57 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 01:41:57 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Sat, 10 Apr 2021 01:41:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 01:41:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 01:41:58 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:65291f8717b3afd99b63cee867dd3e06b956a8ee6aa8580cc31d913b25de209d`  
		Last Modified: Sat, 10 Apr 2021 00:45:48 GMT  
		Size: 25.8 MB (25753787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9daf67acfb0373e31068762d068f1da8d320f2bdcdb0e6651d52b8183ede06c`  
		Last Modified: Sat, 10 Apr 2021 01:42:28 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3d7d9931f0ec1cfcf0a56dc385fc912270f4e0206cd522c6c80cb7b2974d00a`  
		Last Modified: Sat, 10 Apr 2021 01:43:12 GMT  
		Size: 5.1 MB (5129084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acfd8bd57908b5f743beb96b93ffd0dc78d05022bb2e56fd52f8141ee44b34e5`  
		Last Modified: Sat, 10 Apr 2021 01:43:11 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b08d41769fbc19c441d050bd8743213c34be089ff6bc4ca227491f1d301749b2`  
		Last Modified: Sat, 10 Apr 2021 01:43:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:1.7-alpine`

```console
$ docker pull haproxy@sha256:3b90f8f1e60e7c1f23740fa6de7f005512337a01bbab7fecabc773d5512fc765
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
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
$ docker pull haproxy@sha256:5fab95a68a697ba445d135a3cd9bd8069bd4792403722893fd94e62c420e06ca
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 MB (3326542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29f89f5871dc2fa0e9354ef05054008aae384b4a53e7a5c4fea2d657e6e4164c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:49 GMT
ADD file:82fa6a18d24e3f535c9061d2e111d63fe6d8a27710bb34a17b326e605ff478be in / 
# Wed, 14 Apr 2021 18:49:50 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:30:48 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 21:30:57 GMT
ENV HAPROXY_VERSION=1.7.14
# Wed, 14 Apr 2021 21:31:12 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Wed, 14 Apr 2021 21:31:15 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Wed, 14 Apr 2021 21:31:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		CFLAGS+="-Wno-address-of-packed-member" 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 21:31:42 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 21:31:50 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Wed, 14 Apr 2021 21:33:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 21:33:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 21:33:26 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:b452d2916bdfd021add56f1eda6bdea35400671ef07b38316ef82fce92a88fee`  
		Last Modified: Wed, 14 Apr 2021 18:50:38 GMT  
		Size: 2.6 MB (2605253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e34ee72605fbe9151f1949e2d9f44256afe0087ef46291d2370268fdc09193`  
		Last Modified: Wed, 14 Apr 2021 21:35:15 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a33a682697a21398281fd19fe479fd9f66b211f5ef261672a0f1bb6617e0031`  
		Last Modified: Wed, 14 Apr 2021 21:35:23 GMT  
		Size: 719.5 KB (719510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da17ca29438abfc4ca8f1b256b99becaa5f901e4745cafa0562db687dd18a269`  
		Last Modified: Wed, 14 Apr 2021 21:35:15 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a662029ec9324da645c7285f2fe0e654244715aa44d062814e17804fba55ae39`  
		Last Modified: Wed, 14 Apr 2021 21:35:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:c791ca801845bc7f910ef5138afc9c712a140146bdf9451b64307179e4270c50
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3087782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:546676626ca3de1997804688a96b0f776dfb461bf0968ce1da0e9abc02689982`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:50 GMT
ADD file:d844cc7b5e00fb62be39d903a2fb4a08f700e75112c8eef1f31101e846ed010d in / 
# Wed, 14 Apr 2021 18:57:52 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:55:00 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 22:55:01 GMT
ENV HAPROXY_VERSION=1.7.14
# Wed, 14 Apr 2021 22:55:02 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Wed, 14 Apr 2021 22:55:03 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Wed, 14 Apr 2021 22:55:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		CFLAGS+="-Wno-address-of-packed-member" 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 22:55:17 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 22:55:18 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Wed, 14 Apr 2021 22:55:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 22:55:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 22:55:26 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:420c7481a3a76d5d12df768d2745ddbe40357df0af780c756a5a7d1f2a43d288`  
		Last Modified: Wed, 14 Apr 2021 18:58:46 GMT  
		Size: 2.4 MB (2409178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c92f383df2c0c59011d5f915370f3fcc804629595e047106287c2b96cb40f6c`  
		Last Modified: Wed, 14 Apr 2021 22:57:09 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab181a363700a15e9fcc695ab50e344b0ca7fcb9b797d6bf61b0b4af94d643e`  
		Last Modified: Wed, 14 Apr 2021 22:57:10 GMT  
		Size: 676.8 KB (676824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffc8dd2548bacab438293db38856d35b638640f1fed0ce59a99ae9773deaf89f`  
		Last Modified: Wed, 14 Apr 2021 22:57:09 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053058fad8d0c6505b10792b8e60e1c5eeac4f8fe136518fb5987fe5f1c80c65`  
		Last Modified: Wed, 14 Apr 2021 22:57:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:1a6b382c69e3e7e177e3287416d4042e664343e79fae0bc27c282d1333f925c3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3433874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef305d499040e1ba9c7f65f6475b7efa4ed0d0e77bc3d4b331755856b4b60d49`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:54 GMT
ADD file:3db1e10ac5ebf1cb34939eff736f1384f7d3b17355758cec361489fa7a7e19ca in / 
# Wed, 14 Apr 2021 18:42:55 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:36:06 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 20:36:12 GMT
ENV HAPROXY_VERSION=1.7.14
# Wed, 14 Apr 2021 20:36:18 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Wed, 14 Apr 2021 20:36:26 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Wed, 14 Apr 2021 20:36:51 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		CFLAGS+="-Wno-address-of-packed-member" 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 20:36:53 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 20:36:55 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:36:59 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 20:37:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:37:02 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:d2f70382dc9a1658ea3491d7ab4439c22087e426c00e3eb7daf825b83be4ba9c`  
		Last Modified: Wed, 14 Apr 2021 18:43:55 GMT  
		Size: 2.7 MB (2710694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a087057ae14354a8cb5575811ee4d6a4bfe94052f4ad0fb7c8776a102ba4a1`  
		Last Modified: Wed, 14 Apr 2021 20:39:04 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4fb090fb6a4f3e38517ae54ebdddc1222a8e6ba41e398a8544abbcc52e28fa3`  
		Last Modified: Wed, 14 Apr 2021 20:39:04 GMT  
		Size: 721.4 KB (721398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d71ba7ca7294261fe13bb77a28155bf31ce267db5173acaec74245ef17259bed`  
		Last Modified: Wed, 14 Apr 2021 20:39:04 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd584ca034057746eca3d5149ce653f04c3cf1cce19948252a4e86f9b074b89a`  
		Last Modified: Wed, 14 Apr 2021 20:39:04 GMT  
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
$ docker pull haproxy@sha256:3fe95f5e04b018ee893bfef587bae46924daa7279d56ee0b1b74c49b01327e10
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3573874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de6707172b5b2faf5cebdf1e3951a347159c77e40b1ee80d081715ad2e122ff0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:31:22 GMT
ADD file:f8b081207f6d35f8ebd06aa471e350644151d183801f678def586d8f37e81366 in / 
# Wed, 14 Apr 2021 19:31:29 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:35:00 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 23:35:04 GMT
ENV HAPROXY_VERSION=1.7.14
# Wed, 14 Apr 2021 23:35:12 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Wed, 14 Apr 2021 23:35:17 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Wed, 14 Apr 2021 23:35:41 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		CFLAGS+="-Wno-address-of-packed-member" 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 23:35:43 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 23:35:45 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Wed, 14 Apr 2021 23:35:52 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 23:35:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 23:35:59 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:45707b9629c4ab8c6046680737229218fe844f38d08e5458b24605e1dbfd2709`  
		Last Modified: Wed, 14 Apr 2021 19:32:50 GMT  
		Size: 2.8 MB (2806750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ccabd352c510a8ea2f0562208f4f16f8c677e78b2769758faa7a460dc8e0fa`  
		Last Modified: Wed, 14 Apr 2021 23:37:50 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1657c99885b62f2866706170fb7c286e8da44aa6fe5257af8d92dc85b92caa1`  
		Last Modified: Wed, 14 Apr 2021 23:37:50 GMT  
		Size: 765.3 KB (765340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92452a0dc3abcbca973925280190cb7501d8b0c40a9c4f17cff1d79654efba0`  
		Last Modified: Wed, 14 Apr 2021 23:37:50 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13b958ef2e40999648c9cfebb0978dbdbe4cdcb77f6102ea7e016db7a01cb7b`  
		Last Modified: Wed, 14 Apr 2021 23:37:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7-alpine` - linux; s390x

```console
$ docker pull haproxy@sha256:d6ecdb80bbcb96317666b45842f5603759d2903dcd4795ffb5de6de8b2b60e9c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 MB (3346079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4b7fe629af0ab171c3ad1905a110dea72527e52944bfb6c6318d09210c33601`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:42 GMT
ADD file:c73a5ff435939cdc9d621ee9dc2aa5a54a5f5e0241caae8dc948c03c423d9fef in / 
# Wed, 14 Apr 2021 18:41:42 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:58:22 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 20:58:22 GMT
ENV HAPROXY_VERSION=1.7.14
# Wed, 14 Apr 2021 20:58:23 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Wed, 14 Apr 2021 20:58:23 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Wed, 14 Apr 2021 20:58:30 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		CFLAGS+="-Wno-address-of-packed-member" 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 20:58:30 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 20:58:31 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:58:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 20:58:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:58:32 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:27efec644c4207cbc4d1400f84f3402937aab5ce72489976148896e42a219820`  
		Last Modified: Wed, 14 Apr 2021 18:42:24 GMT  
		Size: 2.6 MB (2568428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:503f90387c77c1fc4e68bce67a06e9978c31073dcd4b85bee26367e674a81ed6`  
		Last Modified: Wed, 14 Apr 2021 20:59:51 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96e6b091ead06382abb37e2abbeece360efd0852a51879cc0e4441fbc71098c`  
		Last Modified: Wed, 14 Apr 2021 20:59:51 GMT  
		Size: 775.9 KB (775873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4daef8fbb6977ed6b49701e632cb5b37068aa45dd9621be67a736312baecd497`  
		Last Modified: Wed, 14 Apr 2021 20:59:51 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5977f2b11c8ff7c4155255f370678747c2f168f780e827e4eb223ce50f9dd965`  
		Last Modified: Wed, 14 Apr 2021 20:59:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:1.7.14`

```console
$ docker pull haproxy@sha256:86765641239369793563fc94431094fb03155fa1bd4a62c629e8f66f20354203
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

### `haproxy:1.7.14` - linux; amd64

```console
$ docker pull haproxy@sha256:9485dcd2d4423b92e2d0c601f047b96457bd16aca9f39187202b9947423bdfa7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.5 MB (32534800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3be5a7d35fe52f0890dbf6ac5cd34328096cb4e1d7684fa967224712b37f44f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:29:42 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 06:36:18 GMT
ENV HAPROXY_VERSION=1.7.14
# Sat, 10 Apr 2021 06:36:18 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Sat, 10 Apr 2021 06:36:18 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Sat, 10 Apr 2021 06:37:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 06:37:12 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 06:37:13 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Sat, 10 Apr 2021 06:37:15 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 06:37:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 06:37:16 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7abf58d954de379f38a19e07330116ba6b11f21007bc7b7507d233e5b0aa3fe0`  
		Last Modified: Sat, 10 Apr 2021 06:38:07 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71b4d12088d66d0b010097d7ccdf29d852983431b12fd54bfb27ef76f28d772d`  
		Last Modified: Sat, 10 Apr 2021 06:39:20 GMT  
		Size: 5.4 MB (5393454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3708361d286bf7ea0f198c6ba458905ef44ba431e6015b505899b9d4d15c1ce`  
		Last Modified: Sat, 10 Apr 2021 06:39:19 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a619b7e443cfa8041c2c9b85bd675b0cf4aced43ba03a121044294e7b9c070f`  
		Last Modified: Sat, 10 Apr 2021 06:39:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7.14` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:f06241b916c44402f5e50ccbc8d631f2f107393c5f255074aa054d45a684b673
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.9 MB (29895450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36d3d59f5f1f9a9f1ef78b13ccabb67daccf0b24446f88bf75ea88640662d136`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:51:31 GMT
ADD file:926533a23a69aa2481a9122b667bb6300a347154eea366c9e679a230aa7f373a in / 
# Sat, 10 Apr 2021 00:51:34 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 02:24:17 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 02:34:41 GMT
ENV HAPROXY_VERSION=1.7.14
# Sat, 10 Apr 2021 02:34:44 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Sat, 10 Apr 2021 02:34:48 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Sat, 10 Apr 2021 02:35:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 02:36:01 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 02:36:07 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Sat, 10 Apr 2021 02:36:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 02:36:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 02:36:26 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:33d77752597b664d047cc829e58a223d6fb077b61f69ca0462fcfb9b78d5f69b`  
		Last Modified: Sat, 10 Apr 2021 00:59:22 GMT  
		Size: 24.9 MB (24873199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c107a5973e1ce17cb311e2bf8a0d841875ca9f02219922ca12a9203602b5ce`  
		Last Modified: Sat, 10 Apr 2021 02:36:55 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81a91c28d6dd3e14fce15c11fca2be426efd5d0582469b80bb108d04e8fbbe7b`  
		Last Modified: Sat, 10 Apr 2021 02:37:42 GMT  
		Size: 5.0 MB (5020278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b042298e0abddeb2579b6902b25a6f7add0bb10eaa676c8678180a93f63721`  
		Last Modified: Sat, 10 Apr 2021 02:37:41 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf7a056727806508eccdb522b8db9a445156c0ec24ee14276cde5eee53d478b`  
		Last Modified: Sat, 10 Apr 2021 02:37:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7.14` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:b0b6fc253ad59ff074e6d9f9f05849b0a8d415ccf5ab8bfc6cc784fb3633d280
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.6 MB (27634002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5291a5a95e002009e8ccd80ddeea8c9e1d92709b69155765f029e2f4a54690ca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:59:45 GMT
ADD file:3fbd246a2de82566bcaaf62e3e0bf57175a7ad46b4156366a110661b31eab240 in / 
# Sat, 10 Apr 2021 00:59:47 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 08:58:51 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 09:04:10 GMT
ENV HAPROXY_VERSION=1.7.14
# Sat, 10 Apr 2021 09:04:11 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Sat, 10 Apr 2021 09:04:11 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Sat, 10 Apr 2021 09:04:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 09:04:48 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 09:04:49 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Sat, 10 Apr 2021 09:04:51 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 09:04:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 09:04:52 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:8c6bea184b33030fb923c3c09d634b73235dec3fe2d411db9fd22bda669f2c37`  
		Last Modified: Sat, 10 Apr 2021 01:07:51 GMT  
		Size: 22.7 MB (22739801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5be95d3afdef3cc4c8a37695b513cf41e6cf6ffeecd9ce2426d38cb245a0b52`  
		Last Modified: Sat, 10 Apr 2021 09:05:25 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb8ab14dd1beb0c93a00b06aadd01d3fb77474e66b58564726a449b950b70db4`  
		Last Modified: Sat, 10 Apr 2021 09:06:20 GMT  
		Size: 4.9 MB (4892231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d098795434c94de9c66d34e1bca584e022e1f5bd5af3d84ddcb791c47f82bb`  
		Last Modified: Sat, 10 Apr 2021 09:06:19 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04bfde9a4621e14b08e187449ae3dda95c998963564063e9ab8d8365f1c3bc88`  
		Last Modified: Sat, 10 Apr 2021 09:06:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7.14` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:95d5098892c699ea75bbe15ace7f3210dfa6db41c593284b22b7165d1ed5c35c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31187715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd1e1128cc650bf8352ae830322c84ddec8fda039ce75baf8f1dc515699ba8c3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:41:25 GMT
ADD file:b24da7eb23eeae04e00d0e45da29a89fe8f992e8dcf4ba482afb907b8015b7bf in / 
# Sat, 10 Apr 2021 00:41:28 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:13:29 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 01:19:52 GMT
ENV HAPROXY_VERSION=1.7.14
# Sat, 10 Apr 2021 01:19:53 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Sat, 10 Apr 2021 01:19:55 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Sat, 10 Apr 2021 01:20:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 01:20:43 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 01:20:43 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Sat, 10 Apr 2021 01:20:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 01:20:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 01:20:47 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:15cb40b9c4df1a06940dc2a154c3be46844241235c1a091afa70da0ee2dc811a`  
		Last Modified: Sat, 10 Apr 2021 00:47:53 GMT  
		Size: 25.9 MB (25904582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48cb832c3e00ffed789c3f464caa612fe4996ba4683f72f8cf214d1437268efe`  
		Last Modified: Sat, 10 Apr 2021 01:21:27 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ebf48ef9ec5574efcb786f08ce3e5b52e32cd9834a232b19a8593b3aaaa08c7`  
		Last Modified: Sat, 10 Apr 2021 01:22:21 GMT  
		Size: 5.3 MB (5281159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0768d0b6af82665897144eb3fd5910ee55aa6582abc1d7861b80697b3b23a18`  
		Last Modified: Sat, 10 Apr 2021 01:22:20 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901558bac4fe36e25c875021ad726eda7f74bbaed863c618b921bc606466cab1`  
		Last Modified: Sat, 10 Apr 2021 01:22:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7.14` - linux; 386

```console
$ docker pull haproxy@sha256:9bc5ffa3cddfb4bb907f138684d1a8447ecffd036e334a9c3f76cd7d071468e5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.1 MB (33115032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f75e795c5681951cf4b3d5ca9c47b5bc811f4f216d344f8279f8909f557d474`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:39:42 GMT
ADD file:8885d4d13678543780bb04ba14b621179665f7951d5b261036a7092df9b376e7 in / 
# Sat, 10 Apr 2021 00:39:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 03:48:12 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 03:56:14 GMT
ENV HAPROXY_VERSION=1.7.14
# Sat, 10 Apr 2021 03:56:14 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Sat, 10 Apr 2021 03:56:15 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Sat, 10 Apr 2021 03:57:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 03:57:12 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 03:57:13 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Sat, 10 Apr 2021 03:57:14 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 03:57:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 03:57:15 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:7cc57a8772e5e479618650dfa70f315b474d3f205d04bde7f602f469c1928d84`  
		Last Modified: Sat, 10 Apr 2021 00:46:07 GMT  
		Size: 27.8 MB (27788987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d92d68a52363235dcdfb59fa81e5ef1a4561c958501e4f28d6b79e86f8b8501`  
		Last Modified: Sat, 10 Apr 2021 03:59:08 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:629908cb93e866d44e3508c38cbc066756feadc5348273d3d64bf9102ab28f2a`  
		Last Modified: Sat, 10 Apr 2021 04:01:00 GMT  
		Size: 5.3 MB (5324076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5537909f96855611b54beef42d7ff791fc263dd0f684024ce806243adf6e37c0`  
		Last Modified: Sat, 10 Apr 2021 04:00:58 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9100d54ae5d2cc0b8489fa2575401edf65b8d33d89442caa682ea43e79b1e80f`  
		Last Modified: Sat, 10 Apr 2021 04:00:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7.14` - linux; mips64le

```console
$ docker pull haproxy@sha256:a61f4b6f4d7d92713ae98a11473848ce2b32c2bb5fd903886030d606743d4c6e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.8 MB (30836184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10a09dc9d28c1a946bbcfb047bcabdb758a1fbe3c195e1be75bde071942fe267`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:09:40 GMT
ADD file:0c93801c4a3719dfd4c047d7f2f4d52bf463eba2ab875da1dc54dcc832aae20b in / 
# Sat, 10 Apr 2021 01:09:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:39:36 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 01:51:47 GMT
ENV HAPROXY_VERSION=1.7.14
# Sat, 10 Apr 2021 01:51:47 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Sat, 10 Apr 2021 01:51:47 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Sat, 10 Apr 2021 01:53:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 01:53:14 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 01:53:14 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Sat, 10 Apr 2021 01:53:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 01:53:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 01:53:16 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:09ea659ba566d9c3c62493e5ae0b964f1eee4fcf35aabc91c5c34ca1ad686541`  
		Last Modified: Sat, 10 Apr 2021 01:16:07 GMT  
		Size: 25.8 MB (25806410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10fa5ae1be1fc686c91c15f24ebaaa72d7c4f64321c8ead8386f2f4f9d1a6705`  
		Last Modified: Sat, 10 Apr 2021 01:53:41 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9757bab144db1fb0996ab850993e2de8d8c30f21a1f2fa8e11cc984bfa6f80f3`  
		Last Modified: Sat, 10 Apr 2021 01:55:14 GMT  
		Size: 5.0 MB (5027800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39556ccdc324eabb8b9bd09f741be110bfe117f772a613c7dec675eb3f56ec77`  
		Last Modified: Sat, 10 Apr 2021 01:55:07 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb5414398847953189a815e20fd3b61944bd827c7dacce9b99b2d47775130a2`  
		Last Modified: Sat, 10 Apr 2021 01:55:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7.14` - linux; ppc64le

```console
$ docker pull haproxy@sha256:4bab382a46428053e37eddb8d06b88c81528dfd3efac87b9461a689dc34961f0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36258558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42d662ebb2842077bf6dbe8a8d2621f65d6d3572add1e50cc95743cd3a2ce1e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:26:49 GMT
ADD file:ab87d4854aa8628ce8f4e603c0496499f6f28c3d2525ace782c7369691dafc8c in / 
# Sat, 10 Apr 2021 01:26:56 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 04:45:12 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 05:06:20 GMT
ENV HAPROXY_VERSION=1.7.14
# Sat, 10 Apr 2021 05:06:25 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Sat, 10 Apr 2021 05:06:30 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Sat, 10 Apr 2021 05:08:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 05:08:59 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 05:09:00 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Sat, 10 Apr 2021 05:09:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 05:09:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 05:09:16 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:3e1e599482ca47095f85e429b346b76375aa85015ddcca050e85c2a8b1fdda9c`  
		Last Modified: Sat, 10 Apr 2021 01:33:57 GMT  
		Size: 30.5 MB (30545933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ee41bdc57145d3cb6e9f5fa23eed213567ae52835c7cff5fd57fe17b52f5ec`  
		Last Modified: Sat, 10 Apr 2021 05:09:50 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a71cf39f4df29687ac3b57f39c0fefb91f7898604c6fdb3aa89d548afc02c94`  
		Last Modified: Sat, 10 Apr 2021 05:11:02 GMT  
		Size: 5.7 MB (5710642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea5d73bbd5d3066055cacfd83b3730fb8abf3ae966708fe6b233ad535e52fbf`  
		Last Modified: Sat, 10 Apr 2021 05:11:03 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03372ab2f2d2acf89f5046a84b066fb237f83e5fe47075e6380063fa262e3c84`  
		Last Modified: Sat, 10 Apr 2021 05:11:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7.14` - linux; s390x

```console
$ docker pull haproxy@sha256:5f5f42af0448c88201e26120de1317a85e7f62eefa46fcd819a65c6307490c4e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.9 MB (30884842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2da0f740ecc4c945e2a957512245be48400b38d47d56fe425badefd75949d82c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:42:23 GMT
ADD file:dbe2182f8699f2a6011413ea01862e6c0e85853d922dffd72a28d994d23c79bc in / 
# Sat, 10 Apr 2021 00:42:25 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:38:04 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 01:41:37 GMT
ENV HAPROXY_VERSION=1.7.14
# Sat, 10 Apr 2021 01:41:37 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Sat, 10 Apr 2021 01:41:37 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Sat, 10 Apr 2021 01:41:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 01:41:57 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 01:41:57 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Sat, 10 Apr 2021 01:41:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 01:41:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 01:41:58 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:65291f8717b3afd99b63cee867dd3e06b956a8ee6aa8580cc31d913b25de209d`  
		Last Modified: Sat, 10 Apr 2021 00:45:48 GMT  
		Size: 25.8 MB (25753787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9daf67acfb0373e31068762d068f1da8d320f2bdcdb0e6651d52b8183ede06c`  
		Last Modified: Sat, 10 Apr 2021 01:42:28 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3d7d9931f0ec1cfcf0a56dc385fc912270f4e0206cd522c6c80cb7b2974d00a`  
		Last Modified: Sat, 10 Apr 2021 01:43:12 GMT  
		Size: 5.1 MB (5129084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acfd8bd57908b5f743beb96b93ffd0dc78d05022bb2e56fd52f8141ee44b34e5`  
		Last Modified: Sat, 10 Apr 2021 01:43:11 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b08d41769fbc19c441d050bd8743213c34be089ff6bc4ca227491f1d301749b2`  
		Last Modified: Sat, 10 Apr 2021 01:43:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:1.7.14-alpine`

```console
$ docker pull haproxy@sha256:3b90f8f1e60e7c1f23740fa6de7f005512337a01bbab7fecabc773d5512fc765
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
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
$ docker pull haproxy@sha256:5fab95a68a697ba445d135a3cd9bd8069bd4792403722893fd94e62c420e06ca
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 MB (3326542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29f89f5871dc2fa0e9354ef05054008aae384b4a53e7a5c4fea2d657e6e4164c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:49 GMT
ADD file:82fa6a18d24e3f535c9061d2e111d63fe6d8a27710bb34a17b326e605ff478be in / 
# Wed, 14 Apr 2021 18:49:50 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:30:48 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 21:30:57 GMT
ENV HAPROXY_VERSION=1.7.14
# Wed, 14 Apr 2021 21:31:12 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Wed, 14 Apr 2021 21:31:15 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Wed, 14 Apr 2021 21:31:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		CFLAGS+="-Wno-address-of-packed-member" 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 21:31:42 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 21:31:50 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Wed, 14 Apr 2021 21:33:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 21:33:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 21:33:26 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:b452d2916bdfd021add56f1eda6bdea35400671ef07b38316ef82fce92a88fee`  
		Last Modified: Wed, 14 Apr 2021 18:50:38 GMT  
		Size: 2.6 MB (2605253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e34ee72605fbe9151f1949e2d9f44256afe0087ef46291d2370268fdc09193`  
		Last Modified: Wed, 14 Apr 2021 21:35:15 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a33a682697a21398281fd19fe479fd9f66b211f5ef261672a0f1bb6617e0031`  
		Last Modified: Wed, 14 Apr 2021 21:35:23 GMT  
		Size: 719.5 KB (719510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da17ca29438abfc4ca8f1b256b99becaa5f901e4745cafa0562db687dd18a269`  
		Last Modified: Wed, 14 Apr 2021 21:35:15 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a662029ec9324da645c7285f2fe0e654244715aa44d062814e17804fba55ae39`  
		Last Modified: Wed, 14 Apr 2021 21:35:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7.14-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:c791ca801845bc7f910ef5138afc9c712a140146bdf9451b64307179e4270c50
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3087782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:546676626ca3de1997804688a96b0f776dfb461bf0968ce1da0e9abc02689982`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:50 GMT
ADD file:d844cc7b5e00fb62be39d903a2fb4a08f700e75112c8eef1f31101e846ed010d in / 
# Wed, 14 Apr 2021 18:57:52 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:55:00 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 22:55:01 GMT
ENV HAPROXY_VERSION=1.7.14
# Wed, 14 Apr 2021 22:55:02 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Wed, 14 Apr 2021 22:55:03 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Wed, 14 Apr 2021 22:55:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		CFLAGS+="-Wno-address-of-packed-member" 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 22:55:17 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 22:55:18 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Wed, 14 Apr 2021 22:55:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 22:55:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 22:55:26 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:420c7481a3a76d5d12df768d2745ddbe40357df0af780c756a5a7d1f2a43d288`  
		Last Modified: Wed, 14 Apr 2021 18:58:46 GMT  
		Size: 2.4 MB (2409178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c92f383df2c0c59011d5f915370f3fcc804629595e047106287c2b96cb40f6c`  
		Last Modified: Wed, 14 Apr 2021 22:57:09 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab181a363700a15e9fcc695ab50e344b0ca7fcb9b797d6bf61b0b4af94d643e`  
		Last Modified: Wed, 14 Apr 2021 22:57:10 GMT  
		Size: 676.8 KB (676824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffc8dd2548bacab438293db38856d35b638640f1fed0ce59a99ae9773deaf89f`  
		Last Modified: Wed, 14 Apr 2021 22:57:09 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053058fad8d0c6505b10792b8e60e1c5eeac4f8fe136518fb5987fe5f1c80c65`  
		Last Modified: Wed, 14 Apr 2021 22:57:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7.14-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:1a6b382c69e3e7e177e3287416d4042e664343e79fae0bc27c282d1333f925c3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3433874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef305d499040e1ba9c7f65f6475b7efa4ed0d0e77bc3d4b331755856b4b60d49`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:54 GMT
ADD file:3db1e10ac5ebf1cb34939eff736f1384f7d3b17355758cec361489fa7a7e19ca in / 
# Wed, 14 Apr 2021 18:42:55 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:36:06 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 20:36:12 GMT
ENV HAPROXY_VERSION=1.7.14
# Wed, 14 Apr 2021 20:36:18 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Wed, 14 Apr 2021 20:36:26 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Wed, 14 Apr 2021 20:36:51 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		CFLAGS+="-Wno-address-of-packed-member" 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 20:36:53 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 20:36:55 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:36:59 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 20:37:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:37:02 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:d2f70382dc9a1658ea3491d7ab4439c22087e426c00e3eb7daf825b83be4ba9c`  
		Last Modified: Wed, 14 Apr 2021 18:43:55 GMT  
		Size: 2.7 MB (2710694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a087057ae14354a8cb5575811ee4d6a4bfe94052f4ad0fb7c8776a102ba4a1`  
		Last Modified: Wed, 14 Apr 2021 20:39:04 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4fb090fb6a4f3e38517ae54ebdddc1222a8e6ba41e398a8544abbcc52e28fa3`  
		Last Modified: Wed, 14 Apr 2021 20:39:04 GMT  
		Size: 721.4 KB (721398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d71ba7ca7294261fe13bb77a28155bf31ce267db5173acaec74245ef17259bed`  
		Last Modified: Wed, 14 Apr 2021 20:39:04 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd584ca034057746eca3d5149ce653f04c3cf1cce19948252a4e86f9b074b89a`  
		Last Modified: Wed, 14 Apr 2021 20:39:04 GMT  
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
$ docker pull haproxy@sha256:3fe95f5e04b018ee893bfef587bae46924daa7279d56ee0b1b74c49b01327e10
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3573874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de6707172b5b2faf5cebdf1e3951a347159c77e40b1ee80d081715ad2e122ff0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:31:22 GMT
ADD file:f8b081207f6d35f8ebd06aa471e350644151d183801f678def586d8f37e81366 in / 
# Wed, 14 Apr 2021 19:31:29 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:35:00 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 23:35:04 GMT
ENV HAPROXY_VERSION=1.7.14
# Wed, 14 Apr 2021 23:35:12 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Wed, 14 Apr 2021 23:35:17 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Wed, 14 Apr 2021 23:35:41 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		CFLAGS+="-Wno-address-of-packed-member" 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 23:35:43 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 23:35:45 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Wed, 14 Apr 2021 23:35:52 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 23:35:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 23:35:59 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:45707b9629c4ab8c6046680737229218fe844f38d08e5458b24605e1dbfd2709`  
		Last Modified: Wed, 14 Apr 2021 19:32:50 GMT  
		Size: 2.8 MB (2806750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ccabd352c510a8ea2f0562208f4f16f8c677e78b2769758faa7a460dc8e0fa`  
		Last Modified: Wed, 14 Apr 2021 23:37:50 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1657c99885b62f2866706170fb7c286e8da44aa6fe5257af8d92dc85b92caa1`  
		Last Modified: Wed, 14 Apr 2021 23:37:50 GMT  
		Size: 765.3 KB (765340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92452a0dc3abcbca973925280190cb7501d8b0c40a9c4f17cff1d79654efba0`  
		Last Modified: Wed, 14 Apr 2021 23:37:50 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13b958ef2e40999648c9cfebb0978dbdbe4cdcb77f6102ea7e016db7a01cb7b`  
		Last Modified: Wed, 14 Apr 2021 23:37:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7.14-alpine` - linux; s390x

```console
$ docker pull haproxy@sha256:d6ecdb80bbcb96317666b45842f5603759d2903dcd4795ffb5de6de8b2b60e9c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 MB (3346079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4b7fe629af0ab171c3ad1905a110dea72527e52944bfb6c6318d09210c33601`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:42 GMT
ADD file:c73a5ff435939cdc9d621ee9dc2aa5a54a5f5e0241caae8dc948c03c423d9fef in / 
# Wed, 14 Apr 2021 18:41:42 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:58:22 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 20:58:22 GMT
ENV HAPROXY_VERSION=1.7.14
# Wed, 14 Apr 2021 20:58:23 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Wed, 14 Apr 2021 20:58:23 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Wed, 14 Apr 2021 20:58:30 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		CFLAGS+="-Wno-address-of-packed-member" 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 20:58:30 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 20:58:31 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:58:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 20:58:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:58:32 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:27efec644c4207cbc4d1400f84f3402937aab5ce72489976148896e42a219820`  
		Last Modified: Wed, 14 Apr 2021 18:42:24 GMT  
		Size: 2.6 MB (2568428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:503f90387c77c1fc4e68bce67a06e9978c31073dcd4b85bee26367e674a81ed6`  
		Last Modified: Wed, 14 Apr 2021 20:59:51 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96e6b091ead06382abb37e2abbeece360efd0852a51879cc0e4441fbc71098c`  
		Last Modified: Wed, 14 Apr 2021 20:59:51 GMT  
		Size: 775.9 KB (775873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4daef8fbb6977ed6b49701e632cb5b37068aa45dd9621be67a736312baecd497`  
		Last Modified: Wed, 14 Apr 2021 20:59:51 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5977f2b11c8ff7c4155255f370678747c2f168f780e827e4eb223ce50f9dd965`  
		Last Modified: Wed, 14 Apr 2021 20:59:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:1.8`

```console
$ docker pull haproxy@sha256:c120c1d508d6d97bce60635a113b299bdc4cea14897408bfb32da2ff77f79400
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

### `haproxy:1.8` - linux; amd64

```console
$ docker pull haproxy@sha256:5ea71e4401be9229cbb64c367153abae5b291ee63ddc116f54f8804c326846f1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33793586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57267c9e0fc6faa959f1c379fd6f43c157dcf5df05a7e733176d6d18c57ba168`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:29:42 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 12 Apr 2021 22:20:16 GMT
ENV HAPROXY_VERSION=1.8.30
# Mon, 12 Apr 2021 22:20:16 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Mon, 12 Apr 2021 22:20:16 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Mon, 12 Apr 2021 22:20:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Mon, 12 Apr 2021 22:20:50 GMT
STOPSIGNAL SIGUSR1
# Mon, 12 Apr 2021 22:20:50 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 12 Apr 2021 22:20:51 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 12 Apr 2021 22:20:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Apr 2021 22:20:51 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7abf58d954de379f38a19e07330116ba6b11f21007bc7b7507d233e5b0aa3fe0`  
		Last Modified: Sat, 10 Apr 2021 06:38:07 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b667322505008b9b3452b9dc08d4d010f0acea88e148e8dca4b95bb70f0167ce`  
		Last Modified: Mon, 12 Apr 2021 22:22:28 GMT  
		Size: 6.7 MB (6652262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84c2398d176f0cba05a6ec1c4c5fd55bdbaca582cf5e82c569a3150132058e34`  
		Last Modified: Mon, 12 Apr 2021 22:22:28 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03c4e381f91145e1093fabdc4060fbfad78a1ad56180329ece813ae23b30efcf`  
		Last Modified: Mon, 12 Apr 2021 22:22:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:b8fc5ae57045196899be33ef83760cc1e3f6243383e70962f060eb66ee518880
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.1 MB (31106447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e01f566f18996f57a4898253fda10e816dd3a16ade6b04e985f867a22654b760`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:51:31 GMT
ADD file:926533a23a69aa2481a9122b667bb6300a347154eea366c9e679a230aa7f373a in / 
# Sat, 10 Apr 2021 00:51:34 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 02:24:17 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 12 Apr 2021 22:49:00 GMT
ENV HAPROXY_VERSION=1.8.30
# Mon, 12 Apr 2021 22:49:02 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Mon, 12 Apr 2021 22:49:03 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Mon, 12 Apr 2021 22:50:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Mon, 12 Apr 2021 22:50:18 GMT
STOPSIGNAL SIGUSR1
# Mon, 12 Apr 2021 22:50:24 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 12 Apr 2021 22:50:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 12 Apr 2021 22:50:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Apr 2021 22:50:44 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:33d77752597b664d047cc829e58a223d6fb077b61f69ca0462fcfb9b78d5f69b`  
		Last Modified: Sat, 10 Apr 2021 00:59:22 GMT  
		Size: 24.9 MB (24873199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c107a5973e1ce17cb311e2bf8a0d841875ca9f02219922ca12a9203602b5ce`  
		Last Modified: Sat, 10 Apr 2021 02:36:55 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9030f3be5f39c72490cc990ecc965846dba131ebfb6f03f76b609a5fc08ee776`  
		Last Modified: Mon, 12 Apr 2021 22:51:28 GMT  
		Size: 6.2 MB (6231299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f547bf6b62369b6927547cdc62ac016a7263e5497cccd1937089407d56c51352`  
		Last Modified: Mon, 12 Apr 2021 22:51:27 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59e6db2c56955f9aa3660c1d36425ba71abc7d4527d41aae93940921b0d35205`  
		Last Modified: Mon, 12 Apr 2021 22:51:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:84175a6b76f6d746ba2d78921e743b23b4d14268ee46bb235aa42749434bac78
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.8 MB (28812643 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb85ee015a6c189915d7cfb15a2f245bddb2918a5acd5d8c86651974d7953cc0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:59:45 GMT
ADD file:3fbd246a2de82566bcaaf62e3e0bf57175a7ad46b4156366a110661b31eab240 in / 
# Sat, 10 Apr 2021 00:59:47 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 08:58:51 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 12 Apr 2021 22:00:58 GMT
ENV HAPROXY_VERSION=1.8.30
# Mon, 12 Apr 2021 22:00:59 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Mon, 12 Apr 2021 22:01:01 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Mon, 12 Apr 2021 22:01:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Mon, 12 Apr 2021 22:01:51 GMT
STOPSIGNAL SIGUSR1
# Mon, 12 Apr 2021 22:01:56 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 12 Apr 2021 22:02:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 12 Apr 2021 22:02:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Apr 2021 22:02:12 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:8c6bea184b33030fb923c3c09d634b73235dec3fe2d411db9fd22bda669f2c37`  
		Last Modified: Sat, 10 Apr 2021 01:07:51 GMT  
		Size: 22.7 MB (22739801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5be95d3afdef3cc4c8a37695b513cf41e6cf6ffeecd9ce2426d38cb245a0b52`  
		Last Modified: Sat, 10 Apr 2021 09:05:25 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:725ad5d8dd918e8532c3890d2ef57488b4831dd9389b393536e9f7b722dcf5cf`  
		Last Modified: Mon, 12 Apr 2021 22:05:16 GMT  
		Size: 6.1 MB (6070895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc6e81f055b117b3b27eedfdf47340cede1e527b7c03868a7917f02f6ed94b6`  
		Last Modified: Mon, 12 Apr 2021 22:05:15 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32ea2f0dd426d02247634df0a6b803a91550f5b144172d0b010b3875d496aee7`  
		Last Modified: Mon, 12 Apr 2021 22:05:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:f5b1a12b5b4d7676285a835e24b01ef423e0c048454217f9cbb6a9a7359a645b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.4 MB (32360427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:605480cbdb882ec156da749efb3b428d9f1975474dbe20bbcdaa05da09fed67f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:41:25 GMT
ADD file:b24da7eb23eeae04e00d0e45da29a89fe8f992e8dcf4ba482afb907b8015b7bf in / 
# Sat, 10 Apr 2021 00:41:28 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:13:29 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 12 Apr 2021 22:40:50 GMT
ENV HAPROXY_VERSION=1.8.30
# Mon, 12 Apr 2021 22:40:51 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Mon, 12 Apr 2021 22:40:51 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Mon, 12 Apr 2021 22:41:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Mon, 12 Apr 2021 22:41:32 GMT
STOPSIGNAL SIGUSR1
# Mon, 12 Apr 2021 22:41:33 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 12 Apr 2021 22:41:35 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 12 Apr 2021 22:41:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Apr 2021 22:41:37 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:15cb40b9c4df1a06940dc2a154c3be46844241235c1a091afa70da0ee2dc811a`  
		Last Modified: Sat, 10 Apr 2021 00:47:53 GMT  
		Size: 25.9 MB (25904582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48cb832c3e00ffed789c3f464caa612fe4996ba4683f72f8cf214d1437268efe`  
		Last Modified: Sat, 10 Apr 2021 01:21:27 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bba01495936d86289c927e09d502df955477291815cc2aa6f448ec8e7464575e`  
		Last Modified: Mon, 12 Apr 2021 22:43:15 GMT  
		Size: 6.5 MB (6453893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5edaff3b6f2dc63c064ca9ac01f2f399d6699d549e16ae0793ac42fa6fecbd49`  
		Last Modified: Mon, 12 Apr 2021 22:43:13 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5618ccca8ff74e814a05fce7cf09e5cf1bd8c1b5145c762101940425c274fb93`  
		Last Modified: Mon, 12 Apr 2021 22:43:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8` - linux; 386

```console
$ docker pull haproxy@sha256:c7f598d349aaadda127cbe55f4cad546e9f00962a1ba670343004956dc7d2b7e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.4 MB (34367791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cf5db52029c5d54340ba21b02b2563cb7f09dd6c9fd0cb3ab418f7f8f5d1865`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:39:42 GMT
ADD file:8885d4d13678543780bb04ba14b621179665f7951d5b261036a7092df9b376e7 in / 
# Sat, 10 Apr 2021 00:39:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 03:48:12 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 12 Apr 2021 22:39:18 GMT
ENV HAPROXY_VERSION=1.8.30
# Mon, 12 Apr 2021 22:39:18 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Mon, 12 Apr 2021 22:39:18 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Mon, 12 Apr 2021 22:39:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Mon, 12 Apr 2021 22:39:57 GMT
STOPSIGNAL SIGUSR1
# Mon, 12 Apr 2021 22:39:57 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 12 Apr 2021 22:39:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 12 Apr 2021 22:39:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Apr 2021 22:39:58 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:7cc57a8772e5e479618650dfa70f315b474d3f205d04bde7f602f469c1928d84`  
		Last Modified: Sat, 10 Apr 2021 00:46:07 GMT  
		Size: 27.8 MB (27788987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d92d68a52363235dcdfb59fa81e5ef1a4561c958501e4f28d6b79e86f8b8501`  
		Last Modified: Sat, 10 Apr 2021 03:59:08 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4532cf15fde647b5481d5d63ea8f2fb9a4e0a14deb2d0598531818af43c22314`  
		Last Modified: Mon, 12 Apr 2021 22:42:23 GMT  
		Size: 6.6 MB (6576860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4040138c90d0d0a05d08777bd428f6553be97d80b702f7f94e3ea521e9445350`  
		Last Modified: Mon, 12 Apr 2021 22:42:21 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:589113edc7aa8b025e96d8d16e0dbf90a2d486dfb2a5de9b6d81bef822094584`  
		Last Modified: Mon, 12 Apr 2021 22:42:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8` - linux; mips64le

```console
$ docker pull haproxy@sha256:27ebcf5855ca6783601fc38a2318aa72fb59c584fff4858d0eb5a3dbc99ae42f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.0 MB (31951797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:add5893ad5d9f1cb9888d452af266837a1dbe69193937b924b9f4c8ffb6af899`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:09:40 GMT
ADD file:0c93801c4a3719dfd4c047d7f2f4d52bf463eba2ab875da1dc54dcc832aae20b in / 
# Sat, 10 Apr 2021 01:09:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:39:36 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 12 Apr 2021 22:07:35 GMT
ENV HAPROXY_VERSION=1.8.30
# Mon, 12 Apr 2021 22:07:36 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Mon, 12 Apr 2021 22:07:36 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Mon, 12 Apr 2021 22:09:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Mon, 12 Apr 2021 22:09:20 GMT
STOPSIGNAL SIGUSR1
# Mon, 12 Apr 2021 22:09:20 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 12 Apr 2021 22:09:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 12 Apr 2021 22:09:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Apr 2021 22:09:22 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:09ea659ba566d9c3c62493e5ae0b964f1eee4fcf35aabc91c5c34ca1ad686541`  
		Last Modified: Sat, 10 Apr 2021 01:16:07 GMT  
		Size: 25.8 MB (25806410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10fa5ae1be1fc686c91c15f24ebaaa72d7c4f64321c8ead8386f2f4f9d1a6705`  
		Last Modified: Sat, 10 Apr 2021 01:53:41 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff4240067839d4a5495fc4faf3f193798070234386317bff32dd819dfeab3d7`  
		Last Modified: Mon, 12 Apr 2021 22:09:54 GMT  
		Size: 6.1 MB (6143436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12237aa56599bb94bf4d672fbd0dfbabd29cf16284a8de637f9e7ebf3d33add`  
		Last Modified: Mon, 12 Apr 2021 22:09:50 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c58312012b2364d1652091380def0d1a8a3d768622d34c48fad51154e35844e`  
		Last Modified: Mon, 12 Apr 2021 22:09:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8` - linux; ppc64le

```console
$ docker pull haproxy@sha256:277e39dfdae79fd68bd061821b72cf85a85e2c6f16d4f1d409e91333360aecf3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.5 MB (37491401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75ec75eabe828ca979107b523fc9a76da2af1d6fc8dc4ed468082503d8740341`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:26:49 GMT
ADD file:ab87d4854aa8628ce8f4e603c0496499f6f28c3d2525ace782c7369691dafc8c in / 
# Sat, 10 Apr 2021 01:26:56 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 04:45:12 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 12 Apr 2021 22:19:42 GMT
ENV HAPROXY_VERSION=1.8.30
# Mon, 12 Apr 2021 22:19:48 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Mon, 12 Apr 2021 22:19:52 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Mon, 12 Apr 2021 22:24:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Mon, 12 Apr 2021 22:24:51 GMT
STOPSIGNAL SIGUSR1
# Mon, 12 Apr 2021 22:24:57 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 12 Apr 2021 22:25:15 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 12 Apr 2021 22:25:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Apr 2021 22:25:25 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:3e1e599482ca47095f85e429b346b76375aa85015ddcca050e85c2a8b1fdda9c`  
		Last Modified: Sat, 10 Apr 2021 01:33:57 GMT  
		Size: 30.5 MB (30545933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ee41bdc57145d3cb6e9f5fa23eed213567ae52835c7cff5fd57fe17b52f5ec`  
		Last Modified: Sat, 10 Apr 2021 05:09:50 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f194358be9283e1adaf43a0b49c02bfe870d305c2c2e3625fe80c839ade157`  
		Last Modified: Mon, 12 Apr 2021 22:28:12 GMT  
		Size: 6.9 MB (6943509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46d4a9a7b87d1cbf94f89c84564f1c9bb2509ff5c25dc7d7871850bd0e35fa1`  
		Last Modified: Mon, 12 Apr 2021 22:28:10 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09192951aaf9c4f770653674a6f660fcd69611664059ef3f2fa0f8c16c65d53e`  
		Last Modified: Mon, 12 Apr 2021 22:28:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8` - linux; s390x

```console
$ docker pull haproxy@sha256:247cb53b74bd003d43665b085bbf679aee82f94891962e56beeb5892def5c9b6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.0 MB (31988460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edc661c1b1c2e46c8296d4761697b40cdf1754a9528e3ce82091917cdbe9485d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:42:23 GMT
ADD file:dbe2182f8699f2a6011413ea01862e6c0e85853d922dffd72a28d994d23c79bc in / 
# Sat, 10 Apr 2021 00:42:25 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:38:04 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 12 Apr 2021 22:47:28 GMT
ENV HAPROXY_VERSION=1.8.30
# Mon, 12 Apr 2021 22:47:28 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Mon, 12 Apr 2021 22:47:29 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Mon, 12 Apr 2021 22:47:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Mon, 12 Apr 2021 22:47:59 GMT
STOPSIGNAL SIGUSR1
# Mon, 12 Apr 2021 22:47:59 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 12 Apr 2021 22:48:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 12 Apr 2021 22:48:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Apr 2021 22:48:01 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:65291f8717b3afd99b63cee867dd3e06b956a8ee6aa8580cc31d913b25de209d`  
		Last Modified: Sat, 10 Apr 2021 00:45:48 GMT  
		Size: 25.8 MB (25753787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9daf67acfb0373e31068762d068f1da8d320f2bdcdb0e6651d52b8183ede06c`  
		Last Modified: Sat, 10 Apr 2021 01:42:28 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5909c3cbb24edcbac441f845c2933df3a924c1d59943f62c268394be5e5abab7`  
		Last Modified: Mon, 12 Apr 2021 22:49:29 GMT  
		Size: 6.2 MB (6232726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9213e443eef0729746de2a37d5c116056f86f5365f92b6a3db7053b8b0f5371e`  
		Last Modified: Mon, 12 Apr 2021 22:49:27 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d63c467dec1dd0899a1841da8c284fc70df6deaad877747f39b60f7039d4d879`  
		Last Modified: Mon, 12 Apr 2021 22:49:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:1.8-alpine`

```console
$ docker pull haproxy@sha256:5d1a85a38eb463db2594d9656616f50e4ee53083627730bcf4fc3ee80a9f66d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `haproxy:1.8-alpine` - linux; amd64

```console
$ docker pull haproxy@sha256:7aa80be4697ec40c3e1e535eed6efedb3cda0745a025537b6005f556b855eb18
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6786874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:042bd9e2f5ced740c5a1062945a84d581e014d3e271fe9f54282e6b0a418afdd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:37:38 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 21:42:00 GMT
ENV HAPROXY_VERSION=1.8.30
# Wed, 14 Apr 2021 21:42:00 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Wed, 14 Apr 2021 21:42:00 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Wed, 14 Apr 2021 21:42:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 21:42:34 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 21:42:34 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 21:42:35 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 21:42:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 21:42:36 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4de1862a29af271c1751bf0d03d96f9a881f971d1288c5fafcfba90b517611f8`  
		Last Modified: Wed, 14 Apr 2021 21:43:30 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab6375023e0f348eea62623b20ef82a812babd21178df430d46687d68bc129c6`  
		Last Modified: Wed, 14 Apr 2021 21:44:30 GMT  
		Size: 4.0 MB (3973155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:029bec50a8fb11f1c82b058dc2e98961cace08c7fd68e1a545d7bb6d12deb492`  
		Last Modified: Wed, 14 Apr 2021 21:44:31 GMT  
		Size: 445.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:257a96826bac0da4378faf8bc444ae792620d8b85fe75ea46f58eb6c55d427bc`  
		Last Modified: Wed, 14 Apr 2021 21:44:30 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8-alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:0253305b050988db40f500ffaa9e6130d4762cc689cb83961f09f9e26cc38f64
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6471739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17b9a2c135c2a1d0747dea628e3be6b3e2643cb8c447c03c61d3fc98e07e9af3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:18:05 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 21:28:11 GMT
ENV HAPROXY_VERSION=1.8.30
# Wed, 14 Apr 2021 21:28:12 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Wed, 14 Apr 2021 21:28:14 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Wed, 14 Apr 2021 21:28:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 21:28:46 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 21:29:01 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 21:29:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 21:29:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 21:30:11 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd640f0f76e4e434b444a36110041f2c571b2dbcfca29958b2e90de8d91bd6eb`  
		Last Modified: Wed, 14 Apr 2021 21:34:02 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c08b42b69745a8b297f7c992e7e376cdb755d8b414f2241289c2c640b8cc6731`  
		Last Modified: Wed, 14 Apr 2021 21:35:03 GMT  
		Size: 3.8 MB (3847855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40fe2101fa5977961f426845083c7f74ccdc302dc1ebcd90f470a5e208e88938`  
		Last Modified: Wed, 14 Apr 2021 21:35:01 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1957cee54739c883472e9c60c73726857d7f0303e05725492742a1a3ba19dab2`  
		Last Modified: Wed, 14 Apr 2021 21:35:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:aef314c44d55e41227055ab9b734e2c66f4ff5138bd7644bca5eb5a2b3c59e79
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 MB (6211353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:548b3f8684dd29066ac500d8dbc0f4850715b628dbb1b5ae1d60aaee51345ae7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:47:58 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 22:54:11 GMT
ENV HAPROXY_VERSION=1.8.30
# Wed, 14 Apr 2021 22:54:12 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Wed, 14 Apr 2021 22:54:13 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Wed, 14 Apr 2021 22:54:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 22:54:37 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 22:54:38 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 22:54:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 22:54:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 22:54:46 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ff0f6ee9305bed375c784c12ad4beeac3af6ea1a6b5afeec6b4700259dc194`  
		Last Modified: Wed, 14 Apr 2021 22:56:09 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f10694e95296b12e5159135f1f4efef8bf2c2f7e4bcf17ff596f5f88a385fec`  
		Last Modified: Wed, 14 Apr 2021 22:57:01 GMT  
		Size: 3.8 MB (3785450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58df2c3b524ab440288a20098d50660f1f0bd532787b1a10d0a2c3285976383c`  
		Last Modified: Wed, 14 Apr 2021 22:56:59 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f37c6744cfbb6cfb94fee7e72bff212be2778e68c07268758c1f9f8d0ddc527c`  
		Last Modified: Wed, 14 Apr 2021 22:56:59 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:3921a77ac227a8681b27b5fc48dfbcbf57f9e3b8996ae224b85fb86e07a4f3d3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6645020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99710686127b677776cd6849e5b7ec4fc26282e95137636889c79ccae98a84ab`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:26:01 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 20:34:54 GMT
ENV HAPROXY_VERSION=1.8.30
# Wed, 14 Apr 2021 20:34:55 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Wed, 14 Apr 2021 20:34:57 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Wed, 14 Apr 2021 20:35:24 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 20:35:25 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 20:35:26 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:35:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 20:35:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:35:31 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2ef9646f93509fb43536690b645509d9b653316324583761dd086b8ad6c664`  
		Last Modified: Wed, 14 Apr 2021 20:37:52 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21b3ae94ed2da9c08ac1e69329f5284433b7374a3b78e8ccd58ce7e0f8544829`  
		Last Modified: Wed, 14 Apr 2021 20:38:50 GMT  
		Size: 3.9 MB (3931238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bbfe4e7edcaf4c88aee816d8229edb7c109bbe84fc5337b2e14b3e9459299f6`  
		Last Modified: Wed, 14 Apr 2021 20:38:49 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48c1a36a47cc60896c34de29d11a9a2a9bda14794861b76a6e488a1d8ed343d`  
		Last Modified: Wed, 14 Apr 2021 20:38:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8-alpine` - linux; 386

```console
$ docker pull haproxy@sha256:cf2e4440e19ad869ca510ddb8849eeb04e571585f3b27b707f62f712d0b40df4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6707120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:faa5490725f0af14fe8e63805162e99ef10113bc75b920ab812ed002e133e8f4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 01:50:06 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 15 Apr 2021 01:57:04 GMT
ENV HAPROXY_VERSION=1.8.30
# Thu, 15 Apr 2021 01:57:04 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Thu, 15 Apr 2021 01:57:05 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Thu, 15 Apr 2021 01:58:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 15 Apr 2021 01:58:09 GMT
STOPSIGNAL SIGUSR1
# Thu, 15 Apr 2021 01:58:10 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 15 Apr 2021 01:58:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 15 Apr 2021 01:58:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Apr 2021 01:58:12 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:31b7e7ccca9e17fd08b39c9a4ffd3ded380b62816c489d6c3758c9bb5a632430`  
		Last Modified: Wed, 14 Apr 2021 18:39:24 GMT  
		Size: 2.8 MB (2818900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9104145d2a6b1e0c0837c464bb9d4b331949cfeb6be12e4e7995507661d3386`  
		Last Modified: Thu, 15 Apr 2021 02:00:28 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d41fd64114c3510ddd0edfc27a481a7bdf2480b44496ff032c0fc4afa83c12a`  
		Last Modified: Thu, 15 Apr 2021 02:01:45 GMT  
		Size: 3.9 MB (3886465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:975ac82af1bac203e360a6e37bf354ea4bdf1e84ccc014d7e30c79c21a5c7583`  
		Last Modified: Thu, 15 Apr 2021 02:01:44 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a985c4285f8a13dada006c384bc9153fff675282e5ef96aea12a9940f6c8a0`  
		Last Modified: Thu, 15 Apr 2021 02:01:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8-alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:bf12aefc31f9ed2878030aa1629ffa34e02e5c4d97afb9fdb2667e91da4a8204
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (6951374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0ca09d8b283cccac8124706402486c91c5bffa4264086f1c15d3b1e62592936`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:25:09 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 23:33:06 GMT
ENV HAPROXY_VERSION=1.8.30
# Wed, 14 Apr 2021 23:33:13 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Wed, 14 Apr 2021 23:33:24 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Wed, 14 Apr 2021 23:34:02 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 23:34:11 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 23:34:14 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 23:34:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 23:34:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 23:34:30 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8004273856b1b354059d03a17deec6e79d325ba45d63213dda3d1fa401db8c22`  
		Last Modified: Wed, 14 Apr 2021 23:36:37 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29d12aa95cda61bd069b8b5ab6d273c7159c71153b8ca8f049babc1229db3eeb`  
		Last Modified: Wed, 14 Apr 2021 23:37:39 GMT  
		Size: 4.1 MB (4136478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd52fe809bdc90dce59aaec8b8c453ba7bccbfc54625a51c7d6e42b51920ae49`  
		Last Modified: Wed, 14 Apr 2021 23:37:38 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c1afd74200421d906e566ec8a82109556b90b147e142f3dc7916b5b6a3751e5`  
		Last Modified: Wed, 14 Apr 2021 23:37:38 GMT  
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
$ docker pull haproxy@sha256:c120c1d508d6d97bce60635a113b299bdc4cea14897408bfb32da2ff77f79400
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

### `haproxy:1.8.30` - linux; amd64

```console
$ docker pull haproxy@sha256:5ea71e4401be9229cbb64c367153abae5b291ee63ddc116f54f8804c326846f1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33793586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57267c9e0fc6faa959f1c379fd6f43c157dcf5df05a7e733176d6d18c57ba168`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:29:42 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 12 Apr 2021 22:20:16 GMT
ENV HAPROXY_VERSION=1.8.30
# Mon, 12 Apr 2021 22:20:16 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Mon, 12 Apr 2021 22:20:16 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Mon, 12 Apr 2021 22:20:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Mon, 12 Apr 2021 22:20:50 GMT
STOPSIGNAL SIGUSR1
# Mon, 12 Apr 2021 22:20:50 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 12 Apr 2021 22:20:51 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 12 Apr 2021 22:20:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Apr 2021 22:20:51 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7abf58d954de379f38a19e07330116ba6b11f21007bc7b7507d233e5b0aa3fe0`  
		Last Modified: Sat, 10 Apr 2021 06:38:07 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b667322505008b9b3452b9dc08d4d010f0acea88e148e8dca4b95bb70f0167ce`  
		Last Modified: Mon, 12 Apr 2021 22:22:28 GMT  
		Size: 6.7 MB (6652262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84c2398d176f0cba05a6ec1c4c5fd55bdbaca582cf5e82c569a3150132058e34`  
		Last Modified: Mon, 12 Apr 2021 22:22:28 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03c4e381f91145e1093fabdc4060fbfad78a1ad56180329ece813ae23b30efcf`  
		Last Modified: Mon, 12 Apr 2021 22:22:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8.30` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:b8fc5ae57045196899be33ef83760cc1e3f6243383e70962f060eb66ee518880
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.1 MB (31106447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e01f566f18996f57a4898253fda10e816dd3a16ade6b04e985f867a22654b760`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:51:31 GMT
ADD file:926533a23a69aa2481a9122b667bb6300a347154eea366c9e679a230aa7f373a in / 
# Sat, 10 Apr 2021 00:51:34 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 02:24:17 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 12 Apr 2021 22:49:00 GMT
ENV HAPROXY_VERSION=1.8.30
# Mon, 12 Apr 2021 22:49:02 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Mon, 12 Apr 2021 22:49:03 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Mon, 12 Apr 2021 22:50:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Mon, 12 Apr 2021 22:50:18 GMT
STOPSIGNAL SIGUSR1
# Mon, 12 Apr 2021 22:50:24 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 12 Apr 2021 22:50:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 12 Apr 2021 22:50:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Apr 2021 22:50:44 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:33d77752597b664d047cc829e58a223d6fb077b61f69ca0462fcfb9b78d5f69b`  
		Last Modified: Sat, 10 Apr 2021 00:59:22 GMT  
		Size: 24.9 MB (24873199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c107a5973e1ce17cb311e2bf8a0d841875ca9f02219922ca12a9203602b5ce`  
		Last Modified: Sat, 10 Apr 2021 02:36:55 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9030f3be5f39c72490cc990ecc965846dba131ebfb6f03f76b609a5fc08ee776`  
		Last Modified: Mon, 12 Apr 2021 22:51:28 GMT  
		Size: 6.2 MB (6231299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f547bf6b62369b6927547cdc62ac016a7263e5497cccd1937089407d56c51352`  
		Last Modified: Mon, 12 Apr 2021 22:51:27 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59e6db2c56955f9aa3660c1d36425ba71abc7d4527d41aae93940921b0d35205`  
		Last Modified: Mon, 12 Apr 2021 22:51:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8.30` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:84175a6b76f6d746ba2d78921e743b23b4d14268ee46bb235aa42749434bac78
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.8 MB (28812643 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb85ee015a6c189915d7cfb15a2f245bddb2918a5acd5d8c86651974d7953cc0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:59:45 GMT
ADD file:3fbd246a2de82566bcaaf62e3e0bf57175a7ad46b4156366a110661b31eab240 in / 
# Sat, 10 Apr 2021 00:59:47 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 08:58:51 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 12 Apr 2021 22:00:58 GMT
ENV HAPROXY_VERSION=1.8.30
# Mon, 12 Apr 2021 22:00:59 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Mon, 12 Apr 2021 22:01:01 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Mon, 12 Apr 2021 22:01:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Mon, 12 Apr 2021 22:01:51 GMT
STOPSIGNAL SIGUSR1
# Mon, 12 Apr 2021 22:01:56 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 12 Apr 2021 22:02:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 12 Apr 2021 22:02:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Apr 2021 22:02:12 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:8c6bea184b33030fb923c3c09d634b73235dec3fe2d411db9fd22bda669f2c37`  
		Last Modified: Sat, 10 Apr 2021 01:07:51 GMT  
		Size: 22.7 MB (22739801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5be95d3afdef3cc4c8a37695b513cf41e6cf6ffeecd9ce2426d38cb245a0b52`  
		Last Modified: Sat, 10 Apr 2021 09:05:25 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:725ad5d8dd918e8532c3890d2ef57488b4831dd9389b393536e9f7b722dcf5cf`  
		Last Modified: Mon, 12 Apr 2021 22:05:16 GMT  
		Size: 6.1 MB (6070895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc6e81f055b117b3b27eedfdf47340cede1e527b7c03868a7917f02f6ed94b6`  
		Last Modified: Mon, 12 Apr 2021 22:05:15 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32ea2f0dd426d02247634df0a6b803a91550f5b144172d0b010b3875d496aee7`  
		Last Modified: Mon, 12 Apr 2021 22:05:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8.30` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:f5b1a12b5b4d7676285a835e24b01ef423e0c048454217f9cbb6a9a7359a645b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.4 MB (32360427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:605480cbdb882ec156da749efb3b428d9f1975474dbe20bbcdaa05da09fed67f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:41:25 GMT
ADD file:b24da7eb23eeae04e00d0e45da29a89fe8f992e8dcf4ba482afb907b8015b7bf in / 
# Sat, 10 Apr 2021 00:41:28 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:13:29 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 12 Apr 2021 22:40:50 GMT
ENV HAPROXY_VERSION=1.8.30
# Mon, 12 Apr 2021 22:40:51 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Mon, 12 Apr 2021 22:40:51 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Mon, 12 Apr 2021 22:41:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Mon, 12 Apr 2021 22:41:32 GMT
STOPSIGNAL SIGUSR1
# Mon, 12 Apr 2021 22:41:33 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 12 Apr 2021 22:41:35 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 12 Apr 2021 22:41:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Apr 2021 22:41:37 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:15cb40b9c4df1a06940dc2a154c3be46844241235c1a091afa70da0ee2dc811a`  
		Last Modified: Sat, 10 Apr 2021 00:47:53 GMT  
		Size: 25.9 MB (25904582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48cb832c3e00ffed789c3f464caa612fe4996ba4683f72f8cf214d1437268efe`  
		Last Modified: Sat, 10 Apr 2021 01:21:27 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bba01495936d86289c927e09d502df955477291815cc2aa6f448ec8e7464575e`  
		Last Modified: Mon, 12 Apr 2021 22:43:15 GMT  
		Size: 6.5 MB (6453893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5edaff3b6f2dc63c064ca9ac01f2f399d6699d549e16ae0793ac42fa6fecbd49`  
		Last Modified: Mon, 12 Apr 2021 22:43:13 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5618ccca8ff74e814a05fce7cf09e5cf1bd8c1b5145c762101940425c274fb93`  
		Last Modified: Mon, 12 Apr 2021 22:43:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8.30` - linux; 386

```console
$ docker pull haproxy@sha256:c7f598d349aaadda127cbe55f4cad546e9f00962a1ba670343004956dc7d2b7e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.4 MB (34367791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cf5db52029c5d54340ba21b02b2563cb7f09dd6c9fd0cb3ab418f7f8f5d1865`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:39:42 GMT
ADD file:8885d4d13678543780bb04ba14b621179665f7951d5b261036a7092df9b376e7 in / 
# Sat, 10 Apr 2021 00:39:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 03:48:12 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 12 Apr 2021 22:39:18 GMT
ENV HAPROXY_VERSION=1.8.30
# Mon, 12 Apr 2021 22:39:18 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Mon, 12 Apr 2021 22:39:18 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Mon, 12 Apr 2021 22:39:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Mon, 12 Apr 2021 22:39:57 GMT
STOPSIGNAL SIGUSR1
# Mon, 12 Apr 2021 22:39:57 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 12 Apr 2021 22:39:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 12 Apr 2021 22:39:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Apr 2021 22:39:58 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:7cc57a8772e5e479618650dfa70f315b474d3f205d04bde7f602f469c1928d84`  
		Last Modified: Sat, 10 Apr 2021 00:46:07 GMT  
		Size: 27.8 MB (27788987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d92d68a52363235dcdfb59fa81e5ef1a4561c958501e4f28d6b79e86f8b8501`  
		Last Modified: Sat, 10 Apr 2021 03:59:08 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4532cf15fde647b5481d5d63ea8f2fb9a4e0a14deb2d0598531818af43c22314`  
		Last Modified: Mon, 12 Apr 2021 22:42:23 GMT  
		Size: 6.6 MB (6576860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4040138c90d0d0a05d08777bd428f6553be97d80b702f7f94e3ea521e9445350`  
		Last Modified: Mon, 12 Apr 2021 22:42:21 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:589113edc7aa8b025e96d8d16e0dbf90a2d486dfb2a5de9b6d81bef822094584`  
		Last Modified: Mon, 12 Apr 2021 22:42:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8.30` - linux; mips64le

```console
$ docker pull haproxy@sha256:27ebcf5855ca6783601fc38a2318aa72fb59c584fff4858d0eb5a3dbc99ae42f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.0 MB (31951797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:add5893ad5d9f1cb9888d452af266837a1dbe69193937b924b9f4c8ffb6af899`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:09:40 GMT
ADD file:0c93801c4a3719dfd4c047d7f2f4d52bf463eba2ab875da1dc54dcc832aae20b in / 
# Sat, 10 Apr 2021 01:09:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:39:36 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 12 Apr 2021 22:07:35 GMT
ENV HAPROXY_VERSION=1.8.30
# Mon, 12 Apr 2021 22:07:36 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Mon, 12 Apr 2021 22:07:36 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Mon, 12 Apr 2021 22:09:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Mon, 12 Apr 2021 22:09:20 GMT
STOPSIGNAL SIGUSR1
# Mon, 12 Apr 2021 22:09:20 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 12 Apr 2021 22:09:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 12 Apr 2021 22:09:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Apr 2021 22:09:22 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:09ea659ba566d9c3c62493e5ae0b964f1eee4fcf35aabc91c5c34ca1ad686541`  
		Last Modified: Sat, 10 Apr 2021 01:16:07 GMT  
		Size: 25.8 MB (25806410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10fa5ae1be1fc686c91c15f24ebaaa72d7c4f64321c8ead8386f2f4f9d1a6705`  
		Last Modified: Sat, 10 Apr 2021 01:53:41 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff4240067839d4a5495fc4faf3f193798070234386317bff32dd819dfeab3d7`  
		Last Modified: Mon, 12 Apr 2021 22:09:54 GMT  
		Size: 6.1 MB (6143436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12237aa56599bb94bf4d672fbd0dfbabd29cf16284a8de637f9e7ebf3d33add`  
		Last Modified: Mon, 12 Apr 2021 22:09:50 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c58312012b2364d1652091380def0d1a8a3d768622d34c48fad51154e35844e`  
		Last Modified: Mon, 12 Apr 2021 22:09:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8.30` - linux; ppc64le

```console
$ docker pull haproxy@sha256:277e39dfdae79fd68bd061821b72cf85a85e2c6f16d4f1d409e91333360aecf3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.5 MB (37491401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75ec75eabe828ca979107b523fc9a76da2af1d6fc8dc4ed468082503d8740341`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:26:49 GMT
ADD file:ab87d4854aa8628ce8f4e603c0496499f6f28c3d2525ace782c7369691dafc8c in / 
# Sat, 10 Apr 2021 01:26:56 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 04:45:12 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 12 Apr 2021 22:19:42 GMT
ENV HAPROXY_VERSION=1.8.30
# Mon, 12 Apr 2021 22:19:48 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Mon, 12 Apr 2021 22:19:52 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Mon, 12 Apr 2021 22:24:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Mon, 12 Apr 2021 22:24:51 GMT
STOPSIGNAL SIGUSR1
# Mon, 12 Apr 2021 22:24:57 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 12 Apr 2021 22:25:15 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 12 Apr 2021 22:25:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Apr 2021 22:25:25 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:3e1e599482ca47095f85e429b346b76375aa85015ddcca050e85c2a8b1fdda9c`  
		Last Modified: Sat, 10 Apr 2021 01:33:57 GMT  
		Size: 30.5 MB (30545933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ee41bdc57145d3cb6e9f5fa23eed213567ae52835c7cff5fd57fe17b52f5ec`  
		Last Modified: Sat, 10 Apr 2021 05:09:50 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f194358be9283e1adaf43a0b49c02bfe870d305c2c2e3625fe80c839ade157`  
		Last Modified: Mon, 12 Apr 2021 22:28:12 GMT  
		Size: 6.9 MB (6943509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46d4a9a7b87d1cbf94f89c84564f1c9bb2509ff5c25dc7d7871850bd0e35fa1`  
		Last Modified: Mon, 12 Apr 2021 22:28:10 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09192951aaf9c4f770653674a6f660fcd69611664059ef3f2fa0f8c16c65d53e`  
		Last Modified: Mon, 12 Apr 2021 22:28:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8.30` - linux; s390x

```console
$ docker pull haproxy@sha256:247cb53b74bd003d43665b085bbf679aee82f94891962e56beeb5892def5c9b6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.0 MB (31988460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edc661c1b1c2e46c8296d4761697b40cdf1754a9528e3ce82091917cdbe9485d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:42:23 GMT
ADD file:dbe2182f8699f2a6011413ea01862e6c0e85853d922dffd72a28d994d23c79bc in / 
# Sat, 10 Apr 2021 00:42:25 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:38:04 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 12 Apr 2021 22:47:28 GMT
ENV HAPROXY_VERSION=1.8.30
# Mon, 12 Apr 2021 22:47:28 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Mon, 12 Apr 2021 22:47:29 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Mon, 12 Apr 2021 22:47:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Mon, 12 Apr 2021 22:47:59 GMT
STOPSIGNAL SIGUSR1
# Mon, 12 Apr 2021 22:47:59 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 12 Apr 2021 22:48:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 12 Apr 2021 22:48:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Apr 2021 22:48:01 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:65291f8717b3afd99b63cee867dd3e06b956a8ee6aa8580cc31d913b25de209d`  
		Last Modified: Sat, 10 Apr 2021 00:45:48 GMT  
		Size: 25.8 MB (25753787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9daf67acfb0373e31068762d068f1da8d320f2bdcdb0e6651d52b8183ede06c`  
		Last Modified: Sat, 10 Apr 2021 01:42:28 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5909c3cbb24edcbac441f845c2933df3a924c1d59943f62c268394be5e5abab7`  
		Last Modified: Mon, 12 Apr 2021 22:49:29 GMT  
		Size: 6.2 MB (6232726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9213e443eef0729746de2a37d5c116056f86f5365f92b6a3db7053b8b0f5371e`  
		Last Modified: Mon, 12 Apr 2021 22:49:27 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d63c467dec1dd0899a1841da8c284fc70df6deaad877747f39b60f7039d4d879`  
		Last Modified: Mon, 12 Apr 2021 22:49:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:1.8.30-alpine`

```console
$ docker pull haproxy@sha256:5d1a85a38eb463db2594d9656616f50e4ee53083627730bcf4fc3ee80a9f66d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `haproxy:1.8.30-alpine` - linux; amd64

```console
$ docker pull haproxy@sha256:7aa80be4697ec40c3e1e535eed6efedb3cda0745a025537b6005f556b855eb18
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6786874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:042bd9e2f5ced740c5a1062945a84d581e014d3e271fe9f54282e6b0a418afdd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:37:38 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 21:42:00 GMT
ENV HAPROXY_VERSION=1.8.30
# Wed, 14 Apr 2021 21:42:00 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Wed, 14 Apr 2021 21:42:00 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Wed, 14 Apr 2021 21:42:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 21:42:34 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 21:42:34 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 21:42:35 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 21:42:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 21:42:36 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4de1862a29af271c1751bf0d03d96f9a881f971d1288c5fafcfba90b517611f8`  
		Last Modified: Wed, 14 Apr 2021 21:43:30 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab6375023e0f348eea62623b20ef82a812babd21178df430d46687d68bc129c6`  
		Last Modified: Wed, 14 Apr 2021 21:44:30 GMT  
		Size: 4.0 MB (3973155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:029bec50a8fb11f1c82b058dc2e98961cace08c7fd68e1a545d7bb6d12deb492`  
		Last Modified: Wed, 14 Apr 2021 21:44:31 GMT  
		Size: 445.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:257a96826bac0da4378faf8bc444ae792620d8b85fe75ea46f58eb6c55d427bc`  
		Last Modified: Wed, 14 Apr 2021 21:44:30 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8.30-alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:0253305b050988db40f500ffaa9e6130d4762cc689cb83961f09f9e26cc38f64
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6471739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17b9a2c135c2a1d0747dea628e3be6b3e2643cb8c447c03c61d3fc98e07e9af3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:18:05 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 21:28:11 GMT
ENV HAPROXY_VERSION=1.8.30
# Wed, 14 Apr 2021 21:28:12 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Wed, 14 Apr 2021 21:28:14 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Wed, 14 Apr 2021 21:28:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 21:28:46 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 21:29:01 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 21:29:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 21:29:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 21:30:11 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd640f0f76e4e434b444a36110041f2c571b2dbcfca29958b2e90de8d91bd6eb`  
		Last Modified: Wed, 14 Apr 2021 21:34:02 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c08b42b69745a8b297f7c992e7e376cdb755d8b414f2241289c2c640b8cc6731`  
		Last Modified: Wed, 14 Apr 2021 21:35:03 GMT  
		Size: 3.8 MB (3847855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40fe2101fa5977961f426845083c7f74ccdc302dc1ebcd90f470a5e208e88938`  
		Last Modified: Wed, 14 Apr 2021 21:35:01 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1957cee54739c883472e9c60c73726857d7f0303e05725492742a1a3ba19dab2`  
		Last Modified: Wed, 14 Apr 2021 21:35:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8.30-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:aef314c44d55e41227055ab9b734e2c66f4ff5138bd7644bca5eb5a2b3c59e79
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 MB (6211353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:548b3f8684dd29066ac500d8dbc0f4850715b628dbb1b5ae1d60aaee51345ae7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:47:58 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 22:54:11 GMT
ENV HAPROXY_VERSION=1.8.30
# Wed, 14 Apr 2021 22:54:12 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Wed, 14 Apr 2021 22:54:13 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Wed, 14 Apr 2021 22:54:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 22:54:37 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 22:54:38 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 22:54:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 22:54:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 22:54:46 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ff0f6ee9305bed375c784c12ad4beeac3af6ea1a6b5afeec6b4700259dc194`  
		Last Modified: Wed, 14 Apr 2021 22:56:09 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f10694e95296b12e5159135f1f4efef8bf2c2f7e4bcf17ff596f5f88a385fec`  
		Last Modified: Wed, 14 Apr 2021 22:57:01 GMT  
		Size: 3.8 MB (3785450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58df2c3b524ab440288a20098d50660f1f0bd532787b1a10d0a2c3285976383c`  
		Last Modified: Wed, 14 Apr 2021 22:56:59 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f37c6744cfbb6cfb94fee7e72bff212be2778e68c07268758c1f9f8d0ddc527c`  
		Last Modified: Wed, 14 Apr 2021 22:56:59 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8.30-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:3921a77ac227a8681b27b5fc48dfbcbf57f9e3b8996ae224b85fb86e07a4f3d3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6645020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99710686127b677776cd6849e5b7ec4fc26282e95137636889c79ccae98a84ab`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:26:01 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 20:34:54 GMT
ENV HAPROXY_VERSION=1.8.30
# Wed, 14 Apr 2021 20:34:55 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Wed, 14 Apr 2021 20:34:57 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Wed, 14 Apr 2021 20:35:24 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 20:35:25 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 20:35:26 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:35:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 20:35:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:35:31 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2ef9646f93509fb43536690b645509d9b653316324583761dd086b8ad6c664`  
		Last Modified: Wed, 14 Apr 2021 20:37:52 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21b3ae94ed2da9c08ac1e69329f5284433b7374a3b78e8ccd58ce7e0f8544829`  
		Last Modified: Wed, 14 Apr 2021 20:38:50 GMT  
		Size: 3.9 MB (3931238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bbfe4e7edcaf4c88aee816d8229edb7c109bbe84fc5337b2e14b3e9459299f6`  
		Last Modified: Wed, 14 Apr 2021 20:38:49 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48c1a36a47cc60896c34de29d11a9a2a9bda14794861b76a6e488a1d8ed343d`  
		Last Modified: Wed, 14 Apr 2021 20:38:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8.30-alpine` - linux; 386

```console
$ docker pull haproxy@sha256:cf2e4440e19ad869ca510ddb8849eeb04e571585f3b27b707f62f712d0b40df4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6707120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:faa5490725f0af14fe8e63805162e99ef10113bc75b920ab812ed002e133e8f4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 01:50:06 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 15 Apr 2021 01:57:04 GMT
ENV HAPROXY_VERSION=1.8.30
# Thu, 15 Apr 2021 01:57:04 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Thu, 15 Apr 2021 01:57:05 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Thu, 15 Apr 2021 01:58:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 15 Apr 2021 01:58:09 GMT
STOPSIGNAL SIGUSR1
# Thu, 15 Apr 2021 01:58:10 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 15 Apr 2021 01:58:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 15 Apr 2021 01:58:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Apr 2021 01:58:12 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:31b7e7ccca9e17fd08b39c9a4ffd3ded380b62816c489d6c3758c9bb5a632430`  
		Last Modified: Wed, 14 Apr 2021 18:39:24 GMT  
		Size: 2.8 MB (2818900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9104145d2a6b1e0c0837c464bb9d4b331949cfeb6be12e4e7995507661d3386`  
		Last Modified: Thu, 15 Apr 2021 02:00:28 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d41fd64114c3510ddd0edfc27a481a7bdf2480b44496ff032c0fc4afa83c12a`  
		Last Modified: Thu, 15 Apr 2021 02:01:45 GMT  
		Size: 3.9 MB (3886465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:975ac82af1bac203e360a6e37bf354ea4bdf1e84ccc014d7e30c79c21a5c7583`  
		Last Modified: Thu, 15 Apr 2021 02:01:44 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a985c4285f8a13dada006c384bc9153fff675282e5ef96aea12a9940f6c8a0`  
		Last Modified: Thu, 15 Apr 2021 02:01:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8.30-alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:bf12aefc31f9ed2878030aa1629ffa34e02e5c4d97afb9fdb2667e91da4a8204
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (6951374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0ca09d8b283cccac8124706402486c91c5bffa4264086f1c15d3b1e62592936`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:25:09 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 23:33:06 GMT
ENV HAPROXY_VERSION=1.8.30
# Wed, 14 Apr 2021 23:33:13 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Wed, 14 Apr 2021 23:33:24 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Wed, 14 Apr 2021 23:34:02 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 23:34:11 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 23:34:14 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 23:34:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 23:34:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 23:34:30 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8004273856b1b354059d03a17deec6e79d325ba45d63213dda3d1fa401db8c22`  
		Last Modified: Wed, 14 Apr 2021 23:36:37 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29d12aa95cda61bd069b8b5ab6d273c7159c71153b8ca8f049babc1229db3eeb`  
		Last Modified: Wed, 14 Apr 2021 23:37:39 GMT  
		Size: 4.1 MB (4136478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd52fe809bdc90dce59aaec8b8c453ba7bccbfc54625a51c7d6e42b51920ae49`  
		Last Modified: Wed, 14 Apr 2021 23:37:38 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c1afd74200421d906e566ec8a82109556b90b147e142f3dc7916b5b6a3751e5`  
		Last Modified: Wed, 14 Apr 2021 23:37:38 GMT  
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
$ docker pull haproxy@sha256:af6505e38637df55fd060940c9074fb13c86912a328e25d68858a1690c0666e2
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

### `haproxy:2.0` - linux; amd64

```console
$ docker pull haproxy@sha256:d22e335f036e845d78ca259beff5dc007923c2373ff616ced7abb7672d15a32e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.8 MB (35835009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f5c3a5fcaa1312d5c45aa12ea12bf22b6e0c077c9e52bad166e9090c9a4bd9e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:29:42 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 12 Apr 2021 18:24:02 GMT
ENV HAPROXY_VERSION=2.0.22
# Mon, 12 Apr 2021 18:24:02 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.22.tar.gz
# Mon, 12 Apr 2021 18:24:03 GMT
ENV HAPROXY_SHA256=5e1dccf30a3ad782d1e3298cc4e4955b168e4aa06cad4e3ea1c0334cdc0f966d
# Mon, 12 Apr 2021 18:24:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Mon, 12 Apr 2021 18:24:44 GMT
STOPSIGNAL SIGUSR1
# Mon, 12 Apr 2021 18:24:45 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 12 Apr 2021 18:24:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 12 Apr 2021 18:24:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Apr 2021 18:24:46 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7abf58d954de379f38a19e07330116ba6b11f21007bc7b7507d233e5b0aa3fe0`  
		Last Modified: Sat, 10 Apr 2021 06:38:07 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf8559c4cb3b4af093063e24014fc599a99eac125bc8570d6cae1d629f5ce192`  
		Last Modified: Mon, 12 Apr 2021 18:26:40 GMT  
		Size: 8.7 MB (8693686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaeca2e42fc3dcb820dd40afc8dd47921d2f1f602e978d0e750f40207379d9bf`  
		Last Modified: Mon, 12 Apr 2021 18:26:39 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72170a2df5fa1a4b1f379916b866dd38b43e048d76750b8f4411bf79195b2a79`  
		Last Modified: Mon, 12 Apr 2021 18:26:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:3bab5e0ca970574a9a4e27a8fa6a8fe74448a8473d8359394f6957f5032806a5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.1 MB (33050684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:810a0a1beb6b39b3a5588a675af7352b14e25eb0e49822709721726780d07324`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:51:31 GMT
ADD file:926533a23a69aa2481a9122b667bb6300a347154eea366c9e679a230aa7f373a in / 
# Sat, 10 Apr 2021 00:51:34 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 02:24:17 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 12 Apr 2021 17:49:04 GMT
ENV HAPROXY_VERSION=2.0.22
# Mon, 12 Apr 2021 17:49:05 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.22.tar.gz
# Mon, 12 Apr 2021 17:49:06 GMT
ENV HAPROXY_SHA256=5e1dccf30a3ad782d1e3298cc4e4955b168e4aa06cad4e3ea1c0334cdc0f966d
# Mon, 12 Apr 2021 17:50:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Mon, 12 Apr 2021 17:50:02 GMT
STOPSIGNAL SIGUSR1
# Mon, 12 Apr 2021 17:50:03 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 12 Apr 2021 17:50:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 12 Apr 2021 17:50:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Apr 2021 17:50:07 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:33d77752597b664d047cc829e58a223d6fb077b61f69ca0462fcfb9b78d5f69b`  
		Last Modified: Sat, 10 Apr 2021 00:59:22 GMT  
		Size: 24.9 MB (24873199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c107a5973e1ce17cb311e2bf8a0d841875ca9f02219922ca12a9203602b5ce`  
		Last Modified: Sat, 10 Apr 2021 02:36:55 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a695842d5b3a7d715904c56cb979ded99ebeb34e90d9d720643d7c58ca0a12d2`  
		Last Modified: Mon, 12 Apr 2021 17:51:02 GMT  
		Size: 8.2 MB (8175536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df803aacf2d39c82d93ff0cdf3e342bd9a4e66f427cfb462f3ce73bccf8399da`  
		Last Modified: Mon, 12 Apr 2021 17:50:58 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f0cc428a811f53c34336143a7738671989088880f717762cbbd8fcf70e3c204`  
		Last Modified: Mon, 12 Apr 2021 17:50:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:4dae846f887000e2f21e6e2d668ceaf834529b694d489e94ad1edb849b9ec663
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.9 MB (30864631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e7ca95062d20599f7de1a466fa37624953bdb60f497b4e711214f08e3bb3885`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:59:45 GMT
ADD file:3fbd246a2de82566bcaaf62e3e0bf57175a7ad46b4156366a110661b31eab240 in / 
# Sat, 10 Apr 2021 00:59:47 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 08:58:51 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 12 Apr 2021 18:28:47 GMT
ENV HAPROXY_VERSION=2.0.22
# Mon, 12 Apr 2021 18:28:50 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.22.tar.gz
# Mon, 12 Apr 2021 18:28:52 GMT
ENV HAPROXY_SHA256=5e1dccf30a3ad782d1e3298cc4e4955b168e4aa06cad4e3ea1c0334cdc0f966d
# Mon, 12 Apr 2021 18:29:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Mon, 12 Apr 2021 18:29:35 GMT
STOPSIGNAL SIGUSR1
# Mon, 12 Apr 2021 18:29:36 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 12 Apr 2021 18:29:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 12 Apr 2021 18:29:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Apr 2021 18:29:41 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:8c6bea184b33030fb923c3c09d634b73235dec3fe2d411db9fd22bda669f2c37`  
		Last Modified: Sat, 10 Apr 2021 01:07:51 GMT  
		Size: 22.7 MB (22739801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5be95d3afdef3cc4c8a37695b513cf41e6cf6ffeecd9ce2426d38cb245a0b52`  
		Last Modified: Sat, 10 Apr 2021 09:05:25 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d372da4e007019116f4af10321bf34e48dc6c4806ad68fe226cfbb1ec490cd`  
		Last Modified: Mon, 12 Apr 2021 18:32:02 GMT  
		Size: 8.1 MB (8122884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:675402e3f486334baf119c742f454e8e960a48d50b6289a842e35f4cb90fc53b`  
		Last Modified: Mon, 12 Apr 2021 18:31:59 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:881f59bde771a049db45f8a4b14f96c75a105e16485aae148b0a06daa2d1e6df`  
		Last Modified: Mon, 12 Apr 2021 18:31:59 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:d01e95fc2d486bf1d9ffb641597b510198bee08b4eefb1d76193689649bede61
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.4 MB (34437386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b928a7e49b156c8873cce5cc4161c00e4ed02049215ec118a130e7a3e500137`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:41:25 GMT
ADD file:b24da7eb23eeae04e00d0e45da29a89fe8f992e8dcf4ba482afb907b8015b7bf in / 
# Sat, 10 Apr 2021 00:41:28 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:13:29 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 12 Apr 2021 18:18:53 GMT
ENV HAPROXY_VERSION=2.0.22
# Mon, 12 Apr 2021 18:18:56 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.22.tar.gz
# Mon, 12 Apr 2021 18:19:01 GMT
ENV HAPROXY_SHA256=5e1dccf30a3ad782d1e3298cc4e4955b168e4aa06cad4e3ea1c0334cdc0f966d
# Mon, 12 Apr 2021 18:19:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Mon, 12 Apr 2021 18:19:57 GMT
STOPSIGNAL SIGUSR1
# Mon, 12 Apr 2021 18:19:58 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 12 Apr 2021 18:20:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 12 Apr 2021 18:20:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Apr 2021 18:20:10 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:15cb40b9c4df1a06940dc2a154c3be46844241235c1a091afa70da0ee2dc811a`  
		Last Modified: Sat, 10 Apr 2021 00:47:53 GMT  
		Size: 25.9 MB (25904582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48cb832c3e00ffed789c3f464caa612fe4996ba4683f72f8cf214d1437268efe`  
		Last Modified: Sat, 10 Apr 2021 01:21:27 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17c4b35ef5e3d4f8ac9c98e4fc17d434f443113c6f665313fba5f84fceaffe58`  
		Last Modified: Mon, 12 Apr 2021 18:22:22 GMT  
		Size: 8.5 MB (8530854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde0431b3ddbf51fb7e287872dda9a1e535356ea7f6ced0daf5a6b8f924fad2e`  
		Last Modified: Mon, 12 Apr 2021 18:22:19 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc6730a49e57ae9e3973dda6e22b061a7708697635c732a54ab68672a98087d`  
		Last Modified: Mon, 12 Apr 2021 18:22:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0` - linux; 386

```console
$ docker pull haproxy@sha256:9f921067cf03daf25261e0865a0a128860f0b1908b76687689fda3432ac6b399
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36278633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5f30bae29deb98ba66eebdb03b0ca5a490fbefe5902356350a9bce0cdc57489`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:39:42 GMT
ADD file:8885d4d13678543780bb04ba14b621179665f7951d5b261036a7092df9b376e7 in / 
# Sat, 10 Apr 2021 00:39:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 03:48:12 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 12 Apr 2021 17:39:07 GMT
ENV HAPROXY_VERSION=2.0.22
# Mon, 12 Apr 2021 17:39:08 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.22.tar.gz
# Mon, 12 Apr 2021 17:39:08 GMT
ENV HAPROXY_SHA256=5e1dccf30a3ad782d1e3298cc4e4955b168e4aa06cad4e3ea1c0334cdc0f966d
# Mon, 12 Apr 2021 17:39:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Mon, 12 Apr 2021 17:39:55 GMT
STOPSIGNAL SIGUSR1
# Mon, 12 Apr 2021 17:39:55 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 12 Apr 2021 17:39:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 12 Apr 2021 17:39:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Apr 2021 17:39:56 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:7cc57a8772e5e479618650dfa70f315b474d3f205d04bde7f602f469c1928d84`  
		Last Modified: Sat, 10 Apr 2021 00:46:07 GMT  
		Size: 27.8 MB (27788987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d92d68a52363235dcdfb59fa81e5ef1a4561c958501e4f28d6b79e86f8b8501`  
		Last Modified: Sat, 10 Apr 2021 03:59:08 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff87ee5851bcc802818be3dc63452f46975dd0b1ef78290b0e5b760a98d28409`  
		Last Modified: Mon, 12 Apr 2021 17:42:44 GMT  
		Size: 8.5 MB (8487699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5830c94cc7d1ca0b503f2069591f94320a5b2fd958784710af0b17b0c7d24143`  
		Last Modified: Mon, 12 Apr 2021 17:42:42 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01e766b2588f559ef9d94f4ba7077047d1a9a727ce6da85cf9e7a9618639417`  
		Last Modified: Mon, 12 Apr 2021 17:42:42 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0` - linux; mips64le

```console
$ docker pull haproxy@sha256:4ff1e72efb4fac1b68f23687d476646175f18b3636ca29ba483eb1d1031ed478
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (33960206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb49249fea977cb148bb8062134385a190a4c7e8dd48d811e0e9d815d4a00bed`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:09:40 GMT
ADD file:0c93801c4a3719dfd4c047d7f2f4d52bf463eba2ab875da1dc54dcc832aae20b in / 
# Sat, 10 Apr 2021 01:09:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:39:36 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 12 Apr 2021 18:07:30 GMT
ENV HAPROXY_VERSION=2.0.22
# Mon, 12 Apr 2021 18:07:30 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.22.tar.gz
# Mon, 12 Apr 2021 18:07:30 GMT
ENV HAPROXY_SHA256=5e1dccf30a3ad782d1e3298cc4e4955b168e4aa06cad4e3ea1c0334cdc0f966d
# Mon, 12 Apr 2021 18:09:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Mon, 12 Apr 2021 18:09:42 GMT
STOPSIGNAL SIGUSR1
# Mon, 12 Apr 2021 18:09:43 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 12 Apr 2021 18:09:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 12 Apr 2021 18:09:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Apr 2021 18:09:45 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:09ea659ba566d9c3c62493e5ae0b964f1eee4fcf35aabc91c5c34ca1ad686541`  
		Last Modified: Sat, 10 Apr 2021 01:16:07 GMT  
		Size: 25.8 MB (25806410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10fa5ae1be1fc686c91c15f24ebaaa72d7c4f64321c8ead8386f2f4f9d1a6705`  
		Last Modified: Sat, 10 Apr 2021 01:53:41 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d049db72782b5bccf906aae9fd1cc8c2913f4e019fab7b470cd652764f2678e8`  
		Last Modified: Mon, 12 Apr 2021 18:10:23 GMT  
		Size: 8.2 MB (8151845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4abe0187ab5e15fb04ef1a8dd446f11003ab5d56f1ec8e5ebef4deac8ca74624`  
		Last Modified: Mon, 12 Apr 2021 18:10:18 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c1b70ba8f2cc92bd3202888c9d101288335af9534994c9ffeeae741ee9e7f3`  
		Last Modified: Mon, 12 Apr 2021 18:10:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0` - linux; ppc64le

```console
$ docker pull haproxy@sha256:a498d22cfbb9e767060e7bbaf60234e22f1a0a459f1d695e9f2212a3616667f8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39503810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f708ab07aa4baeb1ddbe0f44dc27033ef2c5bff31e7866eb999c1de3fe282ad5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:26:49 GMT
ADD file:ab87d4854aa8628ce8f4e603c0496499f6f28c3d2525ace782c7369691dafc8c in / 
# Sat, 10 Apr 2021 01:26:56 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 04:45:12 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 12 Apr 2021 18:19:43 GMT
ENV HAPROXY_VERSION=2.0.22
# Mon, 12 Apr 2021 18:19:47 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.22.tar.gz
# Mon, 12 Apr 2021 18:19:53 GMT
ENV HAPROXY_SHA256=5e1dccf30a3ad782d1e3298cc4e4955b168e4aa06cad4e3ea1c0334cdc0f966d
# Mon, 12 Apr 2021 18:23:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Mon, 12 Apr 2021 18:23:34 GMT
STOPSIGNAL SIGUSR1
# Mon, 12 Apr 2021 18:23:35 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 12 Apr 2021 18:23:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 12 Apr 2021 18:23:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Apr 2021 18:23:58 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:3e1e599482ca47095f85e429b346b76375aa85015ddcca050e85c2a8b1fdda9c`  
		Last Modified: Sat, 10 Apr 2021 01:33:57 GMT  
		Size: 30.5 MB (30545933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ee41bdc57145d3cb6e9f5fa23eed213567ae52835c7cff5fd57fe17b52f5ec`  
		Last Modified: Sat, 10 Apr 2021 05:09:50 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316b167bd5ecb65ef995d44f327cf982c6b3063e0903ed3021cc620ca71b40ff`  
		Last Modified: Mon, 12 Apr 2021 18:26:40 GMT  
		Size: 9.0 MB (8955918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bbdd0af159f921687a9c2b67e101dfb30219fa6b8b6f3ee94ec095ebd8a25d3`  
		Last Modified: Mon, 12 Apr 2021 18:26:38 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0900b03c06aaf7cb521b1a6e05d1b2b3131bbb81779e4c33e9139ed138a5879`  
		Last Modified: Mon, 12 Apr 2021 18:26:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0` - linux; s390x

```console
$ docker pull haproxy@sha256:35f932a421c1734aff6f729983e6ee63353b3b5031e0240100b14cca912005a7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (34004073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3fe6979d3c1c93dc9af9e8a2f6df7db5d4f0c24530fd8bbeae60f2f00b81b0ee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:42:23 GMT
ADD file:dbe2182f8699f2a6011413ea01862e6c0e85853d922dffd72a28d994d23c79bc in / 
# Sat, 10 Apr 2021 00:42:25 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:38:04 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 12 Apr 2021 18:01:48 GMT
ENV HAPROXY_VERSION=2.0.22
# Mon, 12 Apr 2021 18:01:49 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.22.tar.gz
# Mon, 12 Apr 2021 18:01:50 GMT
ENV HAPROXY_SHA256=5e1dccf30a3ad782d1e3298cc4e4955b168e4aa06cad4e3ea1c0334cdc0f966d
# Mon, 12 Apr 2021 18:03:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Mon, 12 Apr 2021 18:03:07 GMT
STOPSIGNAL SIGUSR1
# Mon, 12 Apr 2021 18:03:08 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 12 Apr 2021 18:03:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 12 Apr 2021 18:03:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Apr 2021 18:03:10 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:65291f8717b3afd99b63cee867dd3e06b956a8ee6aa8580cc31d913b25de209d`  
		Last Modified: Sat, 10 Apr 2021 00:45:48 GMT  
		Size: 25.8 MB (25753787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9daf67acfb0373e31068762d068f1da8d320f2bdcdb0e6651d52b8183ede06c`  
		Last Modified: Sat, 10 Apr 2021 01:42:28 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3481e94828f8e7c3aee6b3c81f82cbfd8d8bcfe93ea6c818c6da5ff6da9ce668`  
		Last Modified: Mon, 12 Apr 2021 18:05:37 GMT  
		Size: 8.2 MB (8248337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4264cc884583dc22fe86c11b1a4ab2df9614c05e33d8f0786190fcc2e23e61`  
		Last Modified: Mon, 12 Apr 2021 18:05:36 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8b288d6a9b82acc297dd95c643c29d45f832a9e4afca42bfc84717dfbe40c5`  
		Last Modified: Mon, 12 Apr 2021 18:05:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.0-alpine`

```console
$ docker pull haproxy@sha256:d21269268de0ad442bef23557df73b820e8d01c0750c2457a4429ad742821464
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `haproxy:2.0-alpine` - linux; amd64

```console
$ docker pull haproxy@sha256:f02ca82d6b4739d7e8e3c7dbf039eeec28eaccc0b16911e9eb052647df3f942b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8664606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0e4da1a17581c32b6faf5688d003b24845c9c747c9b65c1225da2e61d15beb5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:37:38 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 21:40:57 GMT
ENV HAPROXY_VERSION=2.0.22
# Wed, 14 Apr 2021 21:40:57 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.22.tar.gz
# Wed, 14 Apr 2021 21:40:57 GMT
ENV HAPROXY_SHA256=5e1dccf30a3ad782d1e3298cc4e4955b168e4aa06cad4e3ea1c0334cdc0f966d
# Wed, 14 Apr 2021 21:41:45 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 21:41:45 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 21:41:45 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 21:41:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 21:41:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 21:41:46 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4de1862a29af271c1751bf0d03d96f9a881f971d1288c5fafcfba90b517611f8`  
		Last Modified: Wed, 14 Apr 2021 21:43:30 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85c5756bf5d116ce7b57022d182bd213563c459d235de0f2152fea376442184e`  
		Last Modified: Wed, 14 Apr 2021 21:44:18 GMT  
		Size: 5.9 MB (5850881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88f0fd39c496741ff7b68e75f16eb1c7913f853ea176fe66c12c9cad606c3914`  
		Last Modified: Wed, 14 Apr 2021 21:44:17 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea8c072563ad521165128cce2a6b6d57d66b3bc3881ac7e6f238867fb3fb704`  
		Last Modified: Wed, 14 Apr 2021 21:44:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0-alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:8fdbffd080fe82115f9796601de046571dcbf3b573f1b786b20ca05768204b40
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8316006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70791ac0e74719f988c4c0cf5ae5b5c76d2a475b43b7c9b355a3d3065cc9bf12`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:18:05 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 21:27:23 GMT
ENV HAPROXY_VERSION=2.0.22
# Wed, 14 Apr 2021 21:27:25 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.22.tar.gz
# Wed, 14 Apr 2021 21:27:28 GMT
ENV HAPROXY_SHA256=5e1dccf30a3ad782d1e3298cc4e4955b168e4aa06cad4e3ea1c0334cdc0f966d
# Wed, 14 Apr 2021 21:27:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 21:27:54 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 21:27:55 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 21:27:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 21:28:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 21:28:01 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd640f0f76e4e434b444a36110041f2c571b2dbcfca29958b2e90de8d91bd6eb`  
		Last Modified: Wed, 14 Apr 2021 21:34:02 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6afd82fb556f4a6ff03d177aba7bea7b8d3112bda1deb36cac218066a003df8a`  
		Last Modified: Wed, 14 Apr 2021 21:34:45 GMT  
		Size: 5.7 MB (5692118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9be85f031de5f4055328cb5fd8f189ea36e587a63cbf8600f1e02c761c1fc3`  
		Last Modified: Wed, 14 Apr 2021 21:34:44 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1cac7ec8ab9da443f13bfe42accb64df408a47aa087be68d63838807e25fe24`  
		Last Modified: Wed, 14 Apr 2021 21:34:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:7a91e5a173106f174c1558fd0d4bb8701b315bf86d607ee5363973525f1cc66e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8088757 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:480f9888d0ccf141a98767ac3474562a46609303a7fa5430bb16800623b8f7bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:47:58 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 22:53:26 GMT
ENV HAPROXY_VERSION=2.0.22
# Wed, 14 Apr 2021 22:53:27 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.22.tar.gz
# Wed, 14 Apr 2021 22:53:28 GMT
ENV HAPROXY_SHA256=5e1dccf30a3ad782d1e3298cc4e4955b168e4aa06cad4e3ea1c0334cdc0f966d
# Wed, 14 Apr 2021 22:53:49 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 22:53:52 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 22:53:53 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 22:53:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 22:53:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 22:53:57 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ff0f6ee9305bed375c784c12ad4beeac3af6ea1a6b5afeec6b4700259dc194`  
		Last Modified: Wed, 14 Apr 2021 22:56:09 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a08e02e2df6a5eb6b70e1ffc98bad78878e57c4002e93996f4835f7707743f74`  
		Last Modified: Wed, 14 Apr 2021 22:56:51 GMT  
		Size: 5.7 MB (5662856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44c02981025797ccb7e58e8321d1167d5017e1a51c28c9295afeff0b6df23da6`  
		Last Modified: Wed, 14 Apr 2021 22:56:49 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67ccff635d336e01f80104aa14240eb1d49c76ed0b89c968f3986941529b5875`  
		Last Modified: Wed, 14 Apr 2021 22:56:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:f94500700117d16946e1af1485e3e5c55b104ab29375c6065b848c7d6edec835
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8556914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bee6852ef2c2048bb2c781ae32003de773193b526efaeeaca06f20c6d793dee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:26:01 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 20:32:53 GMT
ENV HAPROXY_VERSION=2.0.22
# Wed, 14 Apr 2021 20:33:01 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.22.tar.gz
# Wed, 14 Apr 2021 20:33:03 GMT
ENV HAPROXY_SHA256=5e1dccf30a3ad782d1e3298cc4e4955b168e4aa06cad4e3ea1c0334cdc0f966d
# Wed, 14 Apr 2021 20:34:06 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 20:34:19 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 20:34:23 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:34:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 20:34:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:34:38 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2ef9646f93509fb43536690b645509d9b653316324583761dd086b8ad6c664`  
		Last Modified: Wed, 14 Apr 2021 20:37:52 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f5923932c30ae8514030714d098f1ca3a08c86000d7204ac7e0ea552efc744`  
		Last Modified: Wed, 14 Apr 2021 20:38:38 GMT  
		Size: 5.8 MB (5843129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2ea26a073be4a5a0f265072b5294266534b7916602a22c420b5de2da64ae99`  
		Last Modified: Wed, 14 Apr 2021 20:38:37 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b500064a4bc11fd23b3a891fbea98dfec3b531210259f4079e64ee4349cd243`  
		Last Modified: Wed, 14 Apr 2021 20:38:37 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0-alpine` - linux; 386

```console
$ docker pull haproxy@sha256:379b155b5635b6bd22532f40fc2767d456167d8e1a1010ca409483a429d905e9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.5 MB (8522077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4b26ee65f1f9d728a64722a38c2f810085748b43b9465c07b3a75997667a791`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 01:50:06 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 15 Apr 2021 01:55:00 GMT
ENV HAPROXY_VERSION=2.0.22
# Thu, 15 Apr 2021 01:55:00 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.22.tar.gz
# Thu, 15 Apr 2021 01:55:01 GMT
ENV HAPROXY_SHA256=5e1dccf30a3ad782d1e3298cc4e4955b168e4aa06cad4e3ea1c0334cdc0f966d
# Thu, 15 Apr 2021 01:56:38 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 15 Apr 2021 01:56:38 GMT
STOPSIGNAL SIGUSR1
# Thu, 15 Apr 2021 01:56:39 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 15 Apr 2021 01:56:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 15 Apr 2021 01:56:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Apr 2021 01:56:41 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:31b7e7ccca9e17fd08b39c9a4ffd3ded380b62816c489d6c3758c9bb5a632430`  
		Last Modified: Wed, 14 Apr 2021 18:39:24 GMT  
		Size: 2.8 MB (2818900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9104145d2a6b1e0c0837c464bb9d4b331949cfeb6be12e4e7995507661d3386`  
		Last Modified: Thu, 15 Apr 2021 02:00:28 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d9999c344e71f2c636d0224087bbb517edf8fbd1102bdc20f32fb607e1bda9d`  
		Last Modified: Thu, 15 Apr 2021 02:01:27 GMT  
		Size: 5.7 MB (5701420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b33a5747798e9e74b213f2b1e57bffef27c5c5ce7d971fb9f19c861209a25b65`  
		Last Modified: Thu, 15 Apr 2021 02:01:23 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b623fa4c0dd48a6f9901e3b15cae57e6890fd8f70233deb2807d3720abc955`  
		Last Modified: Thu, 15 Apr 2021 02:01:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0-alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:db05ac1ad4b62dbb412c8af6527369e255da5127d0b0b6314236ac918ac1c0c7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.9 MB (8862617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bc3ea13a6768d6ca781964325fb2fcae8442d6e9353f7a981b1088268a86f4e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:25:09 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 23:31:23 GMT
ENV HAPROXY_VERSION=2.0.22
# Wed, 14 Apr 2021 23:31:28 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.22.tar.gz
# Wed, 14 Apr 2021 23:31:34 GMT
ENV HAPROXY_SHA256=5e1dccf30a3ad782d1e3298cc4e4955b168e4aa06cad4e3ea1c0334cdc0f966d
# Wed, 14 Apr 2021 23:32:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 23:32:26 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 23:32:30 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 23:32:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 23:32:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 23:32:52 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8004273856b1b354059d03a17deec6e79d325ba45d63213dda3d1fa401db8c22`  
		Last Modified: Wed, 14 Apr 2021 23:36:37 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f05d46b1dab35e38ab8d5fd3d260a51e2fd8e69bd9a925bb8067104539aae2d`  
		Last Modified: Wed, 14 Apr 2021 23:37:27 GMT  
		Size: 6.0 MB (6047719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce2178be9b684fafaf42e171aad3c4016566a1cf5d4ed3156ad85386b8c014f`  
		Last Modified: Wed, 14 Apr 2021 23:37:24 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e1bb59d52cbfb549fad00a22645b6d89696c697c571ac644fe4b60c16664f4c`  
		Last Modified: Wed, 14 Apr 2021 23:37:24 GMT  
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

## `haproxy:2.0.22`

```console
$ docker pull haproxy@sha256:af6505e38637df55fd060940c9074fb13c86912a328e25d68858a1690c0666e2
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

### `haproxy:2.0.22` - linux; amd64

```console
$ docker pull haproxy@sha256:d22e335f036e845d78ca259beff5dc007923c2373ff616ced7abb7672d15a32e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.8 MB (35835009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f5c3a5fcaa1312d5c45aa12ea12bf22b6e0c077c9e52bad166e9090c9a4bd9e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:29:42 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 12 Apr 2021 18:24:02 GMT
ENV HAPROXY_VERSION=2.0.22
# Mon, 12 Apr 2021 18:24:02 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.22.tar.gz
# Mon, 12 Apr 2021 18:24:03 GMT
ENV HAPROXY_SHA256=5e1dccf30a3ad782d1e3298cc4e4955b168e4aa06cad4e3ea1c0334cdc0f966d
# Mon, 12 Apr 2021 18:24:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Mon, 12 Apr 2021 18:24:44 GMT
STOPSIGNAL SIGUSR1
# Mon, 12 Apr 2021 18:24:45 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 12 Apr 2021 18:24:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 12 Apr 2021 18:24:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Apr 2021 18:24:46 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7abf58d954de379f38a19e07330116ba6b11f21007bc7b7507d233e5b0aa3fe0`  
		Last Modified: Sat, 10 Apr 2021 06:38:07 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf8559c4cb3b4af093063e24014fc599a99eac125bc8570d6cae1d629f5ce192`  
		Last Modified: Mon, 12 Apr 2021 18:26:40 GMT  
		Size: 8.7 MB (8693686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaeca2e42fc3dcb820dd40afc8dd47921d2f1f602e978d0e750f40207379d9bf`  
		Last Modified: Mon, 12 Apr 2021 18:26:39 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72170a2df5fa1a4b1f379916b866dd38b43e048d76750b8f4411bf79195b2a79`  
		Last Modified: Mon, 12 Apr 2021 18:26:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0.22` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:3bab5e0ca970574a9a4e27a8fa6a8fe74448a8473d8359394f6957f5032806a5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.1 MB (33050684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:810a0a1beb6b39b3a5588a675af7352b14e25eb0e49822709721726780d07324`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:51:31 GMT
ADD file:926533a23a69aa2481a9122b667bb6300a347154eea366c9e679a230aa7f373a in / 
# Sat, 10 Apr 2021 00:51:34 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 02:24:17 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 12 Apr 2021 17:49:04 GMT
ENV HAPROXY_VERSION=2.0.22
# Mon, 12 Apr 2021 17:49:05 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.22.tar.gz
# Mon, 12 Apr 2021 17:49:06 GMT
ENV HAPROXY_SHA256=5e1dccf30a3ad782d1e3298cc4e4955b168e4aa06cad4e3ea1c0334cdc0f966d
# Mon, 12 Apr 2021 17:50:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Mon, 12 Apr 2021 17:50:02 GMT
STOPSIGNAL SIGUSR1
# Mon, 12 Apr 2021 17:50:03 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 12 Apr 2021 17:50:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 12 Apr 2021 17:50:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Apr 2021 17:50:07 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:33d77752597b664d047cc829e58a223d6fb077b61f69ca0462fcfb9b78d5f69b`  
		Last Modified: Sat, 10 Apr 2021 00:59:22 GMT  
		Size: 24.9 MB (24873199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c107a5973e1ce17cb311e2bf8a0d841875ca9f02219922ca12a9203602b5ce`  
		Last Modified: Sat, 10 Apr 2021 02:36:55 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a695842d5b3a7d715904c56cb979ded99ebeb34e90d9d720643d7c58ca0a12d2`  
		Last Modified: Mon, 12 Apr 2021 17:51:02 GMT  
		Size: 8.2 MB (8175536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df803aacf2d39c82d93ff0cdf3e342bd9a4e66f427cfb462f3ce73bccf8399da`  
		Last Modified: Mon, 12 Apr 2021 17:50:58 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f0cc428a811f53c34336143a7738671989088880f717762cbbd8fcf70e3c204`  
		Last Modified: Mon, 12 Apr 2021 17:50:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0.22` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:4dae846f887000e2f21e6e2d668ceaf834529b694d489e94ad1edb849b9ec663
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.9 MB (30864631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e7ca95062d20599f7de1a466fa37624953bdb60f497b4e711214f08e3bb3885`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:59:45 GMT
ADD file:3fbd246a2de82566bcaaf62e3e0bf57175a7ad46b4156366a110661b31eab240 in / 
# Sat, 10 Apr 2021 00:59:47 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 08:58:51 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 12 Apr 2021 18:28:47 GMT
ENV HAPROXY_VERSION=2.0.22
# Mon, 12 Apr 2021 18:28:50 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.22.tar.gz
# Mon, 12 Apr 2021 18:28:52 GMT
ENV HAPROXY_SHA256=5e1dccf30a3ad782d1e3298cc4e4955b168e4aa06cad4e3ea1c0334cdc0f966d
# Mon, 12 Apr 2021 18:29:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Mon, 12 Apr 2021 18:29:35 GMT
STOPSIGNAL SIGUSR1
# Mon, 12 Apr 2021 18:29:36 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 12 Apr 2021 18:29:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 12 Apr 2021 18:29:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Apr 2021 18:29:41 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:8c6bea184b33030fb923c3c09d634b73235dec3fe2d411db9fd22bda669f2c37`  
		Last Modified: Sat, 10 Apr 2021 01:07:51 GMT  
		Size: 22.7 MB (22739801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5be95d3afdef3cc4c8a37695b513cf41e6cf6ffeecd9ce2426d38cb245a0b52`  
		Last Modified: Sat, 10 Apr 2021 09:05:25 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d372da4e007019116f4af10321bf34e48dc6c4806ad68fe226cfbb1ec490cd`  
		Last Modified: Mon, 12 Apr 2021 18:32:02 GMT  
		Size: 8.1 MB (8122884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:675402e3f486334baf119c742f454e8e960a48d50b6289a842e35f4cb90fc53b`  
		Last Modified: Mon, 12 Apr 2021 18:31:59 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:881f59bde771a049db45f8a4b14f96c75a105e16485aae148b0a06daa2d1e6df`  
		Last Modified: Mon, 12 Apr 2021 18:31:59 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0.22` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:d01e95fc2d486bf1d9ffb641597b510198bee08b4eefb1d76193689649bede61
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.4 MB (34437386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b928a7e49b156c8873cce5cc4161c00e4ed02049215ec118a130e7a3e500137`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:41:25 GMT
ADD file:b24da7eb23eeae04e00d0e45da29a89fe8f992e8dcf4ba482afb907b8015b7bf in / 
# Sat, 10 Apr 2021 00:41:28 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:13:29 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 12 Apr 2021 18:18:53 GMT
ENV HAPROXY_VERSION=2.0.22
# Mon, 12 Apr 2021 18:18:56 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.22.tar.gz
# Mon, 12 Apr 2021 18:19:01 GMT
ENV HAPROXY_SHA256=5e1dccf30a3ad782d1e3298cc4e4955b168e4aa06cad4e3ea1c0334cdc0f966d
# Mon, 12 Apr 2021 18:19:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Mon, 12 Apr 2021 18:19:57 GMT
STOPSIGNAL SIGUSR1
# Mon, 12 Apr 2021 18:19:58 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 12 Apr 2021 18:20:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 12 Apr 2021 18:20:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Apr 2021 18:20:10 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:15cb40b9c4df1a06940dc2a154c3be46844241235c1a091afa70da0ee2dc811a`  
		Last Modified: Sat, 10 Apr 2021 00:47:53 GMT  
		Size: 25.9 MB (25904582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48cb832c3e00ffed789c3f464caa612fe4996ba4683f72f8cf214d1437268efe`  
		Last Modified: Sat, 10 Apr 2021 01:21:27 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17c4b35ef5e3d4f8ac9c98e4fc17d434f443113c6f665313fba5f84fceaffe58`  
		Last Modified: Mon, 12 Apr 2021 18:22:22 GMT  
		Size: 8.5 MB (8530854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde0431b3ddbf51fb7e287872dda9a1e535356ea7f6ced0daf5a6b8f924fad2e`  
		Last Modified: Mon, 12 Apr 2021 18:22:19 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc6730a49e57ae9e3973dda6e22b061a7708697635c732a54ab68672a98087d`  
		Last Modified: Mon, 12 Apr 2021 18:22:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0.22` - linux; 386

```console
$ docker pull haproxy@sha256:9f921067cf03daf25261e0865a0a128860f0b1908b76687689fda3432ac6b399
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36278633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5f30bae29deb98ba66eebdb03b0ca5a490fbefe5902356350a9bce0cdc57489`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:39:42 GMT
ADD file:8885d4d13678543780bb04ba14b621179665f7951d5b261036a7092df9b376e7 in / 
# Sat, 10 Apr 2021 00:39:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 03:48:12 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 12 Apr 2021 17:39:07 GMT
ENV HAPROXY_VERSION=2.0.22
# Mon, 12 Apr 2021 17:39:08 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.22.tar.gz
# Mon, 12 Apr 2021 17:39:08 GMT
ENV HAPROXY_SHA256=5e1dccf30a3ad782d1e3298cc4e4955b168e4aa06cad4e3ea1c0334cdc0f966d
# Mon, 12 Apr 2021 17:39:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Mon, 12 Apr 2021 17:39:55 GMT
STOPSIGNAL SIGUSR1
# Mon, 12 Apr 2021 17:39:55 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 12 Apr 2021 17:39:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 12 Apr 2021 17:39:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Apr 2021 17:39:56 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:7cc57a8772e5e479618650dfa70f315b474d3f205d04bde7f602f469c1928d84`  
		Last Modified: Sat, 10 Apr 2021 00:46:07 GMT  
		Size: 27.8 MB (27788987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d92d68a52363235dcdfb59fa81e5ef1a4561c958501e4f28d6b79e86f8b8501`  
		Last Modified: Sat, 10 Apr 2021 03:59:08 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff87ee5851bcc802818be3dc63452f46975dd0b1ef78290b0e5b760a98d28409`  
		Last Modified: Mon, 12 Apr 2021 17:42:44 GMT  
		Size: 8.5 MB (8487699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5830c94cc7d1ca0b503f2069591f94320a5b2fd958784710af0b17b0c7d24143`  
		Last Modified: Mon, 12 Apr 2021 17:42:42 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01e766b2588f559ef9d94f4ba7077047d1a9a727ce6da85cf9e7a9618639417`  
		Last Modified: Mon, 12 Apr 2021 17:42:42 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0.22` - linux; mips64le

```console
$ docker pull haproxy@sha256:4ff1e72efb4fac1b68f23687d476646175f18b3636ca29ba483eb1d1031ed478
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (33960206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb49249fea977cb148bb8062134385a190a4c7e8dd48d811e0e9d815d4a00bed`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:09:40 GMT
ADD file:0c93801c4a3719dfd4c047d7f2f4d52bf463eba2ab875da1dc54dcc832aae20b in / 
# Sat, 10 Apr 2021 01:09:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:39:36 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 12 Apr 2021 18:07:30 GMT
ENV HAPROXY_VERSION=2.0.22
# Mon, 12 Apr 2021 18:07:30 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.22.tar.gz
# Mon, 12 Apr 2021 18:07:30 GMT
ENV HAPROXY_SHA256=5e1dccf30a3ad782d1e3298cc4e4955b168e4aa06cad4e3ea1c0334cdc0f966d
# Mon, 12 Apr 2021 18:09:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Mon, 12 Apr 2021 18:09:42 GMT
STOPSIGNAL SIGUSR1
# Mon, 12 Apr 2021 18:09:43 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 12 Apr 2021 18:09:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 12 Apr 2021 18:09:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Apr 2021 18:09:45 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:09ea659ba566d9c3c62493e5ae0b964f1eee4fcf35aabc91c5c34ca1ad686541`  
		Last Modified: Sat, 10 Apr 2021 01:16:07 GMT  
		Size: 25.8 MB (25806410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10fa5ae1be1fc686c91c15f24ebaaa72d7c4f64321c8ead8386f2f4f9d1a6705`  
		Last Modified: Sat, 10 Apr 2021 01:53:41 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d049db72782b5bccf906aae9fd1cc8c2913f4e019fab7b470cd652764f2678e8`  
		Last Modified: Mon, 12 Apr 2021 18:10:23 GMT  
		Size: 8.2 MB (8151845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4abe0187ab5e15fb04ef1a8dd446f11003ab5d56f1ec8e5ebef4deac8ca74624`  
		Last Modified: Mon, 12 Apr 2021 18:10:18 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c1b70ba8f2cc92bd3202888c9d101288335af9534994c9ffeeae741ee9e7f3`  
		Last Modified: Mon, 12 Apr 2021 18:10:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0.22` - linux; ppc64le

```console
$ docker pull haproxy@sha256:a498d22cfbb9e767060e7bbaf60234e22f1a0a459f1d695e9f2212a3616667f8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39503810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f708ab07aa4baeb1ddbe0f44dc27033ef2c5bff31e7866eb999c1de3fe282ad5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:26:49 GMT
ADD file:ab87d4854aa8628ce8f4e603c0496499f6f28c3d2525ace782c7369691dafc8c in / 
# Sat, 10 Apr 2021 01:26:56 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 04:45:12 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 12 Apr 2021 18:19:43 GMT
ENV HAPROXY_VERSION=2.0.22
# Mon, 12 Apr 2021 18:19:47 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.22.tar.gz
# Mon, 12 Apr 2021 18:19:53 GMT
ENV HAPROXY_SHA256=5e1dccf30a3ad782d1e3298cc4e4955b168e4aa06cad4e3ea1c0334cdc0f966d
# Mon, 12 Apr 2021 18:23:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Mon, 12 Apr 2021 18:23:34 GMT
STOPSIGNAL SIGUSR1
# Mon, 12 Apr 2021 18:23:35 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 12 Apr 2021 18:23:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 12 Apr 2021 18:23:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Apr 2021 18:23:58 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:3e1e599482ca47095f85e429b346b76375aa85015ddcca050e85c2a8b1fdda9c`  
		Last Modified: Sat, 10 Apr 2021 01:33:57 GMT  
		Size: 30.5 MB (30545933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ee41bdc57145d3cb6e9f5fa23eed213567ae52835c7cff5fd57fe17b52f5ec`  
		Last Modified: Sat, 10 Apr 2021 05:09:50 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316b167bd5ecb65ef995d44f327cf982c6b3063e0903ed3021cc620ca71b40ff`  
		Last Modified: Mon, 12 Apr 2021 18:26:40 GMT  
		Size: 9.0 MB (8955918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bbdd0af159f921687a9c2b67e101dfb30219fa6b8b6f3ee94ec095ebd8a25d3`  
		Last Modified: Mon, 12 Apr 2021 18:26:38 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0900b03c06aaf7cb521b1a6e05d1b2b3131bbb81779e4c33e9139ed138a5879`  
		Last Modified: Mon, 12 Apr 2021 18:26:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0.22` - linux; s390x

```console
$ docker pull haproxy@sha256:35f932a421c1734aff6f729983e6ee63353b3b5031e0240100b14cca912005a7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (34004073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3fe6979d3c1c93dc9af9e8a2f6df7db5d4f0c24530fd8bbeae60f2f00b81b0ee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:42:23 GMT
ADD file:dbe2182f8699f2a6011413ea01862e6c0e85853d922dffd72a28d994d23c79bc in / 
# Sat, 10 Apr 2021 00:42:25 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:38:04 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 12 Apr 2021 18:01:48 GMT
ENV HAPROXY_VERSION=2.0.22
# Mon, 12 Apr 2021 18:01:49 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.22.tar.gz
# Mon, 12 Apr 2021 18:01:50 GMT
ENV HAPROXY_SHA256=5e1dccf30a3ad782d1e3298cc4e4955b168e4aa06cad4e3ea1c0334cdc0f966d
# Mon, 12 Apr 2021 18:03:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Mon, 12 Apr 2021 18:03:07 GMT
STOPSIGNAL SIGUSR1
# Mon, 12 Apr 2021 18:03:08 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 12 Apr 2021 18:03:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Mon, 12 Apr 2021 18:03:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Apr 2021 18:03:10 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:65291f8717b3afd99b63cee867dd3e06b956a8ee6aa8580cc31d913b25de209d`  
		Last Modified: Sat, 10 Apr 2021 00:45:48 GMT  
		Size: 25.8 MB (25753787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9daf67acfb0373e31068762d068f1da8d320f2bdcdb0e6651d52b8183ede06c`  
		Last Modified: Sat, 10 Apr 2021 01:42:28 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3481e94828f8e7c3aee6b3c81f82cbfd8d8bcfe93ea6c818c6da5ff6da9ce668`  
		Last Modified: Mon, 12 Apr 2021 18:05:37 GMT  
		Size: 8.2 MB (8248337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4264cc884583dc22fe86c11b1a4ab2df9614c05e33d8f0786190fcc2e23e61`  
		Last Modified: Mon, 12 Apr 2021 18:05:36 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8b288d6a9b82acc297dd95c643c29d45f832a9e4afca42bfc84717dfbe40c5`  
		Last Modified: Mon, 12 Apr 2021 18:05:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.0.22-alpine`

```console
$ docker pull haproxy@sha256:d21269268de0ad442bef23557df73b820e8d01c0750c2457a4429ad742821464
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `haproxy:2.0.22-alpine` - linux; amd64

```console
$ docker pull haproxy@sha256:f02ca82d6b4739d7e8e3c7dbf039eeec28eaccc0b16911e9eb052647df3f942b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8664606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0e4da1a17581c32b6faf5688d003b24845c9c747c9b65c1225da2e61d15beb5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:37:38 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 21:40:57 GMT
ENV HAPROXY_VERSION=2.0.22
# Wed, 14 Apr 2021 21:40:57 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.22.tar.gz
# Wed, 14 Apr 2021 21:40:57 GMT
ENV HAPROXY_SHA256=5e1dccf30a3ad782d1e3298cc4e4955b168e4aa06cad4e3ea1c0334cdc0f966d
# Wed, 14 Apr 2021 21:41:45 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 21:41:45 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 21:41:45 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 21:41:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 21:41:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 21:41:46 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4de1862a29af271c1751bf0d03d96f9a881f971d1288c5fafcfba90b517611f8`  
		Last Modified: Wed, 14 Apr 2021 21:43:30 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85c5756bf5d116ce7b57022d182bd213563c459d235de0f2152fea376442184e`  
		Last Modified: Wed, 14 Apr 2021 21:44:18 GMT  
		Size: 5.9 MB (5850881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88f0fd39c496741ff7b68e75f16eb1c7913f853ea176fe66c12c9cad606c3914`  
		Last Modified: Wed, 14 Apr 2021 21:44:17 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea8c072563ad521165128cce2a6b6d57d66b3bc3881ac7e6f238867fb3fb704`  
		Last Modified: Wed, 14 Apr 2021 21:44:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0.22-alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:8fdbffd080fe82115f9796601de046571dcbf3b573f1b786b20ca05768204b40
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.3 MB (8316006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70791ac0e74719f988c4c0cf5ae5b5c76d2a475b43b7c9b355a3d3065cc9bf12`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:18:05 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 21:27:23 GMT
ENV HAPROXY_VERSION=2.0.22
# Wed, 14 Apr 2021 21:27:25 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.22.tar.gz
# Wed, 14 Apr 2021 21:27:28 GMT
ENV HAPROXY_SHA256=5e1dccf30a3ad782d1e3298cc4e4955b168e4aa06cad4e3ea1c0334cdc0f966d
# Wed, 14 Apr 2021 21:27:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 21:27:54 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 21:27:55 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 21:27:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 21:28:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 21:28:01 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd640f0f76e4e434b444a36110041f2c571b2dbcfca29958b2e90de8d91bd6eb`  
		Last Modified: Wed, 14 Apr 2021 21:34:02 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6afd82fb556f4a6ff03d177aba7bea7b8d3112bda1deb36cac218066a003df8a`  
		Last Modified: Wed, 14 Apr 2021 21:34:45 GMT  
		Size: 5.7 MB (5692118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9be85f031de5f4055328cb5fd8f189ea36e587a63cbf8600f1e02c761c1fc3`  
		Last Modified: Wed, 14 Apr 2021 21:34:44 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1cac7ec8ab9da443f13bfe42accb64df408a47aa087be68d63838807e25fe24`  
		Last Modified: Wed, 14 Apr 2021 21:34:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0.22-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:7a91e5a173106f174c1558fd0d4bb8701b315bf86d607ee5363973525f1cc66e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.1 MB (8088757 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:480f9888d0ccf141a98767ac3474562a46609303a7fa5430bb16800623b8f7bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:47:58 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 22:53:26 GMT
ENV HAPROXY_VERSION=2.0.22
# Wed, 14 Apr 2021 22:53:27 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.22.tar.gz
# Wed, 14 Apr 2021 22:53:28 GMT
ENV HAPROXY_SHA256=5e1dccf30a3ad782d1e3298cc4e4955b168e4aa06cad4e3ea1c0334cdc0f966d
# Wed, 14 Apr 2021 22:53:49 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 22:53:52 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 22:53:53 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 22:53:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 22:53:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 22:53:57 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ff0f6ee9305bed375c784c12ad4beeac3af6ea1a6b5afeec6b4700259dc194`  
		Last Modified: Wed, 14 Apr 2021 22:56:09 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a08e02e2df6a5eb6b70e1ffc98bad78878e57c4002e93996f4835f7707743f74`  
		Last Modified: Wed, 14 Apr 2021 22:56:51 GMT  
		Size: 5.7 MB (5662856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44c02981025797ccb7e58e8321d1167d5017e1a51c28c9295afeff0b6df23da6`  
		Last Modified: Wed, 14 Apr 2021 22:56:49 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67ccff635d336e01f80104aa14240eb1d49c76ed0b89c968f3986941529b5875`  
		Last Modified: Wed, 14 Apr 2021 22:56:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0.22-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:f94500700117d16946e1af1485e3e5c55b104ab29375c6065b848c7d6edec835
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8556914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bee6852ef2c2048bb2c781ae32003de773193b526efaeeaca06f20c6d793dee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:26:01 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 20:32:53 GMT
ENV HAPROXY_VERSION=2.0.22
# Wed, 14 Apr 2021 20:33:01 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.22.tar.gz
# Wed, 14 Apr 2021 20:33:03 GMT
ENV HAPROXY_SHA256=5e1dccf30a3ad782d1e3298cc4e4955b168e4aa06cad4e3ea1c0334cdc0f966d
# Wed, 14 Apr 2021 20:34:06 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 20:34:19 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 20:34:23 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:34:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 20:34:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:34:38 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2ef9646f93509fb43536690b645509d9b653316324583761dd086b8ad6c664`  
		Last Modified: Wed, 14 Apr 2021 20:37:52 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f5923932c30ae8514030714d098f1ca3a08c86000d7204ac7e0ea552efc744`  
		Last Modified: Wed, 14 Apr 2021 20:38:38 GMT  
		Size: 5.8 MB (5843129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2ea26a073be4a5a0f265072b5294266534b7916602a22c420b5de2da64ae99`  
		Last Modified: Wed, 14 Apr 2021 20:38:37 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b500064a4bc11fd23b3a891fbea98dfec3b531210259f4079e64ee4349cd243`  
		Last Modified: Wed, 14 Apr 2021 20:38:37 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0.22-alpine` - linux; 386

```console
$ docker pull haproxy@sha256:379b155b5635b6bd22532f40fc2767d456167d8e1a1010ca409483a429d905e9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.5 MB (8522077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4b26ee65f1f9d728a64722a38c2f810085748b43b9465c07b3a75997667a791`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 01:50:06 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 15 Apr 2021 01:55:00 GMT
ENV HAPROXY_VERSION=2.0.22
# Thu, 15 Apr 2021 01:55:00 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.22.tar.gz
# Thu, 15 Apr 2021 01:55:01 GMT
ENV HAPROXY_SHA256=5e1dccf30a3ad782d1e3298cc4e4955b168e4aa06cad4e3ea1c0334cdc0f966d
# Thu, 15 Apr 2021 01:56:38 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 15 Apr 2021 01:56:38 GMT
STOPSIGNAL SIGUSR1
# Thu, 15 Apr 2021 01:56:39 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 15 Apr 2021 01:56:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 15 Apr 2021 01:56:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Apr 2021 01:56:41 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:31b7e7ccca9e17fd08b39c9a4ffd3ded380b62816c489d6c3758c9bb5a632430`  
		Last Modified: Wed, 14 Apr 2021 18:39:24 GMT  
		Size: 2.8 MB (2818900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9104145d2a6b1e0c0837c464bb9d4b331949cfeb6be12e4e7995507661d3386`  
		Last Modified: Thu, 15 Apr 2021 02:00:28 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d9999c344e71f2c636d0224087bbb517edf8fbd1102bdc20f32fb607e1bda9d`  
		Last Modified: Thu, 15 Apr 2021 02:01:27 GMT  
		Size: 5.7 MB (5701420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b33a5747798e9e74b213f2b1e57bffef27c5c5ce7d971fb9f19c861209a25b65`  
		Last Modified: Thu, 15 Apr 2021 02:01:23 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b623fa4c0dd48a6f9901e3b15cae57e6890fd8f70233deb2807d3720abc955`  
		Last Modified: Thu, 15 Apr 2021 02:01:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0.22-alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:db05ac1ad4b62dbb412c8af6527369e255da5127d0b0b6314236ac918ac1c0c7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.9 MB (8862617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bc3ea13a6768d6ca781964325fb2fcae8442d6e9353f7a981b1088268a86f4e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:25:09 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 23:31:23 GMT
ENV HAPROXY_VERSION=2.0.22
# Wed, 14 Apr 2021 23:31:28 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.22.tar.gz
# Wed, 14 Apr 2021 23:31:34 GMT
ENV HAPROXY_SHA256=5e1dccf30a3ad782d1e3298cc4e4955b168e4aa06cad4e3ea1c0334cdc0f966d
# Wed, 14 Apr 2021 23:32:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 23:32:26 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 23:32:30 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 23:32:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 23:32:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 23:32:52 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8004273856b1b354059d03a17deec6e79d325ba45d63213dda3d1fa401db8c22`  
		Last Modified: Wed, 14 Apr 2021 23:36:37 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f05d46b1dab35e38ab8d5fd3d260a51e2fd8e69bd9a925bb8067104539aae2d`  
		Last Modified: Wed, 14 Apr 2021 23:37:27 GMT  
		Size: 6.0 MB (6047719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce2178be9b684fafaf42e171aad3c4016566a1cf5d4ed3156ad85386b8c014f`  
		Last Modified: Wed, 14 Apr 2021 23:37:24 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e1bb59d52cbfb549fad00a22645b6d89696c697c571ac644fe4b60c16664f4c`  
		Last Modified: Wed, 14 Apr 2021 23:37:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0.22-alpine` - linux; s390x

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

## `haproxy:2.2`

```console
$ docker pull haproxy@sha256:792ac7e9a42dcb028039bd6ec02cfdde75e94980652121e1fe557e7cf8b847bb
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

### `haproxy:2.2` - linux; amd64

```console
$ docker pull haproxy@sha256:6706d478e4e608c4d7aff4b100c029ed8ed5387f41f6d7d8b4b6ac9ecba3b745
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.5 MB (36450315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b71355e785ee76f43999ed2fa4612e47d61b76c61b3045c4d866b169b192bc99`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:29:42 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 29 Apr 2021 17:29:19 GMT
ENV HAPROXY_VERSION=2.2.14
# Thu, 29 Apr 2021 17:29:20 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Thu, 29 Apr 2021 17:29:20 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Thu, 29 Apr 2021 17:30:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 29 Apr 2021 17:30:04 GMT
STOPSIGNAL SIGUSR1
# Thu, 29 Apr 2021 17:30:04 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 29 Apr 2021 17:30:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 29 Apr 2021 17:30:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Apr 2021 17:30:06 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7abf58d954de379f38a19e07330116ba6b11f21007bc7b7507d233e5b0aa3fe0`  
		Last Modified: Sat, 10 Apr 2021 06:38:07 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ba487cb42887a026b3940ab5d25240db3ae8ca3538a433d33ded6c1e78ad946`  
		Last Modified: Thu, 29 Apr 2021 17:32:22 GMT  
		Size: 9.3 MB (9308992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f13a5faba9b80662ce1beda2cf0d30503c88a5569751155fd6d9fcfe6323ac46`  
		Last Modified: Thu, 29 Apr 2021 17:32:20 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3261bbc066b08611abdde75acf1a7a9a48c2d49f7540dcbc9a3c8e450ba4bd1b`  
		Last Modified: Thu, 29 Apr 2021 17:32:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:c36e6561bbe1be11cfd9b264eb760158871281895cdccacaa2aace07b64e704d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33788380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be71ea57166ad123cfb3dde36d0d110e554e5bbd5762aa5694b2903a5642af2a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:51:31 GMT
ADD file:926533a23a69aa2481a9122b667bb6300a347154eea366c9e679a230aa7f373a in / 
# Sat, 10 Apr 2021 00:51:34 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 02:24:17 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 29 Apr 2021 17:48:45 GMT
ENV HAPROXY_VERSION=2.2.14
# Thu, 29 Apr 2021 17:48:45 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Thu, 29 Apr 2021 17:48:46 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Thu, 29 Apr 2021 17:49:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 29 Apr 2021 17:49:35 GMT
STOPSIGNAL SIGUSR1
# Thu, 29 Apr 2021 17:49:36 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 29 Apr 2021 17:49:39 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 29 Apr 2021 17:49:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Apr 2021 17:49:40 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:33d77752597b664d047cc829e58a223d6fb077b61f69ca0462fcfb9b78d5f69b`  
		Last Modified: Sat, 10 Apr 2021 00:59:22 GMT  
		Size: 24.9 MB (24873199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c107a5973e1ce17cb311e2bf8a0d841875ca9f02219922ca12a9203602b5ce`  
		Last Modified: Sat, 10 Apr 2021 02:36:55 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a77f509b71668a040ff49cefb629a69b38b8703e98ed245bd0a97e97d10dc941`  
		Last Modified: Thu, 29 Apr 2021 17:50:22 GMT  
		Size: 8.9 MB (8913230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465b06ecb24dfbadcc493326bbf81d26de8a87e42dca5391cb9fcce5b693ce68`  
		Last Modified: Thu, 29 Apr 2021 17:50:19 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a57c7b8bed3c607d9c0e9cbe2d9e7538c16f5e02eb14d538227db37c7bb17e28`  
		Last Modified: Thu, 29 Apr 2021 17:50:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:f2d6692932a23d8178cadfbdc361c84a1f9dee4b7f0aeba65040899f65303432
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.5 MB (31464618 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7706d3cb80f141f9f889baea70aa79afc549e227e90bffd1aded90f5703bff2d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:59:45 GMT
ADD file:3fbd246a2de82566bcaaf62e3e0bf57175a7ad46b4156366a110661b31eab240 in / 
# Sat, 10 Apr 2021 00:59:47 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 08:58:51 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 29 Apr 2021 16:59:52 GMT
ENV HAPROXY_VERSION=2.2.14
# Thu, 29 Apr 2021 16:59:52 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Thu, 29 Apr 2021 16:59:53 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Thu, 29 Apr 2021 17:00:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 29 Apr 2021 17:00:35 GMT
STOPSIGNAL SIGUSR1
# Thu, 29 Apr 2021 17:00:36 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 29 Apr 2021 17:00:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 29 Apr 2021 17:00:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Apr 2021 17:00:41 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:8c6bea184b33030fb923c3c09d634b73235dec3fe2d411db9fd22bda669f2c37`  
		Last Modified: Sat, 10 Apr 2021 01:07:51 GMT  
		Size: 22.7 MB (22739801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5be95d3afdef3cc4c8a37695b513cf41e6cf6ffeecd9ce2426d38cb245a0b52`  
		Last Modified: Sat, 10 Apr 2021 09:05:25 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:110847a1cab7ee7d5910a3162e69e05dc4b27b38bbf0690fd5287335ca45d994`  
		Last Modified: Thu, 29 Apr 2021 17:02:34 GMT  
		Size: 8.7 MB (8722868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842fd9bf0561243131b85223fd2121bca335a34398de2805ce2bc49c20f0557f`  
		Last Modified: Thu, 29 Apr 2021 17:02:31 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba857cc76815a69804d81b7b8cfd1cef733d552360b462a6654bb997dc422b2`  
		Last Modified: Thu, 29 Apr 2021 17:02:31 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:a4de49115c06290f0365e78ccfc41c33ae5c7f54f069e8d5ad910d17cd00e1fb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.0 MB (35029567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c6269d7f5a3a3146d838cb1f3d9a89975b839613e3bc29493db15a8c91dd948`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:41:25 GMT
ADD file:b24da7eb23eeae04e00d0e45da29a89fe8f992e8dcf4ba482afb907b8015b7bf in / 
# Sat, 10 Apr 2021 00:41:28 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:13:29 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 29 Apr 2021 17:52:04 GMT
ENV HAPROXY_VERSION=2.2.14
# Thu, 29 Apr 2021 17:52:04 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Thu, 29 Apr 2021 17:52:05 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Thu, 29 Apr 2021 17:52:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 29 Apr 2021 17:52:49 GMT
STOPSIGNAL SIGUSR1
# Thu, 29 Apr 2021 17:52:50 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 29 Apr 2021 17:52:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 29 Apr 2021 17:52:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Apr 2021 17:52:57 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:15cb40b9c4df1a06940dc2a154c3be46844241235c1a091afa70da0ee2dc811a`  
		Last Modified: Sat, 10 Apr 2021 00:47:53 GMT  
		Size: 25.9 MB (25904582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48cb832c3e00ffed789c3f464caa612fe4996ba4683f72f8cf214d1437268efe`  
		Last Modified: Sat, 10 Apr 2021 01:21:27 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecd2d7073326e7be6f17459b1bdbdd24dbca7f0b483761cb137bb319170cdae9`  
		Last Modified: Thu, 29 Apr 2021 17:54:48 GMT  
		Size: 9.1 MB (9123034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af396c216cd462331785256c8eb8b58249a257388636dfba8957a6eea6563656`  
		Last Modified: Thu, 29 Apr 2021 17:54:46 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30df480ff08a19b3b653b87ddd425f40dfeee6416890092a6ee6f39c909f722c`  
		Last Modified: Thu, 29 Apr 2021 17:54:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2` - linux; 386

```console
$ docker pull haproxy@sha256:481622045fb02fb6b31c3c1aac02351d13a0e075c2781dc0d8fe13ddf240a5b2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36980676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23f034ff44a4590fbde461f619710fc01edb99a36cdb948ffd62c756fe1566d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:39:42 GMT
ADD file:8885d4d13678543780bb04ba14b621179665f7951d5b261036a7092df9b376e7 in / 
# Sat, 10 Apr 2021 00:39:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 03:48:12 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 29 Apr 2021 17:39:19 GMT
ENV HAPROXY_VERSION=2.2.14
# Thu, 29 Apr 2021 17:39:19 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Thu, 29 Apr 2021 17:39:20 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Thu, 29 Apr 2021 17:40:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 29 Apr 2021 17:40:27 GMT
STOPSIGNAL SIGUSR1
# Thu, 29 Apr 2021 17:40:28 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 29 Apr 2021 17:40:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 29 Apr 2021 17:40:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Apr 2021 17:40:29 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:7cc57a8772e5e479618650dfa70f315b474d3f205d04bde7f602f469c1928d84`  
		Last Modified: Sat, 10 Apr 2021 00:46:07 GMT  
		Size: 27.8 MB (27788987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d92d68a52363235dcdfb59fa81e5ef1a4561c958501e4f28d6b79e86f8b8501`  
		Last Modified: Sat, 10 Apr 2021 03:59:08 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57229d188189b1e10cc3562b2ffd352969144dfbaf06988a920ed5427ed7906b`  
		Last Modified: Thu, 29 Apr 2021 17:44:22 GMT  
		Size: 9.2 MB (9189740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fb9373ea635024b72729ee73d1d659e91446280256d3fd21762b084584f4c88`  
		Last Modified: Thu, 29 Apr 2021 17:44:20 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a04207b362e717df1206194d656c8b158caffc32107bcd7131b746a848d033e6`  
		Last Modified: Thu, 29 Apr 2021 17:44:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2` - linux; mips64le

```console
$ docker pull haproxy@sha256:e518728537a7d7a9887fad3713fcb11680b0da3376cc3b2ec13eec2655bc5ef4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34678876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2570ecec3e5c74b7b8d58abd69762b1d5ea1641ed6abbf3e8078fed1d1f82ba4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:09:40 GMT
ADD file:0c93801c4a3719dfd4c047d7f2f4d52bf463eba2ab875da1dc54dcc832aae20b in / 
# Sat, 10 Apr 2021 01:09:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:39:36 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 29 Apr 2021 17:07:40 GMT
ENV HAPROXY_VERSION=2.2.14
# Thu, 29 Apr 2021 17:07:40 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Thu, 29 Apr 2021 17:07:40 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Thu, 29 Apr 2021 17:10:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 29 Apr 2021 17:10:06 GMT
STOPSIGNAL SIGUSR1
# Thu, 29 Apr 2021 17:10:06 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 29 Apr 2021 17:10:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 29 Apr 2021 17:10:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Apr 2021 17:10:09 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:09ea659ba566d9c3c62493e5ae0b964f1eee4fcf35aabc91c5c34ca1ad686541`  
		Last Modified: Sat, 10 Apr 2021 01:16:07 GMT  
		Size: 25.8 MB (25806410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10fa5ae1be1fc686c91c15f24ebaaa72d7c4f64321c8ead8386f2f4f9d1a6705`  
		Last Modified: Sat, 10 Apr 2021 01:53:41 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d821f4c7e565a8e4288ffdec5499d4f1fe177393fe2d5774b1e1686ad7257454`  
		Last Modified: Thu, 29 Apr 2021 17:10:49 GMT  
		Size: 8.9 MB (8870513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee294f8c5e00b4207daece747b1984cebe038c75bcb99fde4df34f9d072accff`  
		Last Modified: Thu, 29 Apr 2021 17:10:43 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1327b763af1d0b3e237e5a65eb7a20370ad3bc1a2e5e2d07d6f4a2d7dd217d2`  
		Last Modified: Thu, 29 Apr 2021 17:10:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2` - linux; ppc64le

```console
$ docker pull haproxy@sha256:5f6c4cd389f0eef07efa70a7b79e9034d39ad81308ee3d22b593b48c6e72038f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40323271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0525e4e75533190906a3a3b8fa4c13980187b37c0fe09a98b7d0248ee064c11f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:26:49 GMT
ADD file:ab87d4854aa8628ce8f4e603c0496499f6f28c3d2525ace782c7369691dafc8c in / 
# Sat, 10 Apr 2021 01:26:56 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 04:45:12 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 29 Apr 2021 17:21:53 GMT
ENV HAPROXY_VERSION=2.2.14
# Thu, 29 Apr 2021 17:22:05 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Thu, 29 Apr 2021 17:22:10 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Thu, 29 Apr 2021 17:28:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 29 Apr 2021 17:28:11 GMT
STOPSIGNAL SIGUSR1
# Thu, 29 Apr 2021 17:28:14 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 29 Apr 2021 17:28:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 29 Apr 2021 17:28:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Apr 2021 17:28:35 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:3e1e599482ca47095f85e429b346b76375aa85015ddcca050e85c2a8b1fdda9c`  
		Last Modified: Sat, 10 Apr 2021 01:33:57 GMT  
		Size: 30.5 MB (30545933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ee41bdc57145d3cb6e9f5fa23eed213567ae52835c7cff5fd57fe17b52f5ec`  
		Last Modified: Sat, 10 Apr 2021 05:09:50 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0318a9e0dfae38a427df09950040ec8ac49b3411281c6f4e916df64f3e61a1db`  
		Last Modified: Thu, 29 Apr 2021 17:32:41 GMT  
		Size: 9.8 MB (9775378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15d770c2ff18b8d626e68154c643956016ba3c2bc473db0cf4fe67933eae8e02`  
		Last Modified: Thu, 29 Apr 2021 17:32:39 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ffc03968d4104b120ffb831618293d3c01a3b52a20190f19139d4c400d8dfbd`  
		Last Modified: Thu, 29 Apr 2021 17:32:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2` - linux; s390x

```console
$ docker pull haproxy@sha256:17be434f2b9d7eac603cd7e9d94facfdcc2fcc5547c8b01296254dcfef495242
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34763982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e69d8b1385df56238043045e64f64848efde120e4d71c13431aae7e3647c2ade`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:42:23 GMT
ADD file:dbe2182f8699f2a6011413ea01862e6c0e85853d922dffd72a28d994d23c79bc in / 
# Sat, 10 Apr 2021 00:42:25 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:38:04 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 29 Apr 2021 17:42:25 GMT
ENV HAPROXY_VERSION=2.2.14
# Thu, 29 Apr 2021 17:42:26 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Thu, 29 Apr 2021 17:42:26 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Thu, 29 Apr 2021 17:43:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 29 Apr 2021 17:43:05 GMT
STOPSIGNAL SIGUSR1
# Thu, 29 Apr 2021 17:43:05 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 29 Apr 2021 17:43:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 29 Apr 2021 17:43:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Apr 2021 17:43:07 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:65291f8717b3afd99b63cee867dd3e06b956a8ee6aa8580cc31d913b25de209d`  
		Last Modified: Sat, 10 Apr 2021 00:45:48 GMT  
		Size: 25.8 MB (25753787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9daf67acfb0373e31068762d068f1da8d320f2bdcdb0e6651d52b8183ede06c`  
		Last Modified: Sat, 10 Apr 2021 01:42:28 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:139203a6eacdb0e49cca6af7b193a9727084d9bc018c6c38ecd8e2a70cb4a783`  
		Last Modified: Thu, 29 Apr 2021 17:45:08 GMT  
		Size: 9.0 MB (9008246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22c7c9f250fa0d85359a600dcf6c221949890728910221bf04f9c0550d07f099`  
		Last Modified: Thu, 29 Apr 2021 17:45:07 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b818bccdd69e5cc08f3856520e9beff9d06adaba69bf8fd2820f502abfb90785`  
		Last Modified: Thu, 29 Apr 2021 17:45:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.2-alpine`

```console
$ docker pull haproxy@sha256:865331c119b8c88d15add5b94d0a793e7cd24e273dd520d4b025db6c3797f09b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `haproxy:2.2-alpine` - linux; amd64

```console
$ docker pull haproxy@sha256:351e8b45533cf4c752df579566bf71b8550d984d7b8446e7b8f1c9e511aeb44d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.2 MB (9187819 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04679647ccf7dcdaab910fb8b498a41b5f3526f696fd5166913e56415d70469d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:37:38 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 29 Apr 2021 17:30:10 GMT
ENV HAPROXY_VERSION=2.2.14
# Thu, 29 Apr 2021 17:30:10 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Thu, 29 Apr 2021 17:30:10 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Thu, 29 Apr 2021 17:30:59 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 29 Apr 2021 17:30:59 GMT
STOPSIGNAL SIGUSR1
# Thu, 29 Apr 2021 17:31:00 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 29 Apr 2021 17:31:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 29 Apr 2021 17:31:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Apr 2021 17:31:01 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4de1862a29af271c1751bf0d03d96f9a881f971d1288c5fafcfba90b517611f8`  
		Last Modified: Wed, 14 Apr 2021 21:43:30 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9e43f525730a3c1a71396cd7d8c5e91c013eb29c0e704b13ebc56fa8899a9bc`  
		Last Modified: Thu, 29 Apr 2021 17:32:38 GMT  
		Size: 6.4 MB (6374100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd121de2e7dd938cb509db4091d6e0ad83358a944805a98b6e4802ae196993ef`  
		Last Modified: Thu, 29 Apr 2021 17:32:37 GMT  
		Size: 446.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0952e13028cb45fca71cc160a99915a21adef4382c5a6bdb0c19ac7f888a40f4`  
		Last Modified: Thu, 29 Apr 2021 17:32:37 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2-alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:2330b42228e3f150465089b56aac22e2b98e319f3e3a651b134e3448ef31ee56
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.9 MB (8878321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d063a6d463b78e25e558d428d98ef2c98534ba530b340819315d12988ef7663`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:18:05 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 29 Apr 2021 17:58:25 GMT
ENV HAPROXY_VERSION=2.2.14
# Thu, 29 Apr 2021 17:58:26 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Thu, 29 Apr 2021 17:58:27 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Thu, 29 Apr 2021 17:58:54 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 29 Apr 2021 17:58:55 GMT
STOPSIGNAL SIGUSR1
# Thu, 29 Apr 2021 17:58:56 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 29 Apr 2021 17:59:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 29 Apr 2021 17:59:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Apr 2021 17:59:02 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd640f0f76e4e434b444a36110041f2c571b2dbcfca29958b2e90de8d91bd6eb`  
		Last Modified: Wed, 14 Apr 2021 21:34:02 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5a1dc9635ed4e8266598b43a8021916179f6ecfe26de2edf6f79953d7a6e1ba`  
		Last Modified: Thu, 29 Apr 2021 17:59:44 GMT  
		Size: 6.3 MB (6254438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54b4242bd61d3ebbd2fad2003f9aca4578f035fa51317bd10ded15d1d150442b`  
		Last Modified: Thu, 29 Apr 2021 17:59:42 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5741f31a86fd77efec27f79f54cb17078972cc2ea2f6884988a7a88061925e7d`  
		Last Modified: Thu, 29 Apr 2021 17:59:42 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:b58792ba4c8509a690aed5c18aed41548b2cd4a7444f4db35c646b420d7fd26c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8597095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:795456a00fe0008d4a02f2102d502f563b1dcfeac231a327150652971276712c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:47:58 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 29 Apr 2021 17:00:50 GMT
ENV HAPROXY_VERSION=2.2.14
# Thu, 29 Apr 2021 17:00:51 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Thu, 29 Apr 2021 17:00:52 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Thu, 29 Apr 2021 17:01:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 29 Apr 2021 17:01:16 GMT
STOPSIGNAL SIGUSR1
# Thu, 29 Apr 2021 17:01:17 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 29 Apr 2021 17:01:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 29 Apr 2021 17:01:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Apr 2021 17:01:20 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ff0f6ee9305bed375c784c12ad4beeac3af6ea1a6b5afeec6b4700259dc194`  
		Last Modified: Wed, 14 Apr 2021 22:56:09 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b2ec0b1927bd1d10abbd183f6132825d56a5fe84af8e3151f57a917c6b0c5d9`  
		Last Modified: Thu, 29 Apr 2021 17:03:50 GMT  
		Size: 6.2 MB (6171196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a0891b95532486d3f61c8626238695b04ac750b83bfeff55ddde3c424f1e31`  
		Last Modified: Thu, 29 Apr 2021 17:03:48 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcff54d664dce91ddc63ae2a80ac409ec8ac4323aae79e24be2c04e30364696d`  
		Last Modified: Thu, 29 Apr 2021 17:03:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:ff7750eb3484161e61d6113d2d2a591d285dbefa94eb815da877505ebaec40b5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.1 MB (9093351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c05e833634dc19b1dcf0ec5b6028c9a6a444978ec1edf610425aabb2b4ac381`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:26:01 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 29 Apr 2021 17:53:12 GMT
ENV HAPROXY_VERSION=2.2.14
# Thu, 29 Apr 2021 17:53:13 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Thu, 29 Apr 2021 17:53:14 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Thu, 29 Apr 2021 17:53:39 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 29 Apr 2021 17:53:40 GMT
STOPSIGNAL SIGUSR1
# Thu, 29 Apr 2021 17:53:41 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 29 Apr 2021 17:53:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 29 Apr 2021 17:53:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Apr 2021 17:53:45 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2ef9646f93509fb43536690b645509d9b653316324583761dd086b8ad6c664`  
		Last Modified: Wed, 14 Apr 2021 20:37:52 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecd9d03f24e857a24819b3bffa319b1896aaf04d09ff657d37c44cbf02d870ad`  
		Last Modified: Thu, 29 Apr 2021 17:54:58 GMT  
		Size: 6.4 MB (6379570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a0e9150a4a249e0f658011c7421dbe8cb4f1797738ba92ac98be54f2929799`  
		Last Modified: Thu, 29 Apr 2021 17:54:57 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e7c49ac145b8b9f168fd85e531255cdc8ca36adcd9c5803471ffd3f12cae46`  
		Last Modified: Thu, 29 Apr 2021 17:54:56 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2-alpine` - linux; 386

```console
$ docker pull haproxy@sha256:ca89af1c1cadbb2c546bf88412cedd7d17e4321a4704e7c534f96e50b4a971c6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9028758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42bc524adf636565d4743200d86bce083eeac9b2e4bb6d1e352bc32a908d2132`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 01:50:06 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 29 Apr 2021 17:40:45 GMT
ENV HAPROXY_VERSION=2.2.14
# Thu, 29 Apr 2021 17:40:45 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Thu, 29 Apr 2021 17:40:46 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Thu, 29 Apr 2021 17:41:51 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 29 Apr 2021 17:41:51 GMT
STOPSIGNAL SIGUSR1
# Thu, 29 Apr 2021 17:41:51 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 29 Apr 2021 17:41:52 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 29 Apr 2021 17:41:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Apr 2021 17:41:53 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:31b7e7ccca9e17fd08b39c9a4ffd3ded380b62816c489d6c3758c9bb5a632430`  
		Last Modified: Wed, 14 Apr 2021 18:39:24 GMT  
		Size: 2.8 MB (2818900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9104145d2a6b1e0c0837c464bb9d4b331949cfeb6be12e4e7995507661d3386`  
		Last Modified: Thu, 15 Apr 2021 02:00:28 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c94b7b9918662e243b2f7d32c2c237339e594b90ea119f6bf77f9ac8c4818612`  
		Last Modified: Thu, 29 Apr 2021 17:44:41 GMT  
		Size: 6.2 MB (6208104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89684848b1dc6218657c706cb17469bca0fa286cecc489425b7464f52c770c24`  
		Last Modified: Thu, 29 Apr 2021 17:44:39 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7b3024bbac5c0f491b5e018476a95a61e4ae4a0ad09e826e696f7bceef5a6aa`  
		Last Modified: Thu, 29 Apr 2021 17:44:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2-alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:4d277cabca4bd41dd24d0d04f4cfed03d8988e0830a5c91b24d0a659873beb40
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9503527 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1aff090c2019485bed2a6d56748b9c1d5f909ab4737bb6c8961605abd9191be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:25:09 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 29 Apr 2021 17:29:01 GMT
ENV HAPROXY_VERSION=2.2.14
# Thu, 29 Apr 2021 17:29:18 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Thu, 29 Apr 2021 17:29:30 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Thu, 29 Apr 2021 17:30:26 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 29 Apr 2021 17:30:36 GMT
STOPSIGNAL SIGUSR1
# Thu, 29 Apr 2021 17:30:41 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 29 Apr 2021 17:30:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 29 Apr 2021 17:31:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Apr 2021 17:31:21 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8004273856b1b354059d03a17deec6e79d325ba45d63213dda3d1fa401db8c22`  
		Last Modified: Wed, 14 Apr 2021 23:36:37 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c35b3cdf32810f06f92fc72958c4454a52f6d0dff450335d1420cb5aff7bfb`  
		Last Modified: Thu, 29 Apr 2021 17:32:59 GMT  
		Size: 6.7 MB (6688630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d036ed22faa59df382b510ded6e6b8446ca3f41abfc5b68e85d60e39173ef4e`  
		Last Modified: Thu, 29 Apr 2021 17:32:58 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35d66a9c14deeb7ebd1d75c0aa9dd9d118abd71eb4a2f0762ca6e1daeeb4507`  
		Last Modified: Thu, 29 Apr 2021 17:32:58 GMT  
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

## `haproxy:2.2.14`

```console
$ docker pull haproxy@sha256:792ac7e9a42dcb028039bd6ec02cfdde75e94980652121e1fe557e7cf8b847bb
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

### `haproxy:2.2.14` - linux; amd64

```console
$ docker pull haproxy@sha256:6706d478e4e608c4d7aff4b100c029ed8ed5387f41f6d7d8b4b6ac9ecba3b745
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.5 MB (36450315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b71355e785ee76f43999ed2fa4612e47d61b76c61b3045c4d866b169b192bc99`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:29:42 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 29 Apr 2021 17:29:19 GMT
ENV HAPROXY_VERSION=2.2.14
# Thu, 29 Apr 2021 17:29:20 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Thu, 29 Apr 2021 17:29:20 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Thu, 29 Apr 2021 17:30:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 29 Apr 2021 17:30:04 GMT
STOPSIGNAL SIGUSR1
# Thu, 29 Apr 2021 17:30:04 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 29 Apr 2021 17:30:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 29 Apr 2021 17:30:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Apr 2021 17:30:06 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7abf58d954de379f38a19e07330116ba6b11f21007bc7b7507d233e5b0aa3fe0`  
		Last Modified: Sat, 10 Apr 2021 06:38:07 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ba487cb42887a026b3940ab5d25240db3ae8ca3538a433d33ded6c1e78ad946`  
		Last Modified: Thu, 29 Apr 2021 17:32:22 GMT  
		Size: 9.3 MB (9308992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f13a5faba9b80662ce1beda2cf0d30503c88a5569751155fd6d9fcfe6323ac46`  
		Last Modified: Thu, 29 Apr 2021 17:32:20 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3261bbc066b08611abdde75acf1a7a9a48c2d49f7540dcbc9a3c8e450ba4bd1b`  
		Last Modified: Thu, 29 Apr 2021 17:32:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.14` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:c36e6561bbe1be11cfd9b264eb760158871281895cdccacaa2aace07b64e704d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33788380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be71ea57166ad123cfb3dde36d0d110e554e5bbd5762aa5694b2903a5642af2a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:51:31 GMT
ADD file:926533a23a69aa2481a9122b667bb6300a347154eea366c9e679a230aa7f373a in / 
# Sat, 10 Apr 2021 00:51:34 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 02:24:17 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 29 Apr 2021 17:48:45 GMT
ENV HAPROXY_VERSION=2.2.14
# Thu, 29 Apr 2021 17:48:45 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Thu, 29 Apr 2021 17:48:46 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Thu, 29 Apr 2021 17:49:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 29 Apr 2021 17:49:35 GMT
STOPSIGNAL SIGUSR1
# Thu, 29 Apr 2021 17:49:36 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 29 Apr 2021 17:49:39 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 29 Apr 2021 17:49:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Apr 2021 17:49:40 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:33d77752597b664d047cc829e58a223d6fb077b61f69ca0462fcfb9b78d5f69b`  
		Last Modified: Sat, 10 Apr 2021 00:59:22 GMT  
		Size: 24.9 MB (24873199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c107a5973e1ce17cb311e2bf8a0d841875ca9f02219922ca12a9203602b5ce`  
		Last Modified: Sat, 10 Apr 2021 02:36:55 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a77f509b71668a040ff49cefb629a69b38b8703e98ed245bd0a97e97d10dc941`  
		Last Modified: Thu, 29 Apr 2021 17:50:22 GMT  
		Size: 8.9 MB (8913230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465b06ecb24dfbadcc493326bbf81d26de8a87e42dca5391cb9fcce5b693ce68`  
		Last Modified: Thu, 29 Apr 2021 17:50:19 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a57c7b8bed3c607d9c0e9cbe2d9e7538c16f5e02eb14d538227db37c7bb17e28`  
		Last Modified: Thu, 29 Apr 2021 17:50:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.14` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:f2d6692932a23d8178cadfbdc361c84a1f9dee4b7f0aeba65040899f65303432
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.5 MB (31464618 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7706d3cb80f141f9f889baea70aa79afc549e227e90bffd1aded90f5703bff2d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:59:45 GMT
ADD file:3fbd246a2de82566bcaaf62e3e0bf57175a7ad46b4156366a110661b31eab240 in / 
# Sat, 10 Apr 2021 00:59:47 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 08:58:51 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 29 Apr 2021 16:59:52 GMT
ENV HAPROXY_VERSION=2.2.14
# Thu, 29 Apr 2021 16:59:52 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Thu, 29 Apr 2021 16:59:53 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Thu, 29 Apr 2021 17:00:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 29 Apr 2021 17:00:35 GMT
STOPSIGNAL SIGUSR1
# Thu, 29 Apr 2021 17:00:36 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 29 Apr 2021 17:00:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 29 Apr 2021 17:00:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Apr 2021 17:00:41 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:8c6bea184b33030fb923c3c09d634b73235dec3fe2d411db9fd22bda669f2c37`  
		Last Modified: Sat, 10 Apr 2021 01:07:51 GMT  
		Size: 22.7 MB (22739801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5be95d3afdef3cc4c8a37695b513cf41e6cf6ffeecd9ce2426d38cb245a0b52`  
		Last Modified: Sat, 10 Apr 2021 09:05:25 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:110847a1cab7ee7d5910a3162e69e05dc4b27b38bbf0690fd5287335ca45d994`  
		Last Modified: Thu, 29 Apr 2021 17:02:34 GMT  
		Size: 8.7 MB (8722868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842fd9bf0561243131b85223fd2121bca335a34398de2805ce2bc49c20f0557f`  
		Last Modified: Thu, 29 Apr 2021 17:02:31 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba857cc76815a69804d81b7b8cfd1cef733d552360b462a6654bb997dc422b2`  
		Last Modified: Thu, 29 Apr 2021 17:02:31 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.14` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:a4de49115c06290f0365e78ccfc41c33ae5c7f54f069e8d5ad910d17cd00e1fb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.0 MB (35029567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c6269d7f5a3a3146d838cb1f3d9a89975b839613e3bc29493db15a8c91dd948`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:41:25 GMT
ADD file:b24da7eb23eeae04e00d0e45da29a89fe8f992e8dcf4ba482afb907b8015b7bf in / 
# Sat, 10 Apr 2021 00:41:28 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:13:29 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 29 Apr 2021 17:52:04 GMT
ENV HAPROXY_VERSION=2.2.14
# Thu, 29 Apr 2021 17:52:04 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Thu, 29 Apr 2021 17:52:05 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Thu, 29 Apr 2021 17:52:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 29 Apr 2021 17:52:49 GMT
STOPSIGNAL SIGUSR1
# Thu, 29 Apr 2021 17:52:50 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 29 Apr 2021 17:52:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 29 Apr 2021 17:52:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Apr 2021 17:52:57 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:15cb40b9c4df1a06940dc2a154c3be46844241235c1a091afa70da0ee2dc811a`  
		Last Modified: Sat, 10 Apr 2021 00:47:53 GMT  
		Size: 25.9 MB (25904582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48cb832c3e00ffed789c3f464caa612fe4996ba4683f72f8cf214d1437268efe`  
		Last Modified: Sat, 10 Apr 2021 01:21:27 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecd2d7073326e7be6f17459b1bdbdd24dbca7f0b483761cb137bb319170cdae9`  
		Last Modified: Thu, 29 Apr 2021 17:54:48 GMT  
		Size: 9.1 MB (9123034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af396c216cd462331785256c8eb8b58249a257388636dfba8957a6eea6563656`  
		Last Modified: Thu, 29 Apr 2021 17:54:46 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30df480ff08a19b3b653b87ddd425f40dfeee6416890092a6ee6f39c909f722c`  
		Last Modified: Thu, 29 Apr 2021 17:54:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.14` - linux; 386

```console
$ docker pull haproxy@sha256:481622045fb02fb6b31c3c1aac02351d13a0e075c2781dc0d8fe13ddf240a5b2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36980676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23f034ff44a4590fbde461f619710fc01edb99a36cdb948ffd62c756fe1566d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:39:42 GMT
ADD file:8885d4d13678543780bb04ba14b621179665f7951d5b261036a7092df9b376e7 in / 
# Sat, 10 Apr 2021 00:39:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 03:48:12 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 29 Apr 2021 17:39:19 GMT
ENV HAPROXY_VERSION=2.2.14
# Thu, 29 Apr 2021 17:39:19 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Thu, 29 Apr 2021 17:39:20 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Thu, 29 Apr 2021 17:40:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 29 Apr 2021 17:40:27 GMT
STOPSIGNAL SIGUSR1
# Thu, 29 Apr 2021 17:40:28 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 29 Apr 2021 17:40:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 29 Apr 2021 17:40:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Apr 2021 17:40:29 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:7cc57a8772e5e479618650dfa70f315b474d3f205d04bde7f602f469c1928d84`  
		Last Modified: Sat, 10 Apr 2021 00:46:07 GMT  
		Size: 27.8 MB (27788987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d92d68a52363235dcdfb59fa81e5ef1a4561c958501e4f28d6b79e86f8b8501`  
		Last Modified: Sat, 10 Apr 2021 03:59:08 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57229d188189b1e10cc3562b2ffd352969144dfbaf06988a920ed5427ed7906b`  
		Last Modified: Thu, 29 Apr 2021 17:44:22 GMT  
		Size: 9.2 MB (9189740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fb9373ea635024b72729ee73d1d659e91446280256d3fd21762b084584f4c88`  
		Last Modified: Thu, 29 Apr 2021 17:44:20 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a04207b362e717df1206194d656c8b158caffc32107bcd7131b746a848d033e6`  
		Last Modified: Thu, 29 Apr 2021 17:44:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.14` - linux; mips64le

```console
$ docker pull haproxy@sha256:e518728537a7d7a9887fad3713fcb11680b0da3376cc3b2ec13eec2655bc5ef4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34678876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2570ecec3e5c74b7b8d58abd69762b1d5ea1641ed6abbf3e8078fed1d1f82ba4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:09:40 GMT
ADD file:0c93801c4a3719dfd4c047d7f2f4d52bf463eba2ab875da1dc54dcc832aae20b in / 
# Sat, 10 Apr 2021 01:09:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:39:36 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 29 Apr 2021 17:07:40 GMT
ENV HAPROXY_VERSION=2.2.14
# Thu, 29 Apr 2021 17:07:40 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Thu, 29 Apr 2021 17:07:40 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Thu, 29 Apr 2021 17:10:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 29 Apr 2021 17:10:06 GMT
STOPSIGNAL SIGUSR1
# Thu, 29 Apr 2021 17:10:06 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 29 Apr 2021 17:10:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 29 Apr 2021 17:10:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Apr 2021 17:10:09 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:09ea659ba566d9c3c62493e5ae0b964f1eee4fcf35aabc91c5c34ca1ad686541`  
		Last Modified: Sat, 10 Apr 2021 01:16:07 GMT  
		Size: 25.8 MB (25806410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10fa5ae1be1fc686c91c15f24ebaaa72d7c4f64321c8ead8386f2f4f9d1a6705`  
		Last Modified: Sat, 10 Apr 2021 01:53:41 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d821f4c7e565a8e4288ffdec5499d4f1fe177393fe2d5774b1e1686ad7257454`  
		Last Modified: Thu, 29 Apr 2021 17:10:49 GMT  
		Size: 8.9 MB (8870513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee294f8c5e00b4207daece747b1984cebe038c75bcb99fde4df34f9d072accff`  
		Last Modified: Thu, 29 Apr 2021 17:10:43 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1327b763af1d0b3e237e5a65eb7a20370ad3bc1a2e5e2d07d6f4a2d7dd217d2`  
		Last Modified: Thu, 29 Apr 2021 17:10:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.14` - linux; ppc64le

```console
$ docker pull haproxy@sha256:5f6c4cd389f0eef07efa70a7b79e9034d39ad81308ee3d22b593b48c6e72038f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40323271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0525e4e75533190906a3a3b8fa4c13980187b37c0fe09a98b7d0248ee064c11f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:26:49 GMT
ADD file:ab87d4854aa8628ce8f4e603c0496499f6f28c3d2525ace782c7369691dafc8c in / 
# Sat, 10 Apr 2021 01:26:56 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 04:45:12 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 29 Apr 2021 17:21:53 GMT
ENV HAPROXY_VERSION=2.2.14
# Thu, 29 Apr 2021 17:22:05 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Thu, 29 Apr 2021 17:22:10 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Thu, 29 Apr 2021 17:28:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 29 Apr 2021 17:28:11 GMT
STOPSIGNAL SIGUSR1
# Thu, 29 Apr 2021 17:28:14 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 29 Apr 2021 17:28:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 29 Apr 2021 17:28:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Apr 2021 17:28:35 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:3e1e599482ca47095f85e429b346b76375aa85015ddcca050e85c2a8b1fdda9c`  
		Last Modified: Sat, 10 Apr 2021 01:33:57 GMT  
		Size: 30.5 MB (30545933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ee41bdc57145d3cb6e9f5fa23eed213567ae52835c7cff5fd57fe17b52f5ec`  
		Last Modified: Sat, 10 Apr 2021 05:09:50 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0318a9e0dfae38a427df09950040ec8ac49b3411281c6f4e916df64f3e61a1db`  
		Last Modified: Thu, 29 Apr 2021 17:32:41 GMT  
		Size: 9.8 MB (9775378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15d770c2ff18b8d626e68154c643956016ba3c2bc473db0cf4fe67933eae8e02`  
		Last Modified: Thu, 29 Apr 2021 17:32:39 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ffc03968d4104b120ffb831618293d3c01a3b52a20190f19139d4c400d8dfbd`  
		Last Modified: Thu, 29 Apr 2021 17:32:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.14` - linux; s390x

```console
$ docker pull haproxy@sha256:17be434f2b9d7eac603cd7e9d94facfdcc2fcc5547c8b01296254dcfef495242
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34763982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e69d8b1385df56238043045e64f64848efde120e4d71c13431aae7e3647c2ade`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:42:23 GMT
ADD file:dbe2182f8699f2a6011413ea01862e6c0e85853d922dffd72a28d994d23c79bc in / 
# Sat, 10 Apr 2021 00:42:25 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:38:04 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 29 Apr 2021 17:42:25 GMT
ENV HAPROXY_VERSION=2.2.14
# Thu, 29 Apr 2021 17:42:26 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Thu, 29 Apr 2021 17:42:26 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Thu, 29 Apr 2021 17:43:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 29 Apr 2021 17:43:05 GMT
STOPSIGNAL SIGUSR1
# Thu, 29 Apr 2021 17:43:05 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 29 Apr 2021 17:43:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 29 Apr 2021 17:43:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Apr 2021 17:43:07 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:65291f8717b3afd99b63cee867dd3e06b956a8ee6aa8580cc31d913b25de209d`  
		Last Modified: Sat, 10 Apr 2021 00:45:48 GMT  
		Size: 25.8 MB (25753787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9daf67acfb0373e31068762d068f1da8d320f2bdcdb0e6651d52b8183ede06c`  
		Last Modified: Sat, 10 Apr 2021 01:42:28 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:139203a6eacdb0e49cca6af7b193a9727084d9bc018c6c38ecd8e2a70cb4a783`  
		Last Modified: Thu, 29 Apr 2021 17:45:08 GMT  
		Size: 9.0 MB (9008246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22c7c9f250fa0d85359a600dcf6c221949890728910221bf04f9c0550d07f099`  
		Last Modified: Thu, 29 Apr 2021 17:45:07 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b818bccdd69e5cc08f3856520e9beff9d06adaba69bf8fd2820f502abfb90785`  
		Last Modified: Thu, 29 Apr 2021 17:45:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.2.14-alpine`

```console
$ docker pull haproxy@sha256:865331c119b8c88d15add5b94d0a793e7cd24e273dd520d4b025db6c3797f09b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `haproxy:2.2.14-alpine` - linux; amd64

```console
$ docker pull haproxy@sha256:351e8b45533cf4c752df579566bf71b8550d984d7b8446e7b8f1c9e511aeb44d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.2 MB (9187819 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04679647ccf7dcdaab910fb8b498a41b5f3526f696fd5166913e56415d70469d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:37:38 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 29 Apr 2021 17:30:10 GMT
ENV HAPROXY_VERSION=2.2.14
# Thu, 29 Apr 2021 17:30:10 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Thu, 29 Apr 2021 17:30:10 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Thu, 29 Apr 2021 17:30:59 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 29 Apr 2021 17:30:59 GMT
STOPSIGNAL SIGUSR1
# Thu, 29 Apr 2021 17:31:00 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 29 Apr 2021 17:31:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 29 Apr 2021 17:31:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Apr 2021 17:31:01 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4de1862a29af271c1751bf0d03d96f9a881f971d1288c5fafcfba90b517611f8`  
		Last Modified: Wed, 14 Apr 2021 21:43:30 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9e43f525730a3c1a71396cd7d8c5e91c013eb29c0e704b13ebc56fa8899a9bc`  
		Last Modified: Thu, 29 Apr 2021 17:32:38 GMT  
		Size: 6.4 MB (6374100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd121de2e7dd938cb509db4091d6e0ad83358a944805a98b6e4802ae196993ef`  
		Last Modified: Thu, 29 Apr 2021 17:32:37 GMT  
		Size: 446.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0952e13028cb45fca71cc160a99915a21adef4382c5a6bdb0c19ac7f888a40f4`  
		Last Modified: Thu, 29 Apr 2021 17:32:37 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.14-alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:2330b42228e3f150465089b56aac22e2b98e319f3e3a651b134e3448ef31ee56
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.9 MB (8878321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d063a6d463b78e25e558d428d98ef2c98534ba530b340819315d12988ef7663`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:18:05 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 29 Apr 2021 17:58:25 GMT
ENV HAPROXY_VERSION=2.2.14
# Thu, 29 Apr 2021 17:58:26 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Thu, 29 Apr 2021 17:58:27 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Thu, 29 Apr 2021 17:58:54 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 29 Apr 2021 17:58:55 GMT
STOPSIGNAL SIGUSR1
# Thu, 29 Apr 2021 17:58:56 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 29 Apr 2021 17:59:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 29 Apr 2021 17:59:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Apr 2021 17:59:02 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd640f0f76e4e434b444a36110041f2c571b2dbcfca29958b2e90de8d91bd6eb`  
		Last Modified: Wed, 14 Apr 2021 21:34:02 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5a1dc9635ed4e8266598b43a8021916179f6ecfe26de2edf6f79953d7a6e1ba`  
		Last Modified: Thu, 29 Apr 2021 17:59:44 GMT  
		Size: 6.3 MB (6254438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54b4242bd61d3ebbd2fad2003f9aca4578f035fa51317bd10ded15d1d150442b`  
		Last Modified: Thu, 29 Apr 2021 17:59:42 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5741f31a86fd77efec27f79f54cb17078972cc2ea2f6884988a7a88061925e7d`  
		Last Modified: Thu, 29 Apr 2021 17:59:42 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.14-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:b58792ba4c8509a690aed5c18aed41548b2cd4a7444f4db35c646b420d7fd26c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8597095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:795456a00fe0008d4a02f2102d502f563b1dcfeac231a327150652971276712c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:47:58 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 29 Apr 2021 17:00:50 GMT
ENV HAPROXY_VERSION=2.2.14
# Thu, 29 Apr 2021 17:00:51 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Thu, 29 Apr 2021 17:00:52 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Thu, 29 Apr 2021 17:01:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 29 Apr 2021 17:01:16 GMT
STOPSIGNAL SIGUSR1
# Thu, 29 Apr 2021 17:01:17 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 29 Apr 2021 17:01:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 29 Apr 2021 17:01:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Apr 2021 17:01:20 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ff0f6ee9305bed375c784c12ad4beeac3af6ea1a6b5afeec6b4700259dc194`  
		Last Modified: Wed, 14 Apr 2021 22:56:09 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b2ec0b1927bd1d10abbd183f6132825d56a5fe84af8e3151f57a917c6b0c5d9`  
		Last Modified: Thu, 29 Apr 2021 17:03:50 GMT  
		Size: 6.2 MB (6171196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a0891b95532486d3f61c8626238695b04ac750b83bfeff55ddde3c424f1e31`  
		Last Modified: Thu, 29 Apr 2021 17:03:48 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcff54d664dce91ddc63ae2a80ac409ec8ac4323aae79e24be2c04e30364696d`  
		Last Modified: Thu, 29 Apr 2021 17:03:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.14-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:ff7750eb3484161e61d6113d2d2a591d285dbefa94eb815da877505ebaec40b5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.1 MB (9093351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c05e833634dc19b1dcf0ec5b6028c9a6a444978ec1edf610425aabb2b4ac381`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:26:01 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 29 Apr 2021 17:53:12 GMT
ENV HAPROXY_VERSION=2.2.14
# Thu, 29 Apr 2021 17:53:13 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Thu, 29 Apr 2021 17:53:14 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Thu, 29 Apr 2021 17:53:39 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 29 Apr 2021 17:53:40 GMT
STOPSIGNAL SIGUSR1
# Thu, 29 Apr 2021 17:53:41 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 29 Apr 2021 17:53:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 29 Apr 2021 17:53:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Apr 2021 17:53:45 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2ef9646f93509fb43536690b645509d9b653316324583761dd086b8ad6c664`  
		Last Modified: Wed, 14 Apr 2021 20:37:52 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecd9d03f24e857a24819b3bffa319b1896aaf04d09ff657d37c44cbf02d870ad`  
		Last Modified: Thu, 29 Apr 2021 17:54:58 GMT  
		Size: 6.4 MB (6379570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a0e9150a4a249e0f658011c7421dbe8cb4f1797738ba92ac98be54f2929799`  
		Last Modified: Thu, 29 Apr 2021 17:54:57 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e7c49ac145b8b9f168fd85e531255cdc8ca36adcd9c5803471ffd3f12cae46`  
		Last Modified: Thu, 29 Apr 2021 17:54:56 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.14-alpine` - linux; 386

```console
$ docker pull haproxy@sha256:ca89af1c1cadbb2c546bf88412cedd7d17e4321a4704e7c534f96e50b4a971c6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9028758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42bc524adf636565d4743200d86bce083eeac9b2e4bb6d1e352bc32a908d2132`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 01:50:06 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 29 Apr 2021 17:40:45 GMT
ENV HAPROXY_VERSION=2.2.14
# Thu, 29 Apr 2021 17:40:45 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Thu, 29 Apr 2021 17:40:46 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Thu, 29 Apr 2021 17:41:51 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 29 Apr 2021 17:41:51 GMT
STOPSIGNAL SIGUSR1
# Thu, 29 Apr 2021 17:41:51 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 29 Apr 2021 17:41:52 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 29 Apr 2021 17:41:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Apr 2021 17:41:53 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:31b7e7ccca9e17fd08b39c9a4ffd3ded380b62816c489d6c3758c9bb5a632430`  
		Last Modified: Wed, 14 Apr 2021 18:39:24 GMT  
		Size: 2.8 MB (2818900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9104145d2a6b1e0c0837c464bb9d4b331949cfeb6be12e4e7995507661d3386`  
		Last Modified: Thu, 15 Apr 2021 02:00:28 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c94b7b9918662e243b2f7d32c2c237339e594b90ea119f6bf77f9ac8c4818612`  
		Last Modified: Thu, 29 Apr 2021 17:44:41 GMT  
		Size: 6.2 MB (6208104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89684848b1dc6218657c706cb17469bca0fa286cecc489425b7464f52c770c24`  
		Last Modified: Thu, 29 Apr 2021 17:44:39 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7b3024bbac5c0f491b5e018476a95a61e4ae4a0ad09e826e696f7bceef5a6aa`  
		Last Modified: Thu, 29 Apr 2021 17:44:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.14-alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:4d277cabca4bd41dd24d0d04f4cfed03d8988e0830a5c91b24d0a659873beb40
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9503527 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1aff090c2019485bed2a6d56748b9c1d5f909ab4737bb6c8961605abd9191be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:25:09 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 29 Apr 2021 17:29:01 GMT
ENV HAPROXY_VERSION=2.2.14
# Thu, 29 Apr 2021 17:29:18 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Thu, 29 Apr 2021 17:29:30 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Thu, 29 Apr 2021 17:30:26 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 29 Apr 2021 17:30:36 GMT
STOPSIGNAL SIGUSR1
# Thu, 29 Apr 2021 17:30:41 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 29 Apr 2021 17:30:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 29 Apr 2021 17:31:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Apr 2021 17:31:21 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8004273856b1b354059d03a17deec6e79d325ba45d63213dda3d1fa401db8c22`  
		Last Modified: Wed, 14 Apr 2021 23:36:37 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c35b3cdf32810f06f92fc72958c4454a52f6d0dff450335d1420cb5aff7bfb`  
		Last Modified: Thu, 29 Apr 2021 17:32:59 GMT  
		Size: 6.7 MB (6688630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d036ed22faa59df382b510ded6e6b8446ca3f41abfc5b68e85d60e39173ef4e`  
		Last Modified: Thu, 29 Apr 2021 17:32:58 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35d66a9c14deeb7ebd1d75c0aa9dd9d118abd71eb4a2f0762ca6e1daeeb4507`  
		Last Modified: Thu, 29 Apr 2021 17:32:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.14-alpine` - linux; s390x

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

## `haproxy:2.3`

```console
$ docker pull haproxy@sha256:afbda854ad4e4dc64b71a98f6d185e27758cbc1580549445e27126081dba8f8e
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

### `haproxy:2.3` - linux; amd64

```console
$ docker pull haproxy@sha256:37c2ffe40f2f485a870f13f6974fd2d58c882da58776829612cdc845b595d0e9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.7 MB (36697077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:058875cd29c9463c410c2b570b5af60359322f5eed84da753c5afb0b9d98494b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:29:42 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 23 Apr 2021 20:19:56 GMT
ENV HAPROXY_VERSION=2.3.10
# Fri, 23 Apr 2021 20:19:56 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Fri, 23 Apr 2021 20:19:57 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Fri, 23 Apr 2021 20:20:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 23 Apr 2021 20:20:41 GMT
STOPSIGNAL SIGUSR1
# Fri, 23 Apr 2021 20:20:41 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 23 Apr 2021 20:20:42 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 20:20:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 20:20:42 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7abf58d954de379f38a19e07330116ba6b11f21007bc7b7507d233e5b0aa3fe0`  
		Last Modified: Sat, 10 Apr 2021 06:38:07 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afffe9e17aa10b7f5f89d5f5d2b55dc515f8d762cff20d4a2af6ee4415c875da`  
		Last Modified: Fri, 23 Apr 2021 20:22:40 GMT  
		Size: 9.6 MB (9555753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feae1ae443ea753af3373bfd3a522884ab6700544ff8f21c34be1b038eaa9902`  
		Last Modified: Fri, 23 Apr 2021 20:22:40 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23c1d2a159159248851cd19c28b4aed4acde0c87c647d8e057f2d8ddf3cfc2d`  
		Last Modified: Fri, 23 Apr 2021 20:22:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:f432474954fa25c79340f43b57a02e67903eeafa948d1a5aef55cf66f0a30a49
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (34041416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49787d7d5fd3a955e3efdfbe4783c4001482725f7815058b0c46eaeb6f9b44b5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:51:31 GMT
ADD file:926533a23a69aa2481a9122b667bb6300a347154eea366c9e679a230aa7f373a in / 
# Sat, 10 Apr 2021 00:51:34 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 02:24:17 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 23 Apr 2021 20:48:40 GMT
ENV HAPROXY_VERSION=2.3.10
# Fri, 23 Apr 2021 20:48:40 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Fri, 23 Apr 2021 20:48:41 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Fri, 23 Apr 2021 20:49:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 23 Apr 2021 20:49:26 GMT
STOPSIGNAL SIGUSR1
# Fri, 23 Apr 2021 20:49:28 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 23 Apr 2021 20:49:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 20:49:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 20:49:33 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:33d77752597b664d047cc829e58a223d6fb077b61f69ca0462fcfb9b78d5f69b`  
		Last Modified: Sat, 10 Apr 2021 00:59:22 GMT  
		Size: 24.9 MB (24873199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c107a5973e1ce17cb311e2bf8a0d841875ca9f02219922ca12a9203602b5ce`  
		Last Modified: Sat, 10 Apr 2021 02:36:55 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4fd166622140d354f76734dca13311daf08f4b0e1a2bd667bd8f1237147d592`  
		Last Modified: Fri, 23 Apr 2021 20:50:23 GMT  
		Size: 9.2 MB (9166265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6683d8d529358b8fd7297f933059372813f6a97b67c13987e9e309aeb63e9d7`  
		Last Modified: Fri, 23 Apr 2021 20:50:20 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2740aff641d0d26151406fb76c73059f6f37d65543141d4a46600055c477dbce`  
		Last Modified: Fri, 23 Apr 2021 20:50:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:049069171782a5ea16bc2052ee484dd63b650e108f9e48db799e55c667ee9d29
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31771359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d474b012eeaa8b00ec45f00f784bdaff3606013979b8ed2c920d960e1a6e5c0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:59:45 GMT
ADD file:3fbd246a2de82566bcaaf62e3e0bf57175a7ad46b4156366a110661b31eab240 in / 
# Sat, 10 Apr 2021 00:59:47 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 08:58:51 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 23 Apr 2021 20:59:31 GMT
ENV HAPROXY_VERSION=2.3.10
# Fri, 23 Apr 2021 20:59:31 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Fri, 23 Apr 2021 20:59:32 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Fri, 23 Apr 2021 21:00:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 23 Apr 2021 21:00:18 GMT
STOPSIGNAL SIGUSR1
# Fri, 23 Apr 2021 21:00:18 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 23 Apr 2021 21:00:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 21:00:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 21:00:25 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:8c6bea184b33030fb923c3c09d634b73235dec3fe2d411db9fd22bda669f2c37`  
		Last Modified: Sat, 10 Apr 2021 01:07:51 GMT  
		Size: 22.7 MB (22739801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5be95d3afdef3cc4c8a37695b513cf41e6cf6ffeecd9ce2426d38cb245a0b52`  
		Last Modified: Sat, 10 Apr 2021 09:05:25 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717bc5365fb4bcdb4738770e1f312f2f58a06135e8d00643b6eb56fc013fcfe2`  
		Last Modified: Fri, 23 Apr 2021 21:02:42 GMT  
		Size: 9.0 MB (9029609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3f9836ad3bdc29bcf6b0ea0ca6e1478d1348e1015e7dd6ba91a44f8c523a050`  
		Last Modified: Fri, 23 Apr 2021 21:02:39 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:724e48ed89849e1da6018edaf2c357f02df92850ddb50bf446da7b127792dab7`  
		Last Modified: Fri, 23 Apr 2021 21:02:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:62ef02fde66dea080deea6a17011711125171d1448d475c118f9ea2d691a42be
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.4 MB (35351171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9426ad19c62950e93ccf52c6f26ea94f779739576a8b938e340b22015a08a527`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:41:25 GMT
ADD file:b24da7eb23eeae04e00d0e45da29a89fe8f992e8dcf4ba482afb907b8015b7bf in / 
# Sat, 10 Apr 2021 00:41:28 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:13:29 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 23 Apr 2021 20:40:21 GMT
ENV HAPROXY_VERSION=2.3.10
# Fri, 23 Apr 2021 20:40:22 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Fri, 23 Apr 2021 20:40:22 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Fri, 23 Apr 2021 20:41:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 23 Apr 2021 20:41:03 GMT
STOPSIGNAL SIGUSR1
# Fri, 23 Apr 2021 20:41:04 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 23 Apr 2021 20:41:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 20:41:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 20:41:07 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:15cb40b9c4df1a06940dc2a154c3be46844241235c1a091afa70da0ee2dc811a`  
		Last Modified: Sat, 10 Apr 2021 00:47:53 GMT  
		Size: 25.9 MB (25904582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48cb832c3e00ffed789c3f464caa612fe4996ba4683f72f8cf214d1437268efe`  
		Last Modified: Sat, 10 Apr 2021 01:21:27 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99a4194f9c3742aa2f14d298181297121bb2c902d5eec8249de7c2ccb315d34`  
		Last Modified: Fri, 23 Apr 2021 20:43:01 GMT  
		Size: 9.4 MB (9444636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18eb1616784d5ffc7039165a0a02e92e1d9db3d88f8746a790b2558cd40a4974`  
		Last Modified: Fri, 23 Apr 2021 20:42:58 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baadd6b3908aad2d6176197c1816634a6271f00ce248db43ac40027449ababa2`  
		Last Modified: Fri, 23 Apr 2021 20:42:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3` - linux; 386

```console
$ docker pull haproxy@sha256:31390a54f68d62f3e7c80af3ddd2feb656e92553aa50acba7af43a06dcd5b560
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.2 MB (37209592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cf7eddc35247bbe2921775551965d6f38dbf1ee3be73cfb9f6544aaea2db502`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:39:42 GMT
ADD file:8885d4d13678543780bb04ba14b621179665f7951d5b261036a7092df9b376e7 in / 
# Sat, 10 Apr 2021 00:39:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 03:48:12 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 23 Apr 2021 20:38:45 GMT
ENV HAPROXY_VERSION=2.3.10
# Fri, 23 Apr 2021 20:38:45 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Fri, 23 Apr 2021 20:38:46 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Fri, 23 Apr 2021 20:39:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 23 Apr 2021 20:39:35 GMT
STOPSIGNAL SIGUSR1
# Fri, 23 Apr 2021 20:39:35 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 23 Apr 2021 20:39:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 20:39:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 20:39:36 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:7cc57a8772e5e479618650dfa70f315b474d3f205d04bde7f602f469c1928d84`  
		Last Modified: Sat, 10 Apr 2021 00:46:07 GMT  
		Size: 27.8 MB (27788987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d92d68a52363235dcdfb59fa81e5ef1a4561c958501e4f28d6b79e86f8b8501`  
		Last Modified: Sat, 10 Apr 2021 03:59:08 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c799704f6f7241fe4fe9658644a136f7f3a32cde54d58f63d2271c65f604e88`  
		Last Modified: Fri, 23 Apr 2021 20:42:36 GMT  
		Size: 9.4 MB (9418656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59f1328c2bd9da85a0836e5fd35839fdec1c3e22e0e5c30650827a10891c0ba7`  
		Last Modified: Fri, 23 Apr 2021 20:42:34 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:525b4de4d515d0e1e55046e2b12bc6368f5821f6c311a7bb5e2af64beca2282d`  
		Last Modified: Fri, 23 Apr 2021 20:42:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3` - linux; mips64le

```console
$ docker pull haproxy@sha256:e40a773567ecc6a0378962548f266a89f0651c1f7dc8c1b2a3ca5e2f984fb7c0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.9 MB (34943218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:609cf796bed6fbe5ca0f3ae499bf6d7a955768064cb0d180a60131050dd6fa35`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:09:40 GMT
ADD file:0c93801c4a3719dfd4c047d7f2f4d52bf463eba2ab875da1dc54dcc832aae20b in / 
# Sat, 10 Apr 2021 01:09:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:39:36 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 23 Apr 2021 20:07:26 GMT
ENV HAPROXY_VERSION=2.3.10
# Fri, 23 Apr 2021 20:07:26 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Fri, 23 Apr 2021 20:07:26 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Fri, 23 Apr 2021 20:09:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 23 Apr 2021 20:09:50 GMT
STOPSIGNAL SIGUSR1
# Fri, 23 Apr 2021 20:09:50 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 23 Apr 2021 20:09:52 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 20:09:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 20:09:53 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:09ea659ba566d9c3c62493e5ae0b964f1eee4fcf35aabc91c5c34ca1ad686541`  
		Last Modified: Sat, 10 Apr 2021 01:16:07 GMT  
		Size: 25.8 MB (25806410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10fa5ae1be1fc686c91c15f24ebaaa72d7c4f64321c8ead8386f2f4f9d1a6705`  
		Last Modified: Sat, 10 Apr 2021 01:53:41 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c195a6aaaf12a34216b2d8aca52aa55b0f937fd8618100d1e0e08d9c6f43d8b0`  
		Last Modified: Fri, 23 Apr 2021 20:10:38 GMT  
		Size: 9.1 MB (9134856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba9d4d0ca44a4f5b7349bbea2e1e64c1d3fa001ef5d09b38f803eebe6bcfffb`  
		Last Modified: Fri, 23 Apr 2021 20:10:31 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:725b140d9e91c81a346e8cf6395c2058a6c206f327ef7ec6ecc36e2542838887`  
		Last Modified: Fri, 23 Apr 2021 20:10:31 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3` - linux; ppc64le

```console
$ docker pull haproxy@sha256:ff52706fced2f786b64882c9d1e94ed5284c38c042c0e693e4ed87d7dc33c0c5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40589965 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd48e104b02ba284aa5985fd56e31c4bbf1689501afe8a8cfc5aaa1967626fc5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:26:49 GMT
ADD file:ab87d4854aa8628ce8f4e603c0496499f6f28c3d2525ace782c7369691dafc8c in / 
# Sat, 10 Apr 2021 01:26:56 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 04:45:12 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 23 Apr 2021 20:18:41 GMT
ENV HAPROXY_VERSION=2.3.10
# Fri, 23 Apr 2021 20:18:49 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Fri, 23 Apr 2021 20:18:54 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Fri, 23 Apr 2021 20:22:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 23 Apr 2021 20:22:51 GMT
STOPSIGNAL SIGUSR1
# Fri, 23 Apr 2021 20:22:53 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 23 Apr 2021 20:23:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 20:23:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 20:23:06 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:3e1e599482ca47095f85e429b346b76375aa85015ddcca050e85c2a8b1fdda9c`  
		Last Modified: Sat, 10 Apr 2021 01:33:57 GMT  
		Size: 30.5 MB (30545933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ee41bdc57145d3cb6e9f5fa23eed213567ae52835c7cff5fd57fe17b52f5ec`  
		Last Modified: Sat, 10 Apr 2021 05:09:50 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c841a7f82bff751f994b8799d674c7d4211251a43359351397999911cfa870`  
		Last Modified: Fri, 23 Apr 2021 20:25:56 GMT  
		Size: 10.0 MB (10042073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4641283e776afb6c306c0a6965f7e0b1238d91bc09f304ea32545464581a9f6`  
		Last Modified: Fri, 23 Apr 2021 20:25:53 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5248644a4705a96ac93d3ebbb06d89ed62a29bf7ae76226a7a3fd7cd388554b9`  
		Last Modified: Fri, 23 Apr 2021 20:25:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3` - linux; s390x

```console
$ docker pull haproxy@sha256:65f0248af9b095156adf78d96f4f792c03a87cb2277ef4c8f36d44333921625a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.0 MB (35046751 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84ba273a498e9d8f8422051771b73d62e5f4fedd88d8b5ef771f73d069b6af0f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:42:23 GMT
ADD file:dbe2182f8699f2a6011413ea01862e6c0e85853d922dffd72a28d994d23c79bc in / 
# Sat, 10 Apr 2021 00:42:25 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:38:04 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 23 Apr 2021 20:41:50 GMT
ENV HAPROXY_VERSION=2.3.10
# Fri, 23 Apr 2021 20:41:51 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Fri, 23 Apr 2021 20:41:51 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Fri, 23 Apr 2021 20:42:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 23 Apr 2021 20:42:54 GMT
STOPSIGNAL SIGUSR1
# Fri, 23 Apr 2021 20:42:54 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 23 Apr 2021 20:42:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 20:42:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 20:42:57 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:65291f8717b3afd99b63cee867dd3e06b956a8ee6aa8580cc31d913b25de209d`  
		Last Modified: Sat, 10 Apr 2021 00:45:48 GMT  
		Size: 25.8 MB (25753787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9daf67acfb0373e31068762d068f1da8d320f2bdcdb0e6651d52b8183ede06c`  
		Last Modified: Sat, 10 Apr 2021 01:42:28 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e00467b5656b09a7387dfd6e3adb3b30d4e7bddcaad2d25e8e422f7dcce2a58f`  
		Last Modified: Fri, 23 Apr 2021 20:45:10 GMT  
		Size: 9.3 MB (9291015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd5ec62c92ca691a7dd3e4602bad6d4be9d23dcd5d2f7420b30100f6b361cdbe`  
		Last Modified: Fri, 23 Apr 2021 20:45:09 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670261f5947e500477b59eac7f9966e7e1d4eae57a4132c42252790506139977`  
		Last Modified: Fri, 23 Apr 2021 20:45:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.3-alpine`

```console
$ docker pull haproxy@sha256:1168dcda566f7ce42120fe56135178d78752e7d198b4f96a77c00f1b06af1853
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `haproxy:2.3-alpine` - linux; amd64

```console
$ docker pull haproxy@sha256:6d16465fe404f162ffcfd564eea2774ba06edf7188280484a270cd8862c35a88
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9501835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77414e3b99078b756a62667c18c85f4359518b1610a2cc6f57d682ce7a4f3bb2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:37:38 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 23 Apr 2021 20:20:47 GMT
ENV HAPROXY_VERSION=2.3.10
# Fri, 23 Apr 2021 20:20:47 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Fri, 23 Apr 2021 20:20:47 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Fri, 23 Apr 2021 20:21:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 23 Apr 2021 20:21:37 GMT
STOPSIGNAL SIGUSR1
# Fri, 23 Apr 2021 20:21:37 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 23 Apr 2021 20:21:38 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 20:21:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 20:21:38 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4de1862a29af271c1751bf0d03d96f9a881f971d1288c5fafcfba90b517611f8`  
		Last Modified: Wed, 14 Apr 2021 21:43:30 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cba67cd0abe26102179dbd1deb88405bc4764e51a2b1f6ef06232cb9eca0ce6`  
		Last Modified: Fri, 23 Apr 2021 20:22:54 GMT  
		Size: 6.7 MB (6688111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:500b344a0df360398223362751a2ceab4c0981e06e375ff45905d04507537387`  
		Last Modified: Fri, 23 Apr 2021 20:22:53 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2724c9435ec936799a1c47edd9cb5e46f597d30b3e3cab7b0e32d855741fabb`  
		Last Modified: Fri, 23 Apr 2021 20:22:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3-alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:7e27a3587e72e37010d991363a75b6cc01493a686a23ed0a8a780a49c6ee2494
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.2 MB (9211848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1aec7a3cb069441d455cdee3c8970689988845ee8742770933e8b091a05a52e0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:18:05 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 23 Apr 2021 20:51:06 GMT
ENV HAPROXY_VERSION=2.3.10
# Fri, 23 Apr 2021 20:51:07 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Fri, 23 Apr 2021 20:51:08 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Fri, 23 Apr 2021 20:51:33 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 23 Apr 2021 20:51:35 GMT
STOPSIGNAL SIGUSR1
# Fri, 23 Apr 2021 20:51:35 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 23 Apr 2021 20:51:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 20:51:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 20:51:39 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd640f0f76e4e434b444a36110041f2c571b2dbcfca29958b2e90de8d91bd6eb`  
		Last Modified: Wed, 14 Apr 2021 21:34:02 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54049885ecd472a5548c06de21ae362a2dde172e52f8118579b63d389c596214`  
		Last Modified: Fri, 23 Apr 2021 20:52:23 GMT  
		Size: 6.6 MB (6587961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa68a40a7e61b9513c658b23339f17a1e97ed7660b0c9828c04b65f3fb8ae637`  
		Last Modified: Fri, 23 Apr 2021 20:52:20 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dba2abb2f77db1891b207f81dcc8f6f93862222a15a489e3f153d999d8d6bfb`  
		Last Modified: Fri, 23 Apr 2021 20:52:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:849282abf73b940f2e28483aea32e03a54075b7dbc6714d00412742327a88b5e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.9 MB (8927012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbb9ef13943f7a6fced52d987a05ef61afbdd96efb69d6f263810cb54037b990`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:47:58 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 23 Apr 2021 21:00:39 GMT
ENV HAPROXY_VERSION=2.3.10
# Fri, 23 Apr 2021 21:00:39 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Fri, 23 Apr 2021 21:00:40 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Fri, 23 Apr 2021 21:01:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 23 Apr 2021 21:01:10 GMT
STOPSIGNAL SIGUSR1
# Fri, 23 Apr 2021 21:01:11 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 23 Apr 2021 21:01:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 21:01:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 21:01:21 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ff0f6ee9305bed375c784c12ad4beeac3af6ea1a6b5afeec6b4700259dc194`  
		Last Modified: Wed, 14 Apr 2021 22:56:09 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb1d6019b6548f16be0cfff81a3a38f64337636d40ec6d50697915983ca3887f`  
		Last Modified: Fri, 23 Apr 2021 21:02:54 GMT  
		Size: 6.5 MB (6501111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e17ccc0c26b79d4583ef2907084a53e7a69a87686939491984151ac2ead75b1`  
		Last Modified: Fri, 23 Apr 2021 21:02:52 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f451a3dd3dd7b108fdbe462194e6659be8f76b7a69911c306d74d8fceeed3f`  
		Last Modified: Fri, 23 Apr 2021 21:02:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:ec0989fc82ace88b5cf80c0dc55e695e5a5d6620174e4ed0d5d8c1634630f2e7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9413982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cd73593d809a141875771ab3f582e9a6258ba6fe0f4b707f0ce439cd47a7405`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:26:01 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 23 Apr 2021 20:41:19 GMT
ENV HAPROXY_VERSION=2.3.10
# Fri, 23 Apr 2021 20:41:19 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Fri, 23 Apr 2021 20:41:20 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Fri, 23 Apr 2021 20:41:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 23 Apr 2021 20:41:44 GMT
STOPSIGNAL SIGUSR1
# Fri, 23 Apr 2021 20:41:45 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 23 Apr 2021 20:41:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 20:41:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 20:41:48 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2ef9646f93509fb43536690b645509d9b653316324583761dd086b8ad6c664`  
		Last Modified: Wed, 14 Apr 2021 20:37:52 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffe20dd6ddd5d14baec905dc0c113e8dd01ce5899588c89675a6988ccfe34a48`  
		Last Modified: Fri, 23 Apr 2021 20:43:13 GMT  
		Size: 6.7 MB (6700201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1616786188830f47d2d1ea30821c3aa828e4a87dbc5d075f5f6eee2c1fdaec`  
		Last Modified: Fri, 23 Apr 2021 20:43:09 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c147d090d4db064f2514f9bfa6a9cb2e6d716e448d94b4ab90e2b7a0e50ab03`  
		Last Modified: Fri, 23 Apr 2021 20:43:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3-alpine` - linux; 386

```console
$ docker pull haproxy@sha256:839a53bd7d2f00b0d67b1c764d9811b7491a3d4d645a6abb94ebd84293e4c367
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9356996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b30351ad929f3d405e1ca732a718c6e0fe63e1a52c2407a4d9600fff4e7e439b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 01:50:06 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 23 Apr 2021 20:39:47 GMT
ENV HAPROXY_VERSION=2.3.10
# Fri, 23 Apr 2021 20:39:47 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Fri, 23 Apr 2021 20:39:47 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Fri, 23 Apr 2021 20:40:45 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 23 Apr 2021 20:40:45 GMT
STOPSIGNAL SIGUSR1
# Fri, 23 Apr 2021 20:40:45 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 23 Apr 2021 20:40:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 20:40:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 20:40:47 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:31b7e7ccca9e17fd08b39c9a4ffd3ded380b62816c489d6c3758c9bb5a632430`  
		Last Modified: Wed, 14 Apr 2021 18:39:24 GMT  
		Size: 2.8 MB (2818900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9104145d2a6b1e0c0837c464bb9d4b331949cfeb6be12e4e7995507661d3386`  
		Last Modified: Thu, 15 Apr 2021 02:00:28 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22386ff451c9485cc86547597a9df94ba437d282baedc6b3ff68139348ab838e`  
		Last Modified: Fri, 23 Apr 2021 20:42:53 GMT  
		Size: 6.5 MB (6536340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44c782fb9ce01dfc03b5926dd9052609853265d68ef395e663ca422aba662667`  
		Last Modified: Fri, 23 Apr 2021 20:42:51 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eab34669a9636f82828df5502f0d94263605f7309e0bab880f3d9bc324b052b`  
		Last Modified: Fri, 23 Apr 2021 20:42:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3-alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:a4daa01e291804783faf44842f65f63d7108530d7623efce6d782952fe4bcbf9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.8 MB (9835818 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2ebb4297d3c174774a272e1f8a0042fc3c7c9ca7b1d0cf36d5af3d58b36005c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:25:09 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 23 Apr 2021 20:23:26 GMT
ENV HAPROXY_VERSION=2.3.10
# Fri, 23 Apr 2021 20:23:31 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Fri, 23 Apr 2021 20:23:34 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Fri, 23 Apr 2021 20:24:19 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 23 Apr 2021 20:24:24 GMT
STOPSIGNAL SIGUSR1
# Fri, 23 Apr 2021 20:24:27 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 23 Apr 2021 20:24:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 20:24:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 20:24:42 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8004273856b1b354059d03a17deec6e79d325ba45d63213dda3d1fa401db8c22`  
		Last Modified: Wed, 14 Apr 2021 23:36:37 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b9cdc9560132361ff8957311b5fd6b2bbacc8ec5be9489a16a3b3eea31f3d2`  
		Last Modified: Fri, 23 Apr 2021 20:26:10 GMT  
		Size: 7.0 MB (7020918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac490252619a4b1389b0e3fb3c472b84a443f9bc3d346558d7ac67596be3eb0`  
		Last Modified: Fri, 23 Apr 2021 20:26:11 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554ee7adacda14ba7a4c490cead3c19a063d98a21b022b06f60bff9e6089a817`  
		Last Modified: Fri, 23 Apr 2021 20:26:09 GMT  
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

## `haproxy:2.3.10`

```console
$ docker pull haproxy@sha256:afbda854ad4e4dc64b71a98f6d185e27758cbc1580549445e27126081dba8f8e
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

### `haproxy:2.3.10` - linux; amd64

```console
$ docker pull haproxy@sha256:37c2ffe40f2f485a870f13f6974fd2d58c882da58776829612cdc845b595d0e9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.7 MB (36697077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:058875cd29c9463c410c2b570b5af60359322f5eed84da753c5afb0b9d98494b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:29:42 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 23 Apr 2021 20:19:56 GMT
ENV HAPROXY_VERSION=2.3.10
# Fri, 23 Apr 2021 20:19:56 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Fri, 23 Apr 2021 20:19:57 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Fri, 23 Apr 2021 20:20:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 23 Apr 2021 20:20:41 GMT
STOPSIGNAL SIGUSR1
# Fri, 23 Apr 2021 20:20:41 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 23 Apr 2021 20:20:42 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 20:20:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 20:20:42 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7abf58d954de379f38a19e07330116ba6b11f21007bc7b7507d233e5b0aa3fe0`  
		Last Modified: Sat, 10 Apr 2021 06:38:07 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afffe9e17aa10b7f5f89d5f5d2b55dc515f8d762cff20d4a2af6ee4415c875da`  
		Last Modified: Fri, 23 Apr 2021 20:22:40 GMT  
		Size: 9.6 MB (9555753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feae1ae443ea753af3373bfd3a522884ab6700544ff8f21c34be1b038eaa9902`  
		Last Modified: Fri, 23 Apr 2021 20:22:40 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23c1d2a159159248851cd19c28b4aed4acde0c87c647d8e057f2d8ddf3cfc2d`  
		Last Modified: Fri, 23 Apr 2021 20:22:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.10` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:f432474954fa25c79340f43b57a02e67903eeafa948d1a5aef55cf66f0a30a49
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (34041416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49787d7d5fd3a955e3efdfbe4783c4001482725f7815058b0c46eaeb6f9b44b5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:51:31 GMT
ADD file:926533a23a69aa2481a9122b667bb6300a347154eea366c9e679a230aa7f373a in / 
# Sat, 10 Apr 2021 00:51:34 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 02:24:17 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 23 Apr 2021 20:48:40 GMT
ENV HAPROXY_VERSION=2.3.10
# Fri, 23 Apr 2021 20:48:40 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Fri, 23 Apr 2021 20:48:41 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Fri, 23 Apr 2021 20:49:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 23 Apr 2021 20:49:26 GMT
STOPSIGNAL SIGUSR1
# Fri, 23 Apr 2021 20:49:28 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 23 Apr 2021 20:49:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 20:49:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 20:49:33 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:33d77752597b664d047cc829e58a223d6fb077b61f69ca0462fcfb9b78d5f69b`  
		Last Modified: Sat, 10 Apr 2021 00:59:22 GMT  
		Size: 24.9 MB (24873199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c107a5973e1ce17cb311e2bf8a0d841875ca9f02219922ca12a9203602b5ce`  
		Last Modified: Sat, 10 Apr 2021 02:36:55 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4fd166622140d354f76734dca13311daf08f4b0e1a2bd667bd8f1237147d592`  
		Last Modified: Fri, 23 Apr 2021 20:50:23 GMT  
		Size: 9.2 MB (9166265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6683d8d529358b8fd7297f933059372813f6a97b67c13987e9e309aeb63e9d7`  
		Last Modified: Fri, 23 Apr 2021 20:50:20 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2740aff641d0d26151406fb76c73059f6f37d65543141d4a46600055c477dbce`  
		Last Modified: Fri, 23 Apr 2021 20:50:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.10` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:049069171782a5ea16bc2052ee484dd63b650e108f9e48db799e55c667ee9d29
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31771359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d474b012eeaa8b00ec45f00f784bdaff3606013979b8ed2c920d960e1a6e5c0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:59:45 GMT
ADD file:3fbd246a2de82566bcaaf62e3e0bf57175a7ad46b4156366a110661b31eab240 in / 
# Sat, 10 Apr 2021 00:59:47 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 08:58:51 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 23 Apr 2021 20:59:31 GMT
ENV HAPROXY_VERSION=2.3.10
# Fri, 23 Apr 2021 20:59:31 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Fri, 23 Apr 2021 20:59:32 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Fri, 23 Apr 2021 21:00:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 23 Apr 2021 21:00:18 GMT
STOPSIGNAL SIGUSR1
# Fri, 23 Apr 2021 21:00:18 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 23 Apr 2021 21:00:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 21:00:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 21:00:25 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:8c6bea184b33030fb923c3c09d634b73235dec3fe2d411db9fd22bda669f2c37`  
		Last Modified: Sat, 10 Apr 2021 01:07:51 GMT  
		Size: 22.7 MB (22739801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5be95d3afdef3cc4c8a37695b513cf41e6cf6ffeecd9ce2426d38cb245a0b52`  
		Last Modified: Sat, 10 Apr 2021 09:05:25 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717bc5365fb4bcdb4738770e1f312f2f58a06135e8d00643b6eb56fc013fcfe2`  
		Last Modified: Fri, 23 Apr 2021 21:02:42 GMT  
		Size: 9.0 MB (9029609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3f9836ad3bdc29bcf6b0ea0ca6e1478d1348e1015e7dd6ba91a44f8c523a050`  
		Last Modified: Fri, 23 Apr 2021 21:02:39 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:724e48ed89849e1da6018edaf2c357f02df92850ddb50bf446da7b127792dab7`  
		Last Modified: Fri, 23 Apr 2021 21:02:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.10` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:62ef02fde66dea080deea6a17011711125171d1448d475c118f9ea2d691a42be
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.4 MB (35351171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9426ad19c62950e93ccf52c6f26ea94f779739576a8b938e340b22015a08a527`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:41:25 GMT
ADD file:b24da7eb23eeae04e00d0e45da29a89fe8f992e8dcf4ba482afb907b8015b7bf in / 
# Sat, 10 Apr 2021 00:41:28 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:13:29 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 23 Apr 2021 20:40:21 GMT
ENV HAPROXY_VERSION=2.3.10
# Fri, 23 Apr 2021 20:40:22 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Fri, 23 Apr 2021 20:40:22 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Fri, 23 Apr 2021 20:41:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 23 Apr 2021 20:41:03 GMT
STOPSIGNAL SIGUSR1
# Fri, 23 Apr 2021 20:41:04 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 23 Apr 2021 20:41:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 20:41:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 20:41:07 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:15cb40b9c4df1a06940dc2a154c3be46844241235c1a091afa70da0ee2dc811a`  
		Last Modified: Sat, 10 Apr 2021 00:47:53 GMT  
		Size: 25.9 MB (25904582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48cb832c3e00ffed789c3f464caa612fe4996ba4683f72f8cf214d1437268efe`  
		Last Modified: Sat, 10 Apr 2021 01:21:27 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99a4194f9c3742aa2f14d298181297121bb2c902d5eec8249de7c2ccb315d34`  
		Last Modified: Fri, 23 Apr 2021 20:43:01 GMT  
		Size: 9.4 MB (9444636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18eb1616784d5ffc7039165a0a02e92e1d9db3d88f8746a790b2558cd40a4974`  
		Last Modified: Fri, 23 Apr 2021 20:42:58 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baadd6b3908aad2d6176197c1816634a6271f00ce248db43ac40027449ababa2`  
		Last Modified: Fri, 23 Apr 2021 20:42:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.10` - linux; 386

```console
$ docker pull haproxy@sha256:31390a54f68d62f3e7c80af3ddd2feb656e92553aa50acba7af43a06dcd5b560
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.2 MB (37209592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cf7eddc35247bbe2921775551965d6f38dbf1ee3be73cfb9f6544aaea2db502`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:39:42 GMT
ADD file:8885d4d13678543780bb04ba14b621179665f7951d5b261036a7092df9b376e7 in / 
# Sat, 10 Apr 2021 00:39:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 03:48:12 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 23 Apr 2021 20:38:45 GMT
ENV HAPROXY_VERSION=2.3.10
# Fri, 23 Apr 2021 20:38:45 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Fri, 23 Apr 2021 20:38:46 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Fri, 23 Apr 2021 20:39:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 23 Apr 2021 20:39:35 GMT
STOPSIGNAL SIGUSR1
# Fri, 23 Apr 2021 20:39:35 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 23 Apr 2021 20:39:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 20:39:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 20:39:36 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:7cc57a8772e5e479618650dfa70f315b474d3f205d04bde7f602f469c1928d84`  
		Last Modified: Sat, 10 Apr 2021 00:46:07 GMT  
		Size: 27.8 MB (27788987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d92d68a52363235dcdfb59fa81e5ef1a4561c958501e4f28d6b79e86f8b8501`  
		Last Modified: Sat, 10 Apr 2021 03:59:08 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c799704f6f7241fe4fe9658644a136f7f3a32cde54d58f63d2271c65f604e88`  
		Last Modified: Fri, 23 Apr 2021 20:42:36 GMT  
		Size: 9.4 MB (9418656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59f1328c2bd9da85a0836e5fd35839fdec1c3e22e0e5c30650827a10891c0ba7`  
		Last Modified: Fri, 23 Apr 2021 20:42:34 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:525b4de4d515d0e1e55046e2b12bc6368f5821f6c311a7bb5e2af64beca2282d`  
		Last Modified: Fri, 23 Apr 2021 20:42:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.10` - linux; mips64le

```console
$ docker pull haproxy@sha256:e40a773567ecc6a0378962548f266a89f0651c1f7dc8c1b2a3ca5e2f984fb7c0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.9 MB (34943218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:609cf796bed6fbe5ca0f3ae499bf6d7a955768064cb0d180a60131050dd6fa35`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:09:40 GMT
ADD file:0c93801c4a3719dfd4c047d7f2f4d52bf463eba2ab875da1dc54dcc832aae20b in / 
# Sat, 10 Apr 2021 01:09:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:39:36 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 23 Apr 2021 20:07:26 GMT
ENV HAPROXY_VERSION=2.3.10
# Fri, 23 Apr 2021 20:07:26 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Fri, 23 Apr 2021 20:07:26 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Fri, 23 Apr 2021 20:09:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 23 Apr 2021 20:09:50 GMT
STOPSIGNAL SIGUSR1
# Fri, 23 Apr 2021 20:09:50 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 23 Apr 2021 20:09:52 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 20:09:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 20:09:53 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:09ea659ba566d9c3c62493e5ae0b964f1eee4fcf35aabc91c5c34ca1ad686541`  
		Last Modified: Sat, 10 Apr 2021 01:16:07 GMT  
		Size: 25.8 MB (25806410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10fa5ae1be1fc686c91c15f24ebaaa72d7c4f64321c8ead8386f2f4f9d1a6705`  
		Last Modified: Sat, 10 Apr 2021 01:53:41 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c195a6aaaf12a34216b2d8aca52aa55b0f937fd8618100d1e0e08d9c6f43d8b0`  
		Last Modified: Fri, 23 Apr 2021 20:10:38 GMT  
		Size: 9.1 MB (9134856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba9d4d0ca44a4f5b7349bbea2e1e64c1d3fa001ef5d09b38f803eebe6bcfffb`  
		Last Modified: Fri, 23 Apr 2021 20:10:31 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:725b140d9e91c81a346e8cf6395c2058a6c206f327ef7ec6ecc36e2542838887`  
		Last Modified: Fri, 23 Apr 2021 20:10:31 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.10` - linux; ppc64le

```console
$ docker pull haproxy@sha256:ff52706fced2f786b64882c9d1e94ed5284c38c042c0e693e4ed87d7dc33c0c5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40589965 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd48e104b02ba284aa5985fd56e31c4bbf1689501afe8a8cfc5aaa1967626fc5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:26:49 GMT
ADD file:ab87d4854aa8628ce8f4e603c0496499f6f28c3d2525ace782c7369691dafc8c in / 
# Sat, 10 Apr 2021 01:26:56 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 04:45:12 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 23 Apr 2021 20:18:41 GMT
ENV HAPROXY_VERSION=2.3.10
# Fri, 23 Apr 2021 20:18:49 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Fri, 23 Apr 2021 20:18:54 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Fri, 23 Apr 2021 20:22:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 23 Apr 2021 20:22:51 GMT
STOPSIGNAL SIGUSR1
# Fri, 23 Apr 2021 20:22:53 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 23 Apr 2021 20:23:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 20:23:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 20:23:06 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:3e1e599482ca47095f85e429b346b76375aa85015ddcca050e85c2a8b1fdda9c`  
		Last Modified: Sat, 10 Apr 2021 01:33:57 GMT  
		Size: 30.5 MB (30545933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ee41bdc57145d3cb6e9f5fa23eed213567ae52835c7cff5fd57fe17b52f5ec`  
		Last Modified: Sat, 10 Apr 2021 05:09:50 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c841a7f82bff751f994b8799d674c7d4211251a43359351397999911cfa870`  
		Last Modified: Fri, 23 Apr 2021 20:25:56 GMT  
		Size: 10.0 MB (10042073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4641283e776afb6c306c0a6965f7e0b1238d91bc09f304ea32545464581a9f6`  
		Last Modified: Fri, 23 Apr 2021 20:25:53 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5248644a4705a96ac93d3ebbb06d89ed62a29bf7ae76226a7a3fd7cd388554b9`  
		Last Modified: Fri, 23 Apr 2021 20:25:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.10` - linux; s390x

```console
$ docker pull haproxy@sha256:65f0248af9b095156adf78d96f4f792c03a87cb2277ef4c8f36d44333921625a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.0 MB (35046751 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84ba273a498e9d8f8422051771b73d62e5f4fedd88d8b5ef771f73d069b6af0f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:42:23 GMT
ADD file:dbe2182f8699f2a6011413ea01862e6c0e85853d922dffd72a28d994d23c79bc in / 
# Sat, 10 Apr 2021 00:42:25 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:38:04 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 23 Apr 2021 20:41:50 GMT
ENV HAPROXY_VERSION=2.3.10
# Fri, 23 Apr 2021 20:41:51 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Fri, 23 Apr 2021 20:41:51 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Fri, 23 Apr 2021 20:42:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 23 Apr 2021 20:42:54 GMT
STOPSIGNAL SIGUSR1
# Fri, 23 Apr 2021 20:42:54 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 23 Apr 2021 20:42:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 20:42:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 20:42:57 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:65291f8717b3afd99b63cee867dd3e06b956a8ee6aa8580cc31d913b25de209d`  
		Last Modified: Sat, 10 Apr 2021 00:45:48 GMT  
		Size: 25.8 MB (25753787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9daf67acfb0373e31068762d068f1da8d320f2bdcdb0e6651d52b8183ede06c`  
		Last Modified: Sat, 10 Apr 2021 01:42:28 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e00467b5656b09a7387dfd6e3adb3b30d4e7bddcaad2d25e8e422f7dcce2a58f`  
		Last Modified: Fri, 23 Apr 2021 20:45:10 GMT  
		Size: 9.3 MB (9291015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd5ec62c92ca691a7dd3e4602bad6d4be9d23dcd5d2f7420b30100f6b361cdbe`  
		Last Modified: Fri, 23 Apr 2021 20:45:09 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670261f5947e500477b59eac7f9966e7e1d4eae57a4132c42252790506139977`  
		Last Modified: Fri, 23 Apr 2021 20:45:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.3.10-alpine`

```console
$ docker pull haproxy@sha256:1168dcda566f7ce42120fe56135178d78752e7d198b4f96a77c00f1b06af1853
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `haproxy:2.3.10-alpine` - linux; amd64

```console
$ docker pull haproxy@sha256:6d16465fe404f162ffcfd564eea2774ba06edf7188280484a270cd8862c35a88
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9501835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77414e3b99078b756a62667c18c85f4359518b1610a2cc6f57d682ce7a4f3bb2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:37:38 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 23 Apr 2021 20:20:47 GMT
ENV HAPROXY_VERSION=2.3.10
# Fri, 23 Apr 2021 20:20:47 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Fri, 23 Apr 2021 20:20:47 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Fri, 23 Apr 2021 20:21:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 23 Apr 2021 20:21:37 GMT
STOPSIGNAL SIGUSR1
# Fri, 23 Apr 2021 20:21:37 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 23 Apr 2021 20:21:38 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 20:21:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 20:21:38 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4de1862a29af271c1751bf0d03d96f9a881f971d1288c5fafcfba90b517611f8`  
		Last Modified: Wed, 14 Apr 2021 21:43:30 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cba67cd0abe26102179dbd1deb88405bc4764e51a2b1f6ef06232cb9eca0ce6`  
		Last Modified: Fri, 23 Apr 2021 20:22:54 GMT  
		Size: 6.7 MB (6688111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:500b344a0df360398223362751a2ceab4c0981e06e375ff45905d04507537387`  
		Last Modified: Fri, 23 Apr 2021 20:22:53 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2724c9435ec936799a1c47edd9cb5e46f597d30b3e3cab7b0e32d855741fabb`  
		Last Modified: Fri, 23 Apr 2021 20:22:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.10-alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:7e27a3587e72e37010d991363a75b6cc01493a686a23ed0a8a780a49c6ee2494
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.2 MB (9211848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1aec7a3cb069441d455cdee3c8970689988845ee8742770933e8b091a05a52e0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:18:05 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 23 Apr 2021 20:51:06 GMT
ENV HAPROXY_VERSION=2.3.10
# Fri, 23 Apr 2021 20:51:07 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Fri, 23 Apr 2021 20:51:08 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Fri, 23 Apr 2021 20:51:33 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 23 Apr 2021 20:51:35 GMT
STOPSIGNAL SIGUSR1
# Fri, 23 Apr 2021 20:51:35 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 23 Apr 2021 20:51:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 20:51:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 20:51:39 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd640f0f76e4e434b444a36110041f2c571b2dbcfca29958b2e90de8d91bd6eb`  
		Last Modified: Wed, 14 Apr 2021 21:34:02 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54049885ecd472a5548c06de21ae362a2dde172e52f8118579b63d389c596214`  
		Last Modified: Fri, 23 Apr 2021 20:52:23 GMT  
		Size: 6.6 MB (6587961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa68a40a7e61b9513c658b23339f17a1e97ed7660b0c9828c04b65f3fb8ae637`  
		Last Modified: Fri, 23 Apr 2021 20:52:20 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dba2abb2f77db1891b207f81dcc8f6f93862222a15a489e3f153d999d8d6bfb`  
		Last Modified: Fri, 23 Apr 2021 20:52:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.10-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:849282abf73b940f2e28483aea32e03a54075b7dbc6714d00412742327a88b5e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.9 MB (8927012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbb9ef13943f7a6fced52d987a05ef61afbdd96efb69d6f263810cb54037b990`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:47:58 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 23 Apr 2021 21:00:39 GMT
ENV HAPROXY_VERSION=2.3.10
# Fri, 23 Apr 2021 21:00:39 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Fri, 23 Apr 2021 21:00:40 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Fri, 23 Apr 2021 21:01:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 23 Apr 2021 21:01:10 GMT
STOPSIGNAL SIGUSR1
# Fri, 23 Apr 2021 21:01:11 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 23 Apr 2021 21:01:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 21:01:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 21:01:21 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ff0f6ee9305bed375c784c12ad4beeac3af6ea1a6b5afeec6b4700259dc194`  
		Last Modified: Wed, 14 Apr 2021 22:56:09 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb1d6019b6548f16be0cfff81a3a38f64337636d40ec6d50697915983ca3887f`  
		Last Modified: Fri, 23 Apr 2021 21:02:54 GMT  
		Size: 6.5 MB (6501111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e17ccc0c26b79d4583ef2907084a53e7a69a87686939491984151ac2ead75b1`  
		Last Modified: Fri, 23 Apr 2021 21:02:52 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f451a3dd3dd7b108fdbe462194e6659be8f76b7a69911c306d74d8fceeed3f`  
		Last Modified: Fri, 23 Apr 2021 21:02:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.10-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:ec0989fc82ace88b5cf80c0dc55e695e5a5d6620174e4ed0d5d8c1634630f2e7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9413982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cd73593d809a141875771ab3f582e9a6258ba6fe0f4b707f0ce439cd47a7405`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:26:01 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 23 Apr 2021 20:41:19 GMT
ENV HAPROXY_VERSION=2.3.10
# Fri, 23 Apr 2021 20:41:19 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Fri, 23 Apr 2021 20:41:20 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Fri, 23 Apr 2021 20:41:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 23 Apr 2021 20:41:44 GMT
STOPSIGNAL SIGUSR1
# Fri, 23 Apr 2021 20:41:45 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 23 Apr 2021 20:41:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 20:41:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 20:41:48 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2ef9646f93509fb43536690b645509d9b653316324583761dd086b8ad6c664`  
		Last Modified: Wed, 14 Apr 2021 20:37:52 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffe20dd6ddd5d14baec905dc0c113e8dd01ce5899588c89675a6988ccfe34a48`  
		Last Modified: Fri, 23 Apr 2021 20:43:13 GMT  
		Size: 6.7 MB (6700201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1616786188830f47d2d1ea30821c3aa828e4a87dbc5d075f5f6eee2c1fdaec`  
		Last Modified: Fri, 23 Apr 2021 20:43:09 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c147d090d4db064f2514f9bfa6a9cb2e6d716e448d94b4ab90e2b7a0e50ab03`  
		Last Modified: Fri, 23 Apr 2021 20:43:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.10-alpine` - linux; 386

```console
$ docker pull haproxy@sha256:839a53bd7d2f00b0d67b1c764d9811b7491a3d4d645a6abb94ebd84293e4c367
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9356996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b30351ad929f3d405e1ca732a718c6e0fe63e1a52c2407a4d9600fff4e7e439b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 01:50:06 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 23 Apr 2021 20:39:47 GMT
ENV HAPROXY_VERSION=2.3.10
# Fri, 23 Apr 2021 20:39:47 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Fri, 23 Apr 2021 20:39:47 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Fri, 23 Apr 2021 20:40:45 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 23 Apr 2021 20:40:45 GMT
STOPSIGNAL SIGUSR1
# Fri, 23 Apr 2021 20:40:45 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 23 Apr 2021 20:40:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 20:40:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 20:40:47 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:31b7e7ccca9e17fd08b39c9a4ffd3ded380b62816c489d6c3758c9bb5a632430`  
		Last Modified: Wed, 14 Apr 2021 18:39:24 GMT  
		Size: 2.8 MB (2818900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9104145d2a6b1e0c0837c464bb9d4b331949cfeb6be12e4e7995507661d3386`  
		Last Modified: Thu, 15 Apr 2021 02:00:28 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22386ff451c9485cc86547597a9df94ba437d282baedc6b3ff68139348ab838e`  
		Last Modified: Fri, 23 Apr 2021 20:42:53 GMT  
		Size: 6.5 MB (6536340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44c782fb9ce01dfc03b5926dd9052609853265d68ef395e663ca422aba662667`  
		Last Modified: Fri, 23 Apr 2021 20:42:51 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eab34669a9636f82828df5502f0d94263605f7309e0bab880f3d9bc324b052b`  
		Last Modified: Fri, 23 Apr 2021 20:42:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.10-alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:a4daa01e291804783faf44842f65f63d7108530d7623efce6d782952fe4bcbf9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.8 MB (9835818 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2ebb4297d3c174774a272e1f8a0042fc3c7c9ca7b1d0cf36d5af3d58b36005c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:25:09 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 23 Apr 2021 20:23:26 GMT
ENV HAPROXY_VERSION=2.3.10
# Fri, 23 Apr 2021 20:23:31 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Fri, 23 Apr 2021 20:23:34 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Fri, 23 Apr 2021 20:24:19 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 23 Apr 2021 20:24:24 GMT
STOPSIGNAL SIGUSR1
# Fri, 23 Apr 2021 20:24:27 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 23 Apr 2021 20:24:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 20:24:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 20:24:42 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8004273856b1b354059d03a17deec6e79d325ba45d63213dda3d1fa401db8c22`  
		Last Modified: Wed, 14 Apr 2021 23:36:37 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b9cdc9560132361ff8957311b5fd6b2bbacc8ec5be9489a16a3b3eea31f3d2`  
		Last Modified: Fri, 23 Apr 2021 20:26:10 GMT  
		Size: 7.0 MB (7020918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac490252619a4b1389b0e3fb3c472b84a443f9bc3d346558d7ac67596be3eb0`  
		Last Modified: Fri, 23 Apr 2021 20:26:11 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554ee7adacda14ba7a4c490cead3c19a063d98a21b022b06f60bff9e6089a817`  
		Last Modified: Fri, 23 Apr 2021 20:26:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.10-alpine` - linux; s390x

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

## `haproxy:2.4-dev`

```console
$ docker pull haproxy@sha256:8d64f803387933f9ea728d7a2615b2dab0e8c5a799cc35f975acac7980324d32
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

### `haproxy:2.4-dev` - linux; amd64

```console
$ docker pull haproxy@sha256:20c0f2c5816f9fb2a6ca98d88018da7908c0bc57f9e4a1030f0452f82ec29c1f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37256605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c66ea864d9866ea484632866d37ec47adfc55629f45b0e5795b83f3b0d461354`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:29:42 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 03 May 2021 21:59:58 GMT
ENV HAPROXY_VERSION=2.4-dev18
# Mon, 03 May 2021 21:59:59 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev18.tar.gz
# Mon, 03 May 2021 21:59:59 GMT
ENV HAPROXY_SHA256=fab8b85664afc74c481c91a8f104b6bf87b265f9b5f03054dc926364e9801e74
# Tue, 04 May 2021 00:22:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Tue, 04 May 2021 00:22:36 GMT
STOPSIGNAL SIGUSR1
# Tue, 04 May 2021 00:22:36 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Tue, 04 May 2021 00:22:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 May 2021 00:22:37 GMT
USER haproxy
# Tue, 04 May 2021 00:22:37 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7abf58d954de379f38a19e07330116ba6b11f21007bc7b7507d233e5b0aa3fe0`  
		Last Modified: Sat, 10 Apr 2021 06:38:07 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aac1e92e044b342ae4c034c566fa222f832eb644f4b438b0fb6c3b2bba9e17b`  
		Last Modified: Tue, 04 May 2021 00:24:56 GMT  
		Size: 10.1 MB (10115405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be28c1b468f352e30619ec7fc21e25a6294d76f0cd82df9149814a0784e91c9`  
		Last Modified: Tue, 04 May 2021 00:24:54 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:de596a58d637f4caf06283aecc31abf76e9e054cb97f2d57967ca055a3fdb660
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.6 MB (34623675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a616d5e4075e6d8b7901c0cf40e2601a7538ad6995b43d45302943777c20badf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:51:31 GMT
ADD file:926533a23a69aa2481a9122b667bb6300a347154eea366c9e679a230aa7f373a in / 
# Sat, 10 Apr 2021 00:51:34 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 02:24:17 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 03 May 2021 22:14:51 GMT
ENV HAPROXY_VERSION=2.4-dev18
# Mon, 03 May 2021 22:14:53 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev18.tar.gz
# Mon, 03 May 2021 22:14:54 GMT
ENV HAPROXY_SHA256=fab8b85664afc74c481c91a8f104b6bf87b265f9b5f03054dc926364e9801e74
# Tue, 04 May 2021 01:38:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Tue, 04 May 2021 01:38:02 GMT
STOPSIGNAL SIGUSR1
# Tue, 04 May 2021 01:38:03 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Tue, 04 May 2021 01:38:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 May 2021 01:38:04 GMT
USER haproxy
# Tue, 04 May 2021 01:38:06 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:33d77752597b664d047cc829e58a223d6fb077b61f69ca0462fcfb9b78d5f69b`  
		Last Modified: Sat, 10 Apr 2021 00:59:22 GMT  
		Size: 24.9 MB (24873199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c107a5973e1ce17cb311e2bf8a0d841875ca9f02219922ca12a9203602b5ce`  
		Last Modified: Sat, 10 Apr 2021 02:36:55 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c88150841fcb707acbd9df78ab1b9976a0baee7dffe499ad16c1e724bb17e3d`  
		Last Modified: Tue, 04 May 2021 01:38:53 GMT  
		Size: 9.7 MB (9748646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c10aa05248313ab068e205968ae811fe1a1a3e698c6ce0a1c465446548d62f`  
		Last Modified: Tue, 04 May 2021 01:38:50 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:b0483bbd360567db7dca54a5248197da9d4cb575d76a134c631269d32825332d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.3 MB (32332957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbda1941fa04cc1d1cd51ec3f37d84b46ab4013680a448cb7d1fd38ee859f624`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:59:45 GMT
ADD file:3fbd246a2de82566bcaaf62e3e0bf57175a7ad46b4156366a110661b31eab240 in / 
# Sat, 10 Apr 2021 00:59:47 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 08:58:51 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 03 May 2021 23:03:28 GMT
ENV HAPROXY_VERSION=2.4-dev18
# Mon, 03 May 2021 23:03:30 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev18.tar.gz
# Mon, 03 May 2021 23:03:31 GMT
ENV HAPROXY_SHA256=fab8b85664afc74c481c91a8f104b6bf87b265f9b5f03054dc926364e9801e74
# Tue, 04 May 2021 00:57:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Tue, 04 May 2021 00:57:22 GMT
STOPSIGNAL SIGUSR1
# Tue, 04 May 2021 00:57:23 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Tue, 04 May 2021 00:57:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 May 2021 00:57:25 GMT
USER haproxy
# Tue, 04 May 2021 00:57:26 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:8c6bea184b33030fb923c3c09d634b73235dec3fe2d411db9fd22bda669f2c37`  
		Last Modified: Sat, 10 Apr 2021 01:07:51 GMT  
		Size: 22.7 MB (22739801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5be95d3afdef3cc4c8a37695b513cf41e6cf6ffeecd9ce2426d38cb245a0b52`  
		Last Modified: Sat, 10 Apr 2021 09:05:25 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00eb766cefd963052599432a3eee0f4ed0fb73e0091b589eae5d9fe638fa8295`  
		Last Modified: Tue, 04 May 2021 00:59:32 GMT  
		Size: 9.6 MB (9591332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caae456a9be1f7eb6e4bd21828f1c1ae8df59fcb9846fe31bf383be1a3ac6e7c`  
		Last Modified: Tue, 04 May 2021 00:59:25 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:4b735ce00f4ed0c52833bd3323df7d398e1e3f1ded6fca8d4fd66175c03e14b0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35896311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:988b9033e9005759c723ac872ba6bf5e9641856f4b72349842adc7b6e9287656`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:41:25 GMT
ADD file:b24da7eb23eeae04e00d0e45da29a89fe8f992e8dcf4ba482afb907b8015b7bf in / 
# Sat, 10 Apr 2021 00:41:28 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:13:29 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 03 May 2021 22:00:56 GMT
ENV HAPROXY_VERSION=2.4-dev18
# Mon, 03 May 2021 22:00:58 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev18.tar.gz
# Mon, 03 May 2021 22:01:01 GMT
ENV HAPROXY_SHA256=fab8b85664afc74c481c91a8f104b6bf87b265f9b5f03054dc926364e9801e74
# Tue, 04 May 2021 01:05:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Tue, 04 May 2021 01:05:03 GMT
STOPSIGNAL SIGUSR1
# Tue, 04 May 2021 01:05:03 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Tue, 04 May 2021 01:05:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 May 2021 01:05:05 GMT
USER haproxy
# Tue, 04 May 2021 01:05:06 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:15cb40b9c4df1a06940dc2a154c3be46844241235c1a091afa70da0ee2dc811a`  
		Last Modified: Sat, 10 Apr 2021 00:47:53 GMT  
		Size: 25.9 MB (25904582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48cb832c3e00ffed789c3f464caa612fe4996ba4683f72f8cf214d1437268efe`  
		Last Modified: Sat, 10 Apr 2021 01:21:27 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d925210447f3d0f8b59a238243ccd2b9e02101ed90555f381f7f84d19ae2e1`  
		Last Modified: Tue, 04 May 2021 01:07:14 GMT  
		Size: 10.0 MB (9989898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9736f199f7eef04b231e3eeb0a60f4b428a35680111bd7460d298a79e9b6b43c`  
		Last Modified: Tue, 04 May 2021 01:07:11 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev` - linux; 386

```console
$ docker pull haproxy@sha256:014484389b8ea19d5ef19ebbf4c071ebc87278974b0d28d191adaff3f27b5943
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.7 MB (37741158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2502fb424f9e89dfc69cbbaa8548cc16aae02889c960835b8a151022aa204f2a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:39:42 GMT
ADD file:8885d4d13678543780bb04ba14b621179665f7951d5b261036a7092df9b376e7 in / 
# Sat, 10 Apr 2021 00:39:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 03:48:12 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 03 May 2021 21:38:43 GMT
ENV HAPROXY_VERSION=2.4-dev18
# Mon, 03 May 2021 21:38:43 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev18.tar.gz
# Mon, 03 May 2021 21:38:43 GMT
ENV HAPROXY_SHA256=fab8b85664afc74c481c91a8f104b6bf87b265f9b5f03054dc926364e9801e74
# Tue, 04 May 2021 00:42:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Tue, 04 May 2021 00:42:13 GMT
STOPSIGNAL SIGUSR1
# Tue, 04 May 2021 00:42:13 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Tue, 04 May 2021 00:42:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 May 2021 00:42:13 GMT
USER haproxy
# Tue, 04 May 2021 00:42:13 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:7cc57a8772e5e479618650dfa70f315b474d3f205d04bde7f602f469c1928d84`  
		Last Modified: Sat, 10 Apr 2021 00:46:07 GMT  
		Size: 27.8 MB (27788987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d92d68a52363235dcdfb59fa81e5ef1a4561c958501e4f28d6b79e86f8b8501`  
		Last Modified: Sat, 10 Apr 2021 03:59:08 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:480bf4b481880037cfba39b650627fbf8efa247c10313bc2b6c6998ef7ce36c6`  
		Last Modified: Tue, 04 May 2021 00:45:19 GMT  
		Size: 10.0 MB (9950345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a02e0b403a23b63daf633fba5b1a69af54465eb277681175f3b41300e0e5497`  
		Last Modified: Tue, 04 May 2021 00:45:17 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev` - linux; mips64le

```console
$ docker pull haproxy@sha256:ef40fdcad4f0bc78ae418fb5d258d33d3b6714393e58cb275bb8428ac111557f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.5 MB (35540367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85e4ee3838930d54eb73f8f29dedf4852000465c624a3ba25e2df165468636b0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:09:40 GMT
ADD file:0c93801c4a3719dfd4c047d7f2f4d52bf463eba2ab875da1dc54dcc832aae20b in / 
# Sat, 10 Apr 2021 01:09:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:39:36 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 03 May 2021 21:07:27 GMT
ENV HAPROXY_VERSION=2.4-dev18
# Mon, 03 May 2021 21:07:27 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev18.tar.gz
# Mon, 03 May 2021 21:07:28 GMT
ENV HAPROXY_SHA256=fab8b85664afc74c481c91a8f104b6bf87b265f9b5f03054dc926364e9801e74
# Tue, 04 May 2021 00:11:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Tue, 04 May 2021 00:11:23 GMT
STOPSIGNAL SIGUSR1
# Tue, 04 May 2021 00:11:23 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Tue, 04 May 2021 00:11:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 May 2021 00:11:24 GMT
USER haproxy
# Tue, 04 May 2021 00:11:24 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:09ea659ba566d9c3c62493e5ae0b964f1eee4fcf35aabc91c5c34ca1ad686541`  
		Last Modified: Sat, 10 Apr 2021 01:16:07 GMT  
		Size: 25.8 MB (25806410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10fa5ae1be1fc686c91c15f24ebaaa72d7c4f64321c8ead8386f2f4f9d1a6705`  
		Last Modified: Sat, 10 Apr 2021 01:53:41 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e5f90a2d5f0809c92154b735d248c941c30e4870c26a58a1ec299fb1bbc40d`  
		Last Modified: Tue, 04 May 2021 00:12:08 GMT  
		Size: 9.7 MB (9732125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aed81ba7a628ae4fa904ad01d253875ace9ac629c93b8efef3f84e7016f9f58`  
		Last Modified: Tue, 04 May 2021 00:12:01 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev` - linux; ppc64le

```console
$ docker pull haproxy@sha256:63d8b128a955f475a90352af218b4e89dde12b1dc1f71217cf5065d829eeafec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.2 MB (41160234 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15a908ebe2a68fb86148a7b7f619856caaf5d4aa6dc8b8e063b2d0c9b7b09aec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:26:49 GMT
ADD file:ab87d4854aa8628ce8f4e603c0496499f6f28c3d2525ace782c7369691dafc8c in / 
# Sat, 10 Apr 2021 01:26:56 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 04:45:12 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 03 May 2021 22:08:29 GMT
ENV HAPROXY_VERSION=2.4-dev18
# Mon, 03 May 2021 22:08:45 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev18.tar.gz
# Mon, 03 May 2021 22:08:55 GMT
ENV HAPROXY_SHA256=fab8b85664afc74c481c91a8f104b6bf87b265f9b5f03054dc926364e9801e74
# Tue, 04 May 2021 02:31:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Tue, 04 May 2021 02:31:21 GMT
STOPSIGNAL SIGUSR1
# Tue, 04 May 2021 02:31:24 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Tue, 04 May 2021 02:31:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 May 2021 02:31:33 GMT
USER haproxy
# Tue, 04 May 2021 02:31:40 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:3e1e599482ca47095f85e429b346b76375aa85015ddcca050e85c2a8b1fdda9c`  
		Last Modified: Sat, 10 Apr 2021 01:33:57 GMT  
		Size: 30.5 MB (30545933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ee41bdc57145d3cb6e9f5fa23eed213567ae52835c7cff5fd57fe17b52f5ec`  
		Last Modified: Sat, 10 Apr 2021 05:09:50 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2474a657ff366e5e48721c53c9dfeaa4eb3cd267e4495c90d029798271e965ed`  
		Last Modified: Tue, 04 May 2021 02:35:46 GMT  
		Size: 10.6 MB (10612462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b2724278cfe96d7b12c35bb287a85151d17f358c9b096a8e2e4e2d41a72c85`  
		Last Modified: Tue, 04 May 2021 02:35:43 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev` - linux; s390x

```console
$ docker pull haproxy@sha256:8589ed491dce111157fcb5ee3344bc59d9fb87715a06c1474b63467529d201fc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.5 MB (35543545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:effa514b71f49502a78660c7b8a0a2b86bab0ea2db081a5f104bd24e9941fc3b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:42:23 GMT
ADD file:dbe2182f8699f2a6011413ea01862e6c0e85853d922dffd72a28d994d23c79bc in / 
# Sat, 10 Apr 2021 00:42:25 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:38:04 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 03 May 2021 21:41:44 GMT
ENV HAPROXY_VERSION=2.4-dev18
# Mon, 03 May 2021 21:41:45 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev18.tar.gz
# Mon, 03 May 2021 21:41:46 GMT
ENV HAPROXY_SHA256=fab8b85664afc74c481c91a8f104b6bf87b265f9b5f03054dc926364e9801e74
# Tue, 04 May 2021 00:43:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Tue, 04 May 2021 00:43:46 GMT
STOPSIGNAL SIGUSR1
# Tue, 04 May 2021 00:43:47 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Tue, 04 May 2021 00:43:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 May 2021 00:43:48 GMT
USER haproxy
# Tue, 04 May 2021 00:43:48 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:65291f8717b3afd99b63cee867dd3e06b956a8ee6aa8580cc31d913b25de209d`  
		Last Modified: Sat, 10 Apr 2021 00:45:48 GMT  
		Size: 25.8 MB (25753787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9daf67acfb0373e31068762d068f1da8d320f2bdcdb0e6651d52b8183ede06c`  
		Last Modified: Sat, 10 Apr 2021 01:42:28 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f4b41baeaa740c725a5c78988f23e413b561477be09c0cce0da6c4b36d066e`  
		Last Modified: Tue, 04 May 2021 00:46:07 GMT  
		Size: 9.8 MB (9787929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5434bf5b14bf03c0b62030672f22a05a6aa533b00e4787adb13854bdc203db84`  
		Last Modified: Tue, 04 May 2021 00:46:05 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.4-dev-alpine`

```console
$ docker pull haproxy@sha256:fff3f0655cabdad687de75fb0029908afcc12310f07af48b6862b3f0900b36d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `haproxy:2.4-dev-alpine` - linux; amd64

```console
$ docker pull haproxy@sha256:cd1d4b94bb1e152362a1102c3f39b7aaec40cbe2bbb057c84019c4275f233fde
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.2 MB (10204009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2d1d52d63fa2e771ecaa1dfc84b1656492fa022899f057c65c4aec0caa00397`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:37:38 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 03 May 2021 22:00:59 GMT
ENV HAPROXY_VERSION=2.4-dev18
# Mon, 03 May 2021 22:00:59 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev18.tar.gz
# Mon, 03 May 2021 22:00:59 GMT
ENV HAPROXY_SHA256=fab8b85664afc74c481c91a8f104b6bf87b265f9b5f03054dc926364e9801e74
# Tue, 04 May 2021 00:23:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Tue, 04 May 2021 00:23:46 GMT
STOPSIGNAL SIGUSR1
# Tue, 04 May 2021 00:23:46 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Tue, 04 May 2021 00:23:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 May 2021 00:23:47 GMT
USER haproxy
# Tue, 04 May 2021 00:23:47 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4de1862a29af271c1751bf0d03d96f9a881f971d1288c5fafcfba90b517611f8`  
		Last Modified: Wed, 14 Apr 2021 21:43:30 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5978a5c5417dc9ccc24f889634189055c75a143eb5b561fd12772b4c8bd658c0`  
		Last Modified: Tue, 04 May 2021 00:25:07 GMT  
		Size: 7.4 MB (7390405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aafb9ab3199b8060748b7af8c0c4e9da0aae4fb59400bda69e7f78c47f754bfd`  
		Last Modified: Tue, 04 May 2021 00:25:06 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev-alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:46455529abc15c9ed545e43305a67a2369bb200adb8935792787700f5f7472a1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9884300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec104b9a2fd2c70b6d3baec5fbb3218704bdb54d1ce96917e43ad64614fa4906`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:18:05 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 03 May 2021 22:10:09 GMT
ENV HAPROXY_VERSION=2.4-dev18
# Mon, 03 May 2021 22:10:10 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev18.tar.gz
# Mon, 03 May 2021 22:10:12 GMT
ENV HAPROXY_SHA256=fab8b85664afc74c481c91a8f104b6bf87b265f9b5f03054dc926364e9801e74
# Tue, 04 May 2021 00:53:50 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Tue, 04 May 2021 00:53:52 GMT
STOPSIGNAL SIGUSR1
# Tue, 04 May 2021 00:53:53 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Tue, 04 May 2021 00:53:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 May 2021 00:53:56 GMT
USER haproxy
# Tue, 04 May 2021 00:53:59 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd640f0f76e4e434b444a36110041f2c571b2dbcfca29958b2e90de8d91bd6eb`  
		Last Modified: Wed, 14 Apr 2021 21:34:02 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ced56deda546e1a28592d2c1e53fa305d7779fc8868ee6da4e54b7d6a81162d9`  
		Last Modified: Tue, 04 May 2021 00:54:49 GMT  
		Size: 7.3 MB (7260537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e78f23141b0b075fb3958f32438f4d337e870ced7c3003c7791aa13ba64b9a49`  
		Last Modified: Tue, 04 May 2021 00:54:46 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:1da1e6d181df5ec80ba2567aa60395ff144c642cc81a71ecf15cdd90980db7c3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9539946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:967689b3edae44a1953ea3038714702fa96e624fd3f3ec3171ef66d73e8fa6bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:47:58 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 03 May 2021 23:04:46 GMT
ENV HAPROXY_VERSION=2.4-dev18
# Mon, 03 May 2021 23:04:47 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev18.tar.gz
# Mon, 03 May 2021 23:04:49 GMT
ENV HAPROXY_SHA256=fab8b85664afc74c481c91a8f104b6bf87b265f9b5f03054dc926364e9801e74
# Tue, 04 May 2021 00:58:02 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Tue, 04 May 2021 00:58:03 GMT
STOPSIGNAL SIGUSR1
# Tue, 04 May 2021 00:58:03 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Tue, 04 May 2021 00:58:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 May 2021 00:58:06 GMT
USER haproxy
# Tue, 04 May 2021 00:58:07 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ff0f6ee9305bed375c784c12ad4beeac3af6ea1a6b5afeec6b4700259dc194`  
		Last Modified: Wed, 14 Apr 2021 22:56:09 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84e10884a0e017bd9319579dfcccd2647713ae4197d0a0d3191649ff84bf46d2`  
		Last Modified: Tue, 04 May 2021 00:59:41 GMT  
		Size: 7.1 MB (7114166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a6f22e2a5a631f64448e6d88809e7e0f5a013e2d51f1c96a59a57cd50954ae`  
		Last Modified: Tue, 04 May 2021 00:59:39 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:82aced14adaec465c871858f91902d5ae2862f183c298c03290ebddbea16013a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.1 MB (10119544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b64d57cba37710bb5fefd40e5432edf4c4da3a80692a12dcd2eb2a11f5129eb9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:26:01 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 03 May 2021 22:02:46 GMT
ENV HAPROXY_VERSION=2.4-dev18
# Mon, 03 May 2021 22:02:48 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev18.tar.gz
# Mon, 03 May 2021 22:02:50 GMT
ENV HAPROXY_SHA256=fab8b85664afc74c481c91a8f104b6bf87b265f9b5f03054dc926364e9801e74
# Tue, 04 May 2021 01:05:45 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Tue, 04 May 2021 01:05:46 GMT
STOPSIGNAL SIGUSR1
# Tue, 04 May 2021 01:05:47 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Tue, 04 May 2021 01:05:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 May 2021 01:05:49 GMT
USER haproxy
# Tue, 04 May 2021 01:05:50 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2ef9646f93509fb43536690b645509d9b653316324583761dd086b8ad6c664`  
		Last Modified: Wed, 14 Apr 2021 20:37:52 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cc170b442792d0820be4751eaf9284b5e1f9c8452adc7c7bbae45cf4abc2449`  
		Last Modified: Tue, 04 May 2021 01:07:23 GMT  
		Size: 7.4 MB (7405882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a811f2f75cbf30c7c3768d3727e399af7d53d39391dba3485f972e0958401aa5`  
		Last Modified: Tue, 04 May 2021 01:07:21 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev-alpine` - linux; 386

```console
$ docker pull haproxy@sha256:8050aa2b81fbc31bf2d47ff76170fc198225802a6a672f6beac39d4dd13474a7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (9966930 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eabde26ca343b4e6d06e3ebf5f7eab077dc86ae5b65a2c8c6dc6d48d30167c82`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 01:50:06 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 03 May 2021 21:40:10 GMT
ENV HAPROXY_VERSION=2.4-dev18
# Mon, 03 May 2021 21:40:10 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev18.tar.gz
# Mon, 03 May 2021 21:40:10 GMT
ENV HAPROXY_SHA256=fab8b85664afc74c481c91a8f104b6bf87b265f9b5f03054dc926364e9801e74
# Tue, 04 May 2021 00:43:27 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Tue, 04 May 2021 00:43:27 GMT
STOPSIGNAL SIGUSR1
# Tue, 04 May 2021 00:43:27 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Tue, 04 May 2021 00:43:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 May 2021 00:43:28 GMT
USER haproxy
# Tue, 04 May 2021 00:43:28 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:31b7e7ccca9e17fd08b39c9a4ffd3ded380b62816c489d6c3758c9bb5a632430`  
		Last Modified: Wed, 14 Apr 2021 18:39:24 GMT  
		Size: 2.8 MB (2818900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9104145d2a6b1e0c0837c464bb9d4b331949cfeb6be12e4e7995507661d3386`  
		Last Modified: Thu, 15 Apr 2021 02:00:28 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b8d327b19497f7a82d2a7802891b4b637c5375fd93ac2c296c8411ed46191c`  
		Last Modified: Tue, 04 May 2021 00:45:37 GMT  
		Size: 7.1 MB (7146396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97049f66fdbe40a5dc5419f8cb59bfdc729cef644fe9cbc2b54dd07c6e859beb`  
		Last Modified: Tue, 04 May 2021 00:45:35 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev-alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:b6bc56380c0ff12d3fa3f08f6d15b3dc36a51a2f9f9a2996ecf652c19420d94d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.5 MB (10522791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e02adafc155ab468e09e38b45a2fb4f2fe1d55809615e5329dc6b4329d14164e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:25:09 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 03 May 2021 22:17:14 GMT
ENV HAPROXY_VERSION=2.4-dev18
# Mon, 03 May 2021 22:17:20 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev18.tar.gz
# Mon, 03 May 2021 22:17:24 GMT
ENV HAPROXY_SHA256=fab8b85664afc74c481c91a8f104b6bf87b265f9b5f03054dc926364e9801e74
# Tue, 04 May 2021 02:34:03 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Tue, 04 May 2021 02:34:08 GMT
STOPSIGNAL SIGUSR1
# Tue, 04 May 2021 02:34:12 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Tue, 04 May 2021 02:34:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 May 2021 02:34:24 GMT
USER haproxy
# Tue, 04 May 2021 02:34:29 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8004273856b1b354059d03a17deec6e79d325ba45d63213dda3d1fa401db8c22`  
		Last Modified: Wed, 14 Apr 2021 23:36:37 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2d01c3d76fa82c4d7c15660c556631039a02991913228f2ac9d272637bff02`  
		Last Modified: Tue, 04 May 2021 02:36:01 GMT  
		Size: 7.7 MB (7708015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be3f83810256ffbcc290dfd487039e4547bedd19195eb05bb0046ecd84d232f`  
		Last Modified: Tue, 04 May 2021 02:36:00 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev-alpine` - linux; s390x

```console
$ docker pull haproxy@sha256:a764219bb48566020018c624e90819cc7142651a64baeffc1487c61a4dc4a05d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9916511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6833ad147838c6ffb79dfcd49f30a098ec2628b3a4ab7ce2f39599596a4a8ae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:54:24 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 03 May 2021 21:43:04 GMT
ENV HAPROXY_VERSION=2.4-dev18
# Mon, 03 May 2021 21:43:04 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev18.tar.gz
# Mon, 03 May 2021 21:43:05 GMT
ENV HAPROXY_SHA256=fab8b85664afc74c481c91a8f104b6bf87b265f9b5f03054dc926364e9801e74
# Tue, 04 May 2021 00:44:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Tue, 04 May 2021 00:44:44 GMT
STOPSIGNAL SIGUSR1
# Tue, 04 May 2021 00:44:45 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Tue, 04 May 2021 00:44:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 May 2021 00:44:45 GMT
USER haproxy
# Tue, 04 May 2021 00:44:46 GMT
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
	-	`sha256:2b4cfaaf827d363dc52189f0441a927ff267eb6eea9e081c19f6d728ff52d6a8`  
		Last Modified: Tue, 04 May 2021 00:46:18 GMT  
		Size: 7.3 MB (7312228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0441e6ef4431841df737d4be3294d20151800d805183d15d96602b45568ed2e`  
		Last Modified: Tue, 04 May 2021 00:46:17 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.4-dev18`

```console
$ docker pull haproxy@sha256:8d64f803387933f9ea728d7a2615b2dab0e8c5a799cc35f975acac7980324d32
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

### `haproxy:2.4-dev18` - linux; amd64

```console
$ docker pull haproxy@sha256:20c0f2c5816f9fb2a6ca98d88018da7908c0bc57f9e4a1030f0452f82ec29c1f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37256605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c66ea864d9866ea484632866d37ec47adfc55629f45b0e5795b83f3b0d461354`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:29:42 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 03 May 2021 21:59:58 GMT
ENV HAPROXY_VERSION=2.4-dev18
# Mon, 03 May 2021 21:59:59 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev18.tar.gz
# Mon, 03 May 2021 21:59:59 GMT
ENV HAPROXY_SHA256=fab8b85664afc74c481c91a8f104b6bf87b265f9b5f03054dc926364e9801e74
# Tue, 04 May 2021 00:22:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Tue, 04 May 2021 00:22:36 GMT
STOPSIGNAL SIGUSR1
# Tue, 04 May 2021 00:22:36 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Tue, 04 May 2021 00:22:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 May 2021 00:22:37 GMT
USER haproxy
# Tue, 04 May 2021 00:22:37 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7abf58d954de379f38a19e07330116ba6b11f21007bc7b7507d233e5b0aa3fe0`  
		Last Modified: Sat, 10 Apr 2021 06:38:07 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aac1e92e044b342ae4c034c566fa222f832eb644f4b438b0fb6c3b2bba9e17b`  
		Last Modified: Tue, 04 May 2021 00:24:56 GMT  
		Size: 10.1 MB (10115405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be28c1b468f352e30619ec7fc21e25a6294d76f0cd82df9149814a0784e91c9`  
		Last Modified: Tue, 04 May 2021 00:24:54 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev18` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:de596a58d637f4caf06283aecc31abf76e9e054cb97f2d57967ca055a3fdb660
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.6 MB (34623675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a616d5e4075e6d8b7901c0cf40e2601a7538ad6995b43d45302943777c20badf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:51:31 GMT
ADD file:926533a23a69aa2481a9122b667bb6300a347154eea366c9e679a230aa7f373a in / 
# Sat, 10 Apr 2021 00:51:34 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 02:24:17 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 03 May 2021 22:14:51 GMT
ENV HAPROXY_VERSION=2.4-dev18
# Mon, 03 May 2021 22:14:53 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev18.tar.gz
# Mon, 03 May 2021 22:14:54 GMT
ENV HAPROXY_SHA256=fab8b85664afc74c481c91a8f104b6bf87b265f9b5f03054dc926364e9801e74
# Tue, 04 May 2021 01:38:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Tue, 04 May 2021 01:38:02 GMT
STOPSIGNAL SIGUSR1
# Tue, 04 May 2021 01:38:03 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Tue, 04 May 2021 01:38:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 May 2021 01:38:04 GMT
USER haproxy
# Tue, 04 May 2021 01:38:06 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:33d77752597b664d047cc829e58a223d6fb077b61f69ca0462fcfb9b78d5f69b`  
		Last Modified: Sat, 10 Apr 2021 00:59:22 GMT  
		Size: 24.9 MB (24873199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c107a5973e1ce17cb311e2bf8a0d841875ca9f02219922ca12a9203602b5ce`  
		Last Modified: Sat, 10 Apr 2021 02:36:55 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c88150841fcb707acbd9df78ab1b9976a0baee7dffe499ad16c1e724bb17e3d`  
		Last Modified: Tue, 04 May 2021 01:38:53 GMT  
		Size: 9.7 MB (9748646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c10aa05248313ab068e205968ae811fe1a1a3e698c6ce0a1c465446548d62f`  
		Last Modified: Tue, 04 May 2021 01:38:50 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev18` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:b0483bbd360567db7dca54a5248197da9d4cb575d76a134c631269d32825332d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.3 MB (32332957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbda1941fa04cc1d1cd51ec3f37d84b46ab4013680a448cb7d1fd38ee859f624`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:59:45 GMT
ADD file:3fbd246a2de82566bcaaf62e3e0bf57175a7ad46b4156366a110661b31eab240 in / 
# Sat, 10 Apr 2021 00:59:47 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 08:58:51 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 03 May 2021 23:03:28 GMT
ENV HAPROXY_VERSION=2.4-dev18
# Mon, 03 May 2021 23:03:30 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev18.tar.gz
# Mon, 03 May 2021 23:03:31 GMT
ENV HAPROXY_SHA256=fab8b85664afc74c481c91a8f104b6bf87b265f9b5f03054dc926364e9801e74
# Tue, 04 May 2021 00:57:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Tue, 04 May 2021 00:57:22 GMT
STOPSIGNAL SIGUSR1
# Tue, 04 May 2021 00:57:23 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Tue, 04 May 2021 00:57:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 May 2021 00:57:25 GMT
USER haproxy
# Tue, 04 May 2021 00:57:26 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:8c6bea184b33030fb923c3c09d634b73235dec3fe2d411db9fd22bda669f2c37`  
		Last Modified: Sat, 10 Apr 2021 01:07:51 GMT  
		Size: 22.7 MB (22739801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5be95d3afdef3cc4c8a37695b513cf41e6cf6ffeecd9ce2426d38cb245a0b52`  
		Last Modified: Sat, 10 Apr 2021 09:05:25 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00eb766cefd963052599432a3eee0f4ed0fb73e0091b589eae5d9fe638fa8295`  
		Last Modified: Tue, 04 May 2021 00:59:32 GMT  
		Size: 9.6 MB (9591332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caae456a9be1f7eb6e4bd21828f1c1ae8df59fcb9846fe31bf383be1a3ac6e7c`  
		Last Modified: Tue, 04 May 2021 00:59:25 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev18` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:4b735ce00f4ed0c52833bd3323df7d398e1e3f1ded6fca8d4fd66175c03e14b0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35896311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:988b9033e9005759c723ac872ba6bf5e9641856f4b72349842adc7b6e9287656`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:41:25 GMT
ADD file:b24da7eb23eeae04e00d0e45da29a89fe8f992e8dcf4ba482afb907b8015b7bf in / 
# Sat, 10 Apr 2021 00:41:28 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:13:29 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 03 May 2021 22:00:56 GMT
ENV HAPROXY_VERSION=2.4-dev18
# Mon, 03 May 2021 22:00:58 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev18.tar.gz
# Mon, 03 May 2021 22:01:01 GMT
ENV HAPROXY_SHA256=fab8b85664afc74c481c91a8f104b6bf87b265f9b5f03054dc926364e9801e74
# Tue, 04 May 2021 01:05:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Tue, 04 May 2021 01:05:03 GMT
STOPSIGNAL SIGUSR1
# Tue, 04 May 2021 01:05:03 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Tue, 04 May 2021 01:05:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 May 2021 01:05:05 GMT
USER haproxy
# Tue, 04 May 2021 01:05:06 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:15cb40b9c4df1a06940dc2a154c3be46844241235c1a091afa70da0ee2dc811a`  
		Last Modified: Sat, 10 Apr 2021 00:47:53 GMT  
		Size: 25.9 MB (25904582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48cb832c3e00ffed789c3f464caa612fe4996ba4683f72f8cf214d1437268efe`  
		Last Modified: Sat, 10 Apr 2021 01:21:27 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d925210447f3d0f8b59a238243ccd2b9e02101ed90555f381f7f84d19ae2e1`  
		Last Modified: Tue, 04 May 2021 01:07:14 GMT  
		Size: 10.0 MB (9989898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9736f199f7eef04b231e3eeb0a60f4b428a35680111bd7460d298a79e9b6b43c`  
		Last Modified: Tue, 04 May 2021 01:07:11 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev18` - linux; 386

```console
$ docker pull haproxy@sha256:014484389b8ea19d5ef19ebbf4c071ebc87278974b0d28d191adaff3f27b5943
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.7 MB (37741158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2502fb424f9e89dfc69cbbaa8548cc16aae02889c960835b8a151022aa204f2a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:39:42 GMT
ADD file:8885d4d13678543780bb04ba14b621179665f7951d5b261036a7092df9b376e7 in / 
# Sat, 10 Apr 2021 00:39:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 03:48:12 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 03 May 2021 21:38:43 GMT
ENV HAPROXY_VERSION=2.4-dev18
# Mon, 03 May 2021 21:38:43 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev18.tar.gz
# Mon, 03 May 2021 21:38:43 GMT
ENV HAPROXY_SHA256=fab8b85664afc74c481c91a8f104b6bf87b265f9b5f03054dc926364e9801e74
# Tue, 04 May 2021 00:42:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Tue, 04 May 2021 00:42:13 GMT
STOPSIGNAL SIGUSR1
# Tue, 04 May 2021 00:42:13 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Tue, 04 May 2021 00:42:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 May 2021 00:42:13 GMT
USER haproxy
# Tue, 04 May 2021 00:42:13 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:7cc57a8772e5e479618650dfa70f315b474d3f205d04bde7f602f469c1928d84`  
		Last Modified: Sat, 10 Apr 2021 00:46:07 GMT  
		Size: 27.8 MB (27788987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d92d68a52363235dcdfb59fa81e5ef1a4561c958501e4f28d6b79e86f8b8501`  
		Last Modified: Sat, 10 Apr 2021 03:59:08 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:480bf4b481880037cfba39b650627fbf8efa247c10313bc2b6c6998ef7ce36c6`  
		Last Modified: Tue, 04 May 2021 00:45:19 GMT  
		Size: 10.0 MB (9950345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a02e0b403a23b63daf633fba5b1a69af54465eb277681175f3b41300e0e5497`  
		Last Modified: Tue, 04 May 2021 00:45:17 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev18` - linux; mips64le

```console
$ docker pull haproxy@sha256:ef40fdcad4f0bc78ae418fb5d258d33d3b6714393e58cb275bb8428ac111557f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.5 MB (35540367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85e4ee3838930d54eb73f8f29dedf4852000465c624a3ba25e2df165468636b0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:09:40 GMT
ADD file:0c93801c4a3719dfd4c047d7f2f4d52bf463eba2ab875da1dc54dcc832aae20b in / 
# Sat, 10 Apr 2021 01:09:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:39:36 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 03 May 2021 21:07:27 GMT
ENV HAPROXY_VERSION=2.4-dev18
# Mon, 03 May 2021 21:07:27 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev18.tar.gz
# Mon, 03 May 2021 21:07:28 GMT
ENV HAPROXY_SHA256=fab8b85664afc74c481c91a8f104b6bf87b265f9b5f03054dc926364e9801e74
# Tue, 04 May 2021 00:11:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Tue, 04 May 2021 00:11:23 GMT
STOPSIGNAL SIGUSR1
# Tue, 04 May 2021 00:11:23 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Tue, 04 May 2021 00:11:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 May 2021 00:11:24 GMT
USER haproxy
# Tue, 04 May 2021 00:11:24 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:09ea659ba566d9c3c62493e5ae0b964f1eee4fcf35aabc91c5c34ca1ad686541`  
		Last Modified: Sat, 10 Apr 2021 01:16:07 GMT  
		Size: 25.8 MB (25806410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10fa5ae1be1fc686c91c15f24ebaaa72d7c4f64321c8ead8386f2f4f9d1a6705`  
		Last Modified: Sat, 10 Apr 2021 01:53:41 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e5f90a2d5f0809c92154b735d248c941c30e4870c26a58a1ec299fb1bbc40d`  
		Last Modified: Tue, 04 May 2021 00:12:08 GMT  
		Size: 9.7 MB (9732125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aed81ba7a628ae4fa904ad01d253875ace9ac629c93b8efef3f84e7016f9f58`  
		Last Modified: Tue, 04 May 2021 00:12:01 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev18` - linux; ppc64le

```console
$ docker pull haproxy@sha256:63d8b128a955f475a90352af218b4e89dde12b1dc1f71217cf5065d829eeafec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.2 MB (41160234 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15a908ebe2a68fb86148a7b7f619856caaf5d4aa6dc8b8e063b2d0c9b7b09aec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:26:49 GMT
ADD file:ab87d4854aa8628ce8f4e603c0496499f6f28c3d2525ace782c7369691dafc8c in / 
# Sat, 10 Apr 2021 01:26:56 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 04:45:12 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 03 May 2021 22:08:29 GMT
ENV HAPROXY_VERSION=2.4-dev18
# Mon, 03 May 2021 22:08:45 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev18.tar.gz
# Mon, 03 May 2021 22:08:55 GMT
ENV HAPROXY_SHA256=fab8b85664afc74c481c91a8f104b6bf87b265f9b5f03054dc926364e9801e74
# Tue, 04 May 2021 02:31:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Tue, 04 May 2021 02:31:21 GMT
STOPSIGNAL SIGUSR1
# Tue, 04 May 2021 02:31:24 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Tue, 04 May 2021 02:31:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 May 2021 02:31:33 GMT
USER haproxy
# Tue, 04 May 2021 02:31:40 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:3e1e599482ca47095f85e429b346b76375aa85015ddcca050e85c2a8b1fdda9c`  
		Last Modified: Sat, 10 Apr 2021 01:33:57 GMT  
		Size: 30.5 MB (30545933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ee41bdc57145d3cb6e9f5fa23eed213567ae52835c7cff5fd57fe17b52f5ec`  
		Last Modified: Sat, 10 Apr 2021 05:09:50 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2474a657ff366e5e48721c53c9dfeaa4eb3cd267e4495c90d029798271e965ed`  
		Last Modified: Tue, 04 May 2021 02:35:46 GMT  
		Size: 10.6 MB (10612462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b2724278cfe96d7b12c35bb287a85151d17f358c9b096a8e2e4e2d41a72c85`  
		Last Modified: Tue, 04 May 2021 02:35:43 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev18` - linux; s390x

```console
$ docker pull haproxy@sha256:8589ed491dce111157fcb5ee3344bc59d9fb87715a06c1474b63467529d201fc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.5 MB (35543545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:effa514b71f49502a78660c7b8a0a2b86bab0ea2db081a5f104bd24e9941fc3b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:42:23 GMT
ADD file:dbe2182f8699f2a6011413ea01862e6c0e85853d922dffd72a28d994d23c79bc in / 
# Sat, 10 Apr 2021 00:42:25 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:38:04 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 03 May 2021 21:41:44 GMT
ENV HAPROXY_VERSION=2.4-dev18
# Mon, 03 May 2021 21:41:45 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev18.tar.gz
# Mon, 03 May 2021 21:41:46 GMT
ENV HAPROXY_SHA256=fab8b85664afc74c481c91a8f104b6bf87b265f9b5f03054dc926364e9801e74
# Tue, 04 May 2021 00:43:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Tue, 04 May 2021 00:43:46 GMT
STOPSIGNAL SIGUSR1
# Tue, 04 May 2021 00:43:47 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Tue, 04 May 2021 00:43:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 May 2021 00:43:48 GMT
USER haproxy
# Tue, 04 May 2021 00:43:48 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:65291f8717b3afd99b63cee867dd3e06b956a8ee6aa8580cc31d913b25de209d`  
		Last Modified: Sat, 10 Apr 2021 00:45:48 GMT  
		Size: 25.8 MB (25753787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9daf67acfb0373e31068762d068f1da8d320f2bdcdb0e6651d52b8183ede06c`  
		Last Modified: Sat, 10 Apr 2021 01:42:28 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f4b41baeaa740c725a5c78988f23e413b561477be09c0cce0da6c4b36d066e`  
		Last Modified: Tue, 04 May 2021 00:46:07 GMT  
		Size: 9.8 MB (9787929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5434bf5b14bf03c0b62030672f22a05a6aa533b00e4787adb13854bdc203db84`  
		Last Modified: Tue, 04 May 2021 00:46:05 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.4-dev18-alpine`

```console
$ docker pull haproxy@sha256:fff3f0655cabdad687de75fb0029908afcc12310f07af48b6862b3f0900b36d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `haproxy:2.4-dev18-alpine` - linux; amd64

```console
$ docker pull haproxy@sha256:cd1d4b94bb1e152362a1102c3f39b7aaec40cbe2bbb057c84019c4275f233fde
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.2 MB (10204009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2d1d52d63fa2e771ecaa1dfc84b1656492fa022899f057c65c4aec0caa00397`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:37:38 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 03 May 2021 22:00:59 GMT
ENV HAPROXY_VERSION=2.4-dev18
# Mon, 03 May 2021 22:00:59 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev18.tar.gz
# Mon, 03 May 2021 22:00:59 GMT
ENV HAPROXY_SHA256=fab8b85664afc74c481c91a8f104b6bf87b265f9b5f03054dc926364e9801e74
# Tue, 04 May 2021 00:23:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Tue, 04 May 2021 00:23:46 GMT
STOPSIGNAL SIGUSR1
# Tue, 04 May 2021 00:23:46 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Tue, 04 May 2021 00:23:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 May 2021 00:23:47 GMT
USER haproxy
# Tue, 04 May 2021 00:23:47 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4de1862a29af271c1751bf0d03d96f9a881f971d1288c5fafcfba90b517611f8`  
		Last Modified: Wed, 14 Apr 2021 21:43:30 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5978a5c5417dc9ccc24f889634189055c75a143eb5b561fd12772b4c8bd658c0`  
		Last Modified: Tue, 04 May 2021 00:25:07 GMT  
		Size: 7.4 MB (7390405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aafb9ab3199b8060748b7af8c0c4e9da0aae4fb59400bda69e7f78c47f754bfd`  
		Last Modified: Tue, 04 May 2021 00:25:06 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev18-alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:46455529abc15c9ed545e43305a67a2369bb200adb8935792787700f5f7472a1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9884300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec104b9a2fd2c70b6d3baec5fbb3218704bdb54d1ce96917e43ad64614fa4906`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:18:05 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 03 May 2021 22:10:09 GMT
ENV HAPROXY_VERSION=2.4-dev18
# Mon, 03 May 2021 22:10:10 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev18.tar.gz
# Mon, 03 May 2021 22:10:12 GMT
ENV HAPROXY_SHA256=fab8b85664afc74c481c91a8f104b6bf87b265f9b5f03054dc926364e9801e74
# Tue, 04 May 2021 00:53:50 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Tue, 04 May 2021 00:53:52 GMT
STOPSIGNAL SIGUSR1
# Tue, 04 May 2021 00:53:53 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Tue, 04 May 2021 00:53:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 May 2021 00:53:56 GMT
USER haproxy
# Tue, 04 May 2021 00:53:59 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd640f0f76e4e434b444a36110041f2c571b2dbcfca29958b2e90de8d91bd6eb`  
		Last Modified: Wed, 14 Apr 2021 21:34:02 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ced56deda546e1a28592d2c1e53fa305d7779fc8868ee6da4e54b7d6a81162d9`  
		Last Modified: Tue, 04 May 2021 00:54:49 GMT  
		Size: 7.3 MB (7260537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e78f23141b0b075fb3958f32438f4d337e870ced7c3003c7791aa13ba64b9a49`  
		Last Modified: Tue, 04 May 2021 00:54:46 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev18-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:1da1e6d181df5ec80ba2567aa60395ff144c642cc81a71ecf15cdd90980db7c3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9539946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:967689b3edae44a1953ea3038714702fa96e624fd3f3ec3171ef66d73e8fa6bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:47:58 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 03 May 2021 23:04:46 GMT
ENV HAPROXY_VERSION=2.4-dev18
# Mon, 03 May 2021 23:04:47 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev18.tar.gz
# Mon, 03 May 2021 23:04:49 GMT
ENV HAPROXY_SHA256=fab8b85664afc74c481c91a8f104b6bf87b265f9b5f03054dc926364e9801e74
# Tue, 04 May 2021 00:58:02 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Tue, 04 May 2021 00:58:03 GMT
STOPSIGNAL SIGUSR1
# Tue, 04 May 2021 00:58:03 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Tue, 04 May 2021 00:58:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 May 2021 00:58:06 GMT
USER haproxy
# Tue, 04 May 2021 00:58:07 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ff0f6ee9305bed375c784c12ad4beeac3af6ea1a6b5afeec6b4700259dc194`  
		Last Modified: Wed, 14 Apr 2021 22:56:09 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84e10884a0e017bd9319579dfcccd2647713ae4197d0a0d3191649ff84bf46d2`  
		Last Modified: Tue, 04 May 2021 00:59:41 GMT  
		Size: 7.1 MB (7114166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a6f22e2a5a631f64448e6d88809e7e0f5a013e2d51f1c96a59a57cd50954ae`  
		Last Modified: Tue, 04 May 2021 00:59:39 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev18-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:82aced14adaec465c871858f91902d5ae2862f183c298c03290ebddbea16013a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.1 MB (10119544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b64d57cba37710bb5fefd40e5432edf4c4da3a80692a12dcd2eb2a11f5129eb9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:26:01 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 03 May 2021 22:02:46 GMT
ENV HAPROXY_VERSION=2.4-dev18
# Mon, 03 May 2021 22:02:48 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev18.tar.gz
# Mon, 03 May 2021 22:02:50 GMT
ENV HAPROXY_SHA256=fab8b85664afc74c481c91a8f104b6bf87b265f9b5f03054dc926364e9801e74
# Tue, 04 May 2021 01:05:45 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Tue, 04 May 2021 01:05:46 GMT
STOPSIGNAL SIGUSR1
# Tue, 04 May 2021 01:05:47 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Tue, 04 May 2021 01:05:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 May 2021 01:05:49 GMT
USER haproxy
# Tue, 04 May 2021 01:05:50 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2ef9646f93509fb43536690b645509d9b653316324583761dd086b8ad6c664`  
		Last Modified: Wed, 14 Apr 2021 20:37:52 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cc170b442792d0820be4751eaf9284b5e1f9c8452adc7c7bbae45cf4abc2449`  
		Last Modified: Tue, 04 May 2021 01:07:23 GMT  
		Size: 7.4 MB (7405882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a811f2f75cbf30c7c3768d3727e399af7d53d39391dba3485f972e0958401aa5`  
		Last Modified: Tue, 04 May 2021 01:07:21 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev18-alpine` - linux; 386

```console
$ docker pull haproxy@sha256:8050aa2b81fbc31bf2d47ff76170fc198225802a6a672f6beac39d4dd13474a7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (9966930 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eabde26ca343b4e6d06e3ebf5f7eab077dc86ae5b65a2c8c6dc6d48d30167c82`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 01:50:06 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 03 May 2021 21:40:10 GMT
ENV HAPROXY_VERSION=2.4-dev18
# Mon, 03 May 2021 21:40:10 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev18.tar.gz
# Mon, 03 May 2021 21:40:10 GMT
ENV HAPROXY_SHA256=fab8b85664afc74c481c91a8f104b6bf87b265f9b5f03054dc926364e9801e74
# Tue, 04 May 2021 00:43:27 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Tue, 04 May 2021 00:43:27 GMT
STOPSIGNAL SIGUSR1
# Tue, 04 May 2021 00:43:27 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Tue, 04 May 2021 00:43:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 May 2021 00:43:28 GMT
USER haproxy
# Tue, 04 May 2021 00:43:28 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:31b7e7ccca9e17fd08b39c9a4ffd3ded380b62816c489d6c3758c9bb5a632430`  
		Last Modified: Wed, 14 Apr 2021 18:39:24 GMT  
		Size: 2.8 MB (2818900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9104145d2a6b1e0c0837c464bb9d4b331949cfeb6be12e4e7995507661d3386`  
		Last Modified: Thu, 15 Apr 2021 02:00:28 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b8d327b19497f7a82d2a7802891b4b637c5375fd93ac2c296c8411ed46191c`  
		Last Modified: Tue, 04 May 2021 00:45:37 GMT  
		Size: 7.1 MB (7146396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97049f66fdbe40a5dc5419f8cb59bfdc729cef644fe9cbc2b54dd07c6e859beb`  
		Last Modified: Tue, 04 May 2021 00:45:35 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev18-alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:b6bc56380c0ff12d3fa3f08f6d15b3dc36a51a2f9f9a2996ecf652c19420d94d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.5 MB (10522791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e02adafc155ab468e09e38b45a2fb4f2fe1d55809615e5329dc6b4329d14164e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:25:09 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 03 May 2021 22:17:14 GMT
ENV HAPROXY_VERSION=2.4-dev18
# Mon, 03 May 2021 22:17:20 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev18.tar.gz
# Mon, 03 May 2021 22:17:24 GMT
ENV HAPROXY_SHA256=fab8b85664afc74c481c91a8f104b6bf87b265f9b5f03054dc926364e9801e74
# Tue, 04 May 2021 02:34:03 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Tue, 04 May 2021 02:34:08 GMT
STOPSIGNAL SIGUSR1
# Tue, 04 May 2021 02:34:12 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Tue, 04 May 2021 02:34:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 May 2021 02:34:24 GMT
USER haproxy
# Tue, 04 May 2021 02:34:29 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8004273856b1b354059d03a17deec6e79d325ba45d63213dda3d1fa401db8c22`  
		Last Modified: Wed, 14 Apr 2021 23:36:37 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2d01c3d76fa82c4d7c15660c556631039a02991913228f2ac9d272637bff02`  
		Last Modified: Tue, 04 May 2021 02:36:01 GMT  
		Size: 7.7 MB (7708015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be3f83810256ffbcc290dfd487039e4547bedd19195eb05bb0046ecd84d232f`  
		Last Modified: Tue, 04 May 2021 02:36:00 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev18-alpine` - linux; s390x

```console
$ docker pull haproxy@sha256:a764219bb48566020018c624e90819cc7142651a64baeffc1487c61a4dc4a05d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9916511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6833ad147838c6ffb79dfcd49f30a098ec2628b3a4ab7ce2f39599596a4a8ae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:54:24 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Mon, 03 May 2021 21:43:04 GMT
ENV HAPROXY_VERSION=2.4-dev18
# Mon, 03 May 2021 21:43:04 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev18.tar.gz
# Mon, 03 May 2021 21:43:05 GMT
ENV HAPROXY_SHA256=fab8b85664afc74c481c91a8f104b6bf87b265f9b5f03054dc926364e9801e74
# Tue, 04 May 2021 00:44:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Tue, 04 May 2021 00:44:44 GMT
STOPSIGNAL SIGUSR1
# Tue, 04 May 2021 00:44:45 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Tue, 04 May 2021 00:44:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 04 May 2021 00:44:45 GMT
USER haproxy
# Tue, 04 May 2021 00:44:46 GMT
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
	-	`sha256:2b4cfaaf827d363dc52189f0441a927ff267eb6eea9e081c19f6d728ff52d6a8`  
		Last Modified: Tue, 04 May 2021 00:46:18 GMT  
		Size: 7.3 MB (7312228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0441e6ef4431841df737d4be3294d20151800d805183d15d96602b45568ed2e`  
		Last Modified: Tue, 04 May 2021 00:46:17 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:alpine`

```console
$ docker pull haproxy@sha256:1168dcda566f7ce42120fe56135178d78752e7d198b4f96a77c00f1b06af1853
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `haproxy:alpine` - linux; amd64

```console
$ docker pull haproxy@sha256:6d16465fe404f162ffcfd564eea2774ba06edf7188280484a270cd8862c35a88
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9501835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77414e3b99078b756a62667c18c85f4359518b1610a2cc6f57d682ce7a4f3bb2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:37:38 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 23 Apr 2021 20:20:47 GMT
ENV HAPROXY_VERSION=2.3.10
# Fri, 23 Apr 2021 20:20:47 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Fri, 23 Apr 2021 20:20:47 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Fri, 23 Apr 2021 20:21:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 23 Apr 2021 20:21:37 GMT
STOPSIGNAL SIGUSR1
# Fri, 23 Apr 2021 20:21:37 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 23 Apr 2021 20:21:38 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 20:21:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 20:21:38 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4de1862a29af271c1751bf0d03d96f9a881f971d1288c5fafcfba90b517611f8`  
		Last Modified: Wed, 14 Apr 2021 21:43:30 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cba67cd0abe26102179dbd1deb88405bc4764e51a2b1f6ef06232cb9eca0ce6`  
		Last Modified: Fri, 23 Apr 2021 20:22:54 GMT  
		Size: 6.7 MB (6688111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:500b344a0df360398223362751a2ceab4c0981e06e375ff45905d04507537387`  
		Last Modified: Fri, 23 Apr 2021 20:22:53 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2724c9435ec936799a1c47edd9cb5e46f597d30b3e3cab7b0e32d855741fabb`  
		Last Modified: Fri, 23 Apr 2021 20:22:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:7e27a3587e72e37010d991363a75b6cc01493a686a23ed0a8a780a49c6ee2494
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.2 MB (9211848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1aec7a3cb069441d455cdee3c8970689988845ee8742770933e8b091a05a52e0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:18:05 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 23 Apr 2021 20:51:06 GMT
ENV HAPROXY_VERSION=2.3.10
# Fri, 23 Apr 2021 20:51:07 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Fri, 23 Apr 2021 20:51:08 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Fri, 23 Apr 2021 20:51:33 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 23 Apr 2021 20:51:35 GMT
STOPSIGNAL SIGUSR1
# Fri, 23 Apr 2021 20:51:35 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 23 Apr 2021 20:51:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 20:51:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 20:51:39 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd640f0f76e4e434b444a36110041f2c571b2dbcfca29958b2e90de8d91bd6eb`  
		Last Modified: Wed, 14 Apr 2021 21:34:02 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54049885ecd472a5548c06de21ae362a2dde172e52f8118579b63d389c596214`  
		Last Modified: Fri, 23 Apr 2021 20:52:23 GMT  
		Size: 6.6 MB (6587961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa68a40a7e61b9513c658b23339f17a1e97ed7660b0c9828c04b65f3fb8ae637`  
		Last Modified: Fri, 23 Apr 2021 20:52:20 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dba2abb2f77db1891b207f81dcc8f6f93862222a15a489e3f153d999d8d6bfb`  
		Last Modified: Fri, 23 Apr 2021 20:52:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:849282abf73b940f2e28483aea32e03a54075b7dbc6714d00412742327a88b5e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.9 MB (8927012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbb9ef13943f7a6fced52d987a05ef61afbdd96efb69d6f263810cb54037b990`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:47:58 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 23 Apr 2021 21:00:39 GMT
ENV HAPROXY_VERSION=2.3.10
# Fri, 23 Apr 2021 21:00:39 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Fri, 23 Apr 2021 21:00:40 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Fri, 23 Apr 2021 21:01:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 23 Apr 2021 21:01:10 GMT
STOPSIGNAL SIGUSR1
# Fri, 23 Apr 2021 21:01:11 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 23 Apr 2021 21:01:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 21:01:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 21:01:21 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ff0f6ee9305bed375c784c12ad4beeac3af6ea1a6b5afeec6b4700259dc194`  
		Last Modified: Wed, 14 Apr 2021 22:56:09 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb1d6019b6548f16be0cfff81a3a38f64337636d40ec6d50697915983ca3887f`  
		Last Modified: Fri, 23 Apr 2021 21:02:54 GMT  
		Size: 6.5 MB (6501111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e17ccc0c26b79d4583ef2907084a53e7a69a87686939491984151ac2ead75b1`  
		Last Modified: Fri, 23 Apr 2021 21:02:52 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f451a3dd3dd7b108fdbe462194e6659be8f76b7a69911c306d74d8fceeed3f`  
		Last Modified: Fri, 23 Apr 2021 21:02:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:ec0989fc82ace88b5cf80c0dc55e695e5a5d6620174e4ed0d5d8c1634630f2e7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9413982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cd73593d809a141875771ab3f582e9a6258ba6fe0f4b707f0ce439cd47a7405`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:26:01 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 23 Apr 2021 20:41:19 GMT
ENV HAPROXY_VERSION=2.3.10
# Fri, 23 Apr 2021 20:41:19 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Fri, 23 Apr 2021 20:41:20 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Fri, 23 Apr 2021 20:41:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 23 Apr 2021 20:41:44 GMT
STOPSIGNAL SIGUSR1
# Fri, 23 Apr 2021 20:41:45 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 23 Apr 2021 20:41:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 20:41:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 20:41:48 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2ef9646f93509fb43536690b645509d9b653316324583761dd086b8ad6c664`  
		Last Modified: Wed, 14 Apr 2021 20:37:52 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffe20dd6ddd5d14baec905dc0c113e8dd01ce5899588c89675a6988ccfe34a48`  
		Last Modified: Fri, 23 Apr 2021 20:43:13 GMT  
		Size: 6.7 MB (6700201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1616786188830f47d2d1ea30821c3aa828e4a87dbc5d075f5f6eee2c1fdaec`  
		Last Modified: Fri, 23 Apr 2021 20:43:09 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c147d090d4db064f2514f9bfa6a9cb2e6d716e448d94b4ab90e2b7a0e50ab03`  
		Last Modified: Fri, 23 Apr 2021 20:43:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:alpine` - linux; 386

```console
$ docker pull haproxy@sha256:839a53bd7d2f00b0d67b1c764d9811b7491a3d4d645a6abb94ebd84293e4c367
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9356996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b30351ad929f3d405e1ca732a718c6e0fe63e1a52c2407a4d9600fff4e7e439b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 01:50:06 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 23 Apr 2021 20:39:47 GMT
ENV HAPROXY_VERSION=2.3.10
# Fri, 23 Apr 2021 20:39:47 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Fri, 23 Apr 2021 20:39:47 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Fri, 23 Apr 2021 20:40:45 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 23 Apr 2021 20:40:45 GMT
STOPSIGNAL SIGUSR1
# Fri, 23 Apr 2021 20:40:45 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 23 Apr 2021 20:40:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 20:40:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 20:40:47 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:31b7e7ccca9e17fd08b39c9a4ffd3ded380b62816c489d6c3758c9bb5a632430`  
		Last Modified: Wed, 14 Apr 2021 18:39:24 GMT  
		Size: 2.8 MB (2818900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9104145d2a6b1e0c0837c464bb9d4b331949cfeb6be12e4e7995507661d3386`  
		Last Modified: Thu, 15 Apr 2021 02:00:28 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22386ff451c9485cc86547597a9df94ba437d282baedc6b3ff68139348ab838e`  
		Last Modified: Fri, 23 Apr 2021 20:42:53 GMT  
		Size: 6.5 MB (6536340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44c782fb9ce01dfc03b5926dd9052609853265d68ef395e663ca422aba662667`  
		Last Modified: Fri, 23 Apr 2021 20:42:51 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eab34669a9636f82828df5502f0d94263605f7309e0bab880f3d9bc324b052b`  
		Last Modified: Fri, 23 Apr 2021 20:42:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:a4daa01e291804783faf44842f65f63d7108530d7623efce6d782952fe4bcbf9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.8 MB (9835818 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2ebb4297d3c174774a272e1f8a0042fc3c7c9ca7b1d0cf36d5af3d58b36005c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:25:09 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 23 Apr 2021 20:23:26 GMT
ENV HAPROXY_VERSION=2.3.10
# Fri, 23 Apr 2021 20:23:31 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Fri, 23 Apr 2021 20:23:34 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Fri, 23 Apr 2021 20:24:19 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 23 Apr 2021 20:24:24 GMT
STOPSIGNAL SIGUSR1
# Fri, 23 Apr 2021 20:24:27 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 23 Apr 2021 20:24:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 20:24:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 20:24:42 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8004273856b1b354059d03a17deec6e79d325ba45d63213dda3d1fa401db8c22`  
		Last Modified: Wed, 14 Apr 2021 23:36:37 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b9cdc9560132361ff8957311b5fd6b2bbacc8ec5be9489a16a3b3eea31f3d2`  
		Last Modified: Fri, 23 Apr 2021 20:26:10 GMT  
		Size: 7.0 MB (7020918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac490252619a4b1389b0e3fb3c472b84a443f9bc3d346558d7ac67596be3eb0`  
		Last Modified: Fri, 23 Apr 2021 20:26:11 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554ee7adacda14ba7a4c490cead3c19a063d98a21b022b06f60bff9e6089a817`  
		Last Modified: Fri, 23 Apr 2021 20:26:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:alpine` - linux; s390x

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

## `haproxy:latest`

```console
$ docker pull haproxy@sha256:afbda854ad4e4dc64b71a98f6d185e27758cbc1580549445e27126081dba8f8e
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

### `haproxy:latest` - linux; amd64

```console
$ docker pull haproxy@sha256:37c2ffe40f2f485a870f13f6974fd2d58c882da58776829612cdc845b595d0e9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.7 MB (36697077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:058875cd29c9463c410c2b570b5af60359322f5eed84da753c5afb0b9d98494b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:29:42 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 23 Apr 2021 20:19:56 GMT
ENV HAPROXY_VERSION=2.3.10
# Fri, 23 Apr 2021 20:19:56 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Fri, 23 Apr 2021 20:19:57 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Fri, 23 Apr 2021 20:20:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 23 Apr 2021 20:20:41 GMT
STOPSIGNAL SIGUSR1
# Fri, 23 Apr 2021 20:20:41 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 23 Apr 2021 20:20:42 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 20:20:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 20:20:42 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7abf58d954de379f38a19e07330116ba6b11f21007bc7b7507d233e5b0aa3fe0`  
		Last Modified: Sat, 10 Apr 2021 06:38:07 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afffe9e17aa10b7f5f89d5f5d2b55dc515f8d762cff20d4a2af6ee4415c875da`  
		Last Modified: Fri, 23 Apr 2021 20:22:40 GMT  
		Size: 9.6 MB (9555753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feae1ae443ea753af3373bfd3a522884ab6700544ff8f21c34be1b038eaa9902`  
		Last Modified: Fri, 23 Apr 2021 20:22:40 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23c1d2a159159248851cd19c28b4aed4acde0c87c647d8e057f2d8ddf3cfc2d`  
		Last Modified: Fri, 23 Apr 2021 20:22:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:latest` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:f432474954fa25c79340f43b57a02e67903eeafa948d1a5aef55cf66f0a30a49
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (34041416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49787d7d5fd3a955e3efdfbe4783c4001482725f7815058b0c46eaeb6f9b44b5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:51:31 GMT
ADD file:926533a23a69aa2481a9122b667bb6300a347154eea366c9e679a230aa7f373a in / 
# Sat, 10 Apr 2021 00:51:34 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 02:24:17 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 23 Apr 2021 20:48:40 GMT
ENV HAPROXY_VERSION=2.3.10
# Fri, 23 Apr 2021 20:48:40 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Fri, 23 Apr 2021 20:48:41 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Fri, 23 Apr 2021 20:49:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 23 Apr 2021 20:49:26 GMT
STOPSIGNAL SIGUSR1
# Fri, 23 Apr 2021 20:49:28 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 23 Apr 2021 20:49:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 20:49:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 20:49:33 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:33d77752597b664d047cc829e58a223d6fb077b61f69ca0462fcfb9b78d5f69b`  
		Last Modified: Sat, 10 Apr 2021 00:59:22 GMT  
		Size: 24.9 MB (24873199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c107a5973e1ce17cb311e2bf8a0d841875ca9f02219922ca12a9203602b5ce`  
		Last Modified: Sat, 10 Apr 2021 02:36:55 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4fd166622140d354f76734dca13311daf08f4b0e1a2bd667bd8f1237147d592`  
		Last Modified: Fri, 23 Apr 2021 20:50:23 GMT  
		Size: 9.2 MB (9166265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6683d8d529358b8fd7297f933059372813f6a97b67c13987e9e309aeb63e9d7`  
		Last Modified: Fri, 23 Apr 2021 20:50:20 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2740aff641d0d26151406fb76c73059f6f37d65543141d4a46600055c477dbce`  
		Last Modified: Fri, 23 Apr 2021 20:50:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:latest` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:049069171782a5ea16bc2052ee484dd63b650e108f9e48db799e55c667ee9d29
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31771359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d474b012eeaa8b00ec45f00f784bdaff3606013979b8ed2c920d960e1a6e5c0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:59:45 GMT
ADD file:3fbd246a2de82566bcaaf62e3e0bf57175a7ad46b4156366a110661b31eab240 in / 
# Sat, 10 Apr 2021 00:59:47 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 08:58:51 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 23 Apr 2021 20:59:31 GMT
ENV HAPROXY_VERSION=2.3.10
# Fri, 23 Apr 2021 20:59:31 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Fri, 23 Apr 2021 20:59:32 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Fri, 23 Apr 2021 21:00:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 23 Apr 2021 21:00:18 GMT
STOPSIGNAL SIGUSR1
# Fri, 23 Apr 2021 21:00:18 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 23 Apr 2021 21:00:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 21:00:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 21:00:25 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:8c6bea184b33030fb923c3c09d634b73235dec3fe2d411db9fd22bda669f2c37`  
		Last Modified: Sat, 10 Apr 2021 01:07:51 GMT  
		Size: 22.7 MB (22739801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5be95d3afdef3cc4c8a37695b513cf41e6cf6ffeecd9ce2426d38cb245a0b52`  
		Last Modified: Sat, 10 Apr 2021 09:05:25 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717bc5365fb4bcdb4738770e1f312f2f58a06135e8d00643b6eb56fc013fcfe2`  
		Last Modified: Fri, 23 Apr 2021 21:02:42 GMT  
		Size: 9.0 MB (9029609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3f9836ad3bdc29bcf6b0ea0ca6e1478d1348e1015e7dd6ba91a44f8c523a050`  
		Last Modified: Fri, 23 Apr 2021 21:02:39 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:724e48ed89849e1da6018edaf2c357f02df92850ddb50bf446da7b127792dab7`  
		Last Modified: Fri, 23 Apr 2021 21:02:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:latest` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:62ef02fde66dea080deea6a17011711125171d1448d475c118f9ea2d691a42be
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.4 MB (35351171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9426ad19c62950e93ccf52c6f26ea94f779739576a8b938e340b22015a08a527`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:41:25 GMT
ADD file:b24da7eb23eeae04e00d0e45da29a89fe8f992e8dcf4ba482afb907b8015b7bf in / 
# Sat, 10 Apr 2021 00:41:28 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:13:29 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 23 Apr 2021 20:40:21 GMT
ENV HAPROXY_VERSION=2.3.10
# Fri, 23 Apr 2021 20:40:22 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Fri, 23 Apr 2021 20:40:22 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Fri, 23 Apr 2021 20:41:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 23 Apr 2021 20:41:03 GMT
STOPSIGNAL SIGUSR1
# Fri, 23 Apr 2021 20:41:04 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 23 Apr 2021 20:41:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 20:41:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 20:41:07 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:15cb40b9c4df1a06940dc2a154c3be46844241235c1a091afa70da0ee2dc811a`  
		Last Modified: Sat, 10 Apr 2021 00:47:53 GMT  
		Size: 25.9 MB (25904582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48cb832c3e00ffed789c3f464caa612fe4996ba4683f72f8cf214d1437268efe`  
		Last Modified: Sat, 10 Apr 2021 01:21:27 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99a4194f9c3742aa2f14d298181297121bb2c902d5eec8249de7c2ccb315d34`  
		Last Modified: Fri, 23 Apr 2021 20:43:01 GMT  
		Size: 9.4 MB (9444636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18eb1616784d5ffc7039165a0a02e92e1d9db3d88f8746a790b2558cd40a4974`  
		Last Modified: Fri, 23 Apr 2021 20:42:58 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baadd6b3908aad2d6176197c1816634a6271f00ce248db43ac40027449ababa2`  
		Last Modified: Fri, 23 Apr 2021 20:42:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:latest` - linux; 386

```console
$ docker pull haproxy@sha256:31390a54f68d62f3e7c80af3ddd2feb656e92553aa50acba7af43a06dcd5b560
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.2 MB (37209592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cf7eddc35247bbe2921775551965d6f38dbf1ee3be73cfb9f6544aaea2db502`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:39:42 GMT
ADD file:8885d4d13678543780bb04ba14b621179665f7951d5b261036a7092df9b376e7 in / 
# Sat, 10 Apr 2021 00:39:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 03:48:12 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 23 Apr 2021 20:38:45 GMT
ENV HAPROXY_VERSION=2.3.10
# Fri, 23 Apr 2021 20:38:45 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Fri, 23 Apr 2021 20:38:46 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Fri, 23 Apr 2021 20:39:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 23 Apr 2021 20:39:35 GMT
STOPSIGNAL SIGUSR1
# Fri, 23 Apr 2021 20:39:35 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 23 Apr 2021 20:39:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 20:39:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 20:39:36 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:7cc57a8772e5e479618650dfa70f315b474d3f205d04bde7f602f469c1928d84`  
		Last Modified: Sat, 10 Apr 2021 00:46:07 GMT  
		Size: 27.8 MB (27788987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d92d68a52363235dcdfb59fa81e5ef1a4561c958501e4f28d6b79e86f8b8501`  
		Last Modified: Sat, 10 Apr 2021 03:59:08 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c799704f6f7241fe4fe9658644a136f7f3a32cde54d58f63d2271c65f604e88`  
		Last Modified: Fri, 23 Apr 2021 20:42:36 GMT  
		Size: 9.4 MB (9418656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59f1328c2bd9da85a0836e5fd35839fdec1c3e22e0e5c30650827a10891c0ba7`  
		Last Modified: Fri, 23 Apr 2021 20:42:34 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:525b4de4d515d0e1e55046e2b12bc6368f5821f6c311a7bb5e2af64beca2282d`  
		Last Modified: Fri, 23 Apr 2021 20:42:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:latest` - linux; mips64le

```console
$ docker pull haproxy@sha256:e40a773567ecc6a0378962548f266a89f0651c1f7dc8c1b2a3ca5e2f984fb7c0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.9 MB (34943218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:609cf796bed6fbe5ca0f3ae499bf6d7a955768064cb0d180a60131050dd6fa35`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:09:40 GMT
ADD file:0c93801c4a3719dfd4c047d7f2f4d52bf463eba2ab875da1dc54dcc832aae20b in / 
# Sat, 10 Apr 2021 01:09:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:39:36 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 23 Apr 2021 20:07:26 GMT
ENV HAPROXY_VERSION=2.3.10
# Fri, 23 Apr 2021 20:07:26 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Fri, 23 Apr 2021 20:07:26 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Fri, 23 Apr 2021 20:09:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 23 Apr 2021 20:09:50 GMT
STOPSIGNAL SIGUSR1
# Fri, 23 Apr 2021 20:09:50 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 23 Apr 2021 20:09:52 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 20:09:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 20:09:53 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:09ea659ba566d9c3c62493e5ae0b964f1eee4fcf35aabc91c5c34ca1ad686541`  
		Last Modified: Sat, 10 Apr 2021 01:16:07 GMT  
		Size: 25.8 MB (25806410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10fa5ae1be1fc686c91c15f24ebaaa72d7c4f64321c8ead8386f2f4f9d1a6705`  
		Last Modified: Sat, 10 Apr 2021 01:53:41 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c195a6aaaf12a34216b2d8aca52aa55b0f937fd8618100d1e0e08d9c6f43d8b0`  
		Last Modified: Fri, 23 Apr 2021 20:10:38 GMT  
		Size: 9.1 MB (9134856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ba9d4d0ca44a4f5b7349bbea2e1e64c1d3fa001ef5d09b38f803eebe6bcfffb`  
		Last Modified: Fri, 23 Apr 2021 20:10:31 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:725b140d9e91c81a346e8cf6395c2058a6c206f327ef7ec6ecc36e2542838887`  
		Last Modified: Fri, 23 Apr 2021 20:10:31 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:latest` - linux; ppc64le

```console
$ docker pull haproxy@sha256:ff52706fced2f786b64882c9d1e94ed5284c38c042c0e693e4ed87d7dc33c0c5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40589965 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd48e104b02ba284aa5985fd56e31c4bbf1689501afe8a8cfc5aaa1967626fc5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:26:49 GMT
ADD file:ab87d4854aa8628ce8f4e603c0496499f6f28c3d2525ace782c7369691dafc8c in / 
# Sat, 10 Apr 2021 01:26:56 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 04:45:12 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 23 Apr 2021 20:18:41 GMT
ENV HAPROXY_VERSION=2.3.10
# Fri, 23 Apr 2021 20:18:49 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Fri, 23 Apr 2021 20:18:54 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Fri, 23 Apr 2021 20:22:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 23 Apr 2021 20:22:51 GMT
STOPSIGNAL SIGUSR1
# Fri, 23 Apr 2021 20:22:53 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 23 Apr 2021 20:23:02 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 20:23:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 20:23:06 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:3e1e599482ca47095f85e429b346b76375aa85015ddcca050e85c2a8b1fdda9c`  
		Last Modified: Sat, 10 Apr 2021 01:33:57 GMT  
		Size: 30.5 MB (30545933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ee41bdc57145d3cb6e9f5fa23eed213567ae52835c7cff5fd57fe17b52f5ec`  
		Last Modified: Sat, 10 Apr 2021 05:09:50 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c841a7f82bff751f994b8799d674c7d4211251a43359351397999911cfa870`  
		Last Modified: Fri, 23 Apr 2021 20:25:56 GMT  
		Size: 10.0 MB (10042073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4641283e776afb6c306c0a6965f7e0b1238d91bc09f304ea32545464581a9f6`  
		Last Modified: Fri, 23 Apr 2021 20:25:53 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5248644a4705a96ac93d3ebbb06d89ed62a29bf7ae76226a7a3fd7cd388554b9`  
		Last Modified: Fri, 23 Apr 2021 20:25:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:latest` - linux; s390x

```console
$ docker pull haproxy@sha256:65f0248af9b095156adf78d96f4f792c03a87cb2277ef4c8f36d44333921625a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.0 MB (35046751 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84ba273a498e9d8f8422051771b73d62e5f4fedd88d8b5ef771f73d069b6af0f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:42:23 GMT
ADD file:dbe2182f8699f2a6011413ea01862e6c0e85853d922dffd72a28d994d23c79bc in / 
# Sat, 10 Apr 2021 00:42:25 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:38:04 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 23 Apr 2021 20:41:50 GMT
ENV HAPROXY_VERSION=2.3.10
# Fri, 23 Apr 2021 20:41:51 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Fri, 23 Apr 2021 20:41:51 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Fri, 23 Apr 2021 20:42:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 23 Apr 2021 20:42:54 GMT
STOPSIGNAL SIGUSR1
# Fri, 23 Apr 2021 20:42:54 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 23 Apr 2021 20:42:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Fri, 23 Apr 2021 20:42:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Apr 2021 20:42:57 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:65291f8717b3afd99b63cee867dd3e06b956a8ee6aa8580cc31d913b25de209d`  
		Last Modified: Sat, 10 Apr 2021 00:45:48 GMT  
		Size: 25.8 MB (25753787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9daf67acfb0373e31068762d068f1da8d320f2bdcdb0e6651d52b8183ede06c`  
		Last Modified: Sat, 10 Apr 2021 01:42:28 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e00467b5656b09a7387dfd6e3adb3b30d4e7bddcaad2d25e8e422f7dcce2a58f`  
		Last Modified: Fri, 23 Apr 2021 20:45:10 GMT  
		Size: 9.3 MB (9291015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd5ec62c92ca691a7dd3e4602bad6d4be9d23dcd5d2f7420b30100f6b361cdbe`  
		Last Modified: Fri, 23 Apr 2021 20:45:09 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670261f5947e500477b59eac7f9966e7e1d4eae57a4132c42252790506139977`  
		Last Modified: Fri, 23 Apr 2021 20:45:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:lts`

```console
$ docker pull haproxy@sha256:792ac7e9a42dcb028039bd6ec02cfdde75e94980652121e1fe557e7cf8b847bb
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

### `haproxy:lts` - linux; amd64

```console
$ docker pull haproxy@sha256:6706d478e4e608c4d7aff4b100c029ed8ed5387f41f6d7d8b4b6ac9ecba3b745
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.5 MB (36450315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b71355e785ee76f43999ed2fa4612e47d61b76c61b3045c4d866b169b192bc99`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:29:42 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 29 Apr 2021 17:29:19 GMT
ENV HAPROXY_VERSION=2.2.14
# Thu, 29 Apr 2021 17:29:20 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Thu, 29 Apr 2021 17:29:20 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Thu, 29 Apr 2021 17:30:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 29 Apr 2021 17:30:04 GMT
STOPSIGNAL SIGUSR1
# Thu, 29 Apr 2021 17:30:04 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 29 Apr 2021 17:30:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 29 Apr 2021 17:30:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Apr 2021 17:30:06 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7abf58d954de379f38a19e07330116ba6b11f21007bc7b7507d233e5b0aa3fe0`  
		Last Modified: Sat, 10 Apr 2021 06:38:07 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ba487cb42887a026b3940ab5d25240db3ae8ca3538a433d33ded6c1e78ad946`  
		Last Modified: Thu, 29 Apr 2021 17:32:22 GMT  
		Size: 9.3 MB (9308992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f13a5faba9b80662ce1beda2cf0d30503c88a5569751155fd6d9fcfe6323ac46`  
		Last Modified: Thu, 29 Apr 2021 17:32:20 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3261bbc066b08611abdde75acf1a7a9a48c2d49f7540dcbc9a3c8e450ba4bd1b`  
		Last Modified: Thu, 29 Apr 2021 17:32:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:c36e6561bbe1be11cfd9b264eb760158871281895cdccacaa2aace07b64e704d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33788380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be71ea57166ad123cfb3dde36d0d110e554e5bbd5762aa5694b2903a5642af2a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:51:31 GMT
ADD file:926533a23a69aa2481a9122b667bb6300a347154eea366c9e679a230aa7f373a in / 
# Sat, 10 Apr 2021 00:51:34 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 02:24:17 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 29 Apr 2021 17:48:45 GMT
ENV HAPROXY_VERSION=2.2.14
# Thu, 29 Apr 2021 17:48:45 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Thu, 29 Apr 2021 17:48:46 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Thu, 29 Apr 2021 17:49:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 29 Apr 2021 17:49:35 GMT
STOPSIGNAL SIGUSR1
# Thu, 29 Apr 2021 17:49:36 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 29 Apr 2021 17:49:39 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 29 Apr 2021 17:49:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Apr 2021 17:49:40 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:33d77752597b664d047cc829e58a223d6fb077b61f69ca0462fcfb9b78d5f69b`  
		Last Modified: Sat, 10 Apr 2021 00:59:22 GMT  
		Size: 24.9 MB (24873199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c107a5973e1ce17cb311e2bf8a0d841875ca9f02219922ca12a9203602b5ce`  
		Last Modified: Sat, 10 Apr 2021 02:36:55 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a77f509b71668a040ff49cefb629a69b38b8703e98ed245bd0a97e97d10dc941`  
		Last Modified: Thu, 29 Apr 2021 17:50:22 GMT  
		Size: 8.9 MB (8913230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465b06ecb24dfbadcc493326bbf81d26de8a87e42dca5391cb9fcce5b693ce68`  
		Last Modified: Thu, 29 Apr 2021 17:50:19 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a57c7b8bed3c607d9c0e9cbe2d9e7538c16f5e02eb14d538227db37c7bb17e28`  
		Last Modified: Thu, 29 Apr 2021 17:50:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:f2d6692932a23d8178cadfbdc361c84a1f9dee4b7f0aeba65040899f65303432
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.5 MB (31464618 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7706d3cb80f141f9f889baea70aa79afc549e227e90bffd1aded90f5703bff2d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:59:45 GMT
ADD file:3fbd246a2de82566bcaaf62e3e0bf57175a7ad46b4156366a110661b31eab240 in / 
# Sat, 10 Apr 2021 00:59:47 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 08:58:51 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 29 Apr 2021 16:59:52 GMT
ENV HAPROXY_VERSION=2.2.14
# Thu, 29 Apr 2021 16:59:52 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Thu, 29 Apr 2021 16:59:53 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Thu, 29 Apr 2021 17:00:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 29 Apr 2021 17:00:35 GMT
STOPSIGNAL SIGUSR1
# Thu, 29 Apr 2021 17:00:36 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 29 Apr 2021 17:00:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 29 Apr 2021 17:00:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Apr 2021 17:00:41 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:8c6bea184b33030fb923c3c09d634b73235dec3fe2d411db9fd22bda669f2c37`  
		Last Modified: Sat, 10 Apr 2021 01:07:51 GMT  
		Size: 22.7 MB (22739801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5be95d3afdef3cc4c8a37695b513cf41e6cf6ffeecd9ce2426d38cb245a0b52`  
		Last Modified: Sat, 10 Apr 2021 09:05:25 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:110847a1cab7ee7d5910a3162e69e05dc4b27b38bbf0690fd5287335ca45d994`  
		Last Modified: Thu, 29 Apr 2021 17:02:34 GMT  
		Size: 8.7 MB (8722868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842fd9bf0561243131b85223fd2121bca335a34398de2805ce2bc49c20f0557f`  
		Last Modified: Thu, 29 Apr 2021 17:02:31 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba857cc76815a69804d81b7b8cfd1cef733d552360b462a6654bb997dc422b2`  
		Last Modified: Thu, 29 Apr 2021 17:02:31 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:a4de49115c06290f0365e78ccfc41c33ae5c7f54f069e8d5ad910d17cd00e1fb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.0 MB (35029567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c6269d7f5a3a3146d838cb1f3d9a89975b839613e3bc29493db15a8c91dd948`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:41:25 GMT
ADD file:b24da7eb23eeae04e00d0e45da29a89fe8f992e8dcf4ba482afb907b8015b7bf in / 
# Sat, 10 Apr 2021 00:41:28 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:13:29 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 29 Apr 2021 17:52:04 GMT
ENV HAPROXY_VERSION=2.2.14
# Thu, 29 Apr 2021 17:52:04 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Thu, 29 Apr 2021 17:52:05 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Thu, 29 Apr 2021 17:52:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 29 Apr 2021 17:52:49 GMT
STOPSIGNAL SIGUSR1
# Thu, 29 Apr 2021 17:52:50 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 29 Apr 2021 17:52:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 29 Apr 2021 17:52:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Apr 2021 17:52:57 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:15cb40b9c4df1a06940dc2a154c3be46844241235c1a091afa70da0ee2dc811a`  
		Last Modified: Sat, 10 Apr 2021 00:47:53 GMT  
		Size: 25.9 MB (25904582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48cb832c3e00ffed789c3f464caa612fe4996ba4683f72f8cf214d1437268efe`  
		Last Modified: Sat, 10 Apr 2021 01:21:27 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecd2d7073326e7be6f17459b1bdbdd24dbca7f0b483761cb137bb319170cdae9`  
		Last Modified: Thu, 29 Apr 2021 17:54:48 GMT  
		Size: 9.1 MB (9123034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af396c216cd462331785256c8eb8b58249a257388636dfba8957a6eea6563656`  
		Last Modified: Thu, 29 Apr 2021 17:54:46 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30df480ff08a19b3b653b87ddd425f40dfeee6416890092a6ee6f39c909f722c`  
		Last Modified: Thu, 29 Apr 2021 17:54:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; 386

```console
$ docker pull haproxy@sha256:481622045fb02fb6b31c3c1aac02351d13a0e075c2781dc0d8fe13ddf240a5b2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36980676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23f034ff44a4590fbde461f619710fc01edb99a36cdb948ffd62c756fe1566d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:39:42 GMT
ADD file:8885d4d13678543780bb04ba14b621179665f7951d5b261036a7092df9b376e7 in / 
# Sat, 10 Apr 2021 00:39:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 03:48:12 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 29 Apr 2021 17:39:19 GMT
ENV HAPROXY_VERSION=2.2.14
# Thu, 29 Apr 2021 17:39:19 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Thu, 29 Apr 2021 17:39:20 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Thu, 29 Apr 2021 17:40:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 29 Apr 2021 17:40:27 GMT
STOPSIGNAL SIGUSR1
# Thu, 29 Apr 2021 17:40:28 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 29 Apr 2021 17:40:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 29 Apr 2021 17:40:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Apr 2021 17:40:29 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:7cc57a8772e5e479618650dfa70f315b474d3f205d04bde7f602f469c1928d84`  
		Last Modified: Sat, 10 Apr 2021 00:46:07 GMT  
		Size: 27.8 MB (27788987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d92d68a52363235dcdfb59fa81e5ef1a4561c958501e4f28d6b79e86f8b8501`  
		Last Modified: Sat, 10 Apr 2021 03:59:08 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57229d188189b1e10cc3562b2ffd352969144dfbaf06988a920ed5427ed7906b`  
		Last Modified: Thu, 29 Apr 2021 17:44:22 GMT  
		Size: 9.2 MB (9189740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fb9373ea635024b72729ee73d1d659e91446280256d3fd21762b084584f4c88`  
		Last Modified: Thu, 29 Apr 2021 17:44:20 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a04207b362e717df1206194d656c8b158caffc32107bcd7131b746a848d033e6`  
		Last Modified: Thu, 29 Apr 2021 17:44:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; mips64le

```console
$ docker pull haproxy@sha256:e518728537a7d7a9887fad3713fcb11680b0da3376cc3b2ec13eec2655bc5ef4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34678876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2570ecec3e5c74b7b8d58abd69762b1d5ea1641ed6abbf3e8078fed1d1f82ba4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:09:40 GMT
ADD file:0c93801c4a3719dfd4c047d7f2f4d52bf463eba2ab875da1dc54dcc832aae20b in / 
# Sat, 10 Apr 2021 01:09:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:39:36 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 29 Apr 2021 17:07:40 GMT
ENV HAPROXY_VERSION=2.2.14
# Thu, 29 Apr 2021 17:07:40 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Thu, 29 Apr 2021 17:07:40 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Thu, 29 Apr 2021 17:10:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 29 Apr 2021 17:10:06 GMT
STOPSIGNAL SIGUSR1
# Thu, 29 Apr 2021 17:10:06 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 29 Apr 2021 17:10:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 29 Apr 2021 17:10:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Apr 2021 17:10:09 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:09ea659ba566d9c3c62493e5ae0b964f1eee4fcf35aabc91c5c34ca1ad686541`  
		Last Modified: Sat, 10 Apr 2021 01:16:07 GMT  
		Size: 25.8 MB (25806410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10fa5ae1be1fc686c91c15f24ebaaa72d7c4f64321c8ead8386f2f4f9d1a6705`  
		Last Modified: Sat, 10 Apr 2021 01:53:41 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d821f4c7e565a8e4288ffdec5499d4f1fe177393fe2d5774b1e1686ad7257454`  
		Last Modified: Thu, 29 Apr 2021 17:10:49 GMT  
		Size: 8.9 MB (8870513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee294f8c5e00b4207daece747b1984cebe038c75bcb99fde4df34f9d072accff`  
		Last Modified: Thu, 29 Apr 2021 17:10:43 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1327b763af1d0b3e237e5a65eb7a20370ad3bc1a2e5e2d07d6f4a2d7dd217d2`  
		Last Modified: Thu, 29 Apr 2021 17:10:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; ppc64le

```console
$ docker pull haproxy@sha256:5f6c4cd389f0eef07efa70a7b79e9034d39ad81308ee3d22b593b48c6e72038f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40323271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0525e4e75533190906a3a3b8fa4c13980187b37c0fe09a98b7d0248ee064c11f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:26:49 GMT
ADD file:ab87d4854aa8628ce8f4e603c0496499f6f28c3d2525ace782c7369691dafc8c in / 
# Sat, 10 Apr 2021 01:26:56 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 04:45:12 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 29 Apr 2021 17:21:53 GMT
ENV HAPROXY_VERSION=2.2.14
# Thu, 29 Apr 2021 17:22:05 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Thu, 29 Apr 2021 17:22:10 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Thu, 29 Apr 2021 17:28:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 29 Apr 2021 17:28:11 GMT
STOPSIGNAL SIGUSR1
# Thu, 29 Apr 2021 17:28:14 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 29 Apr 2021 17:28:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 29 Apr 2021 17:28:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Apr 2021 17:28:35 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:3e1e599482ca47095f85e429b346b76375aa85015ddcca050e85c2a8b1fdda9c`  
		Last Modified: Sat, 10 Apr 2021 01:33:57 GMT  
		Size: 30.5 MB (30545933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ee41bdc57145d3cb6e9f5fa23eed213567ae52835c7cff5fd57fe17b52f5ec`  
		Last Modified: Sat, 10 Apr 2021 05:09:50 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0318a9e0dfae38a427df09950040ec8ac49b3411281c6f4e916df64f3e61a1db`  
		Last Modified: Thu, 29 Apr 2021 17:32:41 GMT  
		Size: 9.8 MB (9775378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15d770c2ff18b8d626e68154c643956016ba3c2bc473db0cf4fe67933eae8e02`  
		Last Modified: Thu, 29 Apr 2021 17:32:39 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ffc03968d4104b120ffb831618293d3c01a3b52a20190f19139d4c400d8dfbd`  
		Last Modified: Thu, 29 Apr 2021 17:32:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; s390x

```console
$ docker pull haproxy@sha256:17be434f2b9d7eac603cd7e9d94facfdcc2fcc5547c8b01296254dcfef495242
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34763982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e69d8b1385df56238043045e64f64848efde120e4d71c13431aae7e3647c2ade`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:42:23 GMT
ADD file:dbe2182f8699f2a6011413ea01862e6c0e85853d922dffd72a28d994d23c79bc in / 
# Sat, 10 Apr 2021 00:42:25 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:38:04 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 29 Apr 2021 17:42:25 GMT
ENV HAPROXY_VERSION=2.2.14
# Thu, 29 Apr 2021 17:42:26 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Thu, 29 Apr 2021 17:42:26 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Thu, 29 Apr 2021 17:43:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 29 Apr 2021 17:43:05 GMT
STOPSIGNAL SIGUSR1
# Thu, 29 Apr 2021 17:43:05 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 29 Apr 2021 17:43:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 29 Apr 2021 17:43:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Apr 2021 17:43:07 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:65291f8717b3afd99b63cee867dd3e06b956a8ee6aa8580cc31d913b25de209d`  
		Last Modified: Sat, 10 Apr 2021 00:45:48 GMT  
		Size: 25.8 MB (25753787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9daf67acfb0373e31068762d068f1da8d320f2bdcdb0e6651d52b8183ede06c`  
		Last Modified: Sat, 10 Apr 2021 01:42:28 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:139203a6eacdb0e49cca6af7b193a9727084d9bc018c6c38ecd8e2a70cb4a783`  
		Last Modified: Thu, 29 Apr 2021 17:45:08 GMT  
		Size: 9.0 MB (9008246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22c7c9f250fa0d85359a600dcf6c221949890728910221bf04f9c0550d07f099`  
		Last Modified: Thu, 29 Apr 2021 17:45:07 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b818bccdd69e5cc08f3856520e9beff9d06adaba69bf8fd2820f502abfb90785`  
		Last Modified: Thu, 29 Apr 2021 17:45:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:lts-alpine`

```console
$ docker pull haproxy@sha256:865331c119b8c88d15add5b94d0a793e7cd24e273dd520d4b025db6c3797f09b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `haproxy:lts-alpine` - linux; amd64

```console
$ docker pull haproxy@sha256:351e8b45533cf4c752df579566bf71b8550d984d7b8446e7b8f1c9e511aeb44d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.2 MB (9187819 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04679647ccf7dcdaab910fb8b498a41b5f3526f696fd5166913e56415d70469d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:37:38 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 29 Apr 2021 17:30:10 GMT
ENV HAPROXY_VERSION=2.2.14
# Thu, 29 Apr 2021 17:30:10 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Thu, 29 Apr 2021 17:30:10 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Thu, 29 Apr 2021 17:30:59 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 29 Apr 2021 17:30:59 GMT
STOPSIGNAL SIGUSR1
# Thu, 29 Apr 2021 17:31:00 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 29 Apr 2021 17:31:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 29 Apr 2021 17:31:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Apr 2021 17:31:01 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4de1862a29af271c1751bf0d03d96f9a881f971d1288c5fafcfba90b517611f8`  
		Last Modified: Wed, 14 Apr 2021 21:43:30 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9e43f525730a3c1a71396cd7d8c5e91c013eb29c0e704b13ebc56fa8899a9bc`  
		Last Modified: Thu, 29 Apr 2021 17:32:38 GMT  
		Size: 6.4 MB (6374100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd121de2e7dd938cb509db4091d6e0ad83358a944805a98b6e4802ae196993ef`  
		Last Modified: Thu, 29 Apr 2021 17:32:37 GMT  
		Size: 446.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0952e13028cb45fca71cc160a99915a21adef4382c5a6bdb0c19ac7f888a40f4`  
		Last Modified: Thu, 29 Apr 2021 17:32:37 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts-alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:2330b42228e3f150465089b56aac22e2b98e319f3e3a651b134e3448ef31ee56
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.9 MB (8878321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d063a6d463b78e25e558d428d98ef2c98534ba530b340819315d12988ef7663`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:18:05 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 29 Apr 2021 17:58:25 GMT
ENV HAPROXY_VERSION=2.2.14
# Thu, 29 Apr 2021 17:58:26 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Thu, 29 Apr 2021 17:58:27 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Thu, 29 Apr 2021 17:58:54 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 29 Apr 2021 17:58:55 GMT
STOPSIGNAL SIGUSR1
# Thu, 29 Apr 2021 17:58:56 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 29 Apr 2021 17:59:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 29 Apr 2021 17:59:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Apr 2021 17:59:02 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd640f0f76e4e434b444a36110041f2c571b2dbcfca29958b2e90de8d91bd6eb`  
		Last Modified: Wed, 14 Apr 2021 21:34:02 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5a1dc9635ed4e8266598b43a8021916179f6ecfe26de2edf6f79953d7a6e1ba`  
		Last Modified: Thu, 29 Apr 2021 17:59:44 GMT  
		Size: 6.3 MB (6254438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54b4242bd61d3ebbd2fad2003f9aca4578f035fa51317bd10ded15d1d150442b`  
		Last Modified: Thu, 29 Apr 2021 17:59:42 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5741f31a86fd77efec27f79f54cb17078972cc2ea2f6884988a7a88061925e7d`  
		Last Modified: Thu, 29 Apr 2021 17:59:42 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:b58792ba4c8509a690aed5c18aed41548b2cd4a7444f4db35c646b420d7fd26c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8597095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:795456a00fe0008d4a02f2102d502f563b1dcfeac231a327150652971276712c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:47:58 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 29 Apr 2021 17:00:50 GMT
ENV HAPROXY_VERSION=2.2.14
# Thu, 29 Apr 2021 17:00:51 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Thu, 29 Apr 2021 17:00:52 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Thu, 29 Apr 2021 17:01:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 29 Apr 2021 17:01:16 GMT
STOPSIGNAL SIGUSR1
# Thu, 29 Apr 2021 17:01:17 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 29 Apr 2021 17:01:19 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 29 Apr 2021 17:01:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Apr 2021 17:01:20 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ff0f6ee9305bed375c784c12ad4beeac3af6ea1a6b5afeec6b4700259dc194`  
		Last Modified: Wed, 14 Apr 2021 22:56:09 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b2ec0b1927bd1d10abbd183f6132825d56a5fe84af8e3151f57a917c6b0c5d9`  
		Last Modified: Thu, 29 Apr 2021 17:03:50 GMT  
		Size: 6.2 MB (6171196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a0891b95532486d3f61c8626238695b04ac750b83bfeff55ddde3c424f1e31`  
		Last Modified: Thu, 29 Apr 2021 17:03:48 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcff54d664dce91ddc63ae2a80ac409ec8ac4323aae79e24be2c04e30364696d`  
		Last Modified: Thu, 29 Apr 2021 17:03:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:ff7750eb3484161e61d6113d2d2a591d285dbefa94eb815da877505ebaec40b5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.1 MB (9093351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c05e833634dc19b1dcf0ec5b6028c9a6a444978ec1edf610425aabb2b4ac381`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:26:01 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 29 Apr 2021 17:53:12 GMT
ENV HAPROXY_VERSION=2.2.14
# Thu, 29 Apr 2021 17:53:13 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Thu, 29 Apr 2021 17:53:14 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Thu, 29 Apr 2021 17:53:39 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 29 Apr 2021 17:53:40 GMT
STOPSIGNAL SIGUSR1
# Thu, 29 Apr 2021 17:53:41 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 29 Apr 2021 17:53:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 29 Apr 2021 17:53:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Apr 2021 17:53:45 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2ef9646f93509fb43536690b645509d9b653316324583761dd086b8ad6c664`  
		Last Modified: Wed, 14 Apr 2021 20:37:52 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecd9d03f24e857a24819b3bffa319b1896aaf04d09ff657d37c44cbf02d870ad`  
		Last Modified: Thu, 29 Apr 2021 17:54:58 GMT  
		Size: 6.4 MB (6379570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a0e9150a4a249e0f658011c7421dbe8cb4f1797738ba92ac98be54f2929799`  
		Last Modified: Thu, 29 Apr 2021 17:54:57 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e7c49ac145b8b9f168fd85e531255cdc8ca36adcd9c5803471ffd3f12cae46`  
		Last Modified: Thu, 29 Apr 2021 17:54:56 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts-alpine` - linux; 386

```console
$ docker pull haproxy@sha256:ca89af1c1cadbb2c546bf88412cedd7d17e4321a4704e7c534f96e50b4a971c6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9028758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42bc524adf636565d4743200d86bce083eeac9b2e4bb6d1e352bc32a908d2132`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 01:50:06 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 29 Apr 2021 17:40:45 GMT
ENV HAPROXY_VERSION=2.2.14
# Thu, 29 Apr 2021 17:40:45 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Thu, 29 Apr 2021 17:40:46 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Thu, 29 Apr 2021 17:41:51 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 29 Apr 2021 17:41:51 GMT
STOPSIGNAL SIGUSR1
# Thu, 29 Apr 2021 17:41:51 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 29 Apr 2021 17:41:52 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 29 Apr 2021 17:41:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Apr 2021 17:41:53 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:31b7e7ccca9e17fd08b39c9a4ffd3ded380b62816c489d6c3758c9bb5a632430`  
		Last Modified: Wed, 14 Apr 2021 18:39:24 GMT  
		Size: 2.8 MB (2818900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9104145d2a6b1e0c0837c464bb9d4b331949cfeb6be12e4e7995507661d3386`  
		Last Modified: Thu, 15 Apr 2021 02:00:28 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c94b7b9918662e243b2f7d32c2c237339e594b90ea119f6bf77f9ac8c4818612`  
		Last Modified: Thu, 29 Apr 2021 17:44:41 GMT  
		Size: 6.2 MB (6208104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89684848b1dc6218657c706cb17469bca0fa286cecc489425b7464f52c770c24`  
		Last Modified: Thu, 29 Apr 2021 17:44:39 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7b3024bbac5c0f491b5e018476a95a61e4ae4a0ad09e826e696f7bceef5a6aa`  
		Last Modified: Thu, 29 Apr 2021 17:44:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts-alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:4d277cabca4bd41dd24d0d04f4cfed03d8988e0830a5c91b24d0a659873beb40
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9503527 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1aff090c2019485bed2a6d56748b9c1d5f909ab4737bb6c8961605abd9191be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:25:09 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 29 Apr 2021 17:29:01 GMT
ENV HAPROXY_VERSION=2.2.14
# Thu, 29 Apr 2021 17:29:18 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Thu, 29 Apr 2021 17:29:30 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Thu, 29 Apr 2021 17:30:26 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 29 Apr 2021 17:30:36 GMT
STOPSIGNAL SIGUSR1
# Thu, 29 Apr 2021 17:30:41 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 29 Apr 2021 17:30:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 29 Apr 2021 17:31:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Apr 2021 17:31:21 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8004273856b1b354059d03a17deec6e79d325ba45d63213dda3d1fa401db8c22`  
		Last Modified: Wed, 14 Apr 2021 23:36:37 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c35b3cdf32810f06f92fc72958c4454a52f6d0dff450335d1420cb5aff7bfb`  
		Last Modified: Thu, 29 Apr 2021 17:32:59 GMT  
		Size: 6.7 MB (6688630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d036ed22faa59df382b510ded6e6b8446ca3f41abfc5b68e85d60e39173ef4e`  
		Last Modified: Thu, 29 Apr 2021 17:32:58 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35d66a9c14deeb7ebd1d75c0aa9dd9d118abd71eb4a2f0762ca6e1daeeb4507`  
		Last Modified: Thu, 29 Apr 2021 17:32:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts-alpine` - linux; s390x

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
