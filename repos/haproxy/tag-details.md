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
-	[`haproxy:2.2.13`](#haproxy2213)
-	[`haproxy:2.2.13-alpine`](#haproxy2213-alpine)
-	[`haproxy:2.3`](#haproxy23)
-	[`haproxy:2.3-alpine`](#haproxy23-alpine)
-	[`haproxy:2.3.9`](#haproxy239)
-	[`haproxy:2.3.9-alpine`](#haproxy239-alpine)
-	[`haproxy:2.4-dev`](#haproxy24-dev)
-	[`haproxy:2.4-dev-alpine`](#haproxy24-dev-alpine)
-	[`haproxy:2.4-dev16`](#haproxy24-dev16)
-	[`haproxy:2.4-dev16-alpine`](#haproxy24-dev16-alpine)
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
$ docker pull haproxy@sha256:de91b6e9d7b8ac1c4f55c012cee2a03f766063d61a2c42e70f15ca9ce5cffccf
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
$ docker pull haproxy@sha256:0980ae3a6550c6dc5233f91c14344c70ea334505919584bb78f840e1c040b447
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.4 MB (36446380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d59c0ba74b7e235e5a5728035c1c9b66b79d24aa898a2d994223c069a8d1db49`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:29:42 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 06:32:41 GMT
ENV HAPROXY_VERSION=2.2.13
# Sat, 10 Apr 2021 06:32:41 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.13.tar.gz
# Sat, 10 Apr 2021 06:32:42 GMT
ENV HAPROXY_SHA256=9e3e51441c70bedfb494fc9d4b4d3389a71be9a3c915ba3d6f7e8fd9a57ce160
# Sat, 10 Apr 2021 06:34:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 06:34:01 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 06:34:02 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 06:34:03 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 06:34:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 06:34:03 GMT
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
	-	`sha256:a4ac7a9f13ea2eeb6a8050090e57aee7e14337034b9e7565f30ffb9bc11cc8d0`  
		Last Modified: Sat, 10 Apr 2021 06:38:38 GMT  
		Size: 9.3 MB (9305056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c87b35756f7d827f1af49c1622775093c9d433056286165dfe92a96727e14367`  
		Last Modified: Sat, 10 Apr 2021 06:38:37 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2371bbf56d662c6773a6498b56369e7b8e46fe696a1f53d60becdf9fbc35e249`  
		Last Modified: Sat, 10 Apr 2021 06:38:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:ea8caf1a471b1d052cce885f728ecbd7661e3154b1bd9490b4ead9d6f96e34a4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33784186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42fa781836c103292a015ca6c217ec9009cd1b10e90f8b640780e161fa466dfd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:51:31 GMT
ADD file:926533a23a69aa2481a9122b667bb6300a347154eea366c9e679a230aa7f373a in / 
# Sat, 10 Apr 2021 00:51:34 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 02:24:17 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 02:27:57 GMT
ENV HAPROXY_VERSION=2.2.13
# Sat, 10 Apr 2021 02:28:00 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.13.tar.gz
# Sat, 10 Apr 2021 02:28:03 GMT
ENV HAPROXY_SHA256=9e3e51441c70bedfb494fc9d4b4d3389a71be9a3c915ba3d6f7e8fd9a57ce160
# Sat, 10 Apr 2021 02:29:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 02:29:11 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 02:29:17 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 02:29:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 02:29:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 02:29:37 GMT
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
	-	`sha256:1a9539dc178d3edc26c473a1278c3b8005c9418c35d68e1be1eda3e620e9e9e5`  
		Last Modified: Sat, 10 Apr 2021 02:37:17 GMT  
		Size: 8.9 MB (8909037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90a7f4dd06e8114f46916dd5877eacb048ce77ab5d497b0bb6a356b71262e63`  
		Last Modified: Sat, 10 Apr 2021 02:37:14 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68c6b0e6fee35363aa79edd25b01d996dea7f7748e0db784700ecf512099d35b`  
		Last Modified: Sat, 10 Apr 2021 02:37:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:bba42c59d71ad06be8103a3bedce42b8898bbf3bfa4fb0be2cb06f3e3b01f688
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.5 MB (31461092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1f54b69378fa75b9cfd1ef85e56a15f392411149c29d9e16fbab58cb1c66d2b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:59:45 GMT
ADD file:3fbd246a2de82566bcaaf62e3e0bf57175a7ad46b4156366a110661b31eab240 in / 
# Sat, 10 Apr 2021 00:59:47 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 08:58:51 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 09:00:53 GMT
ENV HAPROXY_VERSION=2.2.13
# Sat, 10 Apr 2021 09:00:54 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.13.tar.gz
# Sat, 10 Apr 2021 09:00:55 GMT
ENV HAPROXY_SHA256=9e3e51441c70bedfb494fc9d4b4d3389a71be9a3c915ba3d6f7e8fd9a57ce160
# Sat, 10 Apr 2021 09:01:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 09:01:37 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 09:01:38 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 09:01:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 09:01:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 09:01:42 GMT
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
	-	`sha256:b75131a6ec2e4adca7605661356ce165e13803d545d79123d0e3330d435596f5`  
		Last Modified: Sat, 10 Apr 2021 09:05:50 GMT  
		Size: 8.7 MB (8719344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9ea1930c5490ff94769de0e8ab8aad2b5c1e4e72d54c27afee12d74411f600`  
		Last Modified: Sat, 10 Apr 2021 09:05:47 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2e34fd9824e23d785f73ea0802107c25f42c9ad3d30abdc87f5e61fd4e17080`  
		Last Modified: Sat, 10 Apr 2021 09:05:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:9ea94a117b8f204c209df772aee3188d13a616efe6ca343149e0ad29fa251507
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.0 MB (35023478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b853740b36a0d8cc1b4c066a09de9600dfaf3e5c09ddeb7d9a627384baa05ec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:41:25 GMT
ADD file:b24da7eb23eeae04e00d0e45da29a89fe8f992e8dcf4ba482afb907b8015b7bf in / 
# Sat, 10 Apr 2021 00:41:28 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:13:29 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 01:15:54 GMT
ENV HAPROXY_VERSION=2.2.13
# Sat, 10 Apr 2021 01:15:55 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.13.tar.gz
# Sat, 10 Apr 2021 01:15:57 GMT
ENV HAPROXY_SHA256=9e3e51441c70bedfb494fc9d4b4d3389a71be9a3c915ba3d6f7e8fd9a57ce160
# Sat, 10 Apr 2021 01:16:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 01:16:49 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 01:16:51 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 01:16:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 01:16:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 01:16:59 GMT
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
	-	`sha256:b208d49b31d425b72f01f4c0579f75de3e8a9e9b5e413d19ad545fcb1cfec498`  
		Last Modified: Sat, 10 Apr 2021 01:21:53 GMT  
		Size: 9.1 MB (9116944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69001e0866df82cbc43b538ac2c4247ac27a02101891fc85d945daa23280ec2e`  
		Last Modified: Sat, 10 Apr 2021 01:21:50 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fb9542d39b52a78dae6dfffd1040b30683aee32cf37f2699e42eae131137abe`  
		Last Modified: Sat, 10 Apr 2021 01:21:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2` - linux; 386

```console
$ docker pull haproxy@sha256:49260af2de07dc187620f290c656da80183c7b1e8ab773755a40ee9f7f6f9aaf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36978050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baf5327943d1ef805085f695725d9d9d120dc638b881ba0daf29bbacdef45fe6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:39:42 GMT
ADD file:8885d4d13678543780bb04ba14b621179665f7951d5b261036a7092df9b376e7 in / 
# Sat, 10 Apr 2021 00:39:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 03:48:12 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 03:50:59 GMT
ENV HAPROXY_VERSION=2.2.13
# Sat, 10 Apr 2021 03:51:00 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.13.tar.gz
# Sat, 10 Apr 2021 03:51:00 GMT
ENV HAPROXY_SHA256=9e3e51441c70bedfb494fc9d4b4d3389a71be9a3c915ba3d6f7e8fd9a57ce160
# Sat, 10 Apr 2021 03:52:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 03:52:26 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 03:52:26 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 03:52:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 03:52:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 03:52:28 GMT
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
	-	`sha256:501040fe44c6490e09a71181c6626bc3bb0bfe93798932941b8c0789c72d1c5e`  
		Last Modified: Sat, 10 Apr 2021 03:59:58 GMT  
		Size: 9.2 MB (9187117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:388ebcc0127bdbcff243568101388f512720854794aa20ab9acddc6b0a922450`  
		Last Modified: Sat, 10 Apr 2021 03:59:50 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:284bc34ec1436775792b35bfa789aa45111707b63c5a95f5df4f6d25e5db332e`  
		Last Modified: Sat, 10 Apr 2021 03:59:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2` - linux; mips64le

```console
$ docker pull haproxy@sha256:24f69608e75a6910345769e9baaa7433a51d911decf979eaaafd1490ff0a5ee2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34674134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:277a2344421652b30bcc8416edef8dfb9cc9ee769ba4ba5ad51bf80a6085bfa0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:09:40 GMT
ADD file:0c93801c4a3719dfd4c047d7f2f4d52bf463eba2ab875da1dc54dcc832aae20b in / 
# Sat, 10 Apr 2021 01:09:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:39:36 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 01:44:43 GMT
ENV HAPROXY_VERSION=2.2.13
# Sat, 10 Apr 2021 01:44:43 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.13.tar.gz
# Sat, 10 Apr 2021 01:44:43 GMT
ENV HAPROXY_SHA256=9e3e51441c70bedfb494fc9d4b4d3389a71be9a3c915ba3d6f7e8fd9a57ce160
# Sat, 10 Apr 2021 01:47:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 01:47:05 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 01:47:06 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 01:47:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 01:47:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 01:47:08 GMT
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
	-	`sha256:34d169508d4b44b7fea30d0806ab3babbfe581b239f681919ae771c048d8213f`  
		Last Modified: Sat, 10 Apr 2021 01:54:23 GMT  
		Size: 8.9 MB (8865773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e41b7b929b9472e4f31050212242ce54c3d7abad584e23967b0ca1f52e3d262`  
		Last Modified: Sat, 10 Apr 2021 01:54:17 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e80eb6485d38caf34db8f19ffc92fd40dd6cf9bbed315177ada12c503c2cdf4`  
		Last Modified: Sat, 10 Apr 2021 01:54:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2` - linux; ppc64le

```console
$ docker pull haproxy@sha256:051c8550a62dede7d06f587afb6946e710050fcf711ff38461c488dcffda9498
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40318021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67d26e25e79a68e404304e5bae82aefa19b2b9d4ee83dcaf8979d716a45e6a10`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:26:49 GMT
ADD file:ab87d4854aa8628ce8f4e603c0496499f6f28c3d2525ace782c7369691dafc8c in / 
# Sat, 10 Apr 2021 01:26:56 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 04:45:12 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 04:55:51 GMT
ENV HAPROXY_VERSION=2.2.13
# Sat, 10 Apr 2021 04:55:53 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.13.tar.gz
# Sat, 10 Apr 2021 04:55:57 GMT
ENV HAPROXY_SHA256=9e3e51441c70bedfb494fc9d4b4d3389a71be9a3c915ba3d6f7e8fd9a57ce160
# Sat, 10 Apr 2021 04:58:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 04:58:42 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 04:58:44 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 04:58:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 04:58:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 04:59:01 GMT
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
	-	`sha256:47d98ea7f5d6d0054eae8b1260b42df2c05e11015c73624875e953c2b5511090`  
		Last Modified: Sat, 10 Apr 2021 05:10:21 GMT  
		Size: 9.8 MB (9770127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a53dae98d3c653079c8dcee254bd233926f95fad7e2bf848e03a672956fd14`  
		Last Modified: Sat, 10 Apr 2021 05:10:19 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78cc95082c4533e2331bcf6b59f548c5ec2d66ac08321631a1350df97f7df0a5`  
		Last Modified: Sat, 10 Apr 2021 05:10:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2` - linux; s390x

```console
$ docker pull haproxy@sha256:883a075a06023316a2ff2ff319689020b42812c4b6da7db73156722fb8e8614c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34759692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:812759d5bb748fe3ab35c1c945a594798c94ee29f65ab389f7d1b3ace8359191`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:42:23 GMT
ADD file:dbe2182f8699f2a6011413ea01862e6c0e85853d922dffd72a28d994d23c79bc in / 
# Sat, 10 Apr 2021 00:42:25 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:38:04 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 01:39:35 GMT
ENV HAPROXY_VERSION=2.2.13
# Sat, 10 Apr 2021 01:39:35 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.13.tar.gz
# Sat, 10 Apr 2021 01:39:36 GMT
ENV HAPROXY_SHA256=9e3e51441c70bedfb494fc9d4b4d3389a71be9a3c915ba3d6f7e8fd9a57ce160
# Sat, 10 Apr 2021 01:40:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 01:40:07 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 01:40:07 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 01:40:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 01:40:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 01:40:08 GMT
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
	-	`sha256:1ca81c5eef5f2d44f041789ed53dbfa0a6453bee245921eade23f4c550c190d8`  
		Last Modified: Sat, 10 Apr 2021 01:42:47 GMT  
		Size: 9.0 MB (9003958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0788fe9c0f74dcb98ef569fdf7251c230f9f2c4adcb7b03df2d7ecf36d8517e8`  
		Last Modified: Sat, 10 Apr 2021 01:42:45 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b6982746ce00451b99cf4beb0304c2d327fbaa5898f24a06c04ce6048d85149`  
		Last Modified: Sat, 10 Apr 2021 01:42:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.2-alpine`

```console
$ docker pull haproxy@sha256:413f24a6ce6057afafb796d156e6b332bdcb37a28f499599aa7c9b4d1434cbbd
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
$ docker pull haproxy@sha256:51528e0da4c91c96e9451d07c0d79fa2c7ec359c9486006b6a2381adb50616ab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.2 MB (9183249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d94ea559268af6d140850108edea1185c786262681f3912e945b540caf8bf47`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:37:38 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 21:39:55 GMT
ENV HAPROXY_VERSION=2.2.13
# Wed, 14 Apr 2021 21:39:55 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.13.tar.gz
# Wed, 14 Apr 2021 21:39:55 GMT
ENV HAPROXY_SHA256=9e3e51441c70bedfb494fc9d4b4d3389a71be9a3c915ba3d6f7e8fd9a57ce160
# Wed, 14 Apr 2021 21:40:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 21:40:44 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 21:40:44 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 21:40:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 21:40:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 21:40:45 GMT
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
	-	`sha256:ba81e90af14a863a9b5685b5085eec923abff1890a6fd2a3f0e07994974e31d7`  
		Last Modified: Wed, 14 Apr 2021 21:44:03 GMT  
		Size: 6.4 MB (6369525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc0670e87880c224e8aaeffba5dcacdd308471d5f995f18cc7457f21d0a2a04`  
		Last Modified: Wed, 14 Apr 2021 21:44:02 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a009871a4c718317430f5cd8acafa4a1c6f3020f699c1e9a4b3b9e06540267c`  
		Last Modified: Wed, 14 Apr 2021 21:44:02 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2-alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:998908d9876cf5186d814914e16aad5bbf9f9fd36cd12e64ab2cf5cd2f9e21ef
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.9 MB (8873199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58b3a8c2e2ff9d47d90f2fb6f7661c6ee64bdb5ab6eb0577bbb9899bd8dceb42`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:18:05 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 21:24:17 GMT
ENV HAPROXY_VERSION=2.2.13
# Wed, 14 Apr 2021 21:24:26 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.13.tar.gz
# Wed, 14 Apr 2021 21:24:33 GMT
ENV HAPROXY_SHA256=9e3e51441c70bedfb494fc9d4b4d3389a71be9a3c915ba3d6f7e8fd9a57ce160
# Wed, 14 Apr 2021 21:25:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 21:26:12 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 21:26:21 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 21:26:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 21:26:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 21:27:07 GMT
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
	-	`sha256:1f961936d3b3f46a3711ffae66d510e2e3587ecc266ffc4228dc5bd3e348e588`  
		Last Modified: Wed, 14 Apr 2021 21:34:29 GMT  
		Size: 6.2 MB (6249312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f89851496a5733b45c2a26de344e1e0888de96a5b2d2c0daa7f0e6e2765ec37`  
		Last Modified: Wed, 14 Apr 2021 21:34:28 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065a09e958b3582c21934c8ef7a6fc65e4573d59cd9e486affab9e9d427bbe8e`  
		Last Modified: Wed, 14 Apr 2021 21:34:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:b7073b291f697c7935c86c245c86fee0cf05b1f51ea7192ccc0f8788a26b76cf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8591663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47b928f6c9cacabd2bcaae105d88e5d2fdeae2e042c3fd34b7b046c718e15150`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:47:58 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 22:52:15 GMT
ENV HAPROXY_VERSION=2.2.13
# Wed, 14 Apr 2021 22:52:18 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.13.tar.gz
# Wed, 14 Apr 2021 22:52:20 GMT
ENV HAPROXY_SHA256=9e3e51441c70bedfb494fc9d4b4d3389a71be9a3c915ba3d6f7e8fd9a57ce160
# Wed, 14 Apr 2021 22:52:54 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 22:52:56 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 22:52:57 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 22:53:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 22:53:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 22:53:04 GMT
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
	-	`sha256:a9db6c809add6fb1c65ed18e490e0aef9ceec249693f5014ad157e8989b2f97a`  
		Last Modified: Wed, 14 Apr 2021 22:56:40 GMT  
		Size: 6.2 MB (6165762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c54a8deef45aafe8d23348b71b1907c6930bd15e2cb8e9b3cbba14f225db81e3`  
		Last Modified: Wed, 14 Apr 2021 22:56:37 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3307625a9b488e9e1c508c95cd16dbee010765a6d9d5561c0723bc7a75a8d5b`  
		Last Modified: Wed, 14 Apr 2021 22:56:37 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:16bca21e897d7c52b2517cf4ba4e89c8ddb5e431b4cccad8fcc225eabcce25ca
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.1 MB (9088539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c6169d0eba5060ded320c17fa92adcdcdf3ee92545eb40d895e0544a4ef71cd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:26:01 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 20:30:39 GMT
ENV HAPROXY_VERSION=2.2.13
# Wed, 14 Apr 2021 20:30:46 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.13.tar.gz
# Wed, 14 Apr 2021 20:30:54 GMT
ENV HAPROXY_SHA256=9e3e51441c70bedfb494fc9d4b4d3389a71be9a3c915ba3d6f7e8fd9a57ce160
# Wed, 14 Apr 2021 20:31:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 20:31:49 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 20:31:50 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:32:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 20:32:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:32:21 GMT
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
	-	`sha256:3f46520f93f138b7f11e9721ba69bfde0f4f1da77e7b5ba2be9de502d0595b54`  
		Last Modified: Wed, 14 Apr 2021 20:38:18 GMT  
		Size: 6.4 MB (6374758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a83203e2d21398703492ebb3881e3ad57ae31c92251d8d94e7be21b51ac3a695`  
		Last Modified: Wed, 14 Apr 2021 20:38:16 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c812aee4a6ede81fd42bd6abae3c0f8300ef5222e074a574be9c861c6de4d0ac`  
		Last Modified: Wed, 14 Apr 2021 20:38:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2-alpine` - linux; 386

```console
$ docker pull haproxy@sha256:a0fbc701001da548b035064db09a6be1e31e17125183345e0a6e9183abb2cb4f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9023341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13c3c2ecf9cd56e8732956bd2c0b272bd99a5a2e5090755c3137696b34ee3889`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 01:50:06 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 15 Apr 2021 01:53:40 GMT
ENV HAPROXY_VERSION=2.2.13
# Thu, 15 Apr 2021 01:53:40 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.13.tar.gz
# Thu, 15 Apr 2021 01:53:40 GMT
ENV HAPROXY_SHA256=9e3e51441c70bedfb494fc9d4b4d3389a71be9a3c915ba3d6f7e8fd9a57ce160
# Thu, 15 Apr 2021 01:54:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 15 Apr 2021 01:54:44 GMT
STOPSIGNAL SIGUSR1
# Thu, 15 Apr 2021 01:54:44 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 15 Apr 2021 01:54:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 15 Apr 2021 01:54:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Apr 2021 01:54:45 GMT
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
	-	`sha256:dd83349dc27b7c6494b326db86b2fb5ab9fded96732b87dcbdfe7ffbf53eb6fd`  
		Last Modified: Thu, 15 Apr 2021 02:01:05 GMT  
		Size: 6.2 MB (6202686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df9e7c12c69c54a160be7a4c5497240b0dffff220b6d1eb44aa7977bc593d408`  
		Last Modified: Thu, 15 Apr 2021 02:01:04 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c24d7fe1943abc1fdfcdef29513a413337092d356e48d6b6b868c73ed4ca4b6b`  
		Last Modified: Thu, 15 Apr 2021 02:01:03 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2-alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:3176f25d3818aaecc48b0cb829219da0864af79b2564b8eecd5ebccfa4f40468
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9499255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27f33cdd58ab09da862b649ad36eb8667c6ee6018e65a43528c3d7a198a44b72`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:25:09 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 23:29:12 GMT
ENV HAPROXY_VERSION=2.2.13
# Wed, 14 Apr 2021 23:29:16 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.13.tar.gz
# Wed, 14 Apr 2021 23:29:20 GMT
ENV HAPROXY_SHA256=9e3e51441c70bedfb494fc9d4b4d3389a71be9a3c915ba3d6f7e8fd9a57ce160
# Wed, 14 Apr 2021 23:30:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 23:30:20 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 23:30:22 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 23:30:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 23:30:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 23:30:47 GMT
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
	-	`sha256:e8a3685c2ec0932a7f73fa0032bf33500306ee2a5d0abf655e8983b0c8a95acd`  
		Last Modified: Wed, 14 Apr 2021 23:37:09 GMT  
		Size: 6.7 MB (6684359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74885306f2f1ac242fa8c216d998632b927a5cd3678771077f7a7f650d8ba37d`  
		Last Modified: Wed, 14 Apr 2021 23:37:07 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32336bc725a4335e246865126dccc149331aa27ef4a8767172fb2cff483b4ca4`  
		Last Modified: Wed, 14 Apr 2021 23:37:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2-alpine` - linux; s390x

```console
$ docker pull haproxy@sha256:5fb7df6e38eea99e9f0e9d4a19cd193a5be4747420d5b38082dfc02df9fb6d1a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.9 MB (8940300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e32f238bf459522abbbbb20a287e8543faf16dd5307b7fa7da33e7edfe3f4b8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:54:24 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 20:56:12 GMT
ENV HAPROXY_VERSION=2.2.13
# Wed, 14 Apr 2021 20:56:12 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.13.tar.gz
# Wed, 14 Apr 2021 20:56:12 GMT
ENV HAPROXY_SHA256=9e3e51441c70bedfb494fc9d4b4d3389a71be9a3c915ba3d6f7e8fd9a57ce160
# Wed, 14 Apr 2021 20:56:47 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 20:56:47 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 20:56:47 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:56:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 20:56:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:56:49 GMT
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
	-	`sha256:9b54506479f94cd6e6ff33fd666b2e4ef038a755e897f69c41e2024451738f22`  
		Last Modified: Wed, 14 Apr 2021 20:59:30 GMT  
		Size: 6.3 MB (6335894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b346055862205d30d0fec1cd13ad03e77403df88ae4b0e999a9fa3f2f5738371`  
		Last Modified: Wed, 14 Apr 2021 20:59:29 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1c0e6cd04f7bb776fd8fc6fcdd6ca22f1247acb507d44b41d9163155c7e5d9`  
		Last Modified: Wed, 14 Apr 2021 20:59:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.2.13`

```console
$ docker pull haproxy@sha256:de91b6e9d7b8ac1c4f55c012cee2a03f766063d61a2c42e70f15ca9ce5cffccf
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

### `haproxy:2.2.13` - linux; amd64

```console
$ docker pull haproxy@sha256:0980ae3a6550c6dc5233f91c14344c70ea334505919584bb78f840e1c040b447
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.4 MB (36446380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d59c0ba74b7e235e5a5728035c1c9b66b79d24aa898a2d994223c069a8d1db49`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:29:42 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 06:32:41 GMT
ENV HAPROXY_VERSION=2.2.13
# Sat, 10 Apr 2021 06:32:41 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.13.tar.gz
# Sat, 10 Apr 2021 06:32:42 GMT
ENV HAPROXY_SHA256=9e3e51441c70bedfb494fc9d4b4d3389a71be9a3c915ba3d6f7e8fd9a57ce160
# Sat, 10 Apr 2021 06:34:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 06:34:01 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 06:34:02 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 06:34:03 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 06:34:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 06:34:03 GMT
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
	-	`sha256:a4ac7a9f13ea2eeb6a8050090e57aee7e14337034b9e7565f30ffb9bc11cc8d0`  
		Last Modified: Sat, 10 Apr 2021 06:38:38 GMT  
		Size: 9.3 MB (9305056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c87b35756f7d827f1af49c1622775093c9d433056286165dfe92a96727e14367`  
		Last Modified: Sat, 10 Apr 2021 06:38:37 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2371bbf56d662c6773a6498b56369e7b8e46fe696a1f53d60becdf9fbc35e249`  
		Last Modified: Sat, 10 Apr 2021 06:38:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.13` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:ea8caf1a471b1d052cce885f728ecbd7661e3154b1bd9490b4ead9d6f96e34a4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33784186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42fa781836c103292a015ca6c217ec9009cd1b10e90f8b640780e161fa466dfd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:51:31 GMT
ADD file:926533a23a69aa2481a9122b667bb6300a347154eea366c9e679a230aa7f373a in / 
# Sat, 10 Apr 2021 00:51:34 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 02:24:17 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 02:27:57 GMT
ENV HAPROXY_VERSION=2.2.13
# Sat, 10 Apr 2021 02:28:00 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.13.tar.gz
# Sat, 10 Apr 2021 02:28:03 GMT
ENV HAPROXY_SHA256=9e3e51441c70bedfb494fc9d4b4d3389a71be9a3c915ba3d6f7e8fd9a57ce160
# Sat, 10 Apr 2021 02:29:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 02:29:11 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 02:29:17 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 02:29:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 02:29:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 02:29:37 GMT
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
	-	`sha256:1a9539dc178d3edc26c473a1278c3b8005c9418c35d68e1be1eda3e620e9e9e5`  
		Last Modified: Sat, 10 Apr 2021 02:37:17 GMT  
		Size: 8.9 MB (8909037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90a7f4dd06e8114f46916dd5877eacb048ce77ab5d497b0bb6a356b71262e63`  
		Last Modified: Sat, 10 Apr 2021 02:37:14 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68c6b0e6fee35363aa79edd25b01d996dea7f7748e0db784700ecf512099d35b`  
		Last Modified: Sat, 10 Apr 2021 02:37:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.13` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:bba42c59d71ad06be8103a3bedce42b8898bbf3bfa4fb0be2cb06f3e3b01f688
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.5 MB (31461092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1f54b69378fa75b9cfd1ef85e56a15f392411149c29d9e16fbab58cb1c66d2b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:59:45 GMT
ADD file:3fbd246a2de82566bcaaf62e3e0bf57175a7ad46b4156366a110661b31eab240 in / 
# Sat, 10 Apr 2021 00:59:47 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 08:58:51 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 09:00:53 GMT
ENV HAPROXY_VERSION=2.2.13
# Sat, 10 Apr 2021 09:00:54 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.13.tar.gz
# Sat, 10 Apr 2021 09:00:55 GMT
ENV HAPROXY_SHA256=9e3e51441c70bedfb494fc9d4b4d3389a71be9a3c915ba3d6f7e8fd9a57ce160
# Sat, 10 Apr 2021 09:01:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 09:01:37 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 09:01:38 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 09:01:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 09:01:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 09:01:42 GMT
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
	-	`sha256:b75131a6ec2e4adca7605661356ce165e13803d545d79123d0e3330d435596f5`  
		Last Modified: Sat, 10 Apr 2021 09:05:50 GMT  
		Size: 8.7 MB (8719344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9ea1930c5490ff94769de0e8ab8aad2b5c1e4e72d54c27afee12d74411f600`  
		Last Modified: Sat, 10 Apr 2021 09:05:47 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2e34fd9824e23d785f73ea0802107c25f42c9ad3d30abdc87f5e61fd4e17080`  
		Last Modified: Sat, 10 Apr 2021 09:05:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.13` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:9ea94a117b8f204c209df772aee3188d13a616efe6ca343149e0ad29fa251507
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.0 MB (35023478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b853740b36a0d8cc1b4c066a09de9600dfaf3e5c09ddeb7d9a627384baa05ec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:41:25 GMT
ADD file:b24da7eb23eeae04e00d0e45da29a89fe8f992e8dcf4ba482afb907b8015b7bf in / 
# Sat, 10 Apr 2021 00:41:28 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:13:29 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 01:15:54 GMT
ENV HAPROXY_VERSION=2.2.13
# Sat, 10 Apr 2021 01:15:55 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.13.tar.gz
# Sat, 10 Apr 2021 01:15:57 GMT
ENV HAPROXY_SHA256=9e3e51441c70bedfb494fc9d4b4d3389a71be9a3c915ba3d6f7e8fd9a57ce160
# Sat, 10 Apr 2021 01:16:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 01:16:49 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 01:16:51 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 01:16:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 01:16:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 01:16:59 GMT
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
	-	`sha256:b208d49b31d425b72f01f4c0579f75de3e8a9e9b5e413d19ad545fcb1cfec498`  
		Last Modified: Sat, 10 Apr 2021 01:21:53 GMT  
		Size: 9.1 MB (9116944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69001e0866df82cbc43b538ac2c4247ac27a02101891fc85d945daa23280ec2e`  
		Last Modified: Sat, 10 Apr 2021 01:21:50 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fb9542d39b52a78dae6dfffd1040b30683aee32cf37f2699e42eae131137abe`  
		Last Modified: Sat, 10 Apr 2021 01:21:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.13` - linux; 386

```console
$ docker pull haproxy@sha256:49260af2de07dc187620f290c656da80183c7b1e8ab773755a40ee9f7f6f9aaf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36978050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baf5327943d1ef805085f695725d9d9d120dc638b881ba0daf29bbacdef45fe6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:39:42 GMT
ADD file:8885d4d13678543780bb04ba14b621179665f7951d5b261036a7092df9b376e7 in / 
# Sat, 10 Apr 2021 00:39:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 03:48:12 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 03:50:59 GMT
ENV HAPROXY_VERSION=2.2.13
# Sat, 10 Apr 2021 03:51:00 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.13.tar.gz
# Sat, 10 Apr 2021 03:51:00 GMT
ENV HAPROXY_SHA256=9e3e51441c70bedfb494fc9d4b4d3389a71be9a3c915ba3d6f7e8fd9a57ce160
# Sat, 10 Apr 2021 03:52:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 03:52:26 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 03:52:26 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 03:52:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 03:52:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 03:52:28 GMT
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
	-	`sha256:501040fe44c6490e09a71181c6626bc3bb0bfe93798932941b8c0789c72d1c5e`  
		Last Modified: Sat, 10 Apr 2021 03:59:58 GMT  
		Size: 9.2 MB (9187117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:388ebcc0127bdbcff243568101388f512720854794aa20ab9acddc6b0a922450`  
		Last Modified: Sat, 10 Apr 2021 03:59:50 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:284bc34ec1436775792b35bfa789aa45111707b63c5a95f5df4f6d25e5db332e`  
		Last Modified: Sat, 10 Apr 2021 03:59:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.13` - linux; mips64le

```console
$ docker pull haproxy@sha256:24f69608e75a6910345769e9baaa7433a51d911decf979eaaafd1490ff0a5ee2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34674134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:277a2344421652b30bcc8416edef8dfb9cc9ee769ba4ba5ad51bf80a6085bfa0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:09:40 GMT
ADD file:0c93801c4a3719dfd4c047d7f2f4d52bf463eba2ab875da1dc54dcc832aae20b in / 
# Sat, 10 Apr 2021 01:09:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:39:36 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 01:44:43 GMT
ENV HAPROXY_VERSION=2.2.13
# Sat, 10 Apr 2021 01:44:43 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.13.tar.gz
# Sat, 10 Apr 2021 01:44:43 GMT
ENV HAPROXY_SHA256=9e3e51441c70bedfb494fc9d4b4d3389a71be9a3c915ba3d6f7e8fd9a57ce160
# Sat, 10 Apr 2021 01:47:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 01:47:05 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 01:47:06 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 01:47:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 01:47:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 01:47:08 GMT
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
	-	`sha256:34d169508d4b44b7fea30d0806ab3babbfe581b239f681919ae771c048d8213f`  
		Last Modified: Sat, 10 Apr 2021 01:54:23 GMT  
		Size: 8.9 MB (8865773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e41b7b929b9472e4f31050212242ce54c3d7abad584e23967b0ca1f52e3d262`  
		Last Modified: Sat, 10 Apr 2021 01:54:17 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e80eb6485d38caf34db8f19ffc92fd40dd6cf9bbed315177ada12c503c2cdf4`  
		Last Modified: Sat, 10 Apr 2021 01:54:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.13` - linux; ppc64le

```console
$ docker pull haproxy@sha256:051c8550a62dede7d06f587afb6946e710050fcf711ff38461c488dcffda9498
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40318021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67d26e25e79a68e404304e5bae82aefa19b2b9d4ee83dcaf8979d716a45e6a10`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:26:49 GMT
ADD file:ab87d4854aa8628ce8f4e603c0496499f6f28c3d2525ace782c7369691dafc8c in / 
# Sat, 10 Apr 2021 01:26:56 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 04:45:12 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 04:55:51 GMT
ENV HAPROXY_VERSION=2.2.13
# Sat, 10 Apr 2021 04:55:53 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.13.tar.gz
# Sat, 10 Apr 2021 04:55:57 GMT
ENV HAPROXY_SHA256=9e3e51441c70bedfb494fc9d4b4d3389a71be9a3c915ba3d6f7e8fd9a57ce160
# Sat, 10 Apr 2021 04:58:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 04:58:42 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 04:58:44 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 04:58:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 04:58:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 04:59:01 GMT
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
	-	`sha256:47d98ea7f5d6d0054eae8b1260b42df2c05e11015c73624875e953c2b5511090`  
		Last Modified: Sat, 10 Apr 2021 05:10:21 GMT  
		Size: 9.8 MB (9770127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a53dae98d3c653079c8dcee254bd233926f95fad7e2bf848e03a672956fd14`  
		Last Modified: Sat, 10 Apr 2021 05:10:19 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78cc95082c4533e2331bcf6b59f548c5ec2d66ac08321631a1350df97f7df0a5`  
		Last Modified: Sat, 10 Apr 2021 05:10:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.13` - linux; s390x

```console
$ docker pull haproxy@sha256:883a075a06023316a2ff2ff319689020b42812c4b6da7db73156722fb8e8614c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34759692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:812759d5bb748fe3ab35c1c945a594798c94ee29f65ab389f7d1b3ace8359191`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:42:23 GMT
ADD file:dbe2182f8699f2a6011413ea01862e6c0e85853d922dffd72a28d994d23c79bc in / 
# Sat, 10 Apr 2021 00:42:25 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:38:04 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 01:39:35 GMT
ENV HAPROXY_VERSION=2.2.13
# Sat, 10 Apr 2021 01:39:35 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.13.tar.gz
# Sat, 10 Apr 2021 01:39:36 GMT
ENV HAPROXY_SHA256=9e3e51441c70bedfb494fc9d4b4d3389a71be9a3c915ba3d6f7e8fd9a57ce160
# Sat, 10 Apr 2021 01:40:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 01:40:07 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 01:40:07 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 01:40:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 01:40:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 01:40:08 GMT
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
	-	`sha256:1ca81c5eef5f2d44f041789ed53dbfa0a6453bee245921eade23f4c550c190d8`  
		Last Modified: Sat, 10 Apr 2021 01:42:47 GMT  
		Size: 9.0 MB (9003958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0788fe9c0f74dcb98ef569fdf7251c230f9f2c4adcb7b03df2d7ecf36d8517e8`  
		Last Modified: Sat, 10 Apr 2021 01:42:45 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b6982746ce00451b99cf4beb0304c2d327fbaa5898f24a06c04ce6048d85149`  
		Last Modified: Sat, 10 Apr 2021 01:42:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.2.13-alpine`

```console
$ docker pull haproxy@sha256:413f24a6ce6057afafb796d156e6b332bdcb37a28f499599aa7c9b4d1434cbbd
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

### `haproxy:2.2.13-alpine` - linux; amd64

```console
$ docker pull haproxy@sha256:51528e0da4c91c96e9451d07c0d79fa2c7ec359c9486006b6a2381adb50616ab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.2 MB (9183249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d94ea559268af6d140850108edea1185c786262681f3912e945b540caf8bf47`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:37:38 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 21:39:55 GMT
ENV HAPROXY_VERSION=2.2.13
# Wed, 14 Apr 2021 21:39:55 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.13.tar.gz
# Wed, 14 Apr 2021 21:39:55 GMT
ENV HAPROXY_SHA256=9e3e51441c70bedfb494fc9d4b4d3389a71be9a3c915ba3d6f7e8fd9a57ce160
# Wed, 14 Apr 2021 21:40:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 21:40:44 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 21:40:44 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 21:40:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 21:40:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 21:40:45 GMT
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
	-	`sha256:ba81e90af14a863a9b5685b5085eec923abff1890a6fd2a3f0e07994974e31d7`  
		Last Modified: Wed, 14 Apr 2021 21:44:03 GMT  
		Size: 6.4 MB (6369525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc0670e87880c224e8aaeffba5dcacdd308471d5f995f18cc7457f21d0a2a04`  
		Last Modified: Wed, 14 Apr 2021 21:44:02 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a009871a4c718317430f5cd8acafa4a1c6f3020f699c1e9a4b3b9e06540267c`  
		Last Modified: Wed, 14 Apr 2021 21:44:02 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.13-alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:998908d9876cf5186d814914e16aad5bbf9f9fd36cd12e64ab2cf5cd2f9e21ef
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.9 MB (8873199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58b3a8c2e2ff9d47d90f2fb6f7661c6ee64bdb5ab6eb0577bbb9899bd8dceb42`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:18:05 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 21:24:17 GMT
ENV HAPROXY_VERSION=2.2.13
# Wed, 14 Apr 2021 21:24:26 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.13.tar.gz
# Wed, 14 Apr 2021 21:24:33 GMT
ENV HAPROXY_SHA256=9e3e51441c70bedfb494fc9d4b4d3389a71be9a3c915ba3d6f7e8fd9a57ce160
# Wed, 14 Apr 2021 21:25:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 21:26:12 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 21:26:21 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 21:26:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 21:26:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 21:27:07 GMT
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
	-	`sha256:1f961936d3b3f46a3711ffae66d510e2e3587ecc266ffc4228dc5bd3e348e588`  
		Last Modified: Wed, 14 Apr 2021 21:34:29 GMT  
		Size: 6.2 MB (6249312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f89851496a5733b45c2a26de344e1e0888de96a5b2d2c0daa7f0e6e2765ec37`  
		Last Modified: Wed, 14 Apr 2021 21:34:28 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065a09e958b3582c21934c8ef7a6fc65e4573d59cd9e486affab9e9d427bbe8e`  
		Last Modified: Wed, 14 Apr 2021 21:34:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.13-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:b7073b291f697c7935c86c245c86fee0cf05b1f51ea7192ccc0f8788a26b76cf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8591663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47b928f6c9cacabd2bcaae105d88e5d2fdeae2e042c3fd34b7b046c718e15150`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:47:58 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 22:52:15 GMT
ENV HAPROXY_VERSION=2.2.13
# Wed, 14 Apr 2021 22:52:18 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.13.tar.gz
# Wed, 14 Apr 2021 22:52:20 GMT
ENV HAPROXY_SHA256=9e3e51441c70bedfb494fc9d4b4d3389a71be9a3c915ba3d6f7e8fd9a57ce160
# Wed, 14 Apr 2021 22:52:54 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 22:52:56 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 22:52:57 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 22:53:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 22:53:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 22:53:04 GMT
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
	-	`sha256:a9db6c809add6fb1c65ed18e490e0aef9ceec249693f5014ad157e8989b2f97a`  
		Last Modified: Wed, 14 Apr 2021 22:56:40 GMT  
		Size: 6.2 MB (6165762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c54a8deef45aafe8d23348b71b1907c6930bd15e2cb8e9b3cbba14f225db81e3`  
		Last Modified: Wed, 14 Apr 2021 22:56:37 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3307625a9b488e9e1c508c95cd16dbee010765a6d9d5561c0723bc7a75a8d5b`  
		Last Modified: Wed, 14 Apr 2021 22:56:37 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.13-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:16bca21e897d7c52b2517cf4ba4e89c8ddb5e431b4cccad8fcc225eabcce25ca
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.1 MB (9088539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c6169d0eba5060ded320c17fa92adcdcdf3ee92545eb40d895e0544a4ef71cd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:26:01 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 20:30:39 GMT
ENV HAPROXY_VERSION=2.2.13
# Wed, 14 Apr 2021 20:30:46 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.13.tar.gz
# Wed, 14 Apr 2021 20:30:54 GMT
ENV HAPROXY_SHA256=9e3e51441c70bedfb494fc9d4b4d3389a71be9a3c915ba3d6f7e8fd9a57ce160
# Wed, 14 Apr 2021 20:31:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 20:31:49 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 20:31:50 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:32:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 20:32:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:32:21 GMT
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
	-	`sha256:3f46520f93f138b7f11e9721ba69bfde0f4f1da77e7b5ba2be9de502d0595b54`  
		Last Modified: Wed, 14 Apr 2021 20:38:18 GMT  
		Size: 6.4 MB (6374758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a83203e2d21398703492ebb3881e3ad57ae31c92251d8d94e7be21b51ac3a695`  
		Last Modified: Wed, 14 Apr 2021 20:38:16 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c812aee4a6ede81fd42bd6abae3c0f8300ef5222e074a574be9c861c6de4d0ac`  
		Last Modified: Wed, 14 Apr 2021 20:38:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.13-alpine` - linux; 386

```console
$ docker pull haproxy@sha256:a0fbc701001da548b035064db09a6be1e31e17125183345e0a6e9183abb2cb4f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9023341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13c3c2ecf9cd56e8732956bd2c0b272bd99a5a2e5090755c3137696b34ee3889`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 01:50:06 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 15 Apr 2021 01:53:40 GMT
ENV HAPROXY_VERSION=2.2.13
# Thu, 15 Apr 2021 01:53:40 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.13.tar.gz
# Thu, 15 Apr 2021 01:53:40 GMT
ENV HAPROXY_SHA256=9e3e51441c70bedfb494fc9d4b4d3389a71be9a3c915ba3d6f7e8fd9a57ce160
# Thu, 15 Apr 2021 01:54:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 15 Apr 2021 01:54:44 GMT
STOPSIGNAL SIGUSR1
# Thu, 15 Apr 2021 01:54:44 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 15 Apr 2021 01:54:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 15 Apr 2021 01:54:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Apr 2021 01:54:45 GMT
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
	-	`sha256:dd83349dc27b7c6494b326db86b2fb5ab9fded96732b87dcbdfe7ffbf53eb6fd`  
		Last Modified: Thu, 15 Apr 2021 02:01:05 GMT  
		Size: 6.2 MB (6202686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df9e7c12c69c54a160be7a4c5497240b0dffff220b6d1eb44aa7977bc593d408`  
		Last Modified: Thu, 15 Apr 2021 02:01:04 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c24d7fe1943abc1fdfcdef29513a413337092d356e48d6b6b868c73ed4ca4b6b`  
		Last Modified: Thu, 15 Apr 2021 02:01:03 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.13-alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:3176f25d3818aaecc48b0cb829219da0864af79b2564b8eecd5ebccfa4f40468
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9499255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27f33cdd58ab09da862b649ad36eb8667c6ee6018e65a43528c3d7a198a44b72`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:25:09 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 23:29:12 GMT
ENV HAPROXY_VERSION=2.2.13
# Wed, 14 Apr 2021 23:29:16 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.13.tar.gz
# Wed, 14 Apr 2021 23:29:20 GMT
ENV HAPROXY_SHA256=9e3e51441c70bedfb494fc9d4b4d3389a71be9a3c915ba3d6f7e8fd9a57ce160
# Wed, 14 Apr 2021 23:30:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 23:30:20 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 23:30:22 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 23:30:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 23:30:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 23:30:47 GMT
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
	-	`sha256:e8a3685c2ec0932a7f73fa0032bf33500306ee2a5d0abf655e8983b0c8a95acd`  
		Last Modified: Wed, 14 Apr 2021 23:37:09 GMT  
		Size: 6.7 MB (6684359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74885306f2f1ac242fa8c216d998632b927a5cd3678771077f7a7f650d8ba37d`  
		Last Modified: Wed, 14 Apr 2021 23:37:07 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32336bc725a4335e246865126dccc149331aa27ef4a8767172fb2cff483b4ca4`  
		Last Modified: Wed, 14 Apr 2021 23:37:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.13-alpine` - linux; s390x

```console
$ docker pull haproxy@sha256:5fb7df6e38eea99e9f0e9d4a19cd193a5be4747420d5b38082dfc02df9fb6d1a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.9 MB (8940300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e32f238bf459522abbbbb20a287e8543faf16dd5307b7fa7da33e7edfe3f4b8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:54:24 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 20:56:12 GMT
ENV HAPROXY_VERSION=2.2.13
# Wed, 14 Apr 2021 20:56:12 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.13.tar.gz
# Wed, 14 Apr 2021 20:56:12 GMT
ENV HAPROXY_SHA256=9e3e51441c70bedfb494fc9d4b4d3389a71be9a3c915ba3d6f7e8fd9a57ce160
# Wed, 14 Apr 2021 20:56:47 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 20:56:47 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 20:56:47 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:56:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 20:56:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:56:49 GMT
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
	-	`sha256:9b54506479f94cd6e6ff33fd666b2e4ef038a755e897f69c41e2024451738f22`  
		Last Modified: Wed, 14 Apr 2021 20:59:30 GMT  
		Size: 6.3 MB (6335894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b346055862205d30d0fec1cd13ad03e77403df88ae4b0e999a9fa3f2f5738371`  
		Last Modified: Wed, 14 Apr 2021 20:59:29 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1c0e6cd04f7bb776fd8fc6fcdd6ca22f1247acb507d44b41d9163155c7e5d9`  
		Last Modified: Wed, 14 Apr 2021 20:59:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.3`

```console
$ docker pull haproxy@sha256:f63aabf39efcd277b04a503d38e59e80224a0c11f47b2568b13b0092698c5a3a
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
$ docker pull haproxy@sha256:fa42cfd9f7ee39c10215258a25308d7ad5f6a3b2e8b99c216d22b8aeab0cd9c1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.7 MB (36695481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15630318f735650284c7afcde2e3c813c4e78340d9ff6761e84bd829a7e51e87`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:29:42 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 06:31:25 GMT
ENV HAPROXY_VERSION=2.3.9
# Sat, 10 Apr 2021 06:31:25 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.9.tar.gz
# Sat, 10 Apr 2021 06:31:25 GMT
ENV HAPROXY_SHA256=77110bc1272bad18fff56b30f4614bcc1deb50600ae42cb0f0b161fc41e2ba96
# Sat, 10 Apr 2021 06:32:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 06:32:21 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 06:32:22 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 06:32:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 06:32:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 06:32:24 GMT
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
	-	`sha256:df883def87ebe557cc46aaeca475a9bd5454161217a472bb8843b275194833ea`  
		Last Modified: Sat, 10 Apr 2021 06:38:23 GMT  
		Size: 9.6 MB (9554157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:038f2c73c3bef00ccb45017c5fa20d688d83dc4a82772af4c286b38d408bc365`  
		Last Modified: Sat, 10 Apr 2021 06:38:21 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62b97027777b1b16f3b053b4b6c440474edf49148b2f249f2649c9e485f88c8d`  
		Last Modified: Sat, 10 Apr 2021 06:38:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:4f4f4468959827b0c860592aaa85abb97caeb8ec0f9aac47c3f522727ffee0fa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (34039733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ca650df4f2b0f360fca1a41bcde309f21b21e62c4f6bb717bdd4c196c4a4c51`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:51:31 GMT
ADD file:926533a23a69aa2481a9122b667bb6300a347154eea366c9e679a230aa7f373a in / 
# Sat, 10 Apr 2021 00:51:34 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 02:24:17 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 02:26:09 GMT
ENV HAPROXY_VERSION=2.3.9
# Sat, 10 Apr 2021 02:26:13 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.9.tar.gz
# Sat, 10 Apr 2021 02:26:16 GMT
ENV HAPROXY_SHA256=77110bc1272bad18fff56b30f4614bcc1deb50600ae42cb0f0b161fc41e2ba96
# Sat, 10 Apr 2021 02:27:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 02:27:18 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 02:27:24 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 02:27:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 02:27:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 02:27:43 GMT
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
	-	`sha256:67f84b9aa74574db91fd776882e7ddc449b036a85d7421fda9ce0b66cd53227c`  
		Last Modified: Sat, 10 Apr 2021 02:37:07 GMT  
		Size: 9.2 MB (9164583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe3f7588980758230b77ae29222ce3a4792fce39a431518a5d2b4601dbfb0ac3`  
		Last Modified: Sat, 10 Apr 2021 02:37:04 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b97190d21dc7f1f4b5cab24efde00b68d49e3f7a5d7b845cfd8a134a3b45f01`  
		Last Modified: Sat, 10 Apr 2021 02:37:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:8546ee0d84b1809008a7d0af2d688fdaad936066fdcfb69f9c15f60969321ec2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31766763 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:154e3a5a493a3254d84194f03dd38b61212efae170ebe3bdfbadbe59e2d25b3b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:59:45 GMT
ADD file:3fbd246a2de82566bcaaf62e3e0bf57175a7ad46b4156366a110661b31eab240 in / 
# Sat, 10 Apr 2021 00:59:47 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 08:58:51 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 08:59:51 GMT
ENV HAPROXY_VERSION=2.3.9
# Sat, 10 Apr 2021 08:59:52 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.9.tar.gz
# Sat, 10 Apr 2021 08:59:53 GMT
ENV HAPROXY_SHA256=77110bc1272bad18fff56b30f4614bcc1deb50600ae42cb0f0b161fc41e2ba96
# Sat, 10 Apr 2021 09:00:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 09:00:33 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 09:00:34 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 09:00:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 09:00:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 09:00:38 GMT
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
	-	`sha256:15bf0834e9efeb35188b41bfa4a66446c609dde5de0ae64e4f59c4192844340f`  
		Last Modified: Sat, 10 Apr 2021 09:05:38 GMT  
		Size: 9.0 MB (9025015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1199d1177880e0e9af691b1d831f9d408004aea8508fe3068df501f64dc7c4e9`  
		Last Modified: Sat, 10 Apr 2021 09:05:35 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62336b3e70f00cdb67d3d3b57f04d4e38fe453cf2a320472b95c1e646e214fb1`  
		Last Modified: Sat, 10 Apr 2021 09:05:35 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:d4152a50e3a1d0c539e2c0da480494cb03173b407e5280fe3377e1c59502c2e8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35347191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35bd0c1cb4a0e6110216a3a3e8e51c671697ce828fb060dcc6e18f991e9d7294`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:41:25 GMT
ADD file:b24da7eb23eeae04e00d0e45da29a89fe8f992e8dcf4ba482afb907b8015b7bf in / 
# Sat, 10 Apr 2021 00:41:28 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:13:29 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 01:14:41 GMT
ENV HAPROXY_VERSION=2.3.9
# Sat, 10 Apr 2021 01:14:42 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.9.tar.gz
# Sat, 10 Apr 2021 01:14:43 GMT
ENV HAPROXY_SHA256=77110bc1272bad18fff56b30f4614bcc1deb50600ae42cb0f0b161fc41e2ba96
# Sat, 10 Apr 2021 01:15:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 01:15:29 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 01:15:30 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 01:15:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 01:15:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 01:15:35 GMT
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
	-	`sha256:50023a581af47a05e808c497ef77767fb715a8faab03f14014f4a0daf9cc95d4`  
		Last Modified: Sat, 10 Apr 2021 01:21:39 GMT  
		Size: 9.4 MB (9440659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d067d1042b01ff19aac1b75558139c81bf8c08f7987b4683f41cee55d25ae1d5`  
		Last Modified: Sat, 10 Apr 2021 01:21:37 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7fbf89cba9a16dac8ecd7198f7adcbd4ba1aacbf3cb6fed25d98af7113cc9e`  
		Last Modified: Sat, 10 Apr 2021 01:21:37 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3` - linux; 386

```console
$ docker pull haproxy@sha256:3f56e9b27fb491e75d845611cd4a286778b258159fb858d433fedf0a67c107c0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.2 MB (37206708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba2c3b8430883fc337b03423ad8f552ebce3c59922aa2848eda4aa4851fedf40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:39:42 GMT
ADD file:8885d4d13678543780bb04ba14b621179665f7951d5b261036a7092df9b376e7 in / 
# Sat, 10 Apr 2021 00:39:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 03:48:12 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 03:49:41 GMT
ENV HAPROXY_VERSION=2.3.9
# Sat, 10 Apr 2021 03:49:42 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.9.tar.gz
# Sat, 10 Apr 2021 03:49:42 GMT
ENV HAPROXY_SHA256=77110bc1272bad18fff56b30f4614bcc1deb50600ae42cb0f0b161fc41e2ba96
# Sat, 10 Apr 2021 03:50:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 03:50:39 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 03:50:39 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 03:50:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 03:50:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 03:50:41 GMT
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
	-	`sha256:b1f6beb31958abbb8f7a9acf66b271bb4dc1d8d0b98388c882495f0ef83610d0`  
		Last Modified: Sat, 10 Apr 2021 03:59:30 GMT  
		Size: 9.4 MB (9415773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15fe6c571e5875233b0a10e1cb7a2f1369c603593dc4a8ff137666839901235b`  
		Last Modified: Sat, 10 Apr 2021 03:59:26 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d481f6e20a049956aa9c45f996c4e1021f9a264880f372a60ea6402b756bfdfa`  
		Last Modified: Sat, 10 Apr 2021 03:59:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3` - linux; mips64le

```console
$ docker pull haproxy@sha256:53436f8b139b3fd4d1aeb5af64fd64728367d88f336c94f214220e29f30ba650
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.9 MB (34940784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87eebec53adc866af1eb6d1f0fa86b198fd2180cea5ca55681b1fb3fe0d41c5d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:09:40 GMT
ADD file:0c93801c4a3719dfd4c047d7f2f4d52bf463eba2ab875da1dc54dcc832aae20b in / 
# Sat, 10 Apr 2021 01:09:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:39:36 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 01:42:16 GMT
ENV HAPROXY_VERSION=2.3.9
# Sat, 10 Apr 2021 01:42:17 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.9.tar.gz
# Sat, 10 Apr 2021 01:42:17 GMT
ENV HAPROXY_SHA256=77110bc1272bad18fff56b30f4614bcc1deb50600ae42cb0f0b161fc41e2ba96
# Sat, 10 Apr 2021 01:44:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 01:44:36 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 01:44:36 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 01:44:38 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 01:44:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 01:44:39 GMT
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
	-	`sha256:d1372285d5ae001a835df04f6feaf805c2b2c652679dde7805ec9bd4e10c47a6`  
		Last Modified: Sat, 10 Apr 2021 01:54:04 GMT  
		Size: 9.1 MB (9132422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:701e913c803ad74ba962379671609f4cb6496d8bfc4bba941ff1f2934d1d6d50`  
		Last Modified: Sat, 10 Apr 2021 01:53:57 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89484a5f3cd65e20b77c9a3f2b34f5a3e21db69bee7cadd04a91f4ff5f24c7f`  
		Last Modified: Sat, 10 Apr 2021 01:53:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3` - linux; ppc64le

```console
$ docker pull haproxy@sha256:d5a1da8f612b8b7bb79e1c462da111fcca84adf2d63955e5656f8c151ca7ad15
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40587797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4392007f5f50e8bc72897aa2e05d25db0685de3a480bd976fc09db92635dbb97`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:26:49 GMT
ADD file:ab87d4854aa8628ce8f4e603c0496499f6f28c3d2525ace782c7369691dafc8c in / 
# Sat, 10 Apr 2021 01:26:56 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 04:45:12 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 04:49:34 GMT
ENV HAPROXY_VERSION=2.3.9
# Sat, 10 Apr 2021 04:49:37 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.9.tar.gz
# Sat, 10 Apr 2021 04:49:42 GMT
ENV HAPROXY_SHA256=77110bc1272bad18fff56b30f4614bcc1deb50600ae42cb0f0b161fc41e2ba96
# Sat, 10 Apr 2021 04:55:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 04:55:04 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 04:55:07 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 04:55:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 04:55:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 04:55:34 GMT
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
	-	`sha256:02dce87e4030362a76d243c695c727400c1fd6e681a33250a0c28bf2959ae752`  
		Last Modified: Sat, 10 Apr 2021 05:10:05 GMT  
		Size: 10.0 MB (10039904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c079ef5cde73a0361b14c8a5f1233d1b99b440f80b935334458e57cf3868804d`  
		Last Modified: Sat, 10 Apr 2021 05:10:03 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27203244b0981a4f3bb61515617544544f43c8b518b565a045b3a3b79db4ce5b`  
		Last Modified: Sat, 10 Apr 2021 05:10:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3` - linux; s390x

```console
$ docker pull haproxy@sha256:19f3d5d79196611de41352b39a99bdf83b98e44349876ab6cdb27b6e1f35c181
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.0 MB (35044591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ede5f02058145c8565168e90cb541d031baba061a845ef0d1083b665e3277965`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:42:23 GMT
ADD file:dbe2182f8699f2a6011413ea01862e6c0e85853d922dffd72a28d994d23c79bc in / 
# Sat, 10 Apr 2021 00:42:25 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:38:04 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 01:38:49 GMT
ENV HAPROXY_VERSION=2.3.9
# Sat, 10 Apr 2021 01:38:50 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.9.tar.gz
# Sat, 10 Apr 2021 01:38:50 GMT
ENV HAPROXY_SHA256=77110bc1272bad18fff56b30f4614bcc1deb50600ae42cb0f0b161fc41e2ba96
# Sat, 10 Apr 2021 01:39:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 01:39:22 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 01:39:22 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 01:39:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 01:39:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 01:39:23 GMT
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
	-	`sha256:278677bd5845b54d7bbc1e1a92c95b6211358dc62bd96f1fc52ec341df16206d`  
		Last Modified: Sat, 10 Apr 2021 01:42:38 GMT  
		Size: 9.3 MB (9288855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edc908ef823f2540bc02f00eeb071894d56eddaf33d48ff9224cda774e4d54be`  
		Last Modified: Sat, 10 Apr 2021 01:42:37 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a4523549f27c304e4a974a37341a467a3bb7fca15bab56a5a5f97613f7ff9b2`  
		Last Modified: Sat, 10 Apr 2021 01:42:37 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.3-alpine`

```console
$ docker pull haproxy@sha256:fd871b2cf0be22d10d148fffe88441167587ea84bad028d4eb81808f28251070
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
$ docker pull haproxy@sha256:101ee16ec0838ee24f3695ccbd3653b735af22c130d6fd0d7be6d7ac9bc879a4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9499607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:383495f19607c1dd21dce3f33aef722f2c94d10c76eb76dce409928ada65c265`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:37:38 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 21:38:52 GMT
ENV HAPROXY_VERSION=2.3.9
# Wed, 14 Apr 2021 21:38:52 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.9.tar.gz
# Wed, 14 Apr 2021 21:38:52 GMT
ENV HAPROXY_SHA256=77110bc1272bad18fff56b30f4614bcc1deb50600ae42cb0f0b161fc41e2ba96
# Wed, 14 Apr 2021 21:39:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 21:39:42 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 21:39:42 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 21:39:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 21:39:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 21:39:44 GMT
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
	-	`sha256:7b412bb59f5511a4cc66e0b0eb2c0b1781069e37fc9fcda8f4e0908c48d6584f`  
		Last Modified: Wed, 14 Apr 2021 21:43:46 GMT  
		Size: 6.7 MB (6685882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:321129059a3aee4d0de22e7b595549eb049c90428cd1e220ce0f904fc2d70c49`  
		Last Modified: Wed, 14 Apr 2021 21:43:45 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16f8e4cbddc48fe0e653ac776e4d1bd90066ace1e53e95d4f01b3179c7a4914e`  
		Last Modified: Wed, 14 Apr 2021 21:43:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3-alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:aa7d553fd0c3bc210b6aa068e134a7b95f07577abecdf0f9eb2318d798d93bfc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.2 MB (9209545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5382bb355f68826f4b9ded72ab54cef0217d776f3172303c578a8c80056ce23c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:18:05 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 21:20:51 GMT
ENV HAPROXY_VERSION=2.3.9
# Wed, 14 Apr 2021 21:21:02 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.9.tar.gz
# Wed, 14 Apr 2021 21:21:11 GMT
ENV HAPROXY_SHA256=77110bc1272bad18fff56b30f4614bcc1deb50600ae42cb0f0b161fc41e2ba96
# Wed, 14 Apr 2021 21:22:23 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 21:22:35 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 21:22:51 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 21:23:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 21:23:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 21:23:45 GMT
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
	-	`sha256:5300d7514c3b8d397433442634825547f6a6612e10c46f4ce3dbb4225d5c7720`  
		Last Modified: Wed, 14 Apr 2021 21:34:16 GMT  
		Size: 6.6 MB (6585661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3c323aab13edc8b368334c6d8ad71cec1535117eaeec134595b17088d37937b`  
		Last Modified: Wed, 14 Apr 2021 21:34:15 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e846321291b72a418aa9ccff5106b00fc25129846b6ac70d6cf51fe0374d797`  
		Last Modified: Wed, 14 Apr 2021 21:34:17 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:75fb3450317233e825f312b8f71b7587d9fd67908e21917728c7a306e6877be5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.9 MB (8926169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acf4585d9e128a18420fdc031947d290650b37b108452804564b0d35e86def6e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:47:58 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 22:49:20 GMT
ENV HAPROXY_VERSION=2.3.9
# Wed, 14 Apr 2021 22:49:29 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.9.tar.gz
# Wed, 14 Apr 2021 22:49:36 GMT
ENV HAPROXY_SHA256=77110bc1272bad18fff56b30f4614bcc1deb50600ae42cb0f0b161fc41e2ba96
# Wed, 14 Apr 2021 22:50:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 22:50:53 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 22:51:05 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 22:51:42 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 22:51:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 22:51:53 GMT
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
	-	`sha256:0b33f8441fa4f8170fcb000f1c6d2614765037bc108661d7ca5e54b529f37010`  
		Last Modified: Wed, 14 Apr 2021 22:56:23 GMT  
		Size: 6.5 MB (6500266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7d61f2b79b5d21794c5d4dcc642a2df4a7c899b2ece6f1a1d7cfc5f4c47496`  
		Last Modified: Wed, 14 Apr 2021 22:56:21 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef906e7aaf5f11781888556cccd267b184bdbecc723469a8747dababde6cae88`  
		Last Modified: Wed, 14 Apr 2021 22:56:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:4697ab52f31a27418b40afce46493f004c96c3a8b4f5b3234f2ad8fd8b7bb612
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9412142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ad4040f240cdfea6361a98a491df6e7c2e8bd00c8c0f1ea0a9ddde03f43254d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:26:01 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 20:28:04 GMT
ENV HAPROXY_VERSION=2.3.9
# Wed, 14 Apr 2021 20:28:12 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.9.tar.gz
# Wed, 14 Apr 2021 20:28:20 GMT
ENV HAPROXY_SHA256=77110bc1272bad18fff56b30f4614bcc1deb50600ae42cb0f0b161fc41e2ba96
# Wed, 14 Apr 2021 20:29:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 20:29:17 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 20:29:25 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:29:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 20:30:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:30:11 GMT
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
	-	`sha256:6c72b09b2c83b9e5a88d98cf15715a3dfdc984d4837af7d7365a07ea6a3d7866`  
		Last Modified: Wed, 14 Apr 2021 20:38:03 GMT  
		Size: 6.7 MB (6698357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bba2f8c9c125c15cccf5572333f7c53e54f6df343fb7e7cce3177d1331ebc8d8`  
		Last Modified: Wed, 14 Apr 2021 20:38:01 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3057815f353087d9bee55cd953f619dd59c84c2f554ea8058882188f9e4f814`  
		Last Modified: Wed, 14 Apr 2021 20:38:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3-alpine` - linux; 386

```console
$ docker pull haproxy@sha256:9f99933bbb9fb8a7b3b040bf9b93ce55dde75211224d44c75e3bcd76299e5d7c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9354648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa6e1a1e81c45d3bc98a25c27b58ff451e0d561ea1f95d289ee3cee4b0c35f4a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 01:50:06 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 15 Apr 2021 01:52:21 GMT
ENV HAPROXY_VERSION=2.3.9
# Thu, 15 Apr 2021 01:52:21 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.9.tar.gz
# Thu, 15 Apr 2021 01:52:21 GMT
ENV HAPROXY_SHA256=77110bc1272bad18fff56b30f4614bcc1deb50600ae42cb0f0b161fc41e2ba96
# Thu, 15 Apr 2021 01:53:27 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 15 Apr 2021 01:53:27 GMT
STOPSIGNAL SIGUSR1
# Thu, 15 Apr 2021 01:53:27 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 15 Apr 2021 01:53:28 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 15 Apr 2021 01:53:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Apr 2021 01:53:29 GMT
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
	-	`sha256:ca59b31cb2383b0cecb9a081d46bc5cb55ff05176d7da51344504b99f485b37c`  
		Last Modified: Thu, 15 Apr 2021 02:00:45 GMT  
		Size: 6.5 MB (6533992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43d9fdba60ae084cf195a2fc170f0358d1eb329ec60f7e3d78f39e3bd42c0599`  
		Last Modified: Thu, 15 Apr 2021 02:00:44 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a98584752f736ec3c38550ffb5a53f52be250c0c3b5b5d2d3cb60d2b08f0fa31`  
		Last Modified: Thu, 15 Apr 2021 02:00:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3-alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:19dc93de5c25a5e87c31214ba644e2d889de9b3834a4f13762711529b7d12a8f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.8 MB (9832346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb9dac528b8dbf1a3a08aeeb1ac86db8bbef3c78e14cbcd1229183af17c6bb12`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:25:09 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 23:26:45 GMT
ENV HAPROXY_VERSION=2.3.9
# Wed, 14 Apr 2021 23:26:47 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.9.tar.gz
# Wed, 14 Apr 2021 23:26:51 GMT
ENV HAPROXY_SHA256=77110bc1272bad18fff56b30f4614bcc1deb50600ae42cb0f0b161fc41e2ba96
# Wed, 14 Apr 2021 23:28:14 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 23:28:20 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 23:28:27 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 23:28:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 23:28:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 23:28:56 GMT
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
	-	`sha256:55517a2814e2dbb00eb7d44f417b8729aa436b00a32a084c238b7d5733011cb2`  
		Last Modified: Wed, 14 Apr 2021 23:36:51 GMT  
		Size: 7.0 MB (7017449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e5587a8b18c5eac4421c6e6dcf2bd5b8aa86e1cc461dd1608c57f7d8208359`  
		Last Modified: Wed, 14 Apr 2021 23:36:50 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e0e401a50336fe2abb496fdd8bae8c8a08a451470c41b530499798a6e9a14f2`  
		Last Modified: Wed, 14 Apr 2021 23:36:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3-alpine` - linux; s390x

```console
$ docker pull haproxy@sha256:5736a38ee6dd2b1a7821b37847aae240638a52c8bac5062883d90fca886909b3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9257346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25cf086b4e421310119b91b6fe47633d277b498487de5549fb997acd6a25cb0f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:54:24 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 20:55:17 GMT
ENV HAPROXY_VERSION=2.3.9
# Wed, 14 Apr 2021 20:55:17 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.9.tar.gz
# Wed, 14 Apr 2021 20:55:18 GMT
ENV HAPROXY_SHA256=77110bc1272bad18fff56b30f4614bcc1deb50600ae42cb0f0b161fc41e2ba96
# Wed, 14 Apr 2021 20:55:58 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 20:55:59 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 20:55:59 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:56:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 20:56:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:56:00 GMT
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
	-	`sha256:ae9e557ff45057778dffe5c56dc419e35c7d970db8ce611466c9b0d09a048305`  
		Last Modified: Wed, 14 Apr 2021 20:59:18 GMT  
		Size: 6.7 MB (6652940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb69cd1d8680cdc862b3d406dbc637a101625886f943068bf0dd5647f78353df`  
		Last Modified: Wed, 14 Apr 2021 20:59:17 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8270e1f8a61ff9eb8008cffc9b5ae5fb3a982db994eaa84d2653ef71236dec1e`  
		Last Modified: Wed, 14 Apr 2021 20:59:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.3.9`

```console
$ docker pull haproxy@sha256:f63aabf39efcd277b04a503d38e59e80224a0c11f47b2568b13b0092698c5a3a
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

### `haproxy:2.3.9` - linux; amd64

```console
$ docker pull haproxy@sha256:fa42cfd9f7ee39c10215258a25308d7ad5f6a3b2e8b99c216d22b8aeab0cd9c1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.7 MB (36695481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15630318f735650284c7afcde2e3c813c4e78340d9ff6761e84bd829a7e51e87`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:29:42 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 06:31:25 GMT
ENV HAPROXY_VERSION=2.3.9
# Sat, 10 Apr 2021 06:31:25 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.9.tar.gz
# Sat, 10 Apr 2021 06:31:25 GMT
ENV HAPROXY_SHA256=77110bc1272bad18fff56b30f4614bcc1deb50600ae42cb0f0b161fc41e2ba96
# Sat, 10 Apr 2021 06:32:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 06:32:21 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 06:32:22 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 06:32:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 06:32:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 06:32:24 GMT
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
	-	`sha256:df883def87ebe557cc46aaeca475a9bd5454161217a472bb8843b275194833ea`  
		Last Modified: Sat, 10 Apr 2021 06:38:23 GMT  
		Size: 9.6 MB (9554157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:038f2c73c3bef00ccb45017c5fa20d688d83dc4a82772af4c286b38d408bc365`  
		Last Modified: Sat, 10 Apr 2021 06:38:21 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62b97027777b1b16f3b053b4b6c440474edf49148b2f249f2649c9e485f88c8d`  
		Last Modified: Sat, 10 Apr 2021 06:38:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.9` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:4f4f4468959827b0c860592aaa85abb97caeb8ec0f9aac47c3f522727ffee0fa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (34039733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ca650df4f2b0f360fca1a41bcde309f21b21e62c4f6bb717bdd4c196c4a4c51`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:51:31 GMT
ADD file:926533a23a69aa2481a9122b667bb6300a347154eea366c9e679a230aa7f373a in / 
# Sat, 10 Apr 2021 00:51:34 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 02:24:17 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 02:26:09 GMT
ENV HAPROXY_VERSION=2.3.9
# Sat, 10 Apr 2021 02:26:13 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.9.tar.gz
# Sat, 10 Apr 2021 02:26:16 GMT
ENV HAPROXY_SHA256=77110bc1272bad18fff56b30f4614bcc1deb50600ae42cb0f0b161fc41e2ba96
# Sat, 10 Apr 2021 02:27:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 02:27:18 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 02:27:24 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 02:27:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 02:27:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 02:27:43 GMT
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
	-	`sha256:67f84b9aa74574db91fd776882e7ddc449b036a85d7421fda9ce0b66cd53227c`  
		Last Modified: Sat, 10 Apr 2021 02:37:07 GMT  
		Size: 9.2 MB (9164583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe3f7588980758230b77ae29222ce3a4792fce39a431518a5d2b4601dbfb0ac3`  
		Last Modified: Sat, 10 Apr 2021 02:37:04 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b97190d21dc7f1f4b5cab24efde00b68d49e3f7a5d7b845cfd8a134a3b45f01`  
		Last Modified: Sat, 10 Apr 2021 02:37:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.9` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:8546ee0d84b1809008a7d0af2d688fdaad936066fdcfb69f9c15f60969321ec2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31766763 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:154e3a5a493a3254d84194f03dd38b61212efae170ebe3bdfbadbe59e2d25b3b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:59:45 GMT
ADD file:3fbd246a2de82566bcaaf62e3e0bf57175a7ad46b4156366a110661b31eab240 in / 
# Sat, 10 Apr 2021 00:59:47 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 08:58:51 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 08:59:51 GMT
ENV HAPROXY_VERSION=2.3.9
# Sat, 10 Apr 2021 08:59:52 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.9.tar.gz
# Sat, 10 Apr 2021 08:59:53 GMT
ENV HAPROXY_SHA256=77110bc1272bad18fff56b30f4614bcc1deb50600ae42cb0f0b161fc41e2ba96
# Sat, 10 Apr 2021 09:00:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 09:00:33 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 09:00:34 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 09:00:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 09:00:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 09:00:38 GMT
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
	-	`sha256:15bf0834e9efeb35188b41bfa4a66446c609dde5de0ae64e4f59c4192844340f`  
		Last Modified: Sat, 10 Apr 2021 09:05:38 GMT  
		Size: 9.0 MB (9025015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1199d1177880e0e9af691b1d831f9d408004aea8508fe3068df501f64dc7c4e9`  
		Last Modified: Sat, 10 Apr 2021 09:05:35 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62336b3e70f00cdb67d3d3b57f04d4e38fe453cf2a320472b95c1e646e214fb1`  
		Last Modified: Sat, 10 Apr 2021 09:05:35 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.9` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:d4152a50e3a1d0c539e2c0da480494cb03173b407e5280fe3377e1c59502c2e8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35347191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35bd0c1cb4a0e6110216a3a3e8e51c671697ce828fb060dcc6e18f991e9d7294`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:41:25 GMT
ADD file:b24da7eb23eeae04e00d0e45da29a89fe8f992e8dcf4ba482afb907b8015b7bf in / 
# Sat, 10 Apr 2021 00:41:28 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:13:29 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 01:14:41 GMT
ENV HAPROXY_VERSION=2.3.9
# Sat, 10 Apr 2021 01:14:42 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.9.tar.gz
# Sat, 10 Apr 2021 01:14:43 GMT
ENV HAPROXY_SHA256=77110bc1272bad18fff56b30f4614bcc1deb50600ae42cb0f0b161fc41e2ba96
# Sat, 10 Apr 2021 01:15:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 01:15:29 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 01:15:30 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 01:15:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 01:15:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 01:15:35 GMT
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
	-	`sha256:50023a581af47a05e808c497ef77767fb715a8faab03f14014f4a0daf9cc95d4`  
		Last Modified: Sat, 10 Apr 2021 01:21:39 GMT  
		Size: 9.4 MB (9440659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d067d1042b01ff19aac1b75558139c81bf8c08f7987b4683f41cee55d25ae1d5`  
		Last Modified: Sat, 10 Apr 2021 01:21:37 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7fbf89cba9a16dac8ecd7198f7adcbd4ba1aacbf3cb6fed25d98af7113cc9e`  
		Last Modified: Sat, 10 Apr 2021 01:21:37 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.9` - linux; 386

```console
$ docker pull haproxy@sha256:3f56e9b27fb491e75d845611cd4a286778b258159fb858d433fedf0a67c107c0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.2 MB (37206708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba2c3b8430883fc337b03423ad8f552ebce3c59922aa2848eda4aa4851fedf40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:39:42 GMT
ADD file:8885d4d13678543780bb04ba14b621179665f7951d5b261036a7092df9b376e7 in / 
# Sat, 10 Apr 2021 00:39:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 03:48:12 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 03:49:41 GMT
ENV HAPROXY_VERSION=2.3.9
# Sat, 10 Apr 2021 03:49:42 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.9.tar.gz
# Sat, 10 Apr 2021 03:49:42 GMT
ENV HAPROXY_SHA256=77110bc1272bad18fff56b30f4614bcc1deb50600ae42cb0f0b161fc41e2ba96
# Sat, 10 Apr 2021 03:50:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 03:50:39 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 03:50:39 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 03:50:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 03:50:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 03:50:41 GMT
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
	-	`sha256:b1f6beb31958abbb8f7a9acf66b271bb4dc1d8d0b98388c882495f0ef83610d0`  
		Last Modified: Sat, 10 Apr 2021 03:59:30 GMT  
		Size: 9.4 MB (9415773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15fe6c571e5875233b0a10e1cb7a2f1369c603593dc4a8ff137666839901235b`  
		Last Modified: Sat, 10 Apr 2021 03:59:26 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d481f6e20a049956aa9c45f996c4e1021f9a264880f372a60ea6402b756bfdfa`  
		Last Modified: Sat, 10 Apr 2021 03:59:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.9` - linux; mips64le

```console
$ docker pull haproxy@sha256:53436f8b139b3fd4d1aeb5af64fd64728367d88f336c94f214220e29f30ba650
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.9 MB (34940784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87eebec53adc866af1eb6d1f0fa86b198fd2180cea5ca55681b1fb3fe0d41c5d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:09:40 GMT
ADD file:0c93801c4a3719dfd4c047d7f2f4d52bf463eba2ab875da1dc54dcc832aae20b in / 
# Sat, 10 Apr 2021 01:09:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:39:36 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 01:42:16 GMT
ENV HAPROXY_VERSION=2.3.9
# Sat, 10 Apr 2021 01:42:17 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.9.tar.gz
# Sat, 10 Apr 2021 01:42:17 GMT
ENV HAPROXY_SHA256=77110bc1272bad18fff56b30f4614bcc1deb50600ae42cb0f0b161fc41e2ba96
# Sat, 10 Apr 2021 01:44:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 01:44:36 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 01:44:36 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 01:44:38 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 01:44:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 01:44:39 GMT
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
	-	`sha256:d1372285d5ae001a835df04f6feaf805c2b2c652679dde7805ec9bd4e10c47a6`  
		Last Modified: Sat, 10 Apr 2021 01:54:04 GMT  
		Size: 9.1 MB (9132422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:701e913c803ad74ba962379671609f4cb6496d8bfc4bba941ff1f2934d1d6d50`  
		Last Modified: Sat, 10 Apr 2021 01:53:57 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89484a5f3cd65e20b77c9a3f2b34f5a3e21db69bee7cadd04a91f4ff5f24c7f`  
		Last Modified: Sat, 10 Apr 2021 01:53:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.9` - linux; ppc64le

```console
$ docker pull haproxy@sha256:d5a1da8f612b8b7bb79e1c462da111fcca84adf2d63955e5656f8c151ca7ad15
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40587797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4392007f5f50e8bc72897aa2e05d25db0685de3a480bd976fc09db92635dbb97`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:26:49 GMT
ADD file:ab87d4854aa8628ce8f4e603c0496499f6f28c3d2525ace782c7369691dafc8c in / 
# Sat, 10 Apr 2021 01:26:56 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 04:45:12 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 04:49:34 GMT
ENV HAPROXY_VERSION=2.3.9
# Sat, 10 Apr 2021 04:49:37 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.9.tar.gz
# Sat, 10 Apr 2021 04:49:42 GMT
ENV HAPROXY_SHA256=77110bc1272bad18fff56b30f4614bcc1deb50600ae42cb0f0b161fc41e2ba96
# Sat, 10 Apr 2021 04:55:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 04:55:04 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 04:55:07 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 04:55:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 04:55:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 04:55:34 GMT
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
	-	`sha256:02dce87e4030362a76d243c695c727400c1fd6e681a33250a0c28bf2959ae752`  
		Last Modified: Sat, 10 Apr 2021 05:10:05 GMT  
		Size: 10.0 MB (10039904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c079ef5cde73a0361b14c8a5f1233d1b99b440f80b935334458e57cf3868804d`  
		Last Modified: Sat, 10 Apr 2021 05:10:03 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27203244b0981a4f3bb61515617544544f43c8b518b565a045b3a3b79db4ce5b`  
		Last Modified: Sat, 10 Apr 2021 05:10:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.9` - linux; s390x

```console
$ docker pull haproxy@sha256:19f3d5d79196611de41352b39a99bdf83b98e44349876ab6cdb27b6e1f35c181
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.0 MB (35044591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ede5f02058145c8565168e90cb541d031baba061a845ef0d1083b665e3277965`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:42:23 GMT
ADD file:dbe2182f8699f2a6011413ea01862e6c0e85853d922dffd72a28d994d23c79bc in / 
# Sat, 10 Apr 2021 00:42:25 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:38:04 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 01:38:49 GMT
ENV HAPROXY_VERSION=2.3.9
# Sat, 10 Apr 2021 01:38:50 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.9.tar.gz
# Sat, 10 Apr 2021 01:38:50 GMT
ENV HAPROXY_SHA256=77110bc1272bad18fff56b30f4614bcc1deb50600ae42cb0f0b161fc41e2ba96
# Sat, 10 Apr 2021 01:39:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 01:39:22 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 01:39:22 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 01:39:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 01:39:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 01:39:23 GMT
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
	-	`sha256:278677bd5845b54d7bbc1e1a92c95b6211358dc62bd96f1fc52ec341df16206d`  
		Last Modified: Sat, 10 Apr 2021 01:42:38 GMT  
		Size: 9.3 MB (9288855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edc908ef823f2540bc02f00eeb071894d56eddaf33d48ff9224cda774e4d54be`  
		Last Modified: Sat, 10 Apr 2021 01:42:37 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a4523549f27c304e4a974a37341a467a3bb7fca15bab56a5a5f97613f7ff9b2`  
		Last Modified: Sat, 10 Apr 2021 01:42:37 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.3.9-alpine`

```console
$ docker pull haproxy@sha256:fd871b2cf0be22d10d148fffe88441167587ea84bad028d4eb81808f28251070
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

### `haproxy:2.3.9-alpine` - linux; amd64

```console
$ docker pull haproxy@sha256:101ee16ec0838ee24f3695ccbd3653b735af22c130d6fd0d7be6d7ac9bc879a4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9499607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:383495f19607c1dd21dce3f33aef722f2c94d10c76eb76dce409928ada65c265`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:37:38 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 21:38:52 GMT
ENV HAPROXY_VERSION=2.3.9
# Wed, 14 Apr 2021 21:38:52 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.9.tar.gz
# Wed, 14 Apr 2021 21:38:52 GMT
ENV HAPROXY_SHA256=77110bc1272bad18fff56b30f4614bcc1deb50600ae42cb0f0b161fc41e2ba96
# Wed, 14 Apr 2021 21:39:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 21:39:42 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 21:39:42 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 21:39:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 21:39:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 21:39:44 GMT
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
	-	`sha256:7b412bb59f5511a4cc66e0b0eb2c0b1781069e37fc9fcda8f4e0908c48d6584f`  
		Last Modified: Wed, 14 Apr 2021 21:43:46 GMT  
		Size: 6.7 MB (6685882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:321129059a3aee4d0de22e7b595549eb049c90428cd1e220ce0f904fc2d70c49`  
		Last Modified: Wed, 14 Apr 2021 21:43:45 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16f8e4cbddc48fe0e653ac776e4d1bd90066ace1e53e95d4f01b3179c7a4914e`  
		Last Modified: Wed, 14 Apr 2021 21:43:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.9-alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:aa7d553fd0c3bc210b6aa068e134a7b95f07577abecdf0f9eb2318d798d93bfc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.2 MB (9209545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5382bb355f68826f4b9ded72ab54cef0217d776f3172303c578a8c80056ce23c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:18:05 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 21:20:51 GMT
ENV HAPROXY_VERSION=2.3.9
# Wed, 14 Apr 2021 21:21:02 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.9.tar.gz
# Wed, 14 Apr 2021 21:21:11 GMT
ENV HAPROXY_SHA256=77110bc1272bad18fff56b30f4614bcc1deb50600ae42cb0f0b161fc41e2ba96
# Wed, 14 Apr 2021 21:22:23 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 21:22:35 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 21:22:51 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 21:23:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 21:23:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 21:23:45 GMT
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
	-	`sha256:5300d7514c3b8d397433442634825547f6a6612e10c46f4ce3dbb4225d5c7720`  
		Last Modified: Wed, 14 Apr 2021 21:34:16 GMT  
		Size: 6.6 MB (6585661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3c323aab13edc8b368334c6d8ad71cec1535117eaeec134595b17088d37937b`  
		Last Modified: Wed, 14 Apr 2021 21:34:15 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e846321291b72a418aa9ccff5106b00fc25129846b6ac70d6cf51fe0374d797`  
		Last Modified: Wed, 14 Apr 2021 21:34:17 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.9-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:75fb3450317233e825f312b8f71b7587d9fd67908e21917728c7a306e6877be5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.9 MB (8926169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acf4585d9e128a18420fdc031947d290650b37b108452804564b0d35e86def6e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:47:58 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 22:49:20 GMT
ENV HAPROXY_VERSION=2.3.9
# Wed, 14 Apr 2021 22:49:29 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.9.tar.gz
# Wed, 14 Apr 2021 22:49:36 GMT
ENV HAPROXY_SHA256=77110bc1272bad18fff56b30f4614bcc1deb50600ae42cb0f0b161fc41e2ba96
# Wed, 14 Apr 2021 22:50:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 22:50:53 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 22:51:05 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 22:51:42 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 22:51:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 22:51:53 GMT
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
	-	`sha256:0b33f8441fa4f8170fcb000f1c6d2614765037bc108661d7ca5e54b529f37010`  
		Last Modified: Wed, 14 Apr 2021 22:56:23 GMT  
		Size: 6.5 MB (6500266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7d61f2b79b5d21794c5d4dcc642a2df4a7c899b2ece6f1a1d7cfc5f4c47496`  
		Last Modified: Wed, 14 Apr 2021 22:56:21 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef906e7aaf5f11781888556cccd267b184bdbecc723469a8747dababde6cae88`  
		Last Modified: Wed, 14 Apr 2021 22:56:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.9-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:4697ab52f31a27418b40afce46493f004c96c3a8b4f5b3234f2ad8fd8b7bb612
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9412142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ad4040f240cdfea6361a98a491df6e7c2e8bd00c8c0f1ea0a9ddde03f43254d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:26:01 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 20:28:04 GMT
ENV HAPROXY_VERSION=2.3.9
# Wed, 14 Apr 2021 20:28:12 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.9.tar.gz
# Wed, 14 Apr 2021 20:28:20 GMT
ENV HAPROXY_SHA256=77110bc1272bad18fff56b30f4614bcc1deb50600ae42cb0f0b161fc41e2ba96
# Wed, 14 Apr 2021 20:29:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 20:29:17 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 20:29:25 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:29:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 20:30:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:30:11 GMT
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
	-	`sha256:6c72b09b2c83b9e5a88d98cf15715a3dfdc984d4837af7d7365a07ea6a3d7866`  
		Last Modified: Wed, 14 Apr 2021 20:38:03 GMT  
		Size: 6.7 MB (6698357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bba2f8c9c125c15cccf5572333f7c53e54f6df343fb7e7cce3177d1331ebc8d8`  
		Last Modified: Wed, 14 Apr 2021 20:38:01 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3057815f353087d9bee55cd953f619dd59c84c2f554ea8058882188f9e4f814`  
		Last Modified: Wed, 14 Apr 2021 20:38:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.9-alpine` - linux; 386

```console
$ docker pull haproxy@sha256:9f99933bbb9fb8a7b3b040bf9b93ce55dde75211224d44c75e3bcd76299e5d7c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9354648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa6e1a1e81c45d3bc98a25c27b58ff451e0d561ea1f95d289ee3cee4b0c35f4a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 01:50:06 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 15 Apr 2021 01:52:21 GMT
ENV HAPROXY_VERSION=2.3.9
# Thu, 15 Apr 2021 01:52:21 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.9.tar.gz
# Thu, 15 Apr 2021 01:52:21 GMT
ENV HAPROXY_SHA256=77110bc1272bad18fff56b30f4614bcc1deb50600ae42cb0f0b161fc41e2ba96
# Thu, 15 Apr 2021 01:53:27 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 15 Apr 2021 01:53:27 GMT
STOPSIGNAL SIGUSR1
# Thu, 15 Apr 2021 01:53:27 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 15 Apr 2021 01:53:28 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 15 Apr 2021 01:53:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Apr 2021 01:53:29 GMT
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
	-	`sha256:ca59b31cb2383b0cecb9a081d46bc5cb55ff05176d7da51344504b99f485b37c`  
		Last Modified: Thu, 15 Apr 2021 02:00:45 GMT  
		Size: 6.5 MB (6533992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43d9fdba60ae084cf195a2fc170f0358d1eb329ec60f7e3d78f39e3bd42c0599`  
		Last Modified: Thu, 15 Apr 2021 02:00:44 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a98584752f736ec3c38550ffb5a53f52be250c0c3b5b5d2d3cb60d2b08f0fa31`  
		Last Modified: Thu, 15 Apr 2021 02:00:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.9-alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:19dc93de5c25a5e87c31214ba644e2d889de9b3834a4f13762711529b7d12a8f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.8 MB (9832346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb9dac528b8dbf1a3a08aeeb1ac86db8bbef3c78e14cbcd1229183af17c6bb12`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:25:09 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 23:26:45 GMT
ENV HAPROXY_VERSION=2.3.9
# Wed, 14 Apr 2021 23:26:47 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.9.tar.gz
# Wed, 14 Apr 2021 23:26:51 GMT
ENV HAPROXY_SHA256=77110bc1272bad18fff56b30f4614bcc1deb50600ae42cb0f0b161fc41e2ba96
# Wed, 14 Apr 2021 23:28:14 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 23:28:20 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 23:28:27 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 23:28:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 23:28:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 23:28:56 GMT
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
	-	`sha256:55517a2814e2dbb00eb7d44f417b8729aa436b00a32a084c238b7d5733011cb2`  
		Last Modified: Wed, 14 Apr 2021 23:36:51 GMT  
		Size: 7.0 MB (7017449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e5587a8b18c5eac4421c6e6dcf2bd5b8aa86e1cc461dd1608c57f7d8208359`  
		Last Modified: Wed, 14 Apr 2021 23:36:50 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e0e401a50336fe2abb496fdd8bae8c8a08a451470c41b530499798a6e9a14f2`  
		Last Modified: Wed, 14 Apr 2021 23:36:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.9-alpine` - linux; s390x

```console
$ docker pull haproxy@sha256:5736a38ee6dd2b1a7821b37847aae240638a52c8bac5062883d90fca886909b3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9257346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25cf086b4e421310119b91b6fe47633d277b498487de5549fb997acd6a25cb0f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:54:24 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 20:55:17 GMT
ENV HAPROXY_VERSION=2.3.9
# Wed, 14 Apr 2021 20:55:17 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.9.tar.gz
# Wed, 14 Apr 2021 20:55:18 GMT
ENV HAPROXY_SHA256=77110bc1272bad18fff56b30f4614bcc1deb50600ae42cb0f0b161fc41e2ba96
# Wed, 14 Apr 2021 20:55:58 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 20:55:59 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 20:55:59 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:56:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 20:56:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:56:00 GMT
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
	-	`sha256:ae9e557ff45057778dffe5c56dc419e35c7d970db8ce611466c9b0d09a048305`  
		Last Modified: Wed, 14 Apr 2021 20:59:18 GMT  
		Size: 6.7 MB (6652940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb69cd1d8680cdc862b3d406dbc637a101625886f943068bf0dd5647f78353df`  
		Last Modified: Wed, 14 Apr 2021 20:59:17 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8270e1f8a61ff9eb8008cffc9b5ae5fb3a982db994eaa84d2653ef71236dec1e`  
		Last Modified: Wed, 14 Apr 2021 20:59:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.4-dev`

```console
$ docker pull haproxy@sha256:31538fa9a2c710d01115e3c043b6d67414b6cdfa0d15838e090c69790bfc7b9c
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
$ docker pull haproxy@sha256:c06dc3e4b18005af98ae5001d1f6455dcd99bec14ca662ab3978d8354390b0b3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37360258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50b1451a5fe02fcf6674beb6d2f1e5102e9e9c6fd33f8d41490193e5be4e1c76`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:29:42 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 06:29:42 GMT
ENV HAPROXY_VERSION=2.4-dev16
# Sat, 10 Apr 2021 06:29:42 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev16.tar.gz
# Sat, 10 Apr 2021 06:29:43 GMT
ENV HAPROXY_SHA256=7ba831c977ce80e26ed3ae6ecbc54c1ff3e8a313118b47b9d877ef44ad17cdf0
# Sat, 10 Apr 2021 06:31:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 06:31:13 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 06:31:13 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 06:31:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 06:31:14 GMT
USER haproxy
# Sat, 10 Apr 2021 06:31:14 GMT
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
	-	`sha256:4851fc3b703004b1674c69bba9e9d684d47a8e387cc60e6a875e51d229b62052`  
		Last Modified: Sat, 10 Apr 2021 06:38:09 GMT  
		Size: 10.2 MB (10219056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5f542a973eda6eb47b92d0def149ac2b898bbf426f952f56170266ba892feab`  
		Last Modified: Sat, 10 Apr 2021 06:38:07 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:d59fd08bf2901697ed902b4276a1c3ed3b66c79734c30b4459e388fe7448d4d0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34693208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6d45684ff520e48007a8ebc41ee3282de24a54c9d01830ff440a0c68f1bf3af`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:51:31 GMT
ADD file:926533a23a69aa2481a9122b667bb6300a347154eea366c9e679a230aa7f373a in / 
# Sat, 10 Apr 2021 00:51:34 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 02:24:17 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 02:24:21 GMT
ENV HAPROXY_VERSION=2.4-dev16
# Sat, 10 Apr 2021 02:24:24 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev16.tar.gz
# Sat, 10 Apr 2021 02:24:24 GMT
ENV HAPROXY_SHA256=7ba831c977ce80e26ed3ae6ecbc54c1ff3e8a313118b47b9d877ef44ad17cdf0
# Sat, 10 Apr 2021 02:25:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 02:25:26 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 02:25:32 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 02:25:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 02:25:40 GMT
USER haproxy
# Sat, 10 Apr 2021 02:25:43 GMT
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
	-	`sha256:bc8597b90427d715e2250e3eaf9061f2f08dee4c8d25ef9b7d7a3b1fd157ce25`  
		Last Modified: Sat, 10 Apr 2021 02:36:58 GMT  
		Size: 9.8 MB (9818179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce35c707bfa27a1e142e0d458908cee0e5214428f4c7717b252fa69ab908a71`  
		Last Modified: Sat, 10 Apr 2021 02:36:54 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:c61347eb45e7339cb227b7ecdad17988afdb8de9380d51c3ab7e0b5bf94612bb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.4 MB (32418585 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f3e5441c5136af1a3601708ac8a1e74efbcffca951cc1f7fac15d49ff95118c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:59:45 GMT
ADD file:3fbd246a2de82566bcaaf62e3e0bf57175a7ad46b4156366a110661b31eab240 in / 
# Sat, 10 Apr 2021 00:59:47 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 08:58:51 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 08:58:52 GMT
ENV HAPROXY_VERSION=2.4-dev16
# Sat, 10 Apr 2021 08:58:52 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev16.tar.gz
# Sat, 10 Apr 2021 08:58:53 GMT
ENV HAPROXY_SHA256=7ba831c977ce80e26ed3ae6ecbc54c1ff3e8a313118b47b9d877ef44ad17cdf0
# Sat, 10 Apr 2021 08:59:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 08:59:33 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 08:59:34 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 08:59:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 08:59:35 GMT
USER haproxy
# Sat, 10 Apr 2021 08:59:36 GMT
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
	-	`sha256:e08ad02f759f5d6082e4886cd0955a0d3c1a249830912ec6cbcac60c5e7aa585`  
		Last Modified: Sat, 10 Apr 2021 09:05:29 GMT  
		Size: 9.7 MB (9676958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdcc567b7402bdeaa6b70b3dd089dbef935dcd6520af155f4fec35792ed4cb51`  
		Last Modified: Sat, 10 Apr 2021 09:05:26 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:ff0973381ad6819a381330b2e16f6e5dfbc27b316f5bb3727a91bbd5208bd39c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.0 MB (36003377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf6c6618f420e296182e5ea02735549bc15f734e82d4f41db6ebf7a619a3c486`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:41:25 GMT
ADD file:b24da7eb23eeae04e00d0e45da29a89fe8f992e8dcf4ba482afb907b8015b7bf in / 
# Sat, 10 Apr 2021 00:41:28 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:13:29 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 01:13:30 GMT
ENV HAPROXY_VERSION=2.4-dev16
# Sat, 10 Apr 2021 01:13:31 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev16.tar.gz
# Sat, 10 Apr 2021 01:13:32 GMT
ENV HAPROXY_SHA256=7ba831c977ce80e26ed3ae6ecbc54c1ff3e8a313118b47b9d877ef44ad17cdf0
# Sat, 10 Apr 2021 01:14:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 01:14:21 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 01:14:22 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 01:14:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 01:14:24 GMT
USER haproxy
# Sat, 10 Apr 2021 01:14:25 GMT
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
	-	`sha256:5c361fc99d2c93406f8aa7627632703471ac3a7bc2c54b1903d00d80215400d7`  
		Last Modified: Sat, 10 Apr 2021 01:21:30 GMT  
		Size: 10.1 MB (10096968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79eea317fef2fa2afa973ccf16aefc64e0901ebcb75262eb55dde21339d891a`  
		Last Modified: Sat, 10 Apr 2021 01:21:31 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev` - linux; 386

```console
$ docker pull haproxy@sha256:6eb21f57d4eda9b1fa0d0e09098b535f88396f1c4f6e28379b65ec98be39858c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.8 MB (37849981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ec40a07ba7c83f02b0944b70386e0dd4b00af8711a0bf30e56507c2f209595b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:39:42 GMT
ADD file:8885d4d13678543780bb04ba14b621179665f7951d5b261036a7092df9b376e7 in / 
# Sat, 10 Apr 2021 00:39:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 03:48:12 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 03:48:13 GMT
ENV HAPROXY_VERSION=2.4-dev16
# Sat, 10 Apr 2021 03:48:13 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev16.tar.gz
# Sat, 10 Apr 2021 03:48:13 GMT
ENV HAPROXY_SHA256=7ba831c977ce80e26ed3ae6ecbc54c1ff3e8a313118b47b9d877ef44ad17cdf0
# Sat, 10 Apr 2021 03:49:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 03:49:26 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 03:49:26 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 03:49:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 03:49:26 GMT
USER haproxy
# Sat, 10 Apr 2021 03:49:27 GMT
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
	-	`sha256:d7e696ab13e0efd7a59646dd45571abd224b808deaebef87daf88186f9371470`  
		Last Modified: Sat, 10 Apr 2021 03:59:11 GMT  
		Size: 10.1 MB (10059167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1eafb921bf057f9e11c4ff6865e5d611f0df6ded208c5b0c988aeb6d5fdde8b`  
		Last Modified: Sat, 10 Apr 2021 03:59:08 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev` - linux; mips64le

```console
$ docker pull haproxy@sha256:2a7f5c3bacd7aec1b5d57d62b25f1dde7c380c6ff78d8aa413b5c047f8c61172
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.6 MB (35605574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f799ae3904dbd43259c1a50f27a2dbeea80c7020665d8a2755505db94fea90d3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:09:40 GMT
ADD file:0c93801c4a3719dfd4c047d7f2f4d52bf463eba2ab875da1dc54dcc832aae20b in / 
# Sat, 10 Apr 2021 01:09:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:39:36 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 01:39:37 GMT
ENV HAPROXY_VERSION=2.4-dev16
# Sat, 10 Apr 2021 01:39:37 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev16.tar.gz
# Sat, 10 Apr 2021 01:39:37 GMT
ENV HAPROXY_SHA256=7ba831c977ce80e26ed3ae6ecbc54c1ff3e8a313118b47b9d877ef44ad17cdf0
# Sat, 10 Apr 2021 01:42:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 01:42:08 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 01:42:09 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 01:42:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 01:42:09 GMT
USER haproxy
# Sat, 10 Apr 2021 01:42:10 GMT
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
	-	`sha256:b36338308a42593db2c49ebb9cfbbd52ab89cd23d3962569b63f5d48fb11ec5a`  
		Last Modified: Sat, 10 Apr 2021 01:53:47 GMT  
		Size: 9.8 MB (9797334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79de5c7178f07f79ec989b9e317f27781ea95a3f9c68c3c9f382720e91164cac`  
		Last Modified: Sat, 10 Apr 2021 01:53:40 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev` - linux; ppc64le

```console
$ docker pull haproxy@sha256:b7689f673f26a006976887e349468d8281adccf6badb9f80cfe271c50352526d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41266534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82b2dbb36ae6bffe4d4dff694d7a0d82921c031590494ecd6e7fce28470c4c7a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:26:49 GMT
ADD file:ab87d4854aa8628ce8f4e603c0496499f6f28c3d2525ace782c7369691dafc8c in / 
# Sat, 10 Apr 2021 01:26:56 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 04:45:12 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 04:45:22 GMT
ENV HAPROXY_VERSION=2.4-dev16
# Sat, 10 Apr 2021 04:45:28 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev16.tar.gz
# Sat, 10 Apr 2021 04:45:35 GMT
ENV HAPROXY_SHA256=7ba831c977ce80e26ed3ae6ecbc54c1ff3e8a313118b47b9d877ef44ad17cdf0
# Sat, 10 Apr 2021 04:49:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 04:49:08 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 04:49:09 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 04:49:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 04:49:15 GMT
USER haproxy
# Sat, 10 Apr 2021 04:49:21 GMT
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
	-	`sha256:135c577abcf78f17ad5860a095b0b73ba6e454a7d739b8bdbceb6105836517d2`  
		Last Modified: Sat, 10 Apr 2021 05:09:53 GMT  
		Size: 10.7 MB (10718763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19076facb83cd399731c39456ef4df4df5c5ce9d216b5148cd84b318fa67fc81`  
		Last Modified: Sat, 10 Apr 2021 05:09:50 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev` - linux; s390x

```console
$ docker pull haproxy@sha256:a0e91e994f98d7a214ff66b13cb3d45bf32ae902ca295201af0394efba40b116
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.7 MB (35663637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7485c1a5a390c030a09e964e53427571722616978f464a41057fde390caa3db7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:42:23 GMT
ADD file:dbe2182f8699f2a6011413ea01862e6c0e85853d922dffd72a28d994d23c79bc in / 
# Sat, 10 Apr 2021 00:42:25 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:38:04 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 01:38:04 GMT
ENV HAPROXY_VERSION=2.4-dev16
# Sat, 10 Apr 2021 01:38:04 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev16.tar.gz
# Sat, 10 Apr 2021 01:38:04 GMT
ENV HAPROXY_SHA256=7ba831c977ce80e26ed3ae6ecbc54c1ff3e8a313118b47b9d877ef44ad17cdf0
# Sat, 10 Apr 2021 01:38:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 01:38:37 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 01:38:37 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 01:38:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 01:38:37 GMT
USER haproxy
# Sat, 10 Apr 2021 01:38:37 GMT
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
	-	`sha256:7886be80180d1c30e0b927bfd36e821582764b3e226074b885ce3491721b702f`  
		Last Modified: Sat, 10 Apr 2021 01:42:30 GMT  
		Size: 9.9 MB (9908022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01f023f3e768539d181dd6443c0ec010ddcf5e44fd2d8bc4ab43004f28e0a184`  
		Last Modified: Sat, 10 Apr 2021 01:42:28 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.4-dev-alpine`

```console
$ docker pull haproxy@sha256:2c5caef0d111c4dd4e6b373328bdf6c1cb2e72f1ffeb02aaaed9733d2742f7ea
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
$ docker pull haproxy@sha256:aec8e4caa2a29cbbe6f3e33e025577df91e379f415b345844eae31e3bca0d7be
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.2 MB (10204306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe4434f52cf91ad6d772e7d40c865c8ee40c2886376dea4d5443a5766a9be3b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:37:38 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 21:37:38 GMT
ENV HAPROXY_VERSION=2.4-dev16
# Wed, 14 Apr 2021 21:37:39 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev16.tar.gz
# Wed, 14 Apr 2021 21:37:39 GMT
ENV HAPROXY_SHA256=7ba831c977ce80e26ed3ae6ecbc54c1ff3e8a313118b47b9d877ef44ad17cdf0
# Wed, 14 Apr 2021 21:38:36 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 21:38:36 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 21:38:36 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 21:38:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 21:38:36 GMT
USER haproxy
# Wed, 14 Apr 2021 21:38:37 GMT
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
	-	`sha256:3ee28b0bae8285ca092a988758ec192886e7a4722eed2760fcd84e1437f78ad9`  
		Last Modified: Wed, 14 Apr 2021 21:43:31 GMT  
		Size: 7.4 MB (7390702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b9fefc276d9a2075ce3c51e7e72d7c9753b34c5d50ee4fceec4991b67a3217`  
		Last Modified: Wed, 14 Apr 2021 21:43:30 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev-alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:18c99b0294acf4a444a344d4c476be34518c138a574c250c7c8750d76cc06597
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9734849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52252a1f5ee12456e41ec6a35ee091bbb9f2d7a0311adfe006f8bfceb0d6a31d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:18:05 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 21:18:07 GMT
ENV HAPROXY_VERSION=2.4-dev16
# Wed, 14 Apr 2021 21:18:14 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev16.tar.gz
# Wed, 14 Apr 2021 21:18:20 GMT
ENV HAPROXY_SHA256=7ba831c977ce80e26ed3ae6ecbc54c1ff3e8a313118b47b9d877ef44ad17cdf0
# Wed, 14 Apr 2021 21:19:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 21:19:47 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 21:20:03 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 21:20:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 21:20:18 GMT
USER haproxy
# Wed, 14 Apr 2021 21:20:25 GMT
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
	-	`sha256:ddb60d9983255b54cb38cb0a251c53b66d2bb77cbea2b33d932954b8be43ab1a`  
		Last Modified: Wed, 14 Apr 2021 21:34:03 GMT  
		Size: 7.1 MB (7111083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83cd0fbccc760a62c97c0b23be21404c7581354f10644f351949349da37c616`  
		Last Modified: Wed, 14 Apr 2021 21:34:00 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:4971a69893cf77341cfb9ec10c142b73cf01d09365e482f5a887e4b56bdf7e7f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9461751 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef6f640418384b5e32ce71e244b71fd543d6a7bd39de9bb8853cb0c3dc8a6eca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:47:58 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 22:47:59 GMT
ENV HAPROXY_VERSION=2.4-dev16
# Wed, 14 Apr 2021 22:48:00 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev16.tar.gz
# Wed, 14 Apr 2021 22:48:01 GMT
ENV HAPROXY_SHA256=7ba831c977ce80e26ed3ae6ecbc54c1ff3e8a313118b47b9d877ef44ad17cdf0
# Wed, 14 Apr 2021 22:48:41 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 22:48:47 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 22:48:48 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 22:48:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 22:48:50 GMT
USER haproxy
# Wed, 14 Apr 2021 22:48:51 GMT
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
	-	`sha256:936542e31ad7c9777cdafccccf5ce7a555aa454fed069d6f2ae79991d79f75b0`  
		Last Modified: Wed, 14 Apr 2021 22:56:11 GMT  
		Size: 7.0 MB (7035971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2a6563452e5781204324a0e0d804848ebe45a55cefb87e605dc3da9c3fc2c21`  
		Last Modified: Wed, 14 Apr 2021 22:56:09 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:c245fdeaaa47cc7630d6b769ac549207537b86dc3a1768892d5276c73a489f03
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (10011014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28d03fd763573258ff5390ca0e0ebf6f62cf30f50bae999580a666eee34e4279`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:26:01 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 20:26:09 GMT
ENV HAPROXY_VERSION=2.4-dev16
# Wed, 14 Apr 2021 20:26:16 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev16.tar.gz
# Wed, 14 Apr 2021 20:26:20 GMT
ENV HAPROXY_SHA256=7ba831c977ce80e26ed3ae6ecbc54c1ff3e8a313118b47b9d877ef44ad17cdf0
# Wed, 14 Apr 2021 20:26:59 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 20:27:06 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 20:27:12 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:27:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:27:25 GMT
USER haproxy
# Wed, 14 Apr 2021 20:27:29 GMT
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
	-	`sha256:c8ed3510eee22484c704a65f38d771d2d6965b046a61cd8490f48d7b789dc13a`  
		Last Modified: Wed, 14 Apr 2021 20:37:52 GMT  
		Size: 7.3 MB (7297348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870fcebc0a3df6042739c38db9b595f4a112ef62133cb18903e6254dc8525678`  
		Last Modified: Wed, 14 Apr 2021 20:37:50 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev-alpine` - linux; 386

```console
$ docker pull haproxy@sha256:f2865df25e682e69fa363d071fc584109a0efbff3712ed086675bc9a4d264aa2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9895508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45a25268a3320d5e276686b082b5307e048869035cb85d50a7016996016f97c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 01:50:06 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 15 Apr 2021 01:50:07 GMT
ENV HAPROXY_VERSION=2.4-dev16
# Thu, 15 Apr 2021 01:50:07 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev16.tar.gz
# Thu, 15 Apr 2021 01:50:07 GMT
ENV HAPROXY_SHA256=7ba831c977ce80e26ed3ae6ecbc54c1ff3e8a313118b47b9d877ef44ad17cdf0
# Thu, 15 Apr 2021 01:52:00 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 15 Apr 2021 01:52:00 GMT
STOPSIGNAL SIGUSR1
# Thu, 15 Apr 2021 01:52:00 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 15 Apr 2021 01:52:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Apr 2021 01:52:01 GMT
USER haproxy
# Thu, 15 Apr 2021 01:52:01 GMT
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
	-	`sha256:0732fbf011caf16c89352454dd21428c5ceef223d490e25a91ca458af0f4cc7e`  
		Last Modified: Thu, 15 Apr 2021 02:00:30 GMT  
		Size: 7.1 MB (7074972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0f2f874bc081911a85b4042df452e69d8cd4dbf1217eee78c9e197438756c2`  
		Last Modified: Thu, 15 Apr 2021 02:00:28 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev-alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:3ccbaaeabac23dc6cfd593703a14f976b7056ffa2313a60712737ad25b3e89e3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.4 MB (10412354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:720292a6554d6bf06fde693ce1c84752350c59fdb23f5c405869f68c6a086190`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:25:09 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 23:25:12 GMT
ENV HAPROXY_VERSION=2.4-dev16
# Wed, 14 Apr 2021 23:25:14 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev16.tar.gz
# Wed, 14 Apr 2021 23:25:15 GMT
ENV HAPROXY_SHA256=7ba831c977ce80e26ed3ae6ecbc54c1ff3e8a313118b47b9d877ef44ad17cdf0
# Wed, 14 Apr 2021 23:26:00 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 23:26:03 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 23:26:07 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 23:26:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 23:26:20 GMT
USER haproxy
# Wed, 14 Apr 2021 23:26:23 GMT
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
	-	`sha256:f8cf06ac8d3b30db55bccd6e3e9a52b654d32699c288c9f8609f5da3f0de9b3f`  
		Last Modified: Wed, 14 Apr 2021 23:36:38 GMT  
		Size: 7.6 MB (7597577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2a8135ce5553616628e564a4aa023c4cbf621914eb9f4da05275bdc022194ba`  
		Last Modified: Wed, 14 Apr 2021 23:36:36 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev-alpine` - linux; s390x

```console
$ docker pull haproxy@sha256:190d5debc6f053ebdd1132223f15357de8fa8265ca6dbe140c116e25c6403253
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.8 MB (9773567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f5408cec121f5ad32c2b0887e1033653577a0a9490825df6bfacdf2bdf4ca89`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:54:24 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 20:54:24 GMT
ENV HAPROXY_VERSION=2.4-dev16
# Wed, 14 Apr 2021 20:54:24 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev16.tar.gz
# Wed, 14 Apr 2021 20:54:24 GMT
ENV HAPROXY_SHA256=7ba831c977ce80e26ed3ae6ecbc54c1ff3e8a313118b47b9d877ef44ad17cdf0
# Wed, 14 Apr 2021 20:55:03 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 20:55:04 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 20:55:04 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:55:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:55:05 GMT
USER haproxy
# Wed, 14 Apr 2021 20:55:05 GMT
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
	-	`sha256:fa0a88436cf32707688ce587a072715e090f00fafffb8c4ac2d928094a85e90b`  
		Last Modified: Wed, 14 Apr 2021 20:59:07 GMT  
		Size: 7.2 MB (7169284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd015e23ad1b5309f4ecccd6b627b5d57330dab0d488cba19cd2f33712d6ad0`  
		Last Modified: Wed, 14 Apr 2021 20:59:06 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.4-dev16`

```console
$ docker pull haproxy@sha256:31538fa9a2c710d01115e3c043b6d67414b6cdfa0d15838e090c69790bfc7b9c
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

### `haproxy:2.4-dev16` - linux; amd64

```console
$ docker pull haproxy@sha256:c06dc3e4b18005af98ae5001d1f6455dcd99bec14ca662ab3978d8354390b0b3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37360258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50b1451a5fe02fcf6674beb6d2f1e5102e9e9c6fd33f8d41490193e5be4e1c76`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:29:42 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 06:29:42 GMT
ENV HAPROXY_VERSION=2.4-dev16
# Sat, 10 Apr 2021 06:29:42 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev16.tar.gz
# Sat, 10 Apr 2021 06:29:43 GMT
ENV HAPROXY_SHA256=7ba831c977ce80e26ed3ae6ecbc54c1ff3e8a313118b47b9d877ef44ad17cdf0
# Sat, 10 Apr 2021 06:31:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 06:31:13 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 06:31:13 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 06:31:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 06:31:14 GMT
USER haproxy
# Sat, 10 Apr 2021 06:31:14 GMT
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
	-	`sha256:4851fc3b703004b1674c69bba9e9d684d47a8e387cc60e6a875e51d229b62052`  
		Last Modified: Sat, 10 Apr 2021 06:38:09 GMT  
		Size: 10.2 MB (10219056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5f542a973eda6eb47b92d0def149ac2b898bbf426f952f56170266ba892feab`  
		Last Modified: Sat, 10 Apr 2021 06:38:07 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev16` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:d59fd08bf2901697ed902b4276a1c3ed3b66c79734c30b4459e388fe7448d4d0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34693208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6d45684ff520e48007a8ebc41ee3282de24a54c9d01830ff440a0c68f1bf3af`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:51:31 GMT
ADD file:926533a23a69aa2481a9122b667bb6300a347154eea366c9e679a230aa7f373a in / 
# Sat, 10 Apr 2021 00:51:34 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 02:24:17 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 02:24:21 GMT
ENV HAPROXY_VERSION=2.4-dev16
# Sat, 10 Apr 2021 02:24:24 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev16.tar.gz
# Sat, 10 Apr 2021 02:24:24 GMT
ENV HAPROXY_SHA256=7ba831c977ce80e26ed3ae6ecbc54c1ff3e8a313118b47b9d877ef44ad17cdf0
# Sat, 10 Apr 2021 02:25:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 02:25:26 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 02:25:32 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 02:25:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 02:25:40 GMT
USER haproxy
# Sat, 10 Apr 2021 02:25:43 GMT
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
	-	`sha256:bc8597b90427d715e2250e3eaf9061f2f08dee4c8d25ef9b7d7a3b1fd157ce25`  
		Last Modified: Sat, 10 Apr 2021 02:36:58 GMT  
		Size: 9.8 MB (9818179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce35c707bfa27a1e142e0d458908cee0e5214428f4c7717b252fa69ab908a71`  
		Last Modified: Sat, 10 Apr 2021 02:36:54 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev16` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:c61347eb45e7339cb227b7ecdad17988afdb8de9380d51c3ab7e0b5bf94612bb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.4 MB (32418585 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f3e5441c5136af1a3601708ac8a1e74efbcffca951cc1f7fac15d49ff95118c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:59:45 GMT
ADD file:3fbd246a2de82566bcaaf62e3e0bf57175a7ad46b4156366a110661b31eab240 in / 
# Sat, 10 Apr 2021 00:59:47 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 08:58:51 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 08:58:52 GMT
ENV HAPROXY_VERSION=2.4-dev16
# Sat, 10 Apr 2021 08:58:52 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev16.tar.gz
# Sat, 10 Apr 2021 08:58:53 GMT
ENV HAPROXY_SHA256=7ba831c977ce80e26ed3ae6ecbc54c1ff3e8a313118b47b9d877ef44ad17cdf0
# Sat, 10 Apr 2021 08:59:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 08:59:33 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 08:59:34 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 08:59:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 08:59:35 GMT
USER haproxy
# Sat, 10 Apr 2021 08:59:36 GMT
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
	-	`sha256:e08ad02f759f5d6082e4886cd0955a0d3c1a249830912ec6cbcac60c5e7aa585`  
		Last Modified: Sat, 10 Apr 2021 09:05:29 GMT  
		Size: 9.7 MB (9676958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdcc567b7402bdeaa6b70b3dd089dbef935dcd6520af155f4fec35792ed4cb51`  
		Last Modified: Sat, 10 Apr 2021 09:05:26 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev16` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:ff0973381ad6819a381330b2e16f6e5dfbc27b316f5bb3727a91bbd5208bd39c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.0 MB (36003377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf6c6618f420e296182e5ea02735549bc15f734e82d4f41db6ebf7a619a3c486`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:41:25 GMT
ADD file:b24da7eb23eeae04e00d0e45da29a89fe8f992e8dcf4ba482afb907b8015b7bf in / 
# Sat, 10 Apr 2021 00:41:28 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:13:29 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 01:13:30 GMT
ENV HAPROXY_VERSION=2.4-dev16
# Sat, 10 Apr 2021 01:13:31 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev16.tar.gz
# Sat, 10 Apr 2021 01:13:32 GMT
ENV HAPROXY_SHA256=7ba831c977ce80e26ed3ae6ecbc54c1ff3e8a313118b47b9d877ef44ad17cdf0
# Sat, 10 Apr 2021 01:14:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 01:14:21 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 01:14:22 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 01:14:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 01:14:24 GMT
USER haproxy
# Sat, 10 Apr 2021 01:14:25 GMT
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
	-	`sha256:5c361fc99d2c93406f8aa7627632703471ac3a7bc2c54b1903d00d80215400d7`  
		Last Modified: Sat, 10 Apr 2021 01:21:30 GMT  
		Size: 10.1 MB (10096968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79eea317fef2fa2afa973ccf16aefc64e0901ebcb75262eb55dde21339d891a`  
		Last Modified: Sat, 10 Apr 2021 01:21:31 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev16` - linux; 386

```console
$ docker pull haproxy@sha256:6eb21f57d4eda9b1fa0d0e09098b535f88396f1c4f6e28379b65ec98be39858c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.8 MB (37849981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ec40a07ba7c83f02b0944b70386e0dd4b00af8711a0bf30e56507c2f209595b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:39:42 GMT
ADD file:8885d4d13678543780bb04ba14b621179665f7951d5b261036a7092df9b376e7 in / 
# Sat, 10 Apr 2021 00:39:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 03:48:12 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 03:48:13 GMT
ENV HAPROXY_VERSION=2.4-dev16
# Sat, 10 Apr 2021 03:48:13 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev16.tar.gz
# Sat, 10 Apr 2021 03:48:13 GMT
ENV HAPROXY_SHA256=7ba831c977ce80e26ed3ae6ecbc54c1ff3e8a313118b47b9d877ef44ad17cdf0
# Sat, 10 Apr 2021 03:49:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 03:49:26 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 03:49:26 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 03:49:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 03:49:26 GMT
USER haproxy
# Sat, 10 Apr 2021 03:49:27 GMT
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
	-	`sha256:d7e696ab13e0efd7a59646dd45571abd224b808deaebef87daf88186f9371470`  
		Last Modified: Sat, 10 Apr 2021 03:59:11 GMT  
		Size: 10.1 MB (10059167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1eafb921bf057f9e11c4ff6865e5d611f0df6ded208c5b0c988aeb6d5fdde8b`  
		Last Modified: Sat, 10 Apr 2021 03:59:08 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev16` - linux; mips64le

```console
$ docker pull haproxy@sha256:2a7f5c3bacd7aec1b5d57d62b25f1dde7c380c6ff78d8aa413b5c047f8c61172
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.6 MB (35605574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f799ae3904dbd43259c1a50f27a2dbeea80c7020665d8a2755505db94fea90d3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:09:40 GMT
ADD file:0c93801c4a3719dfd4c047d7f2f4d52bf463eba2ab875da1dc54dcc832aae20b in / 
# Sat, 10 Apr 2021 01:09:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:39:36 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 01:39:37 GMT
ENV HAPROXY_VERSION=2.4-dev16
# Sat, 10 Apr 2021 01:39:37 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev16.tar.gz
# Sat, 10 Apr 2021 01:39:37 GMT
ENV HAPROXY_SHA256=7ba831c977ce80e26ed3ae6ecbc54c1ff3e8a313118b47b9d877ef44ad17cdf0
# Sat, 10 Apr 2021 01:42:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 01:42:08 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 01:42:09 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 01:42:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 01:42:09 GMT
USER haproxy
# Sat, 10 Apr 2021 01:42:10 GMT
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
	-	`sha256:b36338308a42593db2c49ebb9cfbbd52ab89cd23d3962569b63f5d48fb11ec5a`  
		Last Modified: Sat, 10 Apr 2021 01:53:47 GMT  
		Size: 9.8 MB (9797334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79de5c7178f07f79ec989b9e317f27781ea95a3f9c68c3c9f382720e91164cac`  
		Last Modified: Sat, 10 Apr 2021 01:53:40 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev16` - linux; ppc64le

```console
$ docker pull haproxy@sha256:b7689f673f26a006976887e349468d8281adccf6badb9f80cfe271c50352526d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41266534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82b2dbb36ae6bffe4d4dff694d7a0d82921c031590494ecd6e7fce28470c4c7a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:26:49 GMT
ADD file:ab87d4854aa8628ce8f4e603c0496499f6f28c3d2525ace782c7369691dafc8c in / 
# Sat, 10 Apr 2021 01:26:56 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 04:45:12 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 04:45:22 GMT
ENV HAPROXY_VERSION=2.4-dev16
# Sat, 10 Apr 2021 04:45:28 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev16.tar.gz
# Sat, 10 Apr 2021 04:45:35 GMT
ENV HAPROXY_SHA256=7ba831c977ce80e26ed3ae6ecbc54c1ff3e8a313118b47b9d877ef44ad17cdf0
# Sat, 10 Apr 2021 04:49:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 04:49:08 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 04:49:09 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 04:49:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 04:49:15 GMT
USER haproxy
# Sat, 10 Apr 2021 04:49:21 GMT
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
	-	`sha256:135c577abcf78f17ad5860a095b0b73ba6e454a7d739b8bdbceb6105836517d2`  
		Last Modified: Sat, 10 Apr 2021 05:09:53 GMT  
		Size: 10.7 MB (10718763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19076facb83cd399731c39456ef4df4df5c5ce9d216b5148cd84b318fa67fc81`  
		Last Modified: Sat, 10 Apr 2021 05:09:50 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev16` - linux; s390x

```console
$ docker pull haproxy@sha256:a0e91e994f98d7a214ff66b13cb3d45bf32ae902ca295201af0394efba40b116
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.7 MB (35663637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7485c1a5a390c030a09e964e53427571722616978f464a41057fde390caa3db7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:42:23 GMT
ADD file:dbe2182f8699f2a6011413ea01862e6c0e85853d922dffd72a28d994d23c79bc in / 
# Sat, 10 Apr 2021 00:42:25 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:38:04 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 01:38:04 GMT
ENV HAPROXY_VERSION=2.4-dev16
# Sat, 10 Apr 2021 01:38:04 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev16.tar.gz
# Sat, 10 Apr 2021 01:38:04 GMT
ENV HAPROXY_SHA256=7ba831c977ce80e26ed3ae6ecbc54c1ff3e8a313118b47b9d877ef44ad17cdf0
# Sat, 10 Apr 2021 01:38:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 01:38:37 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 01:38:37 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 01:38:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 01:38:37 GMT
USER haproxy
# Sat, 10 Apr 2021 01:38:37 GMT
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
	-	`sha256:7886be80180d1c30e0b927bfd36e821582764b3e226074b885ce3491721b702f`  
		Last Modified: Sat, 10 Apr 2021 01:42:30 GMT  
		Size: 9.9 MB (9908022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01f023f3e768539d181dd6443c0ec010ddcf5e44fd2d8bc4ab43004f28e0a184`  
		Last Modified: Sat, 10 Apr 2021 01:42:28 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.4-dev16-alpine`

```console
$ docker pull haproxy@sha256:2c5caef0d111c4dd4e6b373328bdf6c1cb2e72f1ffeb02aaaed9733d2742f7ea
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

### `haproxy:2.4-dev16-alpine` - linux; amd64

```console
$ docker pull haproxy@sha256:aec8e4caa2a29cbbe6f3e33e025577df91e379f415b345844eae31e3bca0d7be
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.2 MB (10204306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe4434f52cf91ad6d772e7d40c865c8ee40c2886376dea4d5443a5766a9be3b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:37:38 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 21:37:38 GMT
ENV HAPROXY_VERSION=2.4-dev16
# Wed, 14 Apr 2021 21:37:39 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev16.tar.gz
# Wed, 14 Apr 2021 21:37:39 GMT
ENV HAPROXY_SHA256=7ba831c977ce80e26ed3ae6ecbc54c1ff3e8a313118b47b9d877ef44ad17cdf0
# Wed, 14 Apr 2021 21:38:36 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 21:38:36 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 21:38:36 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 21:38:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 21:38:36 GMT
USER haproxy
# Wed, 14 Apr 2021 21:38:37 GMT
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
	-	`sha256:3ee28b0bae8285ca092a988758ec192886e7a4722eed2760fcd84e1437f78ad9`  
		Last Modified: Wed, 14 Apr 2021 21:43:31 GMT  
		Size: 7.4 MB (7390702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b9fefc276d9a2075ce3c51e7e72d7c9753b34c5d50ee4fceec4991b67a3217`  
		Last Modified: Wed, 14 Apr 2021 21:43:30 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev16-alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:18c99b0294acf4a444a344d4c476be34518c138a574c250c7c8750d76cc06597
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9734849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52252a1f5ee12456e41ec6a35ee091bbb9f2d7a0311adfe006f8bfceb0d6a31d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:18:05 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 21:18:07 GMT
ENV HAPROXY_VERSION=2.4-dev16
# Wed, 14 Apr 2021 21:18:14 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev16.tar.gz
# Wed, 14 Apr 2021 21:18:20 GMT
ENV HAPROXY_SHA256=7ba831c977ce80e26ed3ae6ecbc54c1ff3e8a313118b47b9d877ef44ad17cdf0
# Wed, 14 Apr 2021 21:19:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 21:19:47 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 21:20:03 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 21:20:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 21:20:18 GMT
USER haproxy
# Wed, 14 Apr 2021 21:20:25 GMT
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
	-	`sha256:ddb60d9983255b54cb38cb0a251c53b66d2bb77cbea2b33d932954b8be43ab1a`  
		Last Modified: Wed, 14 Apr 2021 21:34:03 GMT  
		Size: 7.1 MB (7111083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83cd0fbccc760a62c97c0b23be21404c7581354f10644f351949349da37c616`  
		Last Modified: Wed, 14 Apr 2021 21:34:00 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev16-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:4971a69893cf77341cfb9ec10c142b73cf01d09365e482f5a887e4b56bdf7e7f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9461751 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef6f640418384b5e32ce71e244b71fd543d6a7bd39de9bb8853cb0c3dc8a6eca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:47:58 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 22:47:59 GMT
ENV HAPROXY_VERSION=2.4-dev16
# Wed, 14 Apr 2021 22:48:00 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev16.tar.gz
# Wed, 14 Apr 2021 22:48:01 GMT
ENV HAPROXY_SHA256=7ba831c977ce80e26ed3ae6ecbc54c1ff3e8a313118b47b9d877ef44ad17cdf0
# Wed, 14 Apr 2021 22:48:41 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 22:48:47 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 22:48:48 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 22:48:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 22:48:50 GMT
USER haproxy
# Wed, 14 Apr 2021 22:48:51 GMT
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
	-	`sha256:936542e31ad7c9777cdafccccf5ce7a555aa454fed069d6f2ae79991d79f75b0`  
		Last Modified: Wed, 14 Apr 2021 22:56:11 GMT  
		Size: 7.0 MB (7035971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2a6563452e5781204324a0e0d804848ebe45a55cefb87e605dc3da9c3fc2c21`  
		Last Modified: Wed, 14 Apr 2021 22:56:09 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev16-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:c245fdeaaa47cc7630d6b769ac549207537b86dc3a1768892d5276c73a489f03
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (10011014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28d03fd763573258ff5390ca0e0ebf6f62cf30f50bae999580a666eee34e4279`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:26:01 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 20:26:09 GMT
ENV HAPROXY_VERSION=2.4-dev16
# Wed, 14 Apr 2021 20:26:16 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev16.tar.gz
# Wed, 14 Apr 2021 20:26:20 GMT
ENV HAPROXY_SHA256=7ba831c977ce80e26ed3ae6ecbc54c1ff3e8a313118b47b9d877ef44ad17cdf0
# Wed, 14 Apr 2021 20:26:59 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 20:27:06 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 20:27:12 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:27:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:27:25 GMT
USER haproxy
# Wed, 14 Apr 2021 20:27:29 GMT
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
	-	`sha256:c8ed3510eee22484c704a65f38d771d2d6965b046a61cd8490f48d7b789dc13a`  
		Last Modified: Wed, 14 Apr 2021 20:37:52 GMT  
		Size: 7.3 MB (7297348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870fcebc0a3df6042739c38db9b595f4a112ef62133cb18903e6254dc8525678`  
		Last Modified: Wed, 14 Apr 2021 20:37:50 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev16-alpine` - linux; 386

```console
$ docker pull haproxy@sha256:f2865df25e682e69fa363d071fc584109a0efbff3712ed086675bc9a4d264aa2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9895508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45a25268a3320d5e276686b082b5307e048869035cb85d50a7016996016f97c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 01:50:06 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 15 Apr 2021 01:50:07 GMT
ENV HAPROXY_VERSION=2.4-dev16
# Thu, 15 Apr 2021 01:50:07 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev16.tar.gz
# Thu, 15 Apr 2021 01:50:07 GMT
ENV HAPROXY_SHA256=7ba831c977ce80e26ed3ae6ecbc54c1ff3e8a313118b47b9d877ef44ad17cdf0
# Thu, 15 Apr 2021 01:52:00 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 15 Apr 2021 01:52:00 GMT
STOPSIGNAL SIGUSR1
# Thu, 15 Apr 2021 01:52:00 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 15 Apr 2021 01:52:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Apr 2021 01:52:01 GMT
USER haproxy
# Thu, 15 Apr 2021 01:52:01 GMT
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
	-	`sha256:0732fbf011caf16c89352454dd21428c5ceef223d490e25a91ca458af0f4cc7e`  
		Last Modified: Thu, 15 Apr 2021 02:00:30 GMT  
		Size: 7.1 MB (7074972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0f2f874bc081911a85b4042df452e69d8cd4dbf1217eee78c9e197438756c2`  
		Last Modified: Thu, 15 Apr 2021 02:00:28 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev16-alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:3ccbaaeabac23dc6cfd593703a14f976b7056ffa2313a60712737ad25b3e89e3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.4 MB (10412354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:720292a6554d6bf06fde693ce1c84752350c59fdb23f5c405869f68c6a086190`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:25:09 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 23:25:12 GMT
ENV HAPROXY_VERSION=2.4-dev16
# Wed, 14 Apr 2021 23:25:14 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev16.tar.gz
# Wed, 14 Apr 2021 23:25:15 GMT
ENV HAPROXY_SHA256=7ba831c977ce80e26ed3ae6ecbc54c1ff3e8a313118b47b9d877ef44ad17cdf0
# Wed, 14 Apr 2021 23:26:00 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 23:26:03 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 23:26:07 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 23:26:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 23:26:20 GMT
USER haproxy
# Wed, 14 Apr 2021 23:26:23 GMT
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
	-	`sha256:f8cf06ac8d3b30db55bccd6e3e9a52b654d32699c288c9f8609f5da3f0de9b3f`  
		Last Modified: Wed, 14 Apr 2021 23:36:38 GMT  
		Size: 7.6 MB (7597577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2a8135ce5553616628e564a4aa023c4cbf621914eb9f4da05275bdc022194ba`  
		Last Modified: Wed, 14 Apr 2021 23:36:36 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev16-alpine` - linux; s390x

```console
$ docker pull haproxy@sha256:190d5debc6f053ebdd1132223f15357de8fa8265ca6dbe140c116e25c6403253
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.8 MB (9773567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f5408cec121f5ad32c2b0887e1033653577a0a9490825df6bfacdf2bdf4ca89`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:54:24 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 20:54:24 GMT
ENV HAPROXY_VERSION=2.4-dev16
# Wed, 14 Apr 2021 20:54:24 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev16.tar.gz
# Wed, 14 Apr 2021 20:54:24 GMT
ENV HAPROXY_SHA256=7ba831c977ce80e26ed3ae6ecbc54c1ff3e8a313118b47b9d877ef44ad17cdf0
# Wed, 14 Apr 2021 20:55:03 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 20:55:04 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 20:55:04 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:55:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:55:05 GMT
USER haproxy
# Wed, 14 Apr 2021 20:55:05 GMT
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
	-	`sha256:fa0a88436cf32707688ce587a072715e090f00fafffb8c4ac2d928094a85e90b`  
		Last Modified: Wed, 14 Apr 2021 20:59:07 GMT  
		Size: 7.2 MB (7169284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd015e23ad1b5309f4ecccd6b627b5d57330dab0d488cba19cd2f33712d6ad0`  
		Last Modified: Wed, 14 Apr 2021 20:59:06 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:alpine`

```console
$ docker pull haproxy@sha256:fd871b2cf0be22d10d148fffe88441167587ea84bad028d4eb81808f28251070
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
$ docker pull haproxy@sha256:101ee16ec0838ee24f3695ccbd3653b735af22c130d6fd0d7be6d7ac9bc879a4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9499607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:383495f19607c1dd21dce3f33aef722f2c94d10c76eb76dce409928ada65c265`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:37:38 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 21:38:52 GMT
ENV HAPROXY_VERSION=2.3.9
# Wed, 14 Apr 2021 21:38:52 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.9.tar.gz
# Wed, 14 Apr 2021 21:38:52 GMT
ENV HAPROXY_SHA256=77110bc1272bad18fff56b30f4614bcc1deb50600ae42cb0f0b161fc41e2ba96
# Wed, 14 Apr 2021 21:39:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 21:39:42 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 21:39:42 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 21:39:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 21:39:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 21:39:44 GMT
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
	-	`sha256:7b412bb59f5511a4cc66e0b0eb2c0b1781069e37fc9fcda8f4e0908c48d6584f`  
		Last Modified: Wed, 14 Apr 2021 21:43:46 GMT  
		Size: 6.7 MB (6685882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:321129059a3aee4d0de22e7b595549eb049c90428cd1e220ce0f904fc2d70c49`  
		Last Modified: Wed, 14 Apr 2021 21:43:45 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16f8e4cbddc48fe0e653ac776e4d1bd90066ace1e53e95d4f01b3179c7a4914e`  
		Last Modified: Wed, 14 Apr 2021 21:43:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:aa7d553fd0c3bc210b6aa068e134a7b95f07577abecdf0f9eb2318d798d93bfc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.2 MB (9209545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5382bb355f68826f4b9ded72ab54cef0217d776f3172303c578a8c80056ce23c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:18:05 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 21:20:51 GMT
ENV HAPROXY_VERSION=2.3.9
# Wed, 14 Apr 2021 21:21:02 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.9.tar.gz
# Wed, 14 Apr 2021 21:21:11 GMT
ENV HAPROXY_SHA256=77110bc1272bad18fff56b30f4614bcc1deb50600ae42cb0f0b161fc41e2ba96
# Wed, 14 Apr 2021 21:22:23 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 21:22:35 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 21:22:51 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 21:23:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 21:23:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 21:23:45 GMT
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
	-	`sha256:5300d7514c3b8d397433442634825547f6a6612e10c46f4ce3dbb4225d5c7720`  
		Last Modified: Wed, 14 Apr 2021 21:34:16 GMT  
		Size: 6.6 MB (6585661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3c323aab13edc8b368334c6d8ad71cec1535117eaeec134595b17088d37937b`  
		Last Modified: Wed, 14 Apr 2021 21:34:15 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e846321291b72a418aa9ccff5106b00fc25129846b6ac70d6cf51fe0374d797`  
		Last Modified: Wed, 14 Apr 2021 21:34:17 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:75fb3450317233e825f312b8f71b7587d9fd67908e21917728c7a306e6877be5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.9 MB (8926169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acf4585d9e128a18420fdc031947d290650b37b108452804564b0d35e86def6e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:47:58 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 22:49:20 GMT
ENV HAPROXY_VERSION=2.3.9
# Wed, 14 Apr 2021 22:49:29 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.9.tar.gz
# Wed, 14 Apr 2021 22:49:36 GMT
ENV HAPROXY_SHA256=77110bc1272bad18fff56b30f4614bcc1deb50600ae42cb0f0b161fc41e2ba96
# Wed, 14 Apr 2021 22:50:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 22:50:53 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 22:51:05 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 22:51:42 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 22:51:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 22:51:53 GMT
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
	-	`sha256:0b33f8441fa4f8170fcb000f1c6d2614765037bc108661d7ca5e54b529f37010`  
		Last Modified: Wed, 14 Apr 2021 22:56:23 GMT  
		Size: 6.5 MB (6500266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7d61f2b79b5d21794c5d4dcc642a2df4a7c899b2ece6f1a1d7cfc5f4c47496`  
		Last Modified: Wed, 14 Apr 2021 22:56:21 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef906e7aaf5f11781888556cccd267b184bdbecc723469a8747dababde6cae88`  
		Last Modified: Wed, 14 Apr 2021 22:56:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:4697ab52f31a27418b40afce46493f004c96c3a8b4f5b3234f2ad8fd8b7bb612
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9412142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ad4040f240cdfea6361a98a491df6e7c2e8bd00c8c0f1ea0a9ddde03f43254d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:26:01 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 20:28:04 GMT
ENV HAPROXY_VERSION=2.3.9
# Wed, 14 Apr 2021 20:28:12 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.9.tar.gz
# Wed, 14 Apr 2021 20:28:20 GMT
ENV HAPROXY_SHA256=77110bc1272bad18fff56b30f4614bcc1deb50600ae42cb0f0b161fc41e2ba96
# Wed, 14 Apr 2021 20:29:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 20:29:17 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 20:29:25 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:29:56 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 20:30:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:30:11 GMT
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
	-	`sha256:6c72b09b2c83b9e5a88d98cf15715a3dfdc984d4837af7d7365a07ea6a3d7866`  
		Last Modified: Wed, 14 Apr 2021 20:38:03 GMT  
		Size: 6.7 MB (6698357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bba2f8c9c125c15cccf5572333f7c53e54f6df343fb7e7cce3177d1331ebc8d8`  
		Last Modified: Wed, 14 Apr 2021 20:38:01 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3057815f353087d9bee55cd953f619dd59c84c2f554ea8058882188f9e4f814`  
		Last Modified: Wed, 14 Apr 2021 20:38:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:alpine` - linux; 386

```console
$ docker pull haproxy@sha256:9f99933bbb9fb8a7b3b040bf9b93ce55dde75211224d44c75e3bcd76299e5d7c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9354648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa6e1a1e81c45d3bc98a25c27b58ff451e0d561ea1f95d289ee3cee4b0c35f4a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 01:50:06 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 15 Apr 2021 01:52:21 GMT
ENV HAPROXY_VERSION=2.3.9
# Thu, 15 Apr 2021 01:52:21 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.9.tar.gz
# Thu, 15 Apr 2021 01:52:21 GMT
ENV HAPROXY_SHA256=77110bc1272bad18fff56b30f4614bcc1deb50600ae42cb0f0b161fc41e2ba96
# Thu, 15 Apr 2021 01:53:27 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 15 Apr 2021 01:53:27 GMT
STOPSIGNAL SIGUSR1
# Thu, 15 Apr 2021 01:53:27 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 15 Apr 2021 01:53:28 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 15 Apr 2021 01:53:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Apr 2021 01:53:29 GMT
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
	-	`sha256:ca59b31cb2383b0cecb9a081d46bc5cb55ff05176d7da51344504b99f485b37c`  
		Last Modified: Thu, 15 Apr 2021 02:00:45 GMT  
		Size: 6.5 MB (6533992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43d9fdba60ae084cf195a2fc170f0358d1eb329ec60f7e3d78f39e3bd42c0599`  
		Last Modified: Thu, 15 Apr 2021 02:00:44 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a98584752f736ec3c38550ffb5a53f52be250c0c3b5b5d2d3cb60d2b08f0fa31`  
		Last Modified: Thu, 15 Apr 2021 02:00:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:19dc93de5c25a5e87c31214ba644e2d889de9b3834a4f13762711529b7d12a8f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.8 MB (9832346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb9dac528b8dbf1a3a08aeeb1ac86db8bbef3c78e14cbcd1229183af17c6bb12`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:25:09 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 23:26:45 GMT
ENV HAPROXY_VERSION=2.3.9
# Wed, 14 Apr 2021 23:26:47 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.9.tar.gz
# Wed, 14 Apr 2021 23:26:51 GMT
ENV HAPROXY_SHA256=77110bc1272bad18fff56b30f4614bcc1deb50600ae42cb0f0b161fc41e2ba96
# Wed, 14 Apr 2021 23:28:14 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 23:28:20 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 23:28:27 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 23:28:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 23:28:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 23:28:56 GMT
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
	-	`sha256:55517a2814e2dbb00eb7d44f417b8729aa436b00a32a084c238b7d5733011cb2`  
		Last Modified: Wed, 14 Apr 2021 23:36:51 GMT  
		Size: 7.0 MB (7017449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e5587a8b18c5eac4421c6e6dcf2bd5b8aa86e1cc461dd1608c57f7d8208359`  
		Last Modified: Wed, 14 Apr 2021 23:36:50 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e0e401a50336fe2abb496fdd8bae8c8a08a451470c41b530499798a6e9a14f2`  
		Last Modified: Wed, 14 Apr 2021 23:36:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:alpine` - linux; s390x

```console
$ docker pull haproxy@sha256:5736a38ee6dd2b1a7821b37847aae240638a52c8bac5062883d90fca886909b3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9257346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25cf086b4e421310119b91b6fe47633d277b498487de5549fb997acd6a25cb0f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:54:24 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 20:55:17 GMT
ENV HAPROXY_VERSION=2.3.9
# Wed, 14 Apr 2021 20:55:17 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.9.tar.gz
# Wed, 14 Apr 2021 20:55:18 GMT
ENV HAPROXY_SHA256=77110bc1272bad18fff56b30f4614bcc1deb50600ae42cb0f0b161fc41e2ba96
# Wed, 14 Apr 2021 20:55:58 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 20:55:59 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 20:55:59 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:56:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 20:56:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:56:00 GMT
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
	-	`sha256:ae9e557ff45057778dffe5c56dc419e35c7d970db8ce611466c9b0d09a048305`  
		Last Modified: Wed, 14 Apr 2021 20:59:18 GMT  
		Size: 6.7 MB (6652940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb69cd1d8680cdc862b3d406dbc637a101625886f943068bf0dd5647f78353df`  
		Last Modified: Wed, 14 Apr 2021 20:59:17 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8270e1f8a61ff9eb8008cffc9b5ae5fb3a982db994eaa84d2653ef71236dec1e`  
		Last Modified: Wed, 14 Apr 2021 20:59:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:latest`

```console
$ docker pull haproxy@sha256:f63aabf39efcd277b04a503d38e59e80224a0c11f47b2568b13b0092698c5a3a
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
$ docker pull haproxy@sha256:fa42cfd9f7ee39c10215258a25308d7ad5f6a3b2e8b99c216d22b8aeab0cd9c1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.7 MB (36695481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15630318f735650284c7afcde2e3c813c4e78340d9ff6761e84bd829a7e51e87`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:29:42 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 06:31:25 GMT
ENV HAPROXY_VERSION=2.3.9
# Sat, 10 Apr 2021 06:31:25 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.9.tar.gz
# Sat, 10 Apr 2021 06:31:25 GMT
ENV HAPROXY_SHA256=77110bc1272bad18fff56b30f4614bcc1deb50600ae42cb0f0b161fc41e2ba96
# Sat, 10 Apr 2021 06:32:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 06:32:21 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 06:32:22 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 06:32:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 06:32:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 06:32:24 GMT
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
	-	`sha256:df883def87ebe557cc46aaeca475a9bd5454161217a472bb8843b275194833ea`  
		Last Modified: Sat, 10 Apr 2021 06:38:23 GMT  
		Size: 9.6 MB (9554157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:038f2c73c3bef00ccb45017c5fa20d688d83dc4a82772af4c286b38d408bc365`  
		Last Modified: Sat, 10 Apr 2021 06:38:21 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62b97027777b1b16f3b053b4b6c440474edf49148b2f249f2649c9e485f88c8d`  
		Last Modified: Sat, 10 Apr 2021 06:38:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:latest` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:4f4f4468959827b0c860592aaa85abb97caeb8ec0f9aac47c3f522727ffee0fa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (34039733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ca650df4f2b0f360fca1a41bcde309f21b21e62c4f6bb717bdd4c196c4a4c51`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:51:31 GMT
ADD file:926533a23a69aa2481a9122b667bb6300a347154eea366c9e679a230aa7f373a in / 
# Sat, 10 Apr 2021 00:51:34 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 02:24:17 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 02:26:09 GMT
ENV HAPROXY_VERSION=2.3.9
# Sat, 10 Apr 2021 02:26:13 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.9.tar.gz
# Sat, 10 Apr 2021 02:26:16 GMT
ENV HAPROXY_SHA256=77110bc1272bad18fff56b30f4614bcc1deb50600ae42cb0f0b161fc41e2ba96
# Sat, 10 Apr 2021 02:27:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 02:27:18 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 02:27:24 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 02:27:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 02:27:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 02:27:43 GMT
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
	-	`sha256:67f84b9aa74574db91fd776882e7ddc449b036a85d7421fda9ce0b66cd53227c`  
		Last Modified: Sat, 10 Apr 2021 02:37:07 GMT  
		Size: 9.2 MB (9164583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe3f7588980758230b77ae29222ce3a4792fce39a431518a5d2b4601dbfb0ac3`  
		Last Modified: Sat, 10 Apr 2021 02:37:04 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b97190d21dc7f1f4b5cab24efde00b68d49e3f7a5d7b845cfd8a134a3b45f01`  
		Last Modified: Sat, 10 Apr 2021 02:37:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:latest` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:8546ee0d84b1809008a7d0af2d688fdaad936066fdcfb69f9c15f60969321ec2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31766763 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:154e3a5a493a3254d84194f03dd38b61212efae170ebe3bdfbadbe59e2d25b3b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:59:45 GMT
ADD file:3fbd246a2de82566bcaaf62e3e0bf57175a7ad46b4156366a110661b31eab240 in / 
# Sat, 10 Apr 2021 00:59:47 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 08:58:51 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 08:59:51 GMT
ENV HAPROXY_VERSION=2.3.9
# Sat, 10 Apr 2021 08:59:52 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.9.tar.gz
# Sat, 10 Apr 2021 08:59:53 GMT
ENV HAPROXY_SHA256=77110bc1272bad18fff56b30f4614bcc1deb50600ae42cb0f0b161fc41e2ba96
# Sat, 10 Apr 2021 09:00:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 09:00:33 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 09:00:34 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 09:00:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 09:00:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 09:00:38 GMT
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
	-	`sha256:15bf0834e9efeb35188b41bfa4a66446c609dde5de0ae64e4f59c4192844340f`  
		Last Modified: Sat, 10 Apr 2021 09:05:38 GMT  
		Size: 9.0 MB (9025015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1199d1177880e0e9af691b1d831f9d408004aea8508fe3068df501f64dc7c4e9`  
		Last Modified: Sat, 10 Apr 2021 09:05:35 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62336b3e70f00cdb67d3d3b57f04d4e38fe453cf2a320472b95c1e646e214fb1`  
		Last Modified: Sat, 10 Apr 2021 09:05:35 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:latest` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:d4152a50e3a1d0c539e2c0da480494cb03173b407e5280fe3377e1c59502c2e8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35347191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35bd0c1cb4a0e6110216a3a3e8e51c671697ce828fb060dcc6e18f991e9d7294`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:41:25 GMT
ADD file:b24da7eb23eeae04e00d0e45da29a89fe8f992e8dcf4ba482afb907b8015b7bf in / 
# Sat, 10 Apr 2021 00:41:28 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:13:29 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 01:14:41 GMT
ENV HAPROXY_VERSION=2.3.9
# Sat, 10 Apr 2021 01:14:42 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.9.tar.gz
# Sat, 10 Apr 2021 01:14:43 GMT
ENV HAPROXY_SHA256=77110bc1272bad18fff56b30f4614bcc1deb50600ae42cb0f0b161fc41e2ba96
# Sat, 10 Apr 2021 01:15:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 01:15:29 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 01:15:30 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 01:15:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 01:15:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 01:15:35 GMT
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
	-	`sha256:50023a581af47a05e808c497ef77767fb715a8faab03f14014f4a0daf9cc95d4`  
		Last Modified: Sat, 10 Apr 2021 01:21:39 GMT  
		Size: 9.4 MB (9440659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d067d1042b01ff19aac1b75558139c81bf8c08f7987b4683f41cee55d25ae1d5`  
		Last Modified: Sat, 10 Apr 2021 01:21:37 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7fbf89cba9a16dac8ecd7198f7adcbd4ba1aacbf3cb6fed25d98af7113cc9e`  
		Last Modified: Sat, 10 Apr 2021 01:21:37 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:latest` - linux; 386

```console
$ docker pull haproxy@sha256:3f56e9b27fb491e75d845611cd4a286778b258159fb858d433fedf0a67c107c0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.2 MB (37206708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba2c3b8430883fc337b03423ad8f552ebce3c59922aa2848eda4aa4851fedf40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:39:42 GMT
ADD file:8885d4d13678543780bb04ba14b621179665f7951d5b261036a7092df9b376e7 in / 
# Sat, 10 Apr 2021 00:39:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 03:48:12 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 03:49:41 GMT
ENV HAPROXY_VERSION=2.3.9
# Sat, 10 Apr 2021 03:49:42 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.9.tar.gz
# Sat, 10 Apr 2021 03:49:42 GMT
ENV HAPROXY_SHA256=77110bc1272bad18fff56b30f4614bcc1deb50600ae42cb0f0b161fc41e2ba96
# Sat, 10 Apr 2021 03:50:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 03:50:39 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 03:50:39 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 03:50:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 03:50:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 03:50:41 GMT
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
	-	`sha256:b1f6beb31958abbb8f7a9acf66b271bb4dc1d8d0b98388c882495f0ef83610d0`  
		Last Modified: Sat, 10 Apr 2021 03:59:30 GMT  
		Size: 9.4 MB (9415773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15fe6c571e5875233b0a10e1cb7a2f1369c603593dc4a8ff137666839901235b`  
		Last Modified: Sat, 10 Apr 2021 03:59:26 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d481f6e20a049956aa9c45f996c4e1021f9a264880f372a60ea6402b756bfdfa`  
		Last Modified: Sat, 10 Apr 2021 03:59:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:latest` - linux; mips64le

```console
$ docker pull haproxy@sha256:53436f8b139b3fd4d1aeb5af64fd64728367d88f336c94f214220e29f30ba650
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.9 MB (34940784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87eebec53adc866af1eb6d1f0fa86b198fd2180cea5ca55681b1fb3fe0d41c5d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:09:40 GMT
ADD file:0c93801c4a3719dfd4c047d7f2f4d52bf463eba2ab875da1dc54dcc832aae20b in / 
# Sat, 10 Apr 2021 01:09:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:39:36 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 01:42:16 GMT
ENV HAPROXY_VERSION=2.3.9
# Sat, 10 Apr 2021 01:42:17 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.9.tar.gz
# Sat, 10 Apr 2021 01:42:17 GMT
ENV HAPROXY_SHA256=77110bc1272bad18fff56b30f4614bcc1deb50600ae42cb0f0b161fc41e2ba96
# Sat, 10 Apr 2021 01:44:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 01:44:36 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 01:44:36 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 01:44:38 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 01:44:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 01:44:39 GMT
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
	-	`sha256:d1372285d5ae001a835df04f6feaf805c2b2c652679dde7805ec9bd4e10c47a6`  
		Last Modified: Sat, 10 Apr 2021 01:54:04 GMT  
		Size: 9.1 MB (9132422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:701e913c803ad74ba962379671609f4cb6496d8bfc4bba941ff1f2934d1d6d50`  
		Last Modified: Sat, 10 Apr 2021 01:53:57 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89484a5f3cd65e20b77c9a3f2b34f5a3e21db69bee7cadd04a91f4ff5f24c7f`  
		Last Modified: Sat, 10 Apr 2021 01:53:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:latest` - linux; ppc64le

```console
$ docker pull haproxy@sha256:d5a1da8f612b8b7bb79e1c462da111fcca84adf2d63955e5656f8c151ca7ad15
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40587797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4392007f5f50e8bc72897aa2e05d25db0685de3a480bd976fc09db92635dbb97`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:26:49 GMT
ADD file:ab87d4854aa8628ce8f4e603c0496499f6f28c3d2525ace782c7369691dafc8c in / 
# Sat, 10 Apr 2021 01:26:56 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 04:45:12 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 04:49:34 GMT
ENV HAPROXY_VERSION=2.3.9
# Sat, 10 Apr 2021 04:49:37 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.9.tar.gz
# Sat, 10 Apr 2021 04:49:42 GMT
ENV HAPROXY_SHA256=77110bc1272bad18fff56b30f4614bcc1deb50600ae42cb0f0b161fc41e2ba96
# Sat, 10 Apr 2021 04:55:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 04:55:04 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 04:55:07 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 04:55:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 04:55:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 04:55:34 GMT
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
	-	`sha256:02dce87e4030362a76d243c695c727400c1fd6e681a33250a0c28bf2959ae752`  
		Last Modified: Sat, 10 Apr 2021 05:10:05 GMT  
		Size: 10.0 MB (10039904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c079ef5cde73a0361b14c8a5f1233d1b99b440f80b935334458e57cf3868804d`  
		Last Modified: Sat, 10 Apr 2021 05:10:03 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27203244b0981a4f3bb61515617544544f43c8b518b565a045b3a3b79db4ce5b`  
		Last Modified: Sat, 10 Apr 2021 05:10:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:latest` - linux; s390x

```console
$ docker pull haproxy@sha256:19f3d5d79196611de41352b39a99bdf83b98e44349876ab6cdb27b6e1f35c181
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.0 MB (35044591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ede5f02058145c8565168e90cb541d031baba061a845ef0d1083b665e3277965`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:42:23 GMT
ADD file:dbe2182f8699f2a6011413ea01862e6c0e85853d922dffd72a28d994d23c79bc in / 
# Sat, 10 Apr 2021 00:42:25 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:38:04 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 01:38:49 GMT
ENV HAPROXY_VERSION=2.3.9
# Sat, 10 Apr 2021 01:38:50 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.9.tar.gz
# Sat, 10 Apr 2021 01:38:50 GMT
ENV HAPROXY_SHA256=77110bc1272bad18fff56b30f4614bcc1deb50600ae42cb0f0b161fc41e2ba96
# Sat, 10 Apr 2021 01:39:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 01:39:22 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 01:39:22 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 01:39:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 01:39:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 01:39:23 GMT
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
	-	`sha256:278677bd5845b54d7bbc1e1a92c95b6211358dc62bd96f1fc52ec341df16206d`  
		Last Modified: Sat, 10 Apr 2021 01:42:38 GMT  
		Size: 9.3 MB (9288855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edc908ef823f2540bc02f00eeb071894d56eddaf33d48ff9224cda774e4d54be`  
		Last Modified: Sat, 10 Apr 2021 01:42:37 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a4523549f27c304e4a974a37341a467a3bb7fca15bab56a5a5f97613f7ff9b2`  
		Last Modified: Sat, 10 Apr 2021 01:42:37 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:lts`

```console
$ docker pull haproxy@sha256:de91b6e9d7b8ac1c4f55c012cee2a03f766063d61a2c42e70f15ca9ce5cffccf
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
$ docker pull haproxy@sha256:0980ae3a6550c6dc5233f91c14344c70ea334505919584bb78f840e1c040b447
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.4 MB (36446380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d59c0ba74b7e235e5a5728035c1c9b66b79d24aa898a2d994223c069a8d1db49`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:29:42 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 06:32:41 GMT
ENV HAPROXY_VERSION=2.2.13
# Sat, 10 Apr 2021 06:32:41 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.13.tar.gz
# Sat, 10 Apr 2021 06:32:42 GMT
ENV HAPROXY_SHA256=9e3e51441c70bedfb494fc9d4b4d3389a71be9a3c915ba3d6f7e8fd9a57ce160
# Sat, 10 Apr 2021 06:34:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 06:34:01 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 06:34:02 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 06:34:03 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 06:34:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 06:34:03 GMT
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
	-	`sha256:a4ac7a9f13ea2eeb6a8050090e57aee7e14337034b9e7565f30ffb9bc11cc8d0`  
		Last Modified: Sat, 10 Apr 2021 06:38:38 GMT  
		Size: 9.3 MB (9305056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c87b35756f7d827f1af49c1622775093c9d433056286165dfe92a96727e14367`  
		Last Modified: Sat, 10 Apr 2021 06:38:37 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2371bbf56d662c6773a6498b56369e7b8e46fe696a1f53d60becdf9fbc35e249`  
		Last Modified: Sat, 10 Apr 2021 06:38:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:ea8caf1a471b1d052cce885f728ecbd7661e3154b1bd9490b4ead9d6f96e34a4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33784186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42fa781836c103292a015ca6c217ec9009cd1b10e90f8b640780e161fa466dfd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:51:31 GMT
ADD file:926533a23a69aa2481a9122b667bb6300a347154eea366c9e679a230aa7f373a in / 
# Sat, 10 Apr 2021 00:51:34 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 02:24:17 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 02:27:57 GMT
ENV HAPROXY_VERSION=2.2.13
# Sat, 10 Apr 2021 02:28:00 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.13.tar.gz
# Sat, 10 Apr 2021 02:28:03 GMT
ENV HAPROXY_SHA256=9e3e51441c70bedfb494fc9d4b4d3389a71be9a3c915ba3d6f7e8fd9a57ce160
# Sat, 10 Apr 2021 02:29:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 02:29:11 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 02:29:17 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 02:29:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 02:29:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 02:29:37 GMT
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
	-	`sha256:1a9539dc178d3edc26c473a1278c3b8005c9418c35d68e1be1eda3e620e9e9e5`  
		Last Modified: Sat, 10 Apr 2021 02:37:17 GMT  
		Size: 8.9 MB (8909037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90a7f4dd06e8114f46916dd5877eacb048ce77ab5d497b0bb6a356b71262e63`  
		Last Modified: Sat, 10 Apr 2021 02:37:14 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68c6b0e6fee35363aa79edd25b01d996dea7f7748e0db784700ecf512099d35b`  
		Last Modified: Sat, 10 Apr 2021 02:37:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:bba42c59d71ad06be8103a3bedce42b8898bbf3bfa4fb0be2cb06f3e3b01f688
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.5 MB (31461092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1f54b69378fa75b9cfd1ef85e56a15f392411149c29d9e16fbab58cb1c66d2b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:59:45 GMT
ADD file:3fbd246a2de82566bcaaf62e3e0bf57175a7ad46b4156366a110661b31eab240 in / 
# Sat, 10 Apr 2021 00:59:47 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 08:58:51 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 09:00:53 GMT
ENV HAPROXY_VERSION=2.2.13
# Sat, 10 Apr 2021 09:00:54 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.13.tar.gz
# Sat, 10 Apr 2021 09:00:55 GMT
ENV HAPROXY_SHA256=9e3e51441c70bedfb494fc9d4b4d3389a71be9a3c915ba3d6f7e8fd9a57ce160
# Sat, 10 Apr 2021 09:01:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 09:01:37 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 09:01:38 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 09:01:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 09:01:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 09:01:42 GMT
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
	-	`sha256:b75131a6ec2e4adca7605661356ce165e13803d545d79123d0e3330d435596f5`  
		Last Modified: Sat, 10 Apr 2021 09:05:50 GMT  
		Size: 8.7 MB (8719344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9ea1930c5490ff94769de0e8ab8aad2b5c1e4e72d54c27afee12d74411f600`  
		Last Modified: Sat, 10 Apr 2021 09:05:47 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2e34fd9824e23d785f73ea0802107c25f42c9ad3d30abdc87f5e61fd4e17080`  
		Last Modified: Sat, 10 Apr 2021 09:05:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:9ea94a117b8f204c209df772aee3188d13a616efe6ca343149e0ad29fa251507
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.0 MB (35023478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b853740b36a0d8cc1b4c066a09de9600dfaf3e5c09ddeb7d9a627384baa05ec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:41:25 GMT
ADD file:b24da7eb23eeae04e00d0e45da29a89fe8f992e8dcf4ba482afb907b8015b7bf in / 
# Sat, 10 Apr 2021 00:41:28 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:13:29 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 01:15:54 GMT
ENV HAPROXY_VERSION=2.2.13
# Sat, 10 Apr 2021 01:15:55 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.13.tar.gz
# Sat, 10 Apr 2021 01:15:57 GMT
ENV HAPROXY_SHA256=9e3e51441c70bedfb494fc9d4b4d3389a71be9a3c915ba3d6f7e8fd9a57ce160
# Sat, 10 Apr 2021 01:16:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 01:16:49 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 01:16:51 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 01:16:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 01:16:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 01:16:59 GMT
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
	-	`sha256:b208d49b31d425b72f01f4c0579f75de3e8a9e9b5e413d19ad545fcb1cfec498`  
		Last Modified: Sat, 10 Apr 2021 01:21:53 GMT  
		Size: 9.1 MB (9116944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69001e0866df82cbc43b538ac2c4247ac27a02101891fc85d945daa23280ec2e`  
		Last Modified: Sat, 10 Apr 2021 01:21:50 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fb9542d39b52a78dae6dfffd1040b30683aee32cf37f2699e42eae131137abe`  
		Last Modified: Sat, 10 Apr 2021 01:21:50 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; 386

```console
$ docker pull haproxy@sha256:49260af2de07dc187620f290c656da80183c7b1e8ab773755a40ee9f7f6f9aaf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36978050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baf5327943d1ef805085f695725d9d9d120dc638b881ba0daf29bbacdef45fe6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:39:42 GMT
ADD file:8885d4d13678543780bb04ba14b621179665f7951d5b261036a7092df9b376e7 in / 
# Sat, 10 Apr 2021 00:39:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 03:48:12 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 03:50:59 GMT
ENV HAPROXY_VERSION=2.2.13
# Sat, 10 Apr 2021 03:51:00 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.13.tar.gz
# Sat, 10 Apr 2021 03:51:00 GMT
ENV HAPROXY_SHA256=9e3e51441c70bedfb494fc9d4b4d3389a71be9a3c915ba3d6f7e8fd9a57ce160
# Sat, 10 Apr 2021 03:52:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 03:52:26 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 03:52:26 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 03:52:27 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 03:52:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 03:52:28 GMT
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
	-	`sha256:501040fe44c6490e09a71181c6626bc3bb0bfe93798932941b8c0789c72d1c5e`  
		Last Modified: Sat, 10 Apr 2021 03:59:58 GMT  
		Size: 9.2 MB (9187117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:388ebcc0127bdbcff243568101388f512720854794aa20ab9acddc6b0a922450`  
		Last Modified: Sat, 10 Apr 2021 03:59:50 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:284bc34ec1436775792b35bfa789aa45111707b63c5a95f5df4f6d25e5db332e`  
		Last Modified: Sat, 10 Apr 2021 03:59:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; mips64le

```console
$ docker pull haproxy@sha256:24f69608e75a6910345769e9baaa7433a51d911decf979eaaafd1490ff0a5ee2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34674134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:277a2344421652b30bcc8416edef8dfb9cc9ee769ba4ba5ad51bf80a6085bfa0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:09:40 GMT
ADD file:0c93801c4a3719dfd4c047d7f2f4d52bf463eba2ab875da1dc54dcc832aae20b in / 
# Sat, 10 Apr 2021 01:09:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:39:36 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 01:44:43 GMT
ENV HAPROXY_VERSION=2.2.13
# Sat, 10 Apr 2021 01:44:43 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.13.tar.gz
# Sat, 10 Apr 2021 01:44:43 GMT
ENV HAPROXY_SHA256=9e3e51441c70bedfb494fc9d4b4d3389a71be9a3c915ba3d6f7e8fd9a57ce160
# Sat, 10 Apr 2021 01:47:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 01:47:05 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 01:47:06 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 01:47:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 01:47:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 01:47:08 GMT
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
	-	`sha256:34d169508d4b44b7fea30d0806ab3babbfe581b239f681919ae771c048d8213f`  
		Last Modified: Sat, 10 Apr 2021 01:54:23 GMT  
		Size: 8.9 MB (8865773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e41b7b929b9472e4f31050212242ce54c3d7abad584e23967b0ca1f52e3d262`  
		Last Modified: Sat, 10 Apr 2021 01:54:17 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e80eb6485d38caf34db8f19ffc92fd40dd6cf9bbed315177ada12c503c2cdf4`  
		Last Modified: Sat, 10 Apr 2021 01:54:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; ppc64le

```console
$ docker pull haproxy@sha256:051c8550a62dede7d06f587afb6946e710050fcf711ff38461c488dcffda9498
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40318021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67d26e25e79a68e404304e5bae82aefa19b2b9d4ee83dcaf8979d716a45e6a10`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 01:26:49 GMT
ADD file:ab87d4854aa8628ce8f4e603c0496499f6f28c3d2525ace782c7369691dafc8c in / 
# Sat, 10 Apr 2021 01:26:56 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 04:45:12 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 04:55:51 GMT
ENV HAPROXY_VERSION=2.2.13
# Sat, 10 Apr 2021 04:55:53 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.13.tar.gz
# Sat, 10 Apr 2021 04:55:57 GMT
ENV HAPROXY_SHA256=9e3e51441c70bedfb494fc9d4b4d3389a71be9a3c915ba3d6f7e8fd9a57ce160
# Sat, 10 Apr 2021 04:58:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 04:58:42 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 04:58:44 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 04:58:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 04:58:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 04:59:01 GMT
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
	-	`sha256:47d98ea7f5d6d0054eae8b1260b42df2c05e11015c73624875e953c2b5511090`  
		Last Modified: Sat, 10 Apr 2021 05:10:21 GMT  
		Size: 9.8 MB (9770127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a53dae98d3c653079c8dcee254bd233926f95fad7e2bf848e03a672956fd14`  
		Last Modified: Sat, 10 Apr 2021 05:10:19 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78cc95082c4533e2331bcf6b59f548c5ec2d66ac08321631a1350df97f7df0a5`  
		Last Modified: Sat, 10 Apr 2021 05:10:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; s390x

```console
$ docker pull haproxy@sha256:883a075a06023316a2ff2ff319689020b42812c4b6da7db73156722fb8e8614c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34759692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:812759d5bb748fe3ab35c1c945a594798c94ee29f65ab389f7d1b3ace8359191`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 10 Apr 2021 00:42:23 GMT
ADD file:dbe2182f8699f2a6011413ea01862e6c0e85853d922dffd72a28d994d23c79bc in / 
# Sat, 10 Apr 2021 00:42:25 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:38:04 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Sat, 10 Apr 2021 01:39:35 GMT
ENV HAPROXY_VERSION=2.2.13
# Sat, 10 Apr 2021 01:39:35 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.13.tar.gz
# Sat, 10 Apr 2021 01:39:36 GMT
ENV HAPROXY_SHA256=9e3e51441c70bedfb494fc9d4b4d3389a71be9a3c915ba3d6f7e8fd9a57ce160
# Sat, 10 Apr 2021 01:40:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 10 Apr 2021 01:40:07 GMT
STOPSIGNAL SIGUSR1
# Sat, 10 Apr 2021 01:40:07 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 10 Apr 2021 01:40:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Sat, 10 Apr 2021 01:40:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 10 Apr 2021 01:40:08 GMT
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
	-	`sha256:1ca81c5eef5f2d44f041789ed53dbfa0a6453bee245921eade23f4c550c190d8`  
		Last Modified: Sat, 10 Apr 2021 01:42:47 GMT  
		Size: 9.0 MB (9003958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0788fe9c0f74dcb98ef569fdf7251c230f9f2c4adcb7b03df2d7ecf36d8517e8`  
		Last Modified: Sat, 10 Apr 2021 01:42:45 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b6982746ce00451b99cf4beb0304c2d327fbaa5898f24a06c04ce6048d85149`  
		Last Modified: Sat, 10 Apr 2021 01:42:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:lts-alpine`

```console
$ docker pull haproxy@sha256:413f24a6ce6057afafb796d156e6b332bdcb37a28f499599aa7c9b4d1434cbbd
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
$ docker pull haproxy@sha256:51528e0da4c91c96e9451d07c0d79fa2c7ec359c9486006b6a2381adb50616ab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.2 MB (9183249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d94ea559268af6d140850108edea1185c786262681f3912e945b540caf8bf47`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:37:38 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 21:39:55 GMT
ENV HAPROXY_VERSION=2.2.13
# Wed, 14 Apr 2021 21:39:55 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.13.tar.gz
# Wed, 14 Apr 2021 21:39:55 GMT
ENV HAPROXY_SHA256=9e3e51441c70bedfb494fc9d4b4d3389a71be9a3c915ba3d6f7e8fd9a57ce160
# Wed, 14 Apr 2021 21:40:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 21:40:44 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 21:40:44 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 21:40:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 21:40:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 21:40:45 GMT
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
	-	`sha256:ba81e90af14a863a9b5685b5085eec923abff1890a6fd2a3f0e07994974e31d7`  
		Last Modified: Wed, 14 Apr 2021 21:44:03 GMT  
		Size: 6.4 MB (6369525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc0670e87880c224e8aaeffba5dcacdd308471d5f995f18cc7457f21d0a2a04`  
		Last Modified: Wed, 14 Apr 2021 21:44:02 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a009871a4c718317430f5cd8acafa4a1c6f3020f699c1e9a4b3b9e06540267c`  
		Last Modified: Wed, 14 Apr 2021 21:44:02 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts-alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:998908d9876cf5186d814914e16aad5bbf9f9fd36cd12e64ab2cf5cd2f9e21ef
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.9 MB (8873199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58b3a8c2e2ff9d47d90f2fb6f7661c6ee64bdb5ab6eb0577bbb9899bd8dceb42`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:18:05 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 21:24:17 GMT
ENV HAPROXY_VERSION=2.2.13
# Wed, 14 Apr 2021 21:24:26 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.13.tar.gz
# Wed, 14 Apr 2021 21:24:33 GMT
ENV HAPROXY_SHA256=9e3e51441c70bedfb494fc9d4b4d3389a71be9a3c915ba3d6f7e8fd9a57ce160
# Wed, 14 Apr 2021 21:25:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 21:26:12 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 21:26:21 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 21:26:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 21:26:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 21:27:07 GMT
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
	-	`sha256:1f961936d3b3f46a3711ffae66d510e2e3587ecc266ffc4228dc5bd3e348e588`  
		Last Modified: Wed, 14 Apr 2021 21:34:29 GMT  
		Size: 6.2 MB (6249312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f89851496a5733b45c2a26de344e1e0888de96a5b2d2c0daa7f0e6e2765ec37`  
		Last Modified: Wed, 14 Apr 2021 21:34:28 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065a09e958b3582c21934c8ef7a6fc65e4573d59cd9e486affab9e9d427bbe8e`  
		Last Modified: Wed, 14 Apr 2021 21:34:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:b7073b291f697c7935c86c245c86fee0cf05b1f51ea7192ccc0f8788a26b76cf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8591663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47b928f6c9cacabd2bcaae105d88e5d2fdeae2e042c3fd34b7b046c718e15150`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:47:58 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 22:52:15 GMT
ENV HAPROXY_VERSION=2.2.13
# Wed, 14 Apr 2021 22:52:18 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.13.tar.gz
# Wed, 14 Apr 2021 22:52:20 GMT
ENV HAPROXY_SHA256=9e3e51441c70bedfb494fc9d4b4d3389a71be9a3c915ba3d6f7e8fd9a57ce160
# Wed, 14 Apr 2021 22:52:54 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 22:52:56 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 22:52:57 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 22:53:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 22:53:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 22:53:04 GMT
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
	-	`sha256:a9db6c809add6fb1c65ed18e490e0aef9ceec249693f5014ad157e8989b2f97a`  
		Last Modified: Wed, 14 Apr 2021 22:56:40 GMT  
		Size: 6.2 MB (6165762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c54a8deef45aafe8d23348b71b1907c6930bd15e2cb8e9b3cbba14f225db81e3`  
		Last Modified: Wed, 14 Apr 2021 22:56:37 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3307625a9b488e9e1c508c95cd16dbee010765a6d9d5561c0723bc7a75a8d5b`  
		Last Modified: Wed, 14 Apr 2021 22:56:37 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:16bca21e897d7c52b2517cf4ba4e89c8ddb5e431b4cccad8fcc225eabcce25ca
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.1 MB (9088539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c6169d0eba5060ded320c17fa92adcdcdf3ee92545eb40d895e0544a4ef71cd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:26:01 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 20:30:39 GMT
ENV HAPROXY_VERSION=2.2.13
# Wed, 14 Apr 2021 20:30:46 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.13.tar.gz
# Wed, 14 Apr 2021 20:30:54 GMT
ENV HAPROXY_SHA256=9e3e51441c70bedfb494fc9d4b4d3389a71be9a3c915ba3d6f7e8fd9a57ce160
# Wed, 14 Apr 2021 20:31:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 20:31:49 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 20:31:50 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:32:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 20:32:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:32:21 GMT
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
	-	`sha256:3f46520f93f138b7f11e9721ba69bfde0f4f1da77e7b5ba2be9de502d0595b54`  
		Last Modified: Wed, 14 Apr 2021 20:38:18 GMT  
		Size: 6.4 MB (6374758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a83203e2d21398703492ebb3881e3ad57ae31c92251d8d94e7be21b51ac3a695`  
		Last Modified: Wed, 14 Apr 2021 20:38:16 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c812aee4a6ede81fd42bd6abae3c0f8300ef5222e074a574be9c861c6de4d0ac`  
		Last Modified: Wed, 14 Apr 2021 20:38:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts-alpine` - linux; 386

```console
$ docker pull haproxy@sha256:a0fbc701001da548b035064db09a6be1e31e17125183345e0a6e9183abb2cb4f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9023341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13c3c2ecf9cd56e8732956bd2c0b272bd99a5a2e5090755c3137696b34ee3889`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 01:50:06 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 15 Apr 2021 01:53:40 GMT
ENV HAPROXY_VERSION=2.2.13
# Thu, 15 Apr 2021 01:53:40 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.13.tar.gz
# Thu, 15 Apr 2021 01:53:40 GMT
ENV HAPROXY_SHA256=9e3e51441c70bedfb494fc9d4b4d3389a71be9a3c915ba3d6f7e8fd9a57ce160
# Thu, 15 Apr 2021 01:54:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 15 Apr 2021 01:54:44 GMT
STOPSIGNAL SIGUSR1
# Thu, 15 Apr 2021 01:54:44 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 15 Apr 2021 01:54:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Thu, 15 Apr 2021 01:54:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Apr 2021 01:54:45 GMT
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
	-	`sha256:dd83349dc27b7c6494b326db86b2fb5ab9fded96732b87dcbdfe7ffbf53eb6fd`  
		Last Modified: Thu, 15 Apr 2021 02:01:05 GMT  
		Size: 6.2 MB (6202686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df9e7c12c69c54a160be7a4c5497240b0dffff220b6d1eb44aa7977bc593d408`  
		Last Modified: Thu, 15 Apr 2021 02:01:04 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c24d7fe1943abc1fdfcdef29513a413337092d356e48d6b6b868c73ed4ca4b6b`  
		Last Modified: Thu, 15 Apr 2021 02:01:03 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts-alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:3176f25d3818aaecc48b0cb829219da0864af79b2564b8eecd5ebccfa4f40468
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9499255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27f33cdd58ab09da862b649ad36eb8667c6ee6018e65a43528c3d7a198a44b72`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:25:09 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 23:29:12 GMT
ENV HAPROXY_VERSION=2.2.13
# Wed, 14 Apr 2021 23:29:16 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.13.tar.gz
# Wed, 14 Apr 2021 23:29:20 GMT
ENV HAPROXY_SHA256=9e3e51441c70bedfb494fc9d4b4d3389a71be9a3c915ba3d6f7e8fd9a57ce160
# Wed, 14 Apr 2021 23:30:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 23:30:20 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 23:30:22 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 23:30:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 23:30:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 23:30:47 GMT
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
	-	`sha256:e8a3685c2ec0932a7f73fa0032bf33500306ee2a5d0abf655e8983b0c8a95acd`  
		Last Modified: Wed, 14 Apr 2021 23:37:09 GMT  
		Size: 6.7 MB (6684359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74885306f2f1ac242fa8c216d998632b927a5cd3678771077f7a7f650d8ba37d`  
		Last Modified: Wed, 14 Apr 2021 23:37:07 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32336bc725a4335e246865126dccc149331aa27ef4a8767172fb2cff483b4ca4`  
		Last Modified: Wed, 14 Apr 2021 23:37:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts-alpine` - linux; s390x

```console
$ docker pull haproxy@sha256:5fb7df6e38eea99e9f0e9d4a19cd193a5be4747420d5b38082dfc02df9fb6d1a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.9 MB (8940300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e32f238bf459522abbbbb20a287e8543faf16dd5307b7fa7da33e7edfe3f4b8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:54:24 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 14 Apr 2021 20:56:12 GMT
ENV HAPROXY_VERSION=2.2.13
# Wed, 14 Apr 2021 20:56:12 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.13.tar.gz
# Wed, 14 Apr 2021 20:56:12 GMT
ENV HAPROXY_SHA256=9e3e51441c70bedfb494fc9d4b4d3389a71be9a3c915ba3d6f7e8fd9a57ce160
# Wed, 14 Apr 2021 20:56:47 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 14 Apr 2021 20:56:47 GMT
STOPSIGNAL SIGUSR1
# Wed, 14 Apr 2021 20:56:47 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:56:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 14 Apr 2021 20:56:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:56:49 GMT
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
	-	`sha256:9b54506479f94cd6e6ff33fd666b2e4ef038a755e897f69c41e2024451738f22`  
		Last Modified: Wed, 14 Apr 2021 20:59:30 GMT  
		Size: 6.3 MB (6335894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b346055862205d30d0fec1cd13ad03e77403df88ae4b0e999a9fa3f2f5738371`  
		Last Modified: Wed, 14 Apr 2021 20:59:29 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1c0e6cd04f7bb776fd8fc6fcdd6ca22f1247acb507d44b41d9163155c7e5d9`  
		Last Modified: Wed, 14 Apr 2021 20:59:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
