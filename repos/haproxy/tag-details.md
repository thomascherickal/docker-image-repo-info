<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `haproxy`

-	[`haproxy:1.7`](#haproxy17)
-	[`haproxy:1.7.12`](#haproxy1712)
-	[`haproxy:1.7.12-alpine`](#haproxy1712-alpine)
-	[`haproxy:1.7-alpine`](#haproxy17-alpine)
-	[`haproxy:1.8`](#haproxy18)
-	[`haproxy:1.8.27`](#haproxy1827)
-	[`haproxy:1.8.27-alpine`](#haproxy1827-alpine)
-	[`haproxy:1.8-alpine`](#haproxy18-alpine)
-	[`haproxy:2.0`](#haproxy20)
-	[`haproxy:2.0.19`](#haproxy2019)
-	[`haproxy:2.0.19-alpine`](#haproxy2019-alpine)
-	[`haproxy:2.0-alpine`](#haproxy20-alpine)
-	[`haproxy:2.1`](#haproxy21)
-	[`haproxy:2.1.10`](#haproxy2110)
-	[`haproxy:2.1.10-alpine`](#haproxy2110-alpine)
-	[`haproxy:2.1-alpine`](#haproxy21-alpine)
-	[`haproxy:2.2`](#haproxy22)
-	[`haproxy:2.2.6`](#haproxy226)
-	[`haproxy:2.2.6-alpine`](#haproxy226-alpine)
-	[`haproxy:2.2-alpine`](#haproxy22-alpine)
-	[`haproxy:2.3`](#haproxy23)
-	[`haproxy:2.3.2`](#haproxy232)
-	[`haproxy:2.3.2-alpine`](#haproxy232-alpine)
-	[`haproxy:2.3-alpine`](#haproxy23-alpine)
-	[`haproxy:2.4-dev`](#haproxy24-dev)
-	[`haproxy:2.4-dev4`](#haproxy24-dev4)
-	[`haproxy:2.4-dev4-alpine`](#haproxy24-dev4-alpine)
-	[`haproxy:2.4-dev-alpine`](#haproxy24-dev-alpine)
-	[`haproxy:alpine`](#haproxyalpine)
-	[`haproxy:latest`](#haproxylatest)
-	[`haproxy:lts`](#haproxylts)
-	[`haproxy:lts-alpine`](#haproxylts-alpine)

## `haproxy:1.7`

```console
$ docker pull haproxy@sha256:09e3932c4bfe73bd9e636e2aa147966ae6a4f06dc6c2a426c5ed2d7ab93206a4
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
$ docker pull haproxy@sha256:9414e36ce3ca05ce3e54e44dbbf30f20c2e92cd9e0336a09201111d76083fa8e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.5 MB (32476615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff4844108237a4faf2d2875059125cfcf29a63d337625521000e399e96109bb2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:06:10 GMT
ADD file:3a7bff4e139bcacc5831fd70a035c130a91b5da001dd91c08b2acd635c7064e8 in / 
# Fri, 11 Dec 2020 02:06:10 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 06:45:47 GMT
ENV HAPROXY_VERSION=1.7.12
# Fri, 11 Dec 2020 06:45:47 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.12.tar.gz
# Fri, 11 Dec 2020 06:45:47 GMT
ENV HAPROXY_SHA256=4118178b553a107b227f3f84774c7a50ae0b3ac2be39211c3db511ed4efe48ce
# Fri, 11 Dec 2020 06:46:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 06:46:33 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 06:46:34 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in / 
# Fri, 11 Dec 2020 06:46:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 06:46:34 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:6ec7b7d162b24bd6df88abde89ceb6d7bbc2be927f025c9dd061af2b0c328cfe`  
		Last Modified: Fri, 11 Dec 2020 02:12:26 GMT  
		Size: 27.1 MB (27099295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d030faa6ae5f388944fcb884eb063c6f7622b03a5c033baf39f434f37185ab4e`  
		Last Modified: Fri, 11 Dec 2020 06:49:29 GMT  
		Size: 5.4 MB (5376916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:845c4d9e3cb079e43a64c67f6727bd19972e3e9d7ebefd75560428c387e3bd85`  
		Last Modified: Fri, 11 Dec 2020 06:49:27 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:27a90a8a3f7807d15ad2af235af5b5cd8e0b97f0a3c5666b0382eec056e4b250
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.9 MB (29852644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7221889583abf155ce2a11f07647c80666abd0007ebaa954500356a46df88fe`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:49 GMT
ADD file:58ebb3ffaf26d9b7621efba5f109ae9d22832f2f22865cda36604b138cbdb7b8 in / 
# Fri, 11 Dec 2020 02:04:56 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 03:33:01 GMT
ENV HAPROXY_VERSION=1.7.12
# Fri, 11 Dec 2020 03:33:04 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.12.tar.gz
# Fri, 11 Dec 2020 03:33:06 GMT
ENV HAPROXY_SHA256=4118178b553a107b227f3f84774c7a50ae0b3ac2be39211c3db511ed4efe48ce
# Fri, 11 Dec 2020 03:34:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 03:34:21 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 03:34:23 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in / 
# Fri, 11 Dec 2020 03:34:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:34:25 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:8cbd1f790d64c77fcac6c9dbfe4d4c82f0365de9438f1a42b0560dc88f9e6a55`  
		Last Modified: Fri, 11 Dec 2020 02:14:44 GMT  
		Size: 24.8 MB (24843461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c1e7de6b92c40843f49ce2901711e6879ab3043fdde9f600fb16484b95faa9f`  
		Last Modified: Fri, 11 Dec 2020 03:36:09 GMT  
		Size: 5.0 MB (5008780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15e77c3bffc8afd1e55c09283eac7cf6db84391ad74962ffbf3a388842797d94`  
		Last Modified: Fri, 11 Dec 2020 03:36:08 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:9f777d492dc92ef51e882b20e8218bc6f9db6189b524e3b3e230d6970b03542f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.6 MB (27583158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7f0b12e0ba540a2c8102165483ae77fb16243be41688aa8d431b5ed70ac623a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:23:37 GMT
ADD file:75ca842ac2d6e9f6617bb3df280af1e4c9619c9805fd5e00c1c3d6b8b4e3d802 in / 
# Fri, 11 Dec 2020 02:23:39 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 05:02:16 GMT
ENV HAPROXY_VERSION=1.7.12
# Fri, 11 Dec 2020 05:02:17 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.12.tar.gz
# Fri, 11 Dec 2020 05:02:18 GMT
ENV HAPROXY_SHA256=4118178b553a107b227f3f84774c7a50ae0b3ac2be39211c3db511ed4efe48ce
# Fri, 11 Dec 2020 05:03:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 05:03:08 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 05:03:09 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in / 
# Fri, 11 Dec 2020 05:03:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:03:13 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c06905228d4fc5a5c840a70e2e6ced56596a8bc73abc69e6a1867bbb6f7ae7e7`  
		Last Modified: Fri, 11 Dec 2020 02:33:07 GMT  
		Size: 22.7 MB (22707662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac9bcf32c8ac8dbf4bc8c6b365a54f7ba5764675e31703e0cf4a125a107372da`  
		Last Modified: Fri, 11 Dec 2020 05:07:06 GMT  
		Size: 4.9 MB (4875093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b8b3d38107548c19d33d1f5d6af88f4d17c76b07a2b1fc75f4615c8fd95985`  
		Last Modified: Fri, 11 Dec 2020 05:07:05 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:cc7add3bfb66092cf8fe4e27547e721516285705a578d05d45b1b44135110eb7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.1 MB (31120648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1234689747e4f50a7daecc5b62512fd1c4b2ff93c4eb051730f7ba6599d06be`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:45:53 GMT
ADD file:a5a2f039c00bc638b88cefdff4c3cd1865b4d415bf80c4fe6b496d975af7cc1f in / 
# Fri, 11 Dec 2020 02:45:57 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 05:41:33 GMT
ENV HAPROXY_VERSION=1.7.12
# Fri, 11 Dec 2020 05:41:34 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.12.tar.gz
# Fri, 11 Dec 2020 05:41:35 GMT
ENV HAPROXY_SHA256=4118178b553a107b227f3f84774c7a50ae0b3ac2be39211c3db511ed4efe48ce
# Fri, 11 Dec 2020 05:42:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 05:42:18 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 05:42:19 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in / 
# Fri, 11 Dec 2020 05:42:20 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:42:21 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c9648d7fcbb6d597cf33916d8fcd207fde8ec05d764b4480d4f3e884e142a902`  
		Last Modified: Fri, 11 Dec 2020 02:53:14 GMT  
		Size: 25.9 MB (25856191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be39561ad734524af10ec544a6b121e0deb2d438b9af4715c0acd29eebc98913`  
		Last Modified: Fri, 11 Dec 2020 05:45:48 GMT  
		Size: 5.3 MB (5264054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba3502cbd0be33d633a0605cee9631de3fa9ef1fc3b4a26f4bfc532f663288e`  
		Last Modified: Fri, 11 Dec 2020 05:45:46 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7` - linux; 386

```console
$ docker pull haproxy@sha256:c65295388bb00b2eecbb4293ad62037db98ebc3a4b89bbc589e23edd5f18009d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.1 MB (33067407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ca347fd13ac049fb9433da39b28b5f9785c2f8f344087b0b1f84f06ac1a07de`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:07 GMT
ADD file:a0879774b23f70c4db7f7b04736cca142beb0b22e93f5952364ca990a1675552 in / 
# Fri, 11 Dec 2020 02:03:08 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 05:22:44 GMT
ENV HAPROXY_VERSION=1.7.12
# Fri, 11 Dec 2020 05:22:44 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.12.tar.gz
# Fri, 11 Dec 2020 05:22:44 GMT
ENV HAPROXY_SHA256=4118178b553a107b227f3f84774c7a50ae0b3ac2be39211c3db511ed4efe48ce
# Fri, 11 Dec 2020 05:23:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 05:23:45 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 05:23:46 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in / 
# Fri, 11 Dec 2020 05:23:46 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:23:47 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:cfec07a090788e68b692f30d34e11dc7af0f1c8112fbc846e8e40e24faf882d7`  
		Last Modified: Fri, 11 Dec 2020 02:09:41 GMT  
		Size: 27.8 MB (27757584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ff419be61a73bf4950281f036c85ee5dd6e3a12ce80dced05f5102e4ebd3d1`  
		Last Modified: Fri, 11 Dec 2020 05:26:56 GMT  
		Size: 5.3 MB (5309420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db3b480dc9246232b1ef1426974d23a4d96d774de49c8bdd7f24dafd70170171`  
		Last Modified: Fri, 11 Dec 2020 05:26:54 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7` - linux; mips64le

```console
$ docker pull haproxy@sha256:18b999f0f7c1455871eb1d5c8d85430ea65595ae3bec81589f79365fd1bc52d1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.8 MB (30783741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1a89db3c05cb4a74c930939761727d8e71ece0298d6c63622c9e0f21b59af66`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:30 GMT
ADD file:edb758d587972f30ef28b162dcabf79f61b685afa3c6066cb611c61abea124f3 in / 
# Fri, 11 Dec 2020 02:03:30 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 03:30:35 GMT
ENV HAPROXY_VERSION=1.7.12
# Fri, 11 Dec 2020 03:30:36 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.12.tar.gz
# Fri, 11 Dec 2020 03:30:36 GMT
ENV HAPROXY_SHA256=4118178b553a107b227f3f84774c7a50ae0b3ac2be39211c3db511ed4efe48ce
# Fri, 11 Dec 2020 03:32:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 03:32:01 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 03:32:02 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in / 
# Fri, 11 Dec 2020 03:32:02 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:32:02 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:bed35f8e8e003f268bd91c8bc28d93f0b1463296add14ab3ec84c3d3d30e9025`  
		Last Modified: Fri, 11 Dec 2020 02:10:15 GMT  
		Size: 25.8 MB (25769881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646012770a35e1ecdf2865c2c718982c05ac904c23ba12b5e484af6a4230e3d2`  
		Last Modified: Fri, 11 Dec 2020 03:34:44 GMT  
		Size: 5.0 MB (5013457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2ce3078f41be2885f8b9f60a4c0663ed977e23656386fe3c6e5c0fcaa27dce`  
		Last Modified: Fri, 11 Dec 2020 03:34:40 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7` - linux; ppc64le

```console
$ docker pull haproxy@sha256:4b6c1b5c2af59fb97dcf722f5419de0ee854d6ca3d4b5a438865882736552d60
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.2 MB (36218479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c78bb2fd533ef9f9e1c955253df8dd273d9287587373d63fd117d8e0f795503`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 03:34:02 GMT
ADD file:eca1a7737bd5e84ff883c4c284c0cd22492145d9cd7ae3b8e7b490e3d8e5aefb in / 
# Fri, 11 Dec 2020 03:34:11 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 05:48:19 GMT
ENV HAPROXY_VERSION=1.7.12
# Fri, 11 Dec 2020 05:48:22 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.12.tar.gz
# Fri, 11 Dec 2020 05:48:27 GMT
ENV HAPROXY_SHA256=4118178b553a107b227f3f84774c7a50ae0b3ac2be39211c3db511ed4efe48ce
# Fri, 11 Dec 2020 05:50:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 05:51:06 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 05:51:08 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in / 
# Fri, 11 Dec 2020 05:51:13 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:51:17 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c0f0648876332890be87a9f32ec4ad2a939e805be3152ab991a923f7dec2b35d`  
		Last Modified: Fri, 11 Dec 2020 03:41:39 GMT  
		Size: 30.5 MB (30524717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e726de6f39e000e402a89a7f43aa01ea1f0ec8dfcc30a4c2ae038fd29f7a15ab`  
		Last Modified: Fri, 11 Dec 2020 05:55:53 GMT  
		Size: 5.7 MB (5693359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dbb4dfb74ffed4b91ac0463a9724e33d68837da6b6bbfcd1e2bab50dbb8c799`  
		Last Modified: Fri, 11 Dec 2020 05:55:52 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7` - linux; s390x

```console
$ docker pull haproxy@sha256:df888e7ca557499dce5964bc5324fb4db24322750dbb8cb9105007b3a7b24b51
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.8 MB (30823639 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f52af7535f6bdcd2c613a1ecffb1bae7d41daf509ff013041973ed55ab362905`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:12:11 GMT
ADD file:db86ce5a1665b6d8ac734c54ac249a811c58484f569b935b14772445962428aa in / 
# Fri, 11 Dec 2020 02:12:15 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 03:25:47 GMT
ENV HAPROXY_VERSION=1.7.12
# Fri, 11 Dec 2020 03:25:48 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.12.tar.gz
# Fri, 11 Dec 2020 03:25:49 GMT
ENV HAPROXY_SHA256=4118178b553a107b227f3f84774c7a50ae0b3ac2be39211c3db511ed4efe48ce
# Fri, 11 Dec 2020 03:26:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 03:26:22 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 03:26:23 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in / 
# Fri, 11 Dec 2020 03:26:23 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:26:24 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:f4cf10ca9f31aab0854647d7878dc4db838e93b892b843dde3db24f2e909a106`  
		Last Modified: Fri, 11 Dec 2020 02:17:07 GMT  
		Size: 25.7 MB (25713957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86228931bf47464d019f11e9ade0c7a123bcfbfbb0b49e91d719d6a9e7b31234`  
		Last Modified: Fri, 11 Dec 2020 03:29:30 GMT  
		Size: 5.1 MB (5109279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66c3b5d7736c39a0fd251b30b48d90372418b6d4468da7f178b5a5267bdd61e`  
		Last Modified: Fri, 11 Dec 2020 03:29:30 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:1.7.12`

```console
$ docker pull haproxy@sha256:09e3932c4bfe73bd9e636e2aa147966ae6a4f06dc6c2a426c5ed2d7ab93206a4
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

### `haproxy:1.7.12` - linux; amd64

```console
$ docker pull haproxy@sha256:9414e36ce3ca05ce3e54e44dbbf30f20c2e92cd9e0336a09201111d76083fa8e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.5 MB (32476615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff4844108237a4faf2d2875059125cfcf29a63d337625521000e399e96109bb2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:06:10 GMT
ADD file:3a7bff4e139bcacc5831fd70a035c130a91b5da001dd91c08b2acd635c7064e8 in / 
# Fri, 11 Dec 2020 02:06:10 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 06:45:47 GMT
ENV HAPROXY_VERSION=1.7.12
# Fri, 11 Dec 2020 06:45:47 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.12.tar.gz
# Fri, 11 Dec 2020 06:45:47 GMT
ENV HAPROXY_SHA256=4118178b553a107b227f3f84774c7a50ae0b3ac2be39211c3db511ed4efe48ce
# Fri, 11 Dec 2020 06:46:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 06:46:33 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 06:46:34 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in / 
# Fri, 11 Dec 2020 06:46:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 06:46:34 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:6ec7b7d162b24bd6df88abde89ceb6d7bbc2be927f025c9dd061af2b0c328cfe`  
		Last Modified: Fri, 11 Dec 2020 02:12:26 GMT  
		Size: 27.1 MB (27099295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d030faa6ae5f388944fcb884eb063c6f7622b03a5c033baf39f434f37185ab4e`  
		Last Modified: Fri, 11 Dec 2020 06:49:29 GMT  
		Size: 5.4 MB (5376916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:845c4d9e3cb079e43a64c67f6727bd19972e3e9d7ebefd75560428c387e3bd85`  
		Last Modified: Fri, 11 Dec 2020 06:49:27 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7.12` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:27a90a8a3f7807d15ad2af235af5b5cd8e0b97f0a3c5666b0382eec056e4b250
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.9 MB (29852644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7221889583abf155ce2a11f07647c80666abd0007ebaa954500356a46df88fe`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:49 GMT
ADD file:58ebb3ffaf26d9b7621efba5f109ae9d22832f2f22865cda36604b138cbdb7b8 in / 
# Fri, 11 Dec 2020 02:04:56 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 03:33:01 GMT
ENV HAPROXY_VERSION=1.7.12
# Fri, 11 Dec 2020 03:33:04 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.12.tar.gz
# Fri, 11 Dec 2020 03:33:06 GMT
ENV HAPROXY_SHA256=4118178b553a107b227f3f84774c7a50ae0b3ac2be39211c3db511ed4efe48ce
# Fri, 11 Dec 2020 03:34:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 03:34:21 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 03:34:23 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in / 
# Fri, 11 Dec 2020 03:34:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:34:25 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:8cbd1f790d64c77fcac6c9dbfe4d4c82f0365de9438f1a42b0560dc88f9e6a55`  
		Last Modified: Fri, 11 Dec 2020 02:14:44 GMT  
		Size: 24.8 MB (24843461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c1e7de6b92c40843f49ce2901711e6879ab3043fdde9f600fb16484b95faa9f`  
		Last Modified: Fri, 11 Dec 2020 03:36:09 GMT  
		Size: 5.0 MB (5008780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15e77c3bffc8afd1e55c09283eac7cf6db84391ad74962ffbf3a388842797d94`  
		Last Modified: Fri, 11 Dec 2020 03:36:08 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7.12` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:9f777d492dc92ef51e882b20e8218bc6f9db6189b524e3b3e230d6970b03542f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.6 MB (27583158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7f0b12e0ba540a2c8102165483ae77fb16243be41688aa8d431b5ed70ac623a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:23:37 GMT
ADD file:75ca842ac2d6e9f6617bb3df280af1e4c9619c9805fd5e00c1c3d6b8b4e3d802 in / 
# Fri, 11 Dec 2020 02:23:39 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 05:02:16 GMT
ENV HAPROXY_VERSION=1.7.12
# Fri, 11 Dec 2020 05:02:17 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.12.tar.gz
# Fri, 11 Dec 2020 05:02:18 GMT
ENV HAPROXY_SHA256=4118178b553a107b227f3f84774c7a50ae0b3ac2be39211c3db511ed4efe48ce
# Fri, 11 Dec 2020 05:03:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 05:03:08 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 05:03:09 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in / 
# Fri, 11 Dec 2020 05:03:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:03:13 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c06905228d4fc5a5c840a70e2e6ced56596a8bc73abc69e6a1867bbb6f7ae7e7`  
		Last Modified: Fri, 11 Dec 2020 02:33:07 GMT  
		Size: 22.7 MB (22707662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac9bcf32c8ac8dbf4bc8c6b365a54f7ba5764675e31703e0cf4a125a107372da`  
		Last Modified: Fri, 11 Dec 2020 05:07:06 GMT  
		Size: 4.9 MB (4875093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b8b3d38107548c19d33d1f5d6af88f4d17c76b07a2b1fc75f4615c8fd95985`  
		Last Modified: Fri, 11 Dec 2020 05:07:05 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7.12` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:cc7add3bfb66092cf8fe4e27547e721516285705a578d05d45b1b44135110eb7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.1 MB (31120648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1234689747e4f50a7daecc5b62512fd1c4b2ff93c4eb051730f7ba6599d06be`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:45:53 GMT
ADD file:a5a2f039c00bc638b88cefdff4c3cd1865b4d415bf80c4fe6b496d975af7cc1f in / 
# Fri, 11 Dec 2020 02:45:57 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 05:41:33 GMT
ENV HAPROXY_VERSION=1.7.12
# Fri, 11 Dec 2020 05:41:34 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.12.tar.gz
# Fri, 11 Dec 2020 05:41:35 GMT
ENV HAPROXY_SHA256=4118178b553a107b227f3f84774c7a50ae0b3ac2be39211c3db511ed4efe48ce
# Fri, 11 Dec 2020 05:42:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 05:42:18 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 05:42:19 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in / 
# Fri, 11 Dec 2020 05:42:20 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:42:21 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c9648d7fcbb6d597cf33916d8fcd207fde8ec05d764b4480d4f3e884e142a902`  
		Last Modified: Fri, 11 Dec 2020 02:53:14 GMT  
		Size: 25.9 MB (25856191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be39561ad734524af10ec544a6b121e0deb2d438b9af4715c0acd29eebc98913`  
		Last Modified: Fri, 11 Dec 2020 05:45:48 GMT  
		Size: 5.3 MB (5264054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba3502cbd0be33d633a0605cee9631de3fa9ef1fc3b4a26f4bfc532f663288e`  
		Last Modified: Fri, 11 Dec 2020 05:45:46 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7.12` - linux; 386

```console
$ docker pull haproxy@sha256:c65295388bb00b2eecbb4293ad62037db98ebc3a4b89bbc589e23edd5f18009d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.1 MB (33067407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ca347fd13ac049fb9433da39b28b5f9785c2f8f344087b0b1f84f06ac1a07de`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:07 GMT
ADD file:a0879774b23f70c4db7f7b04736cca142beb0b22e93f5952364ca990a1675552 in / 
# Fri, 11 Dec 2020 02:03:08 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 05:22:44 GMT
ENV HAPROXY_VERSION=1.7.12
# Fri, 11 Dec 2020 05:22:44 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.12.tar.gz
# Fri, 11 Dec 2020 05:22:44 GMT
ENV HAPROXY_SHA256=4118178b553a107b227f3f84774c7a50ae0b3ac2be39211c3db511ed4efe48ce
# Fri, 11 Dec 2020 05:23:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 05:23:45 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 05:23:46 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in / 
# Fri, 11 Dec 2020 05:23:46 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:23:47 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:cfec07a090788e68b692f30d34e11dc7af0f1c8112fbc846e8e40e24faf882d7`  
		Last Modified: Fri, 11 Dec 2020 02:09:41 GMT  
		Size: 27.8 MB (27757584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ff419be61a73bf4950281f036c85ee5dd6e3a12ce80dced05f5102e4ebd3d1`  
		Last Modified: Fri, 11 Dec 2020 05:26:56 GMT  
		Size: 5.3 MB (5309420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db3b480dc9246232b1ef1426974d23a4d96d774de49c8bdd7f24dafd70170171`  
		Last Modified: Fri, 11 Dec 2020 05:26:54 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7.12` - linux; mips64le

```console
$ docker pull haproxy@sha256:18b999f0f7c1455871eb1d5c8d85430ea65595ae3bec81589f79365fd1bc52d1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.8 MB (30783741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1a89db3c05cb4a74c930939761727d8e71ece0298d6c63622c9e0f21b59af66`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:30 GMT
ADD file:edb758d587972f30ef28b162dcabf79f61b685afa3c6066cb611c61abea124f3 in / 
# Fri, 11 Dec 2020 02:03:30 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 03:30:35 GMT
ENV HAPROXY_VERSION=1.7.12
# Fri, 11 Dec 2020 03:30:36 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.12.tar.gz
# Fri, 11 Dec 2020 03:30:36 GMT
ENV HAPROXY_SHA256=4118178b553a107b227f3f84774c7a50ae0b3ac2be39211c3db511ed4efe48ce
# Fri, 11 Dec 2020 03:32:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 03:32:01 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 03:32:02 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in / 
# Fri, 11 Dec 2020 03:32:02 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:32:02 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:bed35f8e8e003f268bd91c8bc28d93f0b1463296add14ab3ec84c3d3d30e9025`  
		Last Modified: Fri, 11 Dec 2020 02:10:15 GMT  
		Size: 25.8 MB (25769881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646012770a35e1ecdf2865c2c718982c05ac904c23ba12b5e484af6a4230e3d2`  
		Last Modified: Fri, 11 Dec 2020 03:34:44 GMT  
		Size: 5.0 MB (5013457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2ce3078f41be2885f8b9f60a4c0663ed977e23656386fe3c6e5c0fcaa27dce`  
		Last Modified: Fri, 11 Dec 2020 03:34:40 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7.12` - linux; ppc64le

```console
$ docker pull haproxy@sha256:4b6c1b5c2af59fb97dcf722f5419de0ee854d6ca3d4b5a438865882736552d60
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.2 MB (36218479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c78bb2fd533ef9f9e1c955253df8dd273d9287587373d63fd117d8e0f795503`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 03:34:02 GMT
ADD file:eca1a7737bd5e84ff883c4c284c0cd22492145d9cd7ae3b8e7b490e3d8e5aefb in / 
# Fri, 11 Dec 2020 03:34:11 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 05:48:19 GMT
ENV HAPROXY_VERSION=1.7.12
# Fri, 11 Dec 2020 05:48:22 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.12.tar.gz
# Fri, 11 Dec 2020 05:48:27 GMT
ENV HAPROXY_SHA256=4118178b553a107b227f3f84774c7a50ae0b3ac2be39211c3db511ed4efe48ce
# Fri, 11 Dec 2020 05:50:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 05:51:06 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 05:51:08 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in / 
# Fri, 11 Dec 2020 05:51:13 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:51:17 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c0f0648876332890be87a9f32ec4ad2a939e805be3152ab991a923f7dec2b35d`  
		Last Modified: Fri, 11 Dec 2020 03:41:39 GMT  
		Size: 30.5 MB (30524717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e726de6f39e000e402a89a7f43aa01ea1f0ec8dfcc30a4c2ae038fd29f7a15ab`  
		Last Modified: Fri, 11 Dec 2020 05:55:53 GMT  
		Size: 5.7 MB (5693359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dbb4dfb74ffed4b91ac0463a9724e33d68837da6b6bbfcd1e2bab50dbb8c799`  
		Last Modified: Fri, 11 Dec 2020 05:55:52 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7.12` - linux; s390x

```console
$ docker pull haproxy@sha256:df888e7ca557499dce5964bc5324fb4db24322750dbb8cb9105007b3a7b24b51
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.8 MB (30823639 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f52af7535f6bdcd2c613a1ecffb1bae7d41daf509ff013041973ed55ab362905`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:12:11 GMT
ADD file:db86ce5a1665b6d8ac734c54ac249a811c58484f569b935b14772445962428aa in / 
# Fri, 11 Dec 2020 02:12:15 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 03:25:47 GMT
ENV HAPROXY_VERSION=1.7.12
# Fri, 11 Dec 2020 03:25:48 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.12.tar.gz
# Fri, 11 Dec 2020 03:25:49 GMT
ENV HAPROXY_SHA256=4118178b553a107b227f3f84774c7a50ae0b3ac2be39211c3db511ed4efe48ce
# Fri, 11 Dec 2020 03:26:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 03:26:22 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 03:26:23 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in / 
# Fri, 11 Dec 2020 03:26:23 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:26:24 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:f4cf10ca9f31aab0854647d7878dc4db838e93b892b843dde3db24f2e909a106`  
		Last Modified: Fri, 11 Dec 2020 02:17:07 GMT  
		Size: 25.7 MB (25713957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86228931bf47464d019f11e9ade0c7a123bcfbfbb0b49e91d719d6a9e7b31234`  
		Last Modified: Fri, 11 Dec 2020 03:29:30 GMT  
		Size: 5.1 MB (5109279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66c3b5d7736c39a0fd251b30b48d90372418b6d4468da7f178b5a5267bdd61e`  
		Last Modified: Fri, 11 Dec 2020 03:29:30 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:1.7.12-alpine`

```console
$ docker pull haproxy@sha256:022f91b3d371c69e790773a3052a021203eb4c885f8a1b136ba028c128116622
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

### `haproxy:1.7.12-alpine` - linux; amd64

```console
$ docker pull haproxy@sha256:700d85614f959bbb5e7a2997af991a5544499d07d5c2d89bbe877db1bb8ff2c5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.5 MB (3543449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c902c847c338435d3206eeaaf08e80d9dc636163d147a7fac3389fd65a02941`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:36:41 GMT
ENV HAPROXY_VERSION=1.7.12
# Thu, 17 Dec 2020 13:36:42 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.12.tar.gz
# Thu, 17 Dec 2020 13:36:42 GMT
ENV HAPROXY_SHA256=4118178b553a107b227f3f84774c7a50ae0b3ac2be39211c3db511ed4efe48ce
# Thu, 17 Dec 2020 13:36:56 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		CFLAGS+="-Wno-address-of-packed-member" 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 13:36:56 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 13:36:57 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in / 
# Thu, 17 Dec 2020 13:36:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 13:36:57 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:813bb106fbccc589a259dcc2a755c17a3a85d166d419763baaf3eddda09413b2`  
		Last Modified: Thu, 17 Dec 2020 13:38:57 GMT  
		Size: 744.0 KB (743981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aba7f20857be65be3c9ae2da19d4d93fbae8bb62a0ef3a4c1f293b5c32c6f029`  
		Last Modified: Thu, 17 Dec 2020 13:38:57 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7.12-alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:5880a3e74e53cdc147e362ad81411c86c91ee7ae54f543dd227799dbd2c9e314
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 MB (3319823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b56727b3c6abe2b82dd37ed3e1c0a6140c6a461b6eb93eab6808f352870cdccb`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:40:16 GMT
ENV HAPROXY_VERSION=1.7.12
# Thu, 17 Dec 2020 01:40:16 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.12.tar.gz
# Thu, 17 Dec 2020 01:40:17 GMT
ENV HAPROXY_SHA256=4118178b553a107b227f3f84774c7a50ae0b3ac2be39211c3db511ed4efe48ce
# Thu, 17 Dec 2020 01:40:28 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		CFLAGS+="-Wno-address-of-packed-member" 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:40:29 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:40:30 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in / 
# Thu, 17 Dec 2020 01:40:31 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:40:32 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8035300c37d6944e3e0695c06b1fbaa49df942bb11799a2e3f74733b7fd37db9`  
		Last Modified: Thu, 17 Dec 2020 01:42:15 GMT  
		Size: 715.3 KB (715258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c70f59266efc8ecf62b417d51e6701187a95d3aa77ddaa6693e9a8be4e8eb4a`  
		Last Modified: Thu, 17 Dec 2020 01:42:15 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7.12-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:4ee7c0a140bf0d68206684c8156aee50a82f1bd661363b8e5df68d4617e7acb9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3081221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28e243e2ccd54b13835be0fc57c555cc7e13ffebe95db74f8532e8302b5d7e04`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:42:06 GMT
ENV HAPROXY_VERSION=1.7.12
# Thu, 17 Dec 2020 01:42:07 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.12.tar.gz
# Thu, 17 Dec 2020 01:42:07 GMT
ENV HAPROXY_SHA256=4118178b553a107b227f3f84774c7a50ae0b3ac2be39211c3db511ed4efe48ce
# Thu, 17 Dec 2020 01:42:15 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		CFLAGS+="-Wno-address-of-packed-member" 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:42:16 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:42:17 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in / 
# Thu, 17 Dec 2020 01:42:18 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:42:19 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98a0727b8057547be245454ff3274f49d1a39c81b7aec799a048a223dcb2f812`  
		Last Modified: Thu, 17 Dec 2020 01:44:21 GMT  
		Size: 673.3 KB (673264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d17c36b801b4d7c85b29aff960f39e342fa985b1bfb76849bcb09bd11c632250`  
		Last Modified: Thu, 17 Dec 2020 01:44:21 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7.12-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:98f51b54234d8ba2f373d717d83ef084858ff55f132acc25bd1588ea3166abce
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3429678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90be8842212740ba05a4526435a59208f6d268b6e16f01306177bb5a974c2300`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:28:35 GMT
ENV HAPROXY_VERSION=1.7.12
# Thu, 17 Dec 2020 01:28:36 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.12.tar.gz
# Thu, 17 Dec 2020 01:28:37 GMT
ENV HAPROXY_SHA256=4118178b553a107b227f3f84774c7a50ae0b3ac2be39211c3db511ed4efe48ce
# Thu, 17 Dec 2020 01:28:49 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		CFLAGS+="-Wno-address-of-packed-member" 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:28:52 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:28:54 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in / 
# Thu, 17 Dec 2020 01:28:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:29:06 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0541b74f0efe50b30eba532ee11055d485f2e6cc48f6d6a48459952f27ebdbcd`  
		Last Modified: Thu, 17 Dec 2020 01:31:21 GMT  
		Size: 720.2 KB (720228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:697d23aa30d3fcd1a18da4a1b8650cd4c8590ee780465a79fee9d0ef52da23e5`  
		Last Modified: Thu, 17 Dec 2020 01:31:21 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7.12-alpine` - linux; 386

```console
$ docker pull haproxy@sha256:f12dfde475994ef60095ad7ca405a41e8c93505dbfaf70e213557d47e28c928c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3550338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95e9edd220350abde75e148e3292872e9deda276c6b4f9695f648d9a451393f8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 17 Dec 2020 00:38:32 GMT
ADD file:de33fda50a142403e842620d20bc4404e66fc4ace16edc6946c4539e8a797458 in / 
# Thu, 17 Dec 2020 00:38:32 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:33:26 GMT
ENV HAPROXY_VERSION=1.7.12
# Thu, 17 Dec 2020 02:33:26 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.12.tar.gz
# Thu, 17 Dec 2020 02:33:26 GMT
ENV HAPROXY_SHA256=4118178b553a107b227f3f84774c7a50ae0b3ac2be39211c3db511ed4efe48ce
# Thu, 17 Dec 2020 02:33:41 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		CFLAGS+="-Wno-address-of-packed-member" 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 02:33:42 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 02:33:42 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in / 
# Thu, 17 Dec 2020 02:33:42 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 02:33:42 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:455793c72b878001f0905634ed52a2524ba51796e7377bf00683a85123f7dce9`  
		Last Modified: Thu, 17 Dec 2020 00:39:18 GMT  
		Size: 2.8 MB (2794130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60b0c246534b37a6d37358e8fab44407698b57a4d3e49358a57a9bf596d0b68`  
		Last Modified: Thu, 17 Dec 2020 02:35:28 GMT  
		Size: 755.8 KB (755805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aea5af05952691435ce998dbabd26e514c49c77894b27e19122ede0bd7840b3`  
		Last Modified: Thu, 17 Dec 2020 02:35:28 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7.12-alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:da3f454ded34b8f2da9c49f0418aa47527a7d858f53d13bef39ad479969bbe82
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3569811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:997b9ba8df2291ab889815cc8f70f5c671bcdf8d7723287def174c63bd899773`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 17 Dec 2020 00:20:42 GMT
ADD file:0a38c9b4955f8faa79627c166fca80ef342e443a16ce2925a30eeae317bbd786 in / 
# Thu, 17 Dec 2020 00:20:48 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:48:03 GMT
ENV HAPROXY_VERSION=1.7.12
# Thu, 17 Dec 2020 02:48:06 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.12.tar.gz
# Thu, 17 Dec 2020 02:48:13 GMT
ENV HAPROXY_SHA256=4118178b553a107b227f3f84774c7a50ae0b3ac2be39211c3db511ed4efe48ce
# Thu, 17 Dec 2020 02:48:33 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		CFLAGS+="-Wno-address-of-packed-member" 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 02:48:38 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 02:48:40 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in / 
# Thu, 17 Dec 2020 02:48:44 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 02:48:46 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:a9d343b7bcc225fe7ac17d96a81329510ab7f31a50472311cafe7168d3107317`  
		Last Modified: Thu, 17 Dec 2020 00:21:33 GMT  
		Size: 2.8 MB (2805226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:116e4360bd7d117192c5ecbb74432f12def2735de6d0b0fe4258922793a3a6e6`  
		Last Modified: Thu, 17 Dec 2020 02:51:15 GMT  
		Size: 764.2 KB (764182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b48dfc22e1e98fd561e550405947daef0c49845b39d35934e4de496f7d215549`  
		Last Modified: Thu, 17 Dec 2020 02:51:14 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7.12-alpine` - linux; s390x

```console
$ docker pull haproxy@sha256:b105af9122ab3f9de11dda8ef4e6de86cfa37c7861e7797577197af33926c945
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 MB (3341923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7a771e303abfe548e9564998d535fe9b867b435c6dcdc03efb439ddd2d73a46`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:41:37 GMT
ADD file:3ad3856d165e8760af85574a8ffa75ca44b7e1b97b64d1d6d4608445efa4b860 in / 
# Wed, 16 Dec 2020 23:41:37 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:30:05 GMT
ENV HAPROXY_VERSION=1.7.12
# Thu, 17 Dec 2020 01:30:06 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.12.tar.gz
# Thu, 17 Dec 2020 01:30:06 GMT
ENV HAPROXY_SHA256=4118178b553a107b227f3f84774c7a50ae0b3ac2be39211c3db511ed4efe48ce
# Thu, 17 Dec 2020 01:30:17 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		CFLAGS+="-Wno-address-of-packed-member" 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:30:17 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:30:18 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in / 
# Thu, 17 Dec 2020 01:30:18 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:30:19 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:ee52640a49e15b8b7c8edb66c2d048b26abdee8d828d6e5ef4e10a28cb15a84f`  
		Last Modified: Wed, 16 Dec 2020 23:42:15 GMT  
		Size: 2.6 MB (2567018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38236ead985252be78ac9676e92561c12f2e2a15f00ec7968864352bbd38c824`  
		Last Modified: Thu, 17 Dec 2020 01:32:28 GMT  
		Size: 774.5 KB (774501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b09e8374749034b4a72545d3ab4ed7a2a58cbdce94bcd43269ca6275705bedd3`  
		Last Modified: Thu, 17 Dec 2020 01:32:26 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:1.7-alpine`

```console
$ docker pull haproxy@sha256:022f91b3d371c69e790773a3052a021203eb4c885f8a1b136ba028c128116622
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
$ docker pull haproxy@sha256:700d85614f959bbb5e7a2997af991a5544499d07d5c2d89bbe877db1bb8ff2c5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.5 MB (3543449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c902c847c338435d3206eeaaf08e80d9dc636163d147a7fac3389fd65a02941`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:36:41 GMT
ENV HAPROXY_VERSION=1.7.12
# Thu, 17 Dec 2020 13:36:42 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.12.tar.gz
# Thu, 17 Dec 2020 13:36:42 GMT
ENV HAPROXY_SHA256=4118178b553a107b227f3f84774c7a50ae0b3ac2be39211c3db511ed4efe48ce
# Thu, 17 Dec 2020 13:36:56 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		CFLAGS+="-Wno-address-of-packed-member" 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 13:36:56 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 13:36:57 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in / 
# Thu, 17 Dec 2020 13:36:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 13:36:57 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:813bb106fbccc589a259dcc2a755c17a3a85d166d419763baaf3eddda09413b2`  
		Last Modified: Thu, 17 Dec 2020 13:38:57 GMT  
		Size: 744.0 KB (743981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aba7f20857be65be3c9ae2da19d4d93fbae8bb62a0ef3a4c1f293b5c32c6f029`  
		Last Modified: Thu, 17 Dec 2020 13:38:57 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7-alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:5880a3e74e53cdc147e362ad81411c86c91ee7ae54f543dd227799dbd2c9e314
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 MB (3319823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b56727b3c6abe2b82dd37ed3e1c0a6140c6a461b6eb93eab6808f352870cdccb`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:40:16 GMT
ENV HAPROXY_VERSION=1.7.12
# Thu, 17 Dec 2020 01:40:16 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.12.tar.gz
# Thu, 17 Dec 2020 01:40:17 GMT
ENV HAPROXY_SHA256=4118178b553a107b227f3f84774c7a50ae0b3ac2be39211c3db511ed4efe48ce
# Thu, 17 Dec 2020 01:40:28 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		CFLAGS+="-Wno-address-of-packed-member" 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:40:29 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:40:30 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in / 
# Thu, 17 Dec 2020 01:40:31 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:40:32 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8035300c37d6944e3e0695c06b1fbaa49df942bb11799a2e3f74733b7fd37db9`  
		Last Modified: Thu, 17 Dec 2020 01:42:15 GMT  
		Size: 715.3 KB (715258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c70f59266efc8ecf62b417d51e6701187a95d3aa77ddaa6693e9a8be4e8eb4a`  
		Last Modified: Thu, 17 Dec 2020 01:42:15 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:4ee7c0a140bf0d68206684c8156aee50a82f1bd661363b8e5df68d4617e7acb9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3081221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28e243e2ccd54b13835be0fc57c555cc7e13ffebe95db74f8532e8302b5d7e04`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:42:06 GMT
ENV HAPROXY_VERSION=1.7.12
# Thu, 17 Dec 2020 01:42:07 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.12.tar.gz
# Thu, 17 Dec 2020 01:42:07 GMT
ENV HAPROXY_SHA256=4118178b553a107b227f3f84774c7a50ae0b3ac2be39211c3db511ed4efe48ce
# Thu, 17 Dec 2020 01:42:15 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		CFLAGS+="-Wno-address-of-packed-member" 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:42:16 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:42:17 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in / 
# Thu, 17 Dec 2020 01:42:18 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:42:19 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98a0727b8057547be245454ff3274f49d1a39c81b7aec799a048a223dcb2f812`  
		Last Modified: Thu, 17 Dec 2020 01:44:21 GMT  
		Size: 673.3 KB (673264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d17c36b801b4d7c85b29aff960f39e342fa985b1bfb76849bcb09bd11c632250`  
		Last Modified: Thu, 17 Dec 2020 01:44:21 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:98f51b54234d8ba2f373d717d83ef084858ff55f132acc25bd1588ea3166abce
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3429678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90be8842212740ba05a4526435a59208f6d268b6e16f01306177bb5a974c2300`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:28:35 GMT
ENV HAPROXY_VERSION=1.7.12
# Thu, 17 Dec 2020 01:28:36 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.12.tar.gz
# Thu, 17 Dec 2020 01:28:37 GMT
ENV HAPROXY_SHA256=4118178b553a107b227f3f84774c7a50ae0b3ac2be39211c3db511ed4efe48ce
# Thu, 17 Dec 2020 01:28:49 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		CFLAGS+="-Wno-address-of-packed-member" 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:28:52 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:28:54 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in / 
# Thu, 17 Dec 2020 01:28:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:29:06 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0541b74f0efe50b30eba532ee11055d485f2e6cc48f6d6a48459952f27ebdbcd`  
		Last Modified: Thu, 17 Dec 2020 01:31:21 GMT  
		Size: 720.2 KB (720228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:697d23aa30d3fcd1a18da4a1b8650cd4c8590ee780465a79fee9d0ef52da23e5`  
		Last Modified: Thu, 17 Dec 2020 01:31:21 GMT  
		Size: 402.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7-alpine` - linux; 386

```console
$ docker pull haproxy@sha256:f12dfde475994ef60095ad7ca405a41e8c93505dbfaf70e213557d47e28c928c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3550338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95e9edd220350abde75e148e3292872e9deda276c6b4f9695f648d9a451393f8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 17 Dec 2020 00:38:32 GMT
ADD file:de33fda50a142403e842620d20bc4404e66fc4ace16edc6946c4539e8a797458 in / 
# Thu, 17 Dec 2020 00:38:32 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:33:26 GMT
ENV HAPROXY_VERSION=1.7.12
# Thu, 17 Dec 2020 02:33:26 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.12.tar.gz
# Thu, 17 Dec 2020 02:33:26 GMT
ENV HAPROXY_SHA256=4118178b553a107b227f3f84774c7a50ae0b3ac2be39211c3db511ed4efe48ce
# Thu, 17 Dec 2020 02:33:41 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		CFLAGS+="-Wno-address-of-packed-member" 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 02:33:42 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 02:33:42 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in / 
# Thu, 17 Dec 2020 02:33:42 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 02:33:42 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:455793c72b878001f0905634ed52a2524ba51796e7377bf00683a85123f7dce9`  
		Last Modified: Thu, 17 Dec 2020 00:39:18 GMT  
		Size: 2.8 MB (2794130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60b0c246534b37a6d37358e8fab44407698b57a4d3e49358a57a9bf596d0b68`  
		Last Modified: Thu, 17 Dec 2020 02:35:28 GMT  
		Size: 755.8 KB (755805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aea5af05952691435ce998dbabd26e514c49c77894b27e19122ede0bd7840b3`  
		Last Modified: Thu, 17 Dec 2020 02:35:28 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7-alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:da3f454ded34b8f2da9c49f0418aa47527a7d858f53d13bef39ad479969bbe82
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3569811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:997b9ba8df2291ab889815cc8f70f5c671bcdf8d7723287def174c63bd899773`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 17 Dec 2020 00:20:42 GMT
ADD file:0a38c9b4955f8faa79627c166fca80ef342e443a16ce2925a30eeae317bbd786 in / 
# Thu, 17 Dec 2020 00:20:48 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:48:03 GMT
ENV HAPROXY_VERSION=1.7.12
# Thu, 17 Dec 2020 02:48:06 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.12.tar.gz
# Thu, 17 Dec 2020 02:48:13 GMT
ENV HAPROXY_SHA256=4118178b553a107b227f3f84774c7a50ae0b3ac2be39211c3db511ed4efe48ce
# Thu, 17 Dec 2020 02:48:33 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		CFLAGS+="-Wno-address-of-packed-member" 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 02:48:38 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 02:48:40 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in / 
# Thu, 17 Dec 2020 02:48:44 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 02:48:46 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:a9d343b7bcc225fe7ac17d96a81329510ab7f31a50472311cafe7168d3107317`  
		Last Modified: Thu, 17 Dec 2020 00:21:33 GMT  
		Size: 2.8 MB (2805226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:116e4360bd7d117192c5ecbb74432f12def2735de6d0b0fe4258922793a3a6e6`  
		Last Modified: Thu, 17 Dec 2020 02:51:15 GMT  
		Size: 764.2 KB (764182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b48dfc22e1e98fd561e550405947daef0c49845b39d35934e4de496f7d215549`  
		Last Modified: Thu, 17 Dec 2020 02:51:14 GMT  
		Size: 403.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7-alpine` - linux; s390x

```console
$ docker pull haproxy@sha256:b105af9122ab3f9de11dda8ef4e6de86cfa37c7861e7797577197af33926c945
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 MB (3341923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7a771e303abfe548e9564998d535fe9b867b435c6dcdc03efb439ddd2d73a46`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:41:37 GMT
ADD file:3ad3856d165e8760af85574a8ffa75ca44b7e1b97b64d1d6d4608445efa4b860 in / 
# Wed, 16 Dec 2020 23:41:37 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:30:05 GMT
ENV HAPROXY_VERSION=1.7.12
# Thu, 17 Dec 2020 01:30:06 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.12.tar.gz
# Thu, 17 Dec 2020 01:30:06 GMT
ENV HAPROXY_SHA256=4118178b553a107b227f3f84774c7a50ae0b3ac2be39211c3db511ed4efe48ce
# Thu, 17 Dec 2020 01:30:17 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		CFLAGS+="-Wno-address-of-packed-member" 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:30:17 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:30:18 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in / 
# Thu, 17 Dec 2020 01:30:18 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:30:19 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:ee52640a49e15b8b7c8edb66c2d048b26abdee8d828d6e5ef4e10a28cb15a84f`  
		Last Modified: Wed, 16 Dec 2020 23:42:15 GMT  
		Size: 2.6 MB (2567018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38236ead985252be78ac9676e92561c12f2e2a15f00ec7968864352bbd38c824`  
		Last Modified: Thu, 17 Dec 2020 01:32:28 GMT  
		Size: 774.5 KB (774501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b09e8374749034b4a72545d3ab4ed7a2a58cbdce94bcd43269ca6275705bedd3`  
		Last Modified: Thu, 17 Dec 2020 01:32:26 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:1.8`

```console
$ docker pull haproxy@sha256:ad20819c818cd226e3529ed9749b97d4e1c30d496a8555f34fdcce8cc64b1dea
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
$ docker pull haproxy@sha256:6bc805e721573bbf4e11c69aaa933ce6f899ceb053e3b6b8deac974c6a25c7f9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.7 MB (33725889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5eb549fb1147e37574a0f9df058548b4ffde2020b01a4b229be220c45e58d976`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:06:10 GMT
ADD file:3a7bff4e139bcacc5831fd70a035c130a91b5da001dd91c08b2acd635c7064e8 in / 
# Fri, 11 Dec 2020 02:06:10 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 06:42:43 GMT
ENV HAPROXY_VERSION=1.8.27
# Fri, 11 Dec 2020 06:42:44 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.27.tar.gz
# Fri, 11 Dec 2020 06:42:44 GMT
ENV HAPROXY_SHA256=56ba6a21e13215fae56472ad37d5d68c3f19bde9da94c59e70b869eecf48bf50
# Fri, 11 Dec 2020 06:43:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 06:43:58 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 06:43:59 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 06:43:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 06:43:59 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:6ec7b7d162b24bd6df88abde89ceb6d7bbc2be927f025c9dd061af2b0c328cfe`  
		Last Modified: Fri, 11 Dec 2020 02:12:26 GMT  
		Size: 27.1 MB (27099295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b41d9a5efeafdbe1747522b7ca5e373762a34b3293c3a31c46af8cd0b818e6`  
		Last Modified: Fri, 11 Dec 2020 06:49:14 GMT  
		Size: 6.6 MB (6626214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a523131270058f1023a3ee3661fe2c46f29e07ca3f531433d974a369b21fe9`  
		Last Modified: Fri, 11 Dec 2020 06:49:12 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:c07c45ca0c35d97d660c0c6b9a25f4fec3ed894f7d0ddbb5c3adc7cd7bc91619
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.1 MB (31052539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cce0d5b438ef6c471bcb6507fc72a1d79bc7c28f209efc2582a6cdc78c7ed3b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:49 GMT
ADD file:58ebb3ffaf26d9b7621efba5f109ae9d22832f2f22865cda36604b138cbdb7b8 in / 
# Fri, 11 Dec 2020 02:04:56 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 03:31:26 GMT
ENV HAPROXY_VERSION=1.8.27
# Fri, 11 Dec 2020 03:31:26 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.27.tar.gz
# Fri, 11 Dec 2020 03:31:27 GMT
ENV HAPROXY_SHA256=56ba6a21e13215fae56472ad37d5d68c3f19bde9da94c59e70b869eecf48bf50
# Fri, 11 Dec 2020 03:32:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 03:32:33 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 03:32:34 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 03:32:37 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:32:40 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:8cbd1f790d64c77fcac6c9dbfe4d4c82f0365de9438f1a42b0560dc88f9e6a55`  
		Last Modified: Fri, 11 Dec 2020 02:14:44 GMT  
		Size: 24.8 MB (24843461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f561bc8c13ec4083ef8e5d0918d8738fb5d5678b311251a86b1d6b1fba36727`  
		Last Modified: Fri, 11 Dec 2020 03:35:59 GMT  
		Size: 6.2 MB (6208698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf185293cfc6ecc1a938144a4c0e926233035907a8c58586c2958f2ff1611d3c`  
		Last Modified: Fri, 11 Dec 2020 03:35:57 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:f0d91e956cc46463e408a2f422cd19fd29858757bd8be02fcdbf1c745ff39c90
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.8 MB (28754213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36e454962b7c09d7666569d8330d5e7a83bf1e5e6606f04d36520f6ad44ee4dd`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:23:37 GMT
ADD file:75ca842ac2d6e9f6617bb3df280af1e4c9619c9805fd5e00c1c3d6b8b4e3d802 in / 
# Fri, 11 Dec 2020 02:23:39 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 05:00:29 GMT
ENV HAPROXY_VERSION=1.8.27
# Fri, 11 Dec 2020 05:00:30 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.27.tar.gz
# Fri, 11 Dec 2020 05:00:31 GMT
ENV HAPROXY_SHA256=56ba6a21e13215fae56472ad37d5d68c3f19bde9da94c59e70b869eecf48bf50
# Fri, 11 Dec 2020 05:01:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 05:01:21 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 05:01:22 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 05:01:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:01:23 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c06905228d4fc5a5c840a70e2e6ced56596a8bc73abc69e6a1867bbb6f7ae7e7`  
		Last Modified: Fri, 11 Dec 2020 02:33:07 GMT  
		Size: 22.7 MB (22707662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df5fb80caf5b4f4273d41efb1559b62fc25bd1fe39c0562178de694c0ad8d14`  
		Last Modified: Fri, 11 Dec 2020 05:06:42 GMT  
		Size: 6.0 MB (6046169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da7aae8ebb316ec96288de9f31b294e7a6d6e1e3b7fef4cc2aca46e538f813b0`  
		Last Modified: Fri, 11 Dec 2020 05:06:40 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:b7260efe90874175796db109f779f50a5b7e0a26243d58e6099ddff342c46577
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.3 MB (32285176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:046ecb1042f35a0643897156b2edbbf615972f83fe10ee7a9584b311de113af8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:45:53 GMT
ADD file:a5a2f039c00bc638b88cefdff4c3cd1865b4d415bf80c4fe6b496d975af7cc1f in / 
# Fri, 11 Dec 2020 02:45:57 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 05:39:37 GMT
ENV HAPROXY_VERSION=1.8.27
# Fri, 11 Dec 2020 05:39:38 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.27.tar.gz
# Fri, 11 Dec 2020 05:39:39 GMT
ENV HAPROXY_SHA256=56ba6a21e13215fae56472ad37d5d68c3f19bde9da94c59e70b869eecf48bf50
# Fri, 11 Dec 2020 05:40:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 05:40:27 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 05:40:28 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 05:40:30 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:40:32 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c9648d7fcbb6d597cf33916d8fcd207fde8ec05d764b4480d4f3e884e142a902`  
		Last Modified: Fri, 11 Dec 2020 02:53:14 GMT  
		Size: 25.9 MB (25856191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8bc39abf3e583986a337fe883e3e4fc63d9a4c2c8199e3581f291b3f8061a69`  
		Last Modified: Fri, 11 Dec 2020 05:45:27 GMT  
		Size: 6.4 MB (6428605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5e49f2da713c0fd978f5cd9ff70b50dcd42128af2de2b60c1d011f83e58443`  
		Last Modified: Fri, 11 Dec 2020 05:45:25 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8` - linux; 386

```console
$ docker pull haproxy@sha256:48975d554d27f452fa774dfd21373ea96637f61c37bf5bf855afe0550f54a041
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34311144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a395a184038a8bc40f6215e57a229e0d410e6cd811ddf76cb4caae1f8d8527d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:07 GMT
ADD file:a0879774b23f70c4db7f7b04736cca142beb0b22e93f5952364ca990a1675552 in / 
# Fri, 11 Dec 2020 02:03:08 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 05:20:07 GMT
ENV HAPROXY_VERSION=1.8.27
# Fri, 11 Dec 2020 05:20:07 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.27.tar.gz
# Fri, 11 Dec 2020 05:20:08 GMT
ENV HAPROXY_SHA256=56ba6a21e13215fae56472ad37d5d68c3f19bde9da94c59e70b869eecf48bf50
# Fri, 11 Dec 2020 05:20:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 05:21:00 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 05:21:00 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 05:21:00 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:21:01 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:cfec07a090788e68b692f30d34e11dc7af0f1c8112fbc846e8e40e24faf882d7`  
		Last Modified: Fri, 11 Dec 2020 02:09:41 GMT  
		Size: 27.8 MB (27757584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7e62ab67e74fd0927860e744454d1e84981ba08274d48ad44665a7ef6268d6d`  
		Last Modified: Fri, 11 Dec 2020 05:26:42 GMT  
		Size: 6.6 MB (6553181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6873e3969b5e0d35169ff890d050ec357da08d83eafce3147d82423dcb89b918`  
		Last Modified: Fri, 11 Dec 2020 05:26:39 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8` - linux; mips64le

```console
$ docker pull haproxy@sha256:48574cbf41c8f86103426cbe20a2119324baa88ab558fa378aded675c6c3990c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.9 MB (31888641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2d2d93efad266e4654aa2b86ce71467c5611ff86300a0732eac8b26b9d19a79`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:30 GMT
ADD file:edb758d587972f30ef28b162dcabf79f61b685afa3c6066cb611c61abea124f3 in / 
# Fri, 11 Dec 2020 02:03:30 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 03:28:39 GMT
ENV HAPROXY_VERSION=1.8.27
# Fri, 11 Dec 2020 03:28:39 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.27.tar.gz
# Fri, 11 Dec 2020 03:28:40 GMT
ENV HAPROXY_SHA256=56ba6a21e13215fae56472ad37d5d68c3f19bde9da94c59e70b869eecf48bf50
# Fri, 11 Dec 2020 03:30:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 03:30:20 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 03:30:21 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 03:30:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:30:21 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:bed35f8e8e003f268bd91c8bc28d93f0b1463296add14ab3ec84c3d3d30e9025`  
		Last Modified: Fri, 11 Dec 2020 02:10:15 GMT  
		Size: 25.8 MB (25769881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ffaaa001ca3348ae14389e73e01aba6371f0852cb1fc61f3f2dfb981b7ba6ec`  
		Last Modified: Fri, 11 Dec 2020 03:34:28 GMT  
		Size: 6.1 MB (6118378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669e0a9c6f547724e931925906260ff25c21a7fb833da570f1e53079d235a959`  
		Last Modified: Fri, 11 Dec 2020 03:34:19 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8` - linux; ppc64le

```console
$ docker pull haproxy@sha256:624a570c2072ff28271c36b471314f026d2492532691b732923e973d0d545c34
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37443306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4f9055c5600bad92db45ff4cf633d34f13b3fb100ec83b9529c6c341804b277`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 03:34:02 GMT
ADD file:eca1a7737bd5e84ff883c4c284c0cd22492145d9cd7ae3b8e7b490e3d8e5aefb in / 
# Fri, 11 Dec 2020 03:34:11 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 05:44:22 GMT
ENV HAPROXY_VERSION=1.8.27
# Fri, 11 Dec 2020 05:44:25 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.27.tar.gz
# Fri, 11 Dec 2020 05:44:28 GMT
ENV HAPROXY_SHA256=56ba6a21e13215fae56472ad37d5d68c3f19bde9da94c59e70b869eecf48bf50
# Fri, 11 Dec 2020 05:46:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 05:46:48 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 05:46:50 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 05:46:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:46:58 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c0f0648876332890be87a9f32ec4ad2a939e805be3152ab991a923f7dec2b35d`  
		Last Modified: Fri, 11 Dec 2020 03:41:39 GMT  
		Size: 30.5 MB (30524717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caad9c3282969a9ec2b11f63391c01c962eaa22eda44effa8d3b7ea30fa2bbbe`  
		Last Modified: Fri, 11 Dec 2020 05:55:31 GMT  
		Size: 6.9 MB (6918209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:510790bc44f8f848c7db3ec34fe46646581adcf4814115e9f3ff3d1ddb0fe50f`  
		Last Modified: Fri, 11 Dec 2020 05:55:30 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8` - linux; s390x

```console
$ docker pull haproxy@sha256:548f27578f677afa879e1c59ab960a156daa23e980d965dd766bededabe26670
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.9 MB (31924874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b64471e40b446c80297bf0b89757d43cfa794ed9a55bc4e5270de8d45547cc5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:12:11 GMT
ADD file:db86ce5a1665b6d8ac734c54ac249a811c58484f569b935b14772445962428aa in / 
# Fri, 11 Dec 2020 02:12:15 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 03:24:14 GMT
ENV HAPROXY_VERSION=1.8.27
# Fri, 11 Dec 2020 03:24:14 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.27.tar.gz
# Fri, 11 Dec 2020 03:24:14 GMT
ENV HAPROXY_SHA256=56ba6a21e13215fae56472ad37d5d68c3f19bde9da94c59e70b869eecf48bf50
# Fri, 11 Dec 2020 03:24:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 03:24:59 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 03:24:59 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 03:24:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:25:00 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:f4cf10ca9f31aab0854647d7878dc4db838e93b892b843dde3db24f2e909a106`  
		Last Modified: Fri, 11 Dec 2020 02:17:07 GMT  
		Size: 25.7 MB (25713957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaa07d4f2f3dbab42de8de7e7dfc61a3f396343c444a597e58c78494ad0b29db`  
		Last Modified: Fri, 11 Dec 2020 03:29:12 GMT  
		Size: 6.2 MB (6210536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:278e81d46b851c02f44b963c31b9f6ca21ee80a7ffd7f304d2b3f5f152445193`  
		Last Modified: Fri, 11 Dec 2020 03:29:11 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:1.8.27`

```console
$ docker pull haproxy@sha256:ad20819c818cd226e3529ed9749b97d4e1c30d496a8555f34fdcce8cc64b1dea
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

### `haproxy:1.8.27` - linux; amd64

```console
$ docker pull haproxy@sha256:6bc805e721573bbf4e11c69aaa933ce6f899ceb053e3b6b8deac974c6a25c7f9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.7 MB (33725889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5eb549fb1147e37574a0f9df058548b4ffde2020b01a4b229be220c45e58d976`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:06:10 GMT
ADD file:3a7bff4e139bcacc5831fd70a035c130a91b5da001dd91c08b2acd635c7064e8 in / 
# Fri, 11 Dec 2020 02:06:10 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 06:42:43 GMT
ENV HAPROXY_VERSION=1.8.27
# Fri, 11 Dec 2020 06:42:44 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.27.tar.gz
# Fri, 11 Dec 2020 06:42:44 GMT
ENV HAPROXY_SHA256=56ba6a21e13215fae56472ad37d5d68c3f19bde9da94c59e70b869eecf48bf50
# Fri, 11 Dec 2020 06:43:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 06:43:58 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 06:43:59 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 06:43:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 06:43:59 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:6ec7b7d162b24bd6df88abde89ceb6d7bbc2be927f025c9dd061af2b0c328cfe`  
		Last Modified: Fri, 11 Dec 2020 02:12:26 GMT  
		Size: 27.1 MB (27099295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b41d9a5efeafdbe1747522b7ca5e373762a34b3293c3a31c46af8cd0b818e6`  
		Last Modified: Fri, 11 Dec 2020 06:49:14 GMT  
		Size: 6.6 MB (6626214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a523131270058f1023a3ee3661fe2c46f29e07ca3f531433d974a369b21fe9`  
		Last Modified: Fri, 11 Dec 2020 06:49:12 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8.27` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:c07c45ca0c35d97d660c0c6b9a25f4fec3ed894f7d0ddbb5c3adc7cd7bc91619
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.1 MB (31052539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cce0d5b438ef6c471bcb6507fc72a1d79bc7c28f209efc2582a6cdc78c7ed3b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:49 GMT
ADD file:58ebb3ffaf26d9b7621efba5f109ae9d22832f2f22865cda36604b138cbdb7b8 in / 
# Fri, 11 Dec 2020 02:04:56 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 03:31:26 GMT
ENV HAPROXY_VERSION=1.8.27
# Fri, 11 Dec 2020 03:31:26 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.27.tar.gz
# Fri, 11 Dec 2020 03:31:27 GMT
ENV HAPROXY_SHA256=56ba6a21e13215fae56472ad37d5d68c3f19bde9da94c59e70b869eecf48bf50
# Fri, 11 Dec 2020 03:32:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 03:32:33 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 03:32:34 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 03:32:37 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:32:40 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:8cbd1f790d64c77fcac6c9dbfe4d4c82f0365de9438f1a42b0560dc88f9e6a55`  
		Last Modified: Fri, 11 Dec 2020 02:14:44 GMT  
		Size: 24.8 MB (24843461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f561bc8c13ec4083ef8e5d0918d8738fb5d5678b311251a86b1d6b1fba36727`  
		Last Modified: Fri, 11 Dec 2020 03:35:59 GMT  
		Size: 6.2 MB (6208698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf185293cfc6ecc1a938144a4c0e926233035907a8c58586c2958f2ff1611d3c`  
		Last Modified: Fri, 11 Dec 2020 03:35:57 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8.27` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:f0d91e956cc46463e408a2f422cd19fd29858757bd8be02fcdbf1c745ff39c90
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.8 MB (28754213 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36e454962b7c09d7666569d8330d5e7a83bf1e5e6606f04d36520f6ad44ee4dd`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:23:37 GMT
ADD file:75ca842ac2d6e9f6617bb3df280af1e4c9619c9805fd5e00c1c3d6b8b4e3d802 in / 
# Fri, 11 Dec 2020 02:23:39 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 05:00:29 GMT
ENV HAPROXY_VERSION=1.8.27
# Fri, 11 Dec 2020 05:00:30 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.27.tar.gz
# Fri, 11 Dec 2020 05:00:31 GMT
ENV HAPROXY_SHA256=56ba6a21e13215fae56472ad37d5d68c3f19bde9da94c59e70b869eecf48bf50
# Fri, 11 Dec 2020 05:01:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 05:01:21 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 05:01:22 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 05:01:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:01:23 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c06905228d4fc5a5c840a70e2e6ced56596a8bc73abc69e6a1867bbb6f7ae7e7`  
		Last Modified: Fri, 11 Dec 2020 02:33:07 GMT  
		Size: 22.7 MB (22707662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df5fb80caf5b4f4273d41efb1559b62fc25bd1fe39c0562178de694c0ad8d14`  
		Last Modified: Fri, 11 Dec 2020 05:06:42 GMT  
		Size: 6.0 MB (6046169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da7aae8ebb316ec96288de9f31b294e7a6d6e1e3b7fef4cc2aca46e538f813b0`  
		Last Modified: Fri, 11 Dec 2020 05:06:40 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8.27` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:b7260efe90874175796db109f779f50a5b7e0a26243d58e6099ddff342c46577
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.3 MB (32285176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:046ecb1042f35a0643897156b2edbbf615972f83fe10ee7a9584b311de113af8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:45:53 GMT
ADD file:a5a2f039c00bc638b88cefdff4c3cd1865b4d415bf80c4fe6b496d975af7cc1f in / 
# Fri, 11 Dec 2020 02:45:57 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 05:39:37 GMT
ENV HAPROXY_VERSION=1.8.27
# Fri, 11 Dec 2020 05:39:38 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.27.tar.gz
# Fri, 11 Dec 2020 05:39:39 GMT
ENV HAPROXY_SHA256=56ba6a21e13215fae56472ad37d5d68c3f19bde9da94c59e70b869eecf48bf50
# Fri, 11 Dec 2020 05:40:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 05:40:27 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 05:40:28 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 05:40:30 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:40:32 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c9648d7fcbb6d597cf33916d8fcd207fde8ec05d764b4480d4f3e884e142a902`  
		Last Modified: Fri, 11 Dec 2020 02:53:14 GMT  
		Size: 25.9 MB (25856191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8bc39abf3e583986a337fe883e3e4fc63d9a4c2c8199e3581f291b3f8061a69`  
		Last Modified: Fri, 11 Dec 2020 05:45:27 GMT  
		Size: 6.4 MB (6428605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5e49f2da713c0fd978f5cd9ff70b50dcd42128af2de2b60c1d011f83e58443`  
		Last Modified: Fri, 11 Dec 2020 05:45:25 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8.27` - linux; 386

```console
$ docker pull haproxy@sha256:48975d554d27f452fa774dfd21373ea96637f61c37bf5bf855afe0550f54a041
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34311144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a395a184038a8bc40f6215e57a229e0d410e6cd811ddf76cb4caae1f8d8527d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:07 GMT
ADD file:a0879774b23f70c4db7f7b04736cca142beb0b22e93f5952364ca990a1675552 in / 
# Fri, 11 Dec 2020 02:03:08 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 05:20:07 GMT
ENV HAPROXY_VERSION=1.8.27
# Fri, 11 Dec 2020 05:20:07 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.27.tar.gz
# Fri, 11 Dec 2020 05:20:08 GMT
ENV HAPROXY_SHA256=56ba6a21e13215fae56472ad37d5d68c3f19bde9da94c59e70b869eecf48bf50
# Fri, 11 Dec 2020 05:20:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 05:21:00 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 05:21:00 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 05:21:00 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:21:01 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:cfec07a090788e68b692f30d34e11dc7af0f1c8112fbc846e8e40e24faf882d7`  
		Last Modified: Fri, 11 Dec 2020 02:09:41 GMT  
		Size: 27.8 MB (27757584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7e62ab67e74fd0927860e744454d1e84981ba08274d48ad44665a7ef6268d6d`  
		Last Modified: Fri, 11 Dec 2020 05:26:42 GMT  
		Size: 6.6 MB (6553181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6873e3969b5e0d35169ff890d050ec357da08d83eafce3147d82423dcb89b918`  
		Last Modified: Fri, 11 Dec 2020 05:26:39 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8.27` - linux; mips64le

```console
$ docker pull haproxy@sha256:48574cbf41c8f86103426cbe20a2119324baa88ab558fa378aded675c6c3990c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.9 MB (31888641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2d2d93efad266e4654aa2b86ce71467c5611ff86300a0732eac8b26b9d19a79`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:30 GMT
ADD file:edb758d587972f30ef28b162dcabf79f61b685afa3c6066cb611c61abea124f3 in / 
# Fri, 11 Dec 2020 02:03:30 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 03:28:39 GMT
ENV HAPROXY_VERSION=1.8.27
# Fri, 11 Dec 2020 03:28:39 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.27.tar.gz
# Fri, 11 Dec 2020 03:28:40 GMT
ENV HAPROXY_SHA256=56ba6a21e13215fae56472ad37d5d68c3f19bde9da94c59e70b869eecf48bf50
# Fri, 11 Dec 2020 03:30:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 03:30:20 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 03:30:21 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 03:30:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:30:21 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:bed35f8e8e003f268bd91c8bc28d93f0b1463296add14ab3ec84c3d3d30e9025`  
		Last Modified: Fri, 11 Dec 2020 02:10:15 GMT  
		Size: 25.8 MB (25769881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ffaaa001ca3348ae14389e73e01aba6371f0852cb1fc61f3f2dfb981b7ba6ec`  
		Last Modified: Fri, 11 Dec 2020 03:34:28 GMT  
		Size: 6.1 MB (6118378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669e0a9c6f547724e931925906260ff25c21a7fb833da570f1e53079d235a959`  
		Last Modified: Fri, 11 Dec 2020 03:34:19 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8.27` - linux; ppc64le

```console
$ docker pull haproxy@sha256:624a570c2072ff28271c36b471314f026d2492532691b732923e973d0d545c34
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37443306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4f9055c5600bad92db45ff4cf633d34f13b3fb100ec83b9529c6c341804b277`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 03:34:02 GMT
ADD file:eca1a7737bd5e84ff883c4c284c0cd22492145d9cd7ae3b8e7b490e3d8e5aefb in / 
# Fri, 11 Dec 2020 03:34:11 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 05:44:22 GMT
ENV HAPROXY_VERSION=1.8.27
# Fri, 11 Dec 2020 05:44:25 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.27.tar.gz
# Fri, 11 Dec 2020 05:44:28 GMT
ENV HAPROXY_SHA256=56ba6a21e13215fae56472ad37d5d68c3f19bde9da94c59e70b869eecf48bf50
# Fri, 11 Dec 2020 05:46:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 05:46:48 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 05:46:50 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 05:46:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:46:58 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c0f0648876332890be87a9f32ec4ad2a939e805be3152ab991a923f7dec2b35d`  
		Last Modified: Fri, 11 Dec 2020 03:41:39 GMT  
		Size: 30.5 MB (30524717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caad9c3282969a9ec2b11f63391c01c962eaa22eda44effa8d3b7ea30fa2bbbe`  
		Last Modified: Fri, 11 Dec 2020 05:55:31 GMT  
		Size: 6.9 MB (6918209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:510790bc44f8f848c7db3ec34fe46646581adcf4814115e9f3ff3d1ddb0fe50f`  
		Last Modified: Fri, 11 Dec 2020 05:55:30 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8.27` - linux; s390x

```console
$ docker pull haproxy@sha256:548f27578f677afa879e1c59ab960a156daa23e980d965dd766bededabe26670
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.9 MB (31924874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b64471e40b446c80297bf0b89757d43cfa794ed9a55bc4e5270de8d45547cc5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:12:11 GMT
ADD file:db86ce5a1665b6d8ac734c54ac249a811c58484f569b935b14772445962428aa in / 
# Fri, 11 Dec 2020 02:12:15 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 03:24:14 GMT
ENV HAPROXY_VERSION=1.8.27
# Fri, 11 Dec 2020 03:24:14 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.27.tar.gz
# Fri, 11 Dec 2020 03:24:14 GMT
ENV HAPROXY_SHA256=56ba6a21e13215fae56472ad37d5d68c3f19bde9da94c59e70b869eecf48bf50
# Fri, 11 Dec 2020 03:24:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 03:24:59 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 03:24:59 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 03:24:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:25:00 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:f4cf10ca9f31aab0854647d7878dc4db838e93b892b843dde3db24f2e909a106`  
		Last Modified: Fri, 11 Dec 2020 02:17:07 GMT  
		Size: 25.7 MB (25713957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaa07d4f2f3dbab42de8de7e7dfc61a3f396343c444a597e58c78494ad0b29db`  
		Last Modified: Fri, 11 Dec 2020 03:29:12 GMT  
		Size: 6.2 MB (6210536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:278e81d46b851c02f44b963c31b9f6ca21ee80a7ffd7f304d2b3f5f152445193`  
		Last Modified: Fri, 11 Dec 2020 03:29:11 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:1.8.27-alpine`

```console
$ docker pull haproxy@sha256:41a8d5f8876b2d3719bd4dadababff88fdd18b1373b32d02b6d0ead28baf986c
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

### `haproxy:1.8.27-alpine` - linux; amd64

```console
$ docker pull haproxy@sha256:ecdabc34bcbc69e08895a7e27ba38eb9be09facaf006ec82cce6ca6a29edd2e3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7130860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b7149b7b37cf17cb6d88ed2e4236e0ef45a13bcb3bc5b3e454e3bc7c0d43c34`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:35:43 GMT
ENV HAPROXY_VERSION=1.8.27
# Thu, 17 Dec 2020 13:35:43 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.27.tar.gz
# Thu, 17 Dec 2020 13:35:43 GMT
ENV HAPROXY_SHA256=56ba6a21e13215fae56472ad37d5d68c3f19bde9da94c59e70b869eecf48bf50
# Thu, 17 Dec 2020 13:36:31 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 13:36:32 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 13:36:32 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 13:36:32 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 13:36:32 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:130b7b112032c76f27d50ad73d85ba806deb893f199b90c4c013326ea7b8c6bf`  
		Last Modified: Thu, 17 Dec 2020 13:38:44 GMT  
		Size: 4.3 MB (4331413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6af17520b7b716d5fae79964e8d9fd717e6fa2065313e45fe0044641ab3bf01`  
		Last Modified: Thu, 17 Dec 2020 13:38:45 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8.27-alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:0b2981905105c293a8fcb04eec8a6182e34ae2d15deff9f074a4426d22a5b055
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6701141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:752e82b827404d5ad7f2b1aab9f38b2fa745b75f10cdd6390042a01925757d76`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:39:35 GMT
ENV HAPROXY_VERSION=1.8.27
# Thu, 17 Dec 2020 01:39:36 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.27.tar.gz
# Thu, 17 Dec 2020 01:39:38 GMT
ENV HAPROXY_SHA256=56ba6a21e13215fae56472ad37d5d68c3f19bde9da94c59e70b869eecf48bf50
# Thu, 17 Dec 2020 01:40:06 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:40:07 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:40:07 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 01:40:08 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:40:09 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63dee0f82e03429b1b51e812b8127b1319c770da3e8eec3ada4d35e98c79bca9`  
		Last Modified: Thu, 17 Dec 2020 01:42:06 GMT  
		Size: 4.1 MB (4096597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d189e99caceef8656ca140ce65657d24d212dbec56afb8e712bee41fa22fb94b`  
		Last Modified: Thu, 17 Dec 2020 01:42:05 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8.27-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:7b25ea80881a5f272b45357addc28558961c903643836d5b296daedb56c7ab68
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6524041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26c67f43fb182a31f40e822b86699e71362ef7c6246f7a639621075ce815ffc7`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:41:31 GMT
ENV HAPROXY_VERSION=1.8.27
# Thu, 17 Dec 2020 01:41:31 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.27.tar.gz
# Thu, 17 Dec 2020 01:41:32 GMT
ENV HAPROXY_SHA256=56ba6a21e13215fae56472ad37d5d68c3f19bde9da94c59e70b869eecf48bf50
# Thu, 17 Dec 2020 01:41:50 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:41:50 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:41:51 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 01:41:52 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:41:52 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f8a1ce40257ffeaaaa48f32dd98596d5a26e185d85c130b54a293a240fcad26`  
		Last Modified: Thu, 17 Dec 2020 01:44:11 GMT  
		Size: 4.1 MB (4116107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45777c30e5431e72fcb9e4961dfd5177c5c3e5d5f4c2dfca4adb7b26d86c3e16`  
		Last Modified: Thu, 17 Dec 2020 01:44:10 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8.27-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:edac18a8791f608dbc44daad0821cfecf386981cc96f19152903aeb0632207e6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (6964092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1a814cac09084c191c5ffe39520911842071ebc854534bcedeec80c224389b6`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:27:37 GMT
ENV HAPROXY_VERSION=1.8.27
# Thu, 17 Dec 2020 01:27:39 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.27.tar.gz
# Thu, 17 Dec 2020 01:27:41 GMT
ENV HAPROXY_SHA256=56ba6a21e13215fae56472ad37d5d68c3f19bde9da94c59e70b869eecf48bf50
# Thu, 17 Dec 2020 01:28:08 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:28:14 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:28:15 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 01:28:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:28:18 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0aa4e5a05fc4c9c380f1a4964344145973651566f78fed027a8edd3719aa6a6`  
		Last Modified: Thu, 17 Dec 2020 01:31:12 GMT  
		Size: 4.3 MB (4254664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff7c8addaf2203dba4fc699178202235065d4e44b6cb896420c2d095243aa22`  
		Last Modified: Thu, 17 Dec 2020 01:31:11 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8.27-alpine` - linux; 386

```console
$ docker pull haproxy@sha256:271c4f8938cbef1633c5e909ba113d5b719ce56737275bf06e668ecd21663e35
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7053685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba4272b269f5e0acce169b31fca4dc5fd4752bff17742a4869d9788ab7564113`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 17 Dec 2020 00:38:32 GMT
ADD file:de33fda50a142403e842620d20bc4404e66fc4ace16edc6946c4539e8a797458 in / 
# Thu, 17 Dec 2020 00:38:32 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:32:27 GMT
ENV HAPROXY_VERSION=1.8.27
# Thu, 17 Dec 2020 02:32:28 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.27.tar.gz
# Thu, 17 Dec 2020 02:32:28 GMT
ENV HAPROXY_SHA256=56ba6a21e13215fae56472ad37d5d68c3f19bde9da94c59e70b869eecf48bf50
# Thu, 17 Dec 2020 02:33:13 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 02:33:13 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 02:33:13 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 02:33:13 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 02:33:13 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:455793c72b878001f0905634ed52a2524ba51796e7377bf00683a85123f7dce9`  
		Last Modified: Thu, 17 Dec 2020 00:39:18 GMT  
		Size: 2.8 MB (2794130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c98fda7960b2230872876ea5741102d8366e79bf192ac863b1c5ccf4232050`  
		Last Modified: Thu, 17 Dec 2020 02:35:22 GMT  
		Size: 4.3 MB (4259174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:622ed629023167187c78b3464e7abf8ec6de0d559d1b960ab45788f5c17e0b6d`  
		Last Modified: Thu, 17 Dec 2020 02:35:21 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8.27-alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:ba7151b6a32f1588a3eb256bceb581246b5c69b59a58322581e179870d213029
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7272118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91a67fd88c06d1f17a439512737353879e3e1e702b0a1b682f67cfbee23df256`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 17 Dec 2020 00:20:42 GMT
ADD file:0a38c9b4955f8faa79627c166fca80ef342e443a16ce2925a30eeae317bbd786 in / 
# Thu, 17 Dec 2020 00:20:48 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:46:34 GMT
ENV HAPROXY_VERSION=1.8.27
# Thu, 17 Dec 2020 02:46:38 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.27.tar.gz
# Thu, 17 Dec 2020 02:46:40 GMT
ENV HAPROXY_SHA256=56ba6a21e13215fae56472ad37d5d68c3f19bde9da94c59e70b869eecf48bf50
# Thu, 17 Dec 2020 02:47:10 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 02:47:17 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 02:47:22 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 02:47:29 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 02:47:37 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:a9d343b7bcc225fe7ac17d96a81329510ab7f31a50472311cafe7168d3107317`  
		Last Modified: Thu, 17 Dec 2020 00:21:33 GMT  
		Size: 2.8 MB (2805226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:819f8c1e0c2f59ebe07ece1641e6dfb77ac5ac07125af14a6f6338dc25836a74`  
		Last Modified: Thu, 17 Dec 2020 02:51:02 GMT  
		Size: 4.5 MB (4466511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216678e02dc25201b01b6f42162ce81cf382a2169c84f04a97f39b2f82331580`  
		Last Modified: Thu, 17 Dec 2020 02:51:01 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8.27-alpine` - linux; s390x

```console
$ docker pull haproxy@sha256:2e1a3f18cc2d517485499bd6a49f0d21afe8c56f4fab10dfd8080582b9b546fc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6782397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56ce926f0281d4db908b7892bc775344cfe4943515e0315ce67eadc63e94527b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:41:37 GMT
ADD file:3ad3856d165e8760af85574a8ffa75ca44b7e1b97b64d1d6d4608445efa4b860 in / 
# Wed, 16 Dec 2020 23:41:37 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:29:24 GMT
ENV HAPROXY_VERSION=1.8.27
# Thu, 17 Dec 2020 01:29:25 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.27.tar.gz
# Thu, 17 Dec 2020 01:29:25 GMT
ENV HAPROXY_SHA256=56ba6a21e13215fae56472ad37d5d68c3f19bde9da94c59e70b869eecf48bf50
# Thu, 17 Dec 2020 01:29:53 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:29:54 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:29:54 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 01:29:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:29:56 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:ee52640a49e15b8b7c8edb66c2d048b26abdee8d828d6e5ef4e10a28cb15a84f`  
		Last Modified: Wed, 16 Dec 2020 23:42:15 GMT  
		Size: 2.6 MB (2567018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2700369c652f0c6c0af6d27fd9964a82241918bc8c9003301f8309ac2a137a7`  
		Last Modified: Thu, 17 Dec 2020 01:32:14 GMT  
		Size: 4.2 MB (4214999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f3cdb7cf41456ff0176c59342d94bbd0b26489a140fe0a4c5f4bb11e451fe07`  
		Last Modified: Thu, 17 Dec 2020 01:32:13 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:1.8-alpine`

```console
$ docker pull haproxy@sha256:41a8d5f8876b2d3719bd4dadababff88fdd18b1373b32d02b6d0ead28baf986c
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
$ docker pull haproxy@sha256:ecdabc34bcbc69e08895a7e27ba38eb9be09facaf006ec82cce6ca6a29edd2e3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7130860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b7149b7b37cf17cb6d88ed2e4236e0ef45a13bcb3bc5b3e454e3bc7c0d43c34`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:35:43 GMT
ENV HAPROXY_VERSION=1.8.27
# Thu, 17 Dec 2020 13:35:43 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.27.tar.gz
# Thu, 17 Dec 2020 13:35:43 GMT
ENV HAPROXY_SHA256=56ba6a21e13215fae56472ad37d5d68c3f19bde9da94c59e70b869eecf48bf50
# Thu, 17 Dec 2020 13:36:31 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 13:36:32 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 13:36:32 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 13:36:32 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 13:36:32 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:130b7b112032c76f27d50ad73d85ba806deb893f199b90c4c013326ea7b8c6bf`  
		Last Modified: Thu, 17 Dec 2020 13:38:44 GMT  
		Size: 4.3 MB (4331413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6af17520b7b716d5fae79964e8d9fd717e6fa2065313e45fe0044641ab3bf01`  
		Last Modified: Thu, 17 Dec 2020 13:38:45 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8-alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:0b2981905105c293a8fcb04eec8a6182e34ae2d15deff9f074a4426d22a5b055
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6701141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:752e82b827404d5ad7f2b1aab9f38b2fa745b75f10cdd6390042a01925757d76`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:39:35 GMT
ENV HAPROXY_VERSION=1.8.27
# Thu, 17 Dec 2020 01:39:36 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.27.tar.gz
# Thu, 17 Dec 2020 01:39:38 GMT
ENV HAPROXY_SHA256=56ba6a21e13215fae56472ad37d5d68c3f19bde9da94c59e70b869eecf48bf50
# Thu, 17 Dec 2020 01:40:06 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:40:07 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:40:07 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 01:40:08 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:40:09 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63dee0f82e03429b1b51e812b8127b1319c770da3e8eec3ada4d35e98c79bca9`  
		Last Modified: Thu, 17 Dec 2020 01:42:06 GMT  
		Size: 4.1 MB (4096597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d189e99caceef8656ca140ce65657d24d212dbec56afb8e712bee41fa22fb94b`  
		Last Modified: Thu, 17 Dec 2020 01:42:05 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:7b25ea80881a5f272b45357addc28558961c903643836d5b296daedb56c7ab68
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6524041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26c67f43fb182a31f40e822b86699e71362ef7c6246f7a639621075ce815ffc7`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:41:31 GMT
ENV HAPROXY_VERSION=1.8.27
# Thu, 17 Dec 2020 01:41:31 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.27.tar.gz
# Thu, 17 Dec 2020 01:41:32 GMT
ENV HAPROXY_SHA256=56ba6a21e13215fae56472ad37d5d68c3f19bde9da94c59e70b869eecf48bf50
# Thu, 17 Dec 2020 01:41:50 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:41:50 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:41:51 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 01:41:52 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:41:52 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f8a1ce40257ffeaaaa48f32dd98596d5a26e185d85c130b54a293a240fcad26`  
		Last Modified: Thu, 17 Dec 2020 01:44:11 GMT  
		Size: 4.1 MB (4116107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45777c30e5431e72fcb9e4961dfd5177c5c3e5d5f4c2dfca4adb7b26d86c3e16`  
		Last Modified: Thu, 17 Dec 2020 01:44:10 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:edac18a8791f608dbc44daad0821cfecf386981cc96f19152903aeb0632207e6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (6964092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1a814cac09084c191c5ffe39520911842071ebc854534bcedeec80c224389b6`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:27:37 GMT
ENV HAPROXY_VERSION=1.8.27
# Thu, 17 Dec 2020 01:27:39 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.27.tar.gz
# Thu, 17 Dec 2020 01:27:41 GMT
ENV HAPROXY_SHA256=56ba6a21e13215fae56472ad37d5d68c3f19bde9da94c59e70b869eecf48bf50
# Thu, 17 Dec 2020 01:28:08 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:28:14 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:28:15 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 01:28:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:28:18 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0aa4e5a05fc4c9c380f1a4964344145973651566f78fed027a8edd3719aa6a6`  
		Last Modified: Thu, 17 Dec 2020 01:31:12 GMT  
		Size: 4.3 MB (4254664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff7c8addaf2203dba4fc699178202235065d4e44b6cb896420c2d095243aa22`  
		Last Modified: Thu, 17 Dec 2020 01:31:11 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8-alpine` - linux; 386

```console
$ docker pull haproxy@sha256:271c4f8938cbef1633c5e909ba113d5b719ce56737275bf06e668ecd21663e35
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7053685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba4272b269f5e0acce169b31fca4dc5fd4752bff17742a4869d9788ab7564113`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 17 Dec 2020 00:38:32 GMT
ADD file:de33fda50a142403e842620d20bc4404e66fc4ace16edc6946c4539e8a797458 in / 
# Thu, 17 Dec 2020 00:38:32 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:32:27 GMT
ENV HAPROXY_VERSION=1.8.27
# Thu, 17 Dec 2020 02:32:28 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.27.tar.gz
# Thu, 17 Dec 2020 02:32:28 GMT
ENV HAPROXY_SHA256=56ba6a21e13215fae56472ad37d5d68c3f19bde9da94c59e70b869eecf48bf50
# Thu, 17 Dec 2020 02:33:13 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 02:33:13 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 02:33:13 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 02:33:13 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 02:33:13 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:455793c72b878001f0905634ed52a2524ba51796e7377bf00683a85123f7dce9`  
		Last Modified: Thu, 17 Dec 2020 00:39:18 GMT  
		Size: 2.8 MB (2794130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c98fda7960b2230872876ea5741102d8366e79bf192ac863b1c5ccf4232050`  
		Last Modified: Thu, 17 Dec 2020 02:35:22 GMT  
		Size: 4.3 MB (4259174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:622ed629023167187c78b3464e7abf8ec6de0d559d1b960ab45788f5c17e0b6d`  
		Last Modified: Thu, 17 Dec 2020 02:35:21 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8-alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:ba7151b6a32f1588a3eb256bceb581246b5c69b59a58322581e179870d213029
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7272118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91a67fd88c06d1f17a439512737353879e3e1e702b0a1b682f67cfbee23df256`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 17 Dec 2020 00:20:42 GMT
ADD file:0a38c9b4955f8faa79627c166fca80ef342e443a16ce2925a30eeae317bbd786 in / 
# Thu, 17 Dec 2020 00:20:48 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:46:34 GMT
ENV HAPROXY_VERSION=1.8.27
# Thu, 17 Dec 2020 02:46:38 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.27.tar.gz
# Thu, 17 Dec 2020 02:46:40 GMT
ENV HAPROXY_SHA256=56ba6a21e13215fae56472ad37d5d68c3f19bde9da94c59e70b869eecf48bf50
# Thu, 17 Dec 2020 02:47:10 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 02:47:17 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 02:47:22 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 02:47:29 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 02:47:37 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:a9d343b7bcc225fe7ac17d96a81329510ab7f31a50472311cafe7168d3107317`  
		Last Modified: Thu, 17 Dec 2020 00:21:33 GMT  
		Size: 2.8 MB (2805226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:819f8c1e0c2f59ebe07ece1641e6dfb77ac5ac07125af14a6f6338dc25836a74`  
		Last Modified: Thu, 17 Dec 2020 02:51:02 GMT  
		Size: 4.5 MB (4466511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216678e02dc25201b01b6f42162ce81cf382a2169c84f04a97f39b2f82331580`  
		Last Modified: Thu, 17 Dec 2020 02:51:01 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8-alpine` - linux; s390x

```console
$ docker pull haproxy@sha256:2e1a3f18cc2d517485499bd6a49f0d21afe8c56f4fab10dfd8080582b9b546fc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6782397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56ce926f0281d4db908b7892bc775344cfe4943515e0315ce67eadc63e94527b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:41:37 GMT
ADD file:3ad3856d165e8760af85574a8ffa75ca44b7e1b97b64d1d6d4608445efa4b860 in / 
# Wed, 16 Dec 2020 23:41:37 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:29:24 GMT
ENV HAPROXY_VERSION=1.8.27
# Thu, 17 Dec 2020 01:29:25 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.27.tar.gz
# Thu, 17 Dec 2020 01:29:25 GMT
ENV HAPROXY_SHA256=56ba6a21e13215fae56472ad37d5d68c3f19bde9da94c59e70b869eecf48bf50
# Thu, 17 Dec 2020 01:29:53 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:29:54 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:29:54 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 01:29:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:29:56 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:ee52640a49e15b8b7c8edb66c2d048b26abdee8d828d6e5ef4e10a28cb15a84f`  
		Last Modified: Wed, 16 Dec 2020 23:42:15 GMT  
		Size: 2.6 MB (2567018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2700369c652f0c6c0af6d27fd9964a82241918bc8c9003301f8309ac2a137a7`  
		Last Modified: Thu, 17 Dec 2020 01:32:14 GMT  
		Size: 4.2 MB (4214999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f3cdb7cf41456ff0176c59342d94bbd0b26489a140fe0a4c5f4bb11e451fe07`  
		Last Modified: Thu, 17 Dec 2020 01:32:13 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.0`

```console
$ docker pull haproxy@sha256:2ac5122c552b876d986b9f90b3a8f37694339b58e6d6fda34b60992f8a926290
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
$ docker pull haproxy@sha256:7135fc678bfce1c23397af6b7b53122e9bef329c734ca2aabfe811adee11298c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.8 MB (35769472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41c49d795fc5c4cd061c666353ad2f19fcd6eb50329b510ac56382ecf978e7b9`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:06:10 GMT
ADD file:3a7bff4e139bcacc5831fd70a035c130a91b5da001dd91c08b2acd635c7064e8 in / 
# Fri, 11 Dec 2020 02:06:10 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 06:38:51 GMT
ENV HAPROXY_VERSION=2.0.19
# Fri, 11 Dec 2020 06:38:51 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.19.tar.gz
# Fri, 11 Dec 2020 06:38:52 GMT
ENV HAPROXY_SHA256=dcc444ac0aca0917e289653134333f7c29d05d844e6cd60dd04e23b5ff80c92d
# Fri, 11 Dec 2020 06:40:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 06:40:27 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 06:40:27 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 06:40:28 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 06:40:28 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:6ec7b7d162b24bd6df88abde89ceb6d7bbc2be927f025c9dd061af2b0c328cfe`  
		Last Modified: Fri, 11 Dec 2020 02:12:26 GMT  
		Size: 27.1 MB (27099295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b758f232c7dc4d22024916753373991a0466a6457ca0bc1215ad9e8c9a8dec51`  
		Last Modified: Fri, 11 Dec 2020 06:48:59 GMT  
		Size: 8.7 MB (8669797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638894b0b628d7ddbbaee45c55af12b372261a9c8b5337b7c9dd17c16fad49fd`  
		Last Modified: Fri, 11 Dec 2020 06:48:57 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:8cc258bd57409cff7e2b4542c8db6fa2d995817940ac5841f0e3f06ccfd74ac1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32997877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de2de4e21ec94306dedbddd4a737ff19e9b518b494c58e1e3e3af07e28e8a571`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:49 GMT
ADD file:58ebb3ffaf26d9b7621efba5f109ae9d22832f2f22865cda36604b138cbdb7b8 in / 
# Fri, 11 Dec 2020 02:04:56 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 03:29:51 GMT
ENV HAPROXY_VERSION=2.0.19
# Fri, 11 Dec 2020 03:29:52 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.19.tar.gz
# Fri, 11 Dec 2020 03:29:53 GMT
ENV HAPROXY_SHA256=dcc444ac0aca0917e289653134333f7c29d05d844e6cd60dd04e23b5ff80c92d
# Fri, 11 Dec 2020 03:31:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 03:31:13 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 03:31:14 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 03:31:15 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:31:16 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:8cbd1f790d64c77fcac6c9dbfe4d4c82f0365de9438f1a42b0560dc88f9e6a55`  
		Last Modified: Fri, 11 Dec 2020 02:14:44 GMT  
		Size: 24.8 MB (24843461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7bc3bf5fc96c30185881a3ae3a6bcca28e5b3ea16d8f0372b1dbf39fe4a8155`  
		Last Modified: Fri, 11 Dec 2020 03:35:49 GMT  
		Size: 8.2 MB (8154034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac96e80c96c1d123d8e40d58695108514091a3304fa8cd85d8806b46fe97fd0c`  
		Last Modified: Fri, 11 Dec 2020 03:35:46 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:45060ef6221834966e1db3a9dc9874352a7c968ab529246764f36d6f28008c65
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.8 MB (30808479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bddac759ec2de3eb1b79f071bba71989f3a0dd3d62ef31fad1839b0121cb942c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:23:37 GMT
ADD file:75ca842ac2d6e9f6617bb3df280af1e4c9619c9805fd5e00c1c3d6b8b4e3d802 in / 
# Fri, 11 Dec 2020 02:23:39 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 04:59:00 GMT
ENV HAPROXY_VERSION=2.0.19
# Fri, 11 Dec 2020 04:59:01 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.19.tar.gz
# Fri, 11 Dec 2020 04:59:02 GMT
ENV HAPROXY_SHA256=dcc444ac0aca0917e289653134333f7c29d05d844e6cd60dd04e23b5ff80c92d
# Fri, 11 Dec 2020 04:59:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 04:59:43 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 04:59:44 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 04:59:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 04:59:46 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c06905228d4fc5a5c840a70e2e6ced56596a8bc73abc69e6a1867bbb6f7ae7e7`  
		Last Modified: Fri, 11 Dec 2020 02:33:07 GMT  
		Size: 22.7 MB (22707662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9b9d726198fd52fe47bb9440d5179e503ba9e93683afa8bdb2bd8fd75424910`  
		Last Modified: Fri, 11 Dec 2020 05:06:19 GMT  
		Size: 8.1 MB (8100436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bffa2f708c937ce8bf07ef6dfb6cf7cf52b97b6e5bbc062e9ee191e754658752`  
		Last Modified: Fri, 11 Dec 2020 05:06:17 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:f7d269721a59b6a73a096a5869c764242e4e9cfd3e10b02914c458323cb16966
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.4 MB (34358891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1c4c10615319a0ae64d61027d680e7075a88565a776ec60bff4649c85cb3189`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:45:53 GMT
ADD file:a5a2f039c00bc638b88cefdff4c3cd1865b4d415bf80c4fe6b496d975af7cc1f in / 
# Fri, 11 Dec 2020 02:45:57 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 05:37:47 GMT
ENV HAPROXY_VERSION=2.0.19
# Fri, 11 Dec 2020 05:37:47 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.19.tar.gz
# Fri, 11 Dec 2020 05:37:48 GMT
ENV HAPROXY_SHA256=dcc444ac0aca0917e289653134333f7c29d05d844e6cd60dd04e23b5ff80c92d
# Fri, 11 Dec 2020 05:38:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 05:38:39 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 05:38:40 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 05:38:42 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:38:43 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c9648d7fcbb6d597cf33916d8fcd207fde8ec05d764b4480d4f3e884e142a902`  
		Last Modified: Fri, 11 Dec 2020 02:53:14 GMT  
		Size: 25.9 MB (25856191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fb0cc0076100081d451a9c79e8cc68352d7301ac2c34c60fb97275fe89c8ea7`  
		Last Modified: Fri, 11 Dec 2020 05:45:05 GMT  
		Size: 8.5 MB (8502320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18f20df09e352301bb5b30d0fd2fcfca525d966e177f7b8a03b7b5fd999e96e9`  
		Last Modified: Fri, 11 Dec 2020 05:45:03 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0` - linux; 386

```console
$ docker pull haproxy@sha256:675cbed42ec3858a775421834e929ab3a9fc3b380e5722ab3a59634f23f12ff1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.2 MB (36221513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1362820d36b8bf6bc7a5075d172692befb1952adf3691822f8d69ae19992b11d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:07 GMT
ADD file:a0879774b23f70c4db7f7b04736cca142beb0b22e93f5952364ca990a1675552 in / 
# Fri, 11 Dec 2020 02:03:08 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 05:17:20 GMT
ENV HAPROXY_VERSION=2.0.19
# Fri, 11 Dec 2020 05:17:20 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.19.tar.gz
# Fri, 11 Dec 2020 05:17:20 GMT
ENV HAPROXY_SHA256=dcc444ac0aca0917e289653134333f7c29d05d844e6cd60dd04e23b5ff80c92d
# Fri, 11 Dec 2020 05:18:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 05:18:24 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 05:18:24 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 05:18:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:18:25 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:cfec07a090788e68b692f30d34e11dc7af0f1c8112fbc846e8e40e24faf882d7`  
		Last Modified: Fri, 11 Dec 2020 02:09:41 GMT  
		Size: 27.8 MB (27757584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754f7d49fdacc86229f5a48e66fd5e749ff27893fcdb6700dbf1b119326a222c`  
		Last Modified: Fri, 11 Dec 2020 05:26:23 GMT  
		Size: 8.5 MB (8463549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34cd4a021af386720954307723207c719f4330f46ed9c363b7cd2539e33e9cd4`  
		Last Modified: Fri, 11 Dec 2020 05:26:21 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0` - linux; mips64le

```console
$ docker pull haproxy@sha256:6cc4dd47d018ce652aa82d6cec016588b780343db76136477561b44a8688e22e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33893293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4837ae5262f3c202ed08d60e86c7282eadeae0663ee3ac5963a816446c6757ba`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:30 GMT
ADD file:edb758d587972f30ef28b162dcabf79f61b685afa3c6066cb611c61abea124f3 in / 
# Fri, 11 Dec 2020 02:03:30 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 03:26:13 GMT
ENV HAPROXY_VERSION=2.0.19
# Fri, 11 Dec 2020 03:26:13 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.19.tar.gz
# Fri, 11 Dec 2020 03:26:13 GMT
ENV HAPROXY_SHA256=dcc444ac0aca0917e289653134333f7c29d05d844e6cd60dd04e23b5ff80c92d
# Fri, 11 Dec 2020 03:28:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 03:28:22 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 03:28:22 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 03:28:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:28:23 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:bed35f8e8e003f268bd91c8bc28d93f0b1463296add14ab3ec84c3d3d30e9025`  
		Last Modified: Fri, 11 Dec 2020 02:10:15 GMT  
		Size: 25.8 MB (25769881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0697ad7e10458a6ada5c07957eccb7bded5f2cec3789ee90b8d1684633c7ee5a`  
		Last Modified: Fri, 11 Dec 2020 03:34:01 GMT  
		Size: 8.1 MB (8123031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a420df40214af9b461d35080f3bafb80e7a460ccf423a0dd17edb3d8eaaa389`  
		Last Modified: Fri, 11 Dec 2020 03:33:56 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0` - linux; ppc64le

```console
$ docker pull haproxy@sha256:3b80238c4903a78b6a13c9291f1e14ed51f8836cb5bee207344e74583e6f528a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39458539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:762d066d8f12621a3d401ac8d6f3c8b6e73eb47c5ad0502758257a8feb8bec47`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 03:34:02 GMT
ADD file:eca1a7737bd5e84ff883c4c284c0cd22492145d9cd7ae3b8e7b490e3d8e5aefb in / 
# Fri, 11 Dec 2020 03:34:11 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 05:40:01 GMT
ENV HAPROXY_VERSION=2.0.19
# Fri, 11 Dec 2020 05:40:05 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.19.tar.gz
# Fri, 11 Dec 2020 05:40:09 GMT
ENV HAPROXY_SHA256=dcc444ac0aca0917e289653134333f7c29d05d844e6cd60dd04e23b5ff80c92d
# Fri, 11 Dec 2020 05:42:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 05:42:44 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 05:42:47 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 05:42:53 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:42:55 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c0f0648876332890be87a9f32ec4ad2a939e805be3152ab991a923f7dec2b35d`  
		Last Modified: Fri, 11 Dec 2020 03:41:39 GMT  
		Size: 30.5 MB (30524717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:559b32d0d078ef78d189a11af1eecca8cf90713f33c69e69b15219d831f0037d`  
		Last Modified: Fri, 11 Dec 2020 05:55:05 GMT  
		Size: 8.9 MB (8933442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:306aef5e924471e4d849915be88683632813bda3cad2dd930235e12a0af6b1cb`  
		Last Modified: Fri, 11 Dec 2020 05:55:03 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0` - linux; s390x

```console
$ docker pull haproxy@sha256:88f012f756f1881102c30804eeca1084b820e42092f923d9fc2a5f97a2800920
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33935731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23fdd23ee3ec79b6d13637e05f156baea54f090738da1e37fe1a5a980d98a58b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:12:11 GMT
ADD file:db86ce5a1665b6d8ac734c54ac249a811c58484f569b935b14772445962428aa in / 
# Fri, 11 Dec 2020 02:12:15 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 03:22:28 GMT
ENV HAPROXY_VERSION=2.0.19
# Fri, 11 Dec 2020 03:22:29 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.19.tar.gz
# Fri, 11 Dec 2020 03:22:29 GMT
ENV HAPROXY_SHA256=dcc444ac0aca0917e289653134333f7c29d05d844e6cd60dd04e23b5ff80c92d
# Fri, 11 Dec 2020 03:23:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 03:23:16 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 03:23:16 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 03:23:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:23:16 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:f4cf10ca9f31aab0854647d7878dc4db838e93b892b843dde3db24f2e909a106`  
		Last Modified: Fri, 11 Dec 2020 02:17:07 GMT  
		Size: 25.7 MB (25713957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d49688e932cfd1172e54b89f394b4808b410211cb9e130e48d70154edccaede`  
		Last Modified: Fri, 11 Dec 2020 03:28:53 GMT  
		Size: 8.2 MB (8221393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:323cbfdef2ecd0916ac4bf8fda513e65902e918d5c9dc0ace76fa03ef499fb8c`  
		Last Modified: Fri, 11 Dec 2020 03:28:52 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.0.19`

```console
$ docker pull haproxy@sha256:2ac5122c552b876d986b9f90b3a8f37694339b58e6d6fda34b60992f8a926290
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

### `haproxy:2.0.19` - linux; amd64

```console
$ docker pull haproxy@sha256:7135fc678bfce1c23397af6b7b53122e9bef329c734ca2aabfe811adee11298c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.8 MB (35769472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41c49d795fc5c4cd061c666353ad2f19fcd6eb50329b510ac56382ecf978e7b9`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:06:10 GMT
ADD file:3a7bff4e139bcacc5831fd70a035c130a91b5da001dd91c08b2acd635c7064e8 in / 
# Fri, 11 Dec 2020 02:06:10 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 06:38:51 GMT
ENV HAPROXY_VERSION=2.0.19
# Fri, 11 Dec 2020 06:38:51 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.19.tar.gz
# Fri, 11 Dec 2020 06:38:52 GMT
ENV HAPROXY_SHA256=dcc444ac0aca0917e289653134333f7c29d05d844e6cd60dd04e23b5ff80c92d
# Fri, 11 Dec 2020 06:40:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 06:40:27 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 06:40:27 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 06:40:28 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 06:40:28 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:6ec7b7d162b24bd6df88abde89ceb6d7bbc2be927f025c9dd061af2b0c328cfe`  
		Last Modified: Fri, 11 Dec 2020 02:12:26 GMT  
		Size: 27.1 MB (27099295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b758f232c7dc4d22024916753373991a0466a6457ca0bc1215ad9e8c9a8dec51`  
		Last Modified: Fri, 11 Dec 2020 06:48:59 GMT  
		Size: 8.7 MB (8669797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638894b0b628d7ddbbaee45c55af12b372261a9c8b5337b7c9dd17c16fad49fd`  
		Last Modified: Fri, 11 Dec 2020 06:48:57 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0.19` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:8cc258bd57409cff7e2b4542c8db6fa2d995817940ac5841f0e3f06ccfd74ac1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32997877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de2de4e21ec94306dedbddd4a737ff19e9b518b494c58e1e3e3af07e28e8a571`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:49 GMT
ADD file:58ebb3ffaf26d9b7621efba5f109ae9d22832f2f22865cda36604b138cbdb7b8 in / 
# Fri, 11 Dec 2020 02:04:56 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 03:29:51 GMT
ENV HAPROXY_VERSION=2.0.19
# Fri, 11 Dec 2020 03:29:52 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.19.tar.gz
# Fri, 11 Dec 2020 03:29:53 GMT
ENV HAPROXY_SHA256=dcc444ac0aca0917e289653134333f7c29d05d844e6cd60dd04e23b5ff80c92d
# Fri, 11 Dec 2020 03:31:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 03:31:13 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 03:31:14 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 03:31:15 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:31:16 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:8cbd1f790d64c77fcac6c9dbfe4d4c82f0365de9438f1a42b0560dc88f9e6a55`  
		Last Modified: Fri, 11 Dec 2020 02:14:44 GMT  
		Size: 24.8 MB (24843461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7bc3bf5fc96c30185881a3ae3a6bcca28e5b3ea16d8f0372b1dbf39fe4a8155`  
		Last Modified: Fri, 11 Dec 2020 03:35:49 GMT  
		Size: 8.2 MB (8154034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac96e80c96c1d123d8e40d58695108514091a3304fa8cd85d8806b46fe97fd0c`  
		Last Modified: Fri, 11 Dec 2020 03:35:46 GMT  
		Size: 382.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0.19` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:45060ef6221834966e1db3a9dc9874352a7c968ab529246764f36d6f28008c65
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.8 MB (30808479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bddac759ec2de3eb1b79f071bba71989f3a0dd3d62ef31fad1839b0121cb942c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:23:37 GMT
ADD file:75ca842ac2d6e9f6617bb3df280af1e4c9619c9805fd5e00c1c3d6b8b4e3d802 in / 
# Fri, 11 Dec 2020 02:23:39 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 04:59:00 GMT
ENV HAPROXY_VERSION=2.0.19
# Fri, 11 Dec 2020 04:59:01 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.19.tar.gz
# Fri, 11 Dec 2020 04:59:02 GMT
ENV HAPROXY_SHA256=dcc444ac0aca0917e289653134333f7c29d05d844e6cd60dd04e23b5ff80c92d
# Fri, 11 Dec 2020 04:59:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 04:59:43 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 04:59:44 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 04:59:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 04:59:46 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c06905228d4fc5a5c840a70e2e6ced56596a8bc73abc69e6a1867bbb6f7ae7e7`  
		Last Modified: Fri, 11 Dec 2020 02:33:07 GMT  
		Size: 22.7 MB (22707662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9b9d726198fd52fe47bb9440d5179e503ba9e93683afa8bdb2bd8fd75424910`  
		Last Modified: Fri, 11 Dec 2020 05:06:19 GMT  
		Size: 8.1 MB (8100436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bffa2f708c937ce8bf07ef6dfb6cf7cf52b97b6e5bbc062e9ee191e754658752`  
		Last Modified: Fri, 11 Dec 2020 05:06:17 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0.19` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:f7d269721a59b6a73a096a5869c764242e4e9cfd3e10b02914c458323cb16966
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.4 MB (34358891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1c4c10615319a0ae64d61027d680e7075a88565a776ec60bff4649c85cb3189`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:45:53 GMT
ADD file:a5a2f039c00bc638b88cefdff4c3cd1865b4d415bf80c4fe6b496d975af7cc1f in / 
# Fri, 11 Dec 2020 02:45:57 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 05:37:47 GMT
ENV HAPROXY_VERSION=2.0.19
# Fri, 11 Dec 2020 05:37:47 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.19.tar.gz
# Fri, 11 Dec 2020 05:37:48 GMT
ENV HAPROXY_SHA256=dcc444ac0aca0917e289653134333f7c29d05d844e6cd60dd04e23b5ff80c92d
# Fri, 11 Dec 2020 05:38:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 05:38:39 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 05:38:40 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 05:38:42 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:38:43 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c9648d7fcbb6d597cf33916d8fcd207fde8ec05d764b4480d4f3e884e142a902`  
		Last Modified: Fri, 11 Dec 2020 02:53:14 GMT  
		Size: 25.9 MB (25856191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fb0cc0076100081d451a9c79e8cc68352d7301ac2c34c60fb97275fe89c8ea7`  
		Last Modified: Fri, 11 Dec 2020 05:45:05 GMT  
		Size: 8.5 MB (8502320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18f20df09e352301bb5b30d0fd2fcfca525d966e177f7b8a03b7b5fd999e96e9`  
		Last Modified: Fri, 11 Dec 2020 05:45:03 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0.19` - linux; 386

```console
$ docker pull haproxy@sha256:675cbed42ec3858a775421834e929ab3a9fc3b380e5722ab3a59634f23f12ff1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.2 MB (36221513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1362820d36b8bf6bc7a5075d172692befb1952adf3691822f8d69ae19992b11d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:07 GMT
ADD file:a0879774b23f70c4db7f7b04736cca142beb0b22e93f5952364ca990a1675552 in / 
# Fri, 11 Dec 2020 02:03:08 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 05:17:20 GMT
ENV HAPROXY_VERSION=2.0.19
# Fri, 11 Dec 2020 05:17:20 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.19.tar.gz
# Fri, 11 Dec 2020 05:17:20 GMT
ENV HAPROXY_SHA256=dcc444ac0aca0917e289653134333f7c29d05d844e6cd60dd04e23b5ff80c92d
# Fri, 11 Dec 2020 05:18:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 05:18:24 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 05:18:24 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 05:18:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:18:25 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:cfec07a090788e68b692f30d34e11dc7af0f1c8112fbc846e8e40e24faf882d7`  
		Last Modified: Fri, 11 Dec 2020 02:09:41 GMT  
		Size: 27.8 MB (27757584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:754f7d49fdacc86229f5a48e66fd5e749ff27893fcdb6700dbf1b119326a222c`  
		Last Modified: Fri, 11 Dec 2020 05:26:23 GMT  
		Size: 8.5 MB (8463549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34cd4a021af386720954307723207c719f4330f46ed9c363b7cd2539e33e9cd4`  
		Last Modified: Fri, 11 Dec 2020 05:26:21 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0.19` - linux; mips64le

```console
$ docker pull haproxy@sha256:6cc4dd47d018ce652aa82d6cec016588b780343db76136477561b44a8688e22e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33893293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4837ae5262f3c202ed08d60e86c7282eadeae0663ee3ac5963a816446c6757ba`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:30 GMT
ADD file:edb758d587972f30ef28b162dcabf79f61b685afa3c6066cb611c61abea124f3 in / 
# Fri, 11 Dec 2020 02:03:30 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 03:26:13 GMT
ENV HAPROXY_VERSION=2.0.19
# Fri, 11 Dec 2020 03:26:13 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.19.tar.gz
# Fri, 11 Dec 2020 03:26:13 GMT
ENV HAPROXY_SHA256=dcc444ac0aca0917e289653134333f7c29d05d844e6cd60dd04e23b5ff80c92d
# Fri, 11 Dec 2020 03:28:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 03:28:22 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 03:28:22 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 03:28:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:28:23 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:bed35f8e8e003f268bd91c8bc28d93f0b1463296add14ab3ec84c3d3d30e9025`  
		Last Modified: Fri, 11 Dec 2020 02:10:15 GMT  
		Size: 25.8 MB (25769881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0697ad7e10458a6ada5c07957eccb7bded5f2cec3789ee90b8d1684633c7ee5a`  
		Last Modified: Fri, 11 Dec 2020 03:34:01 GMT  
		Size: 8.1 MB (8123031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a420df40214af9b461d35080f3bafb80e7a460ccf423a0dd17edb3d8eaaa389`  
		Last Modified: Fri, 11 Dec 2020 03:33:56 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0.19` - linux; ppc64le

```console
$ docker pull haproxy@sha256:3b80238c4903a78b6a13c9291f1e14ed51f8836cb5bee207344e74583e6f528a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39458539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:762d066d8f12621a3d401ac8d6f3c8b6e73eb47c5ad0502758257a8feb8bec47`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 03:34:02 GMT
ADD file:eca1a7737bd5e84ff883c4c284c0cd22492145d9cd7ae3b8e7b490e3d8e5aefb in / 
# Fri, 11 Dec 2020 03:34:11 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 05:40:01 GMT
ENV HAPROXY_VERSION=2.0.19
# Fri, 11 Dec 2020 05:40:05 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.19.tar.gz
# Fri, 11 Dec 2020 05:40:09 GMT
ENV HAPROXY_SHA256=dcc444ac0aca0917e289653134333f7c29d05d844e6cd60dd04e23b5ff80c92d
# Fri, 11 Dec 2020 05:42:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 05:42:44 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 05:42:47 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 05:42:53 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:42:55 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c0f0648876332890be87a9f32ec4ad2a939e805be3152ab991a923f7dec2b35d`  
		Last Modified: Fri, 11 Dec 2020 03:41:39 GMT  
		Size: 30.5 MB (30524717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:559b32d0d078ef78d189a11af1eecca8cf90713f33c69e69b15219d831f0037d`  
		Last Modified: Fri, 11 Dec 2020 05:55:05 GMT  
		Size: 8.9 MB (8933442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:306aef5e924471e4d849915be88683632813bda3cad2dd930235e12a0af6b1cb`  
		Last Modified: Fri, 11 Dec 2020 05:55:03 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0.19` - linux; s390x

```console
$ docker pull haproxy@sha256:88f012f756f1881102c30804eeca1084b820e42092f923d9fc2a5f97a2800920
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33935731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23fdd23ee3ec79b6d13637e05f156baea54f090738da1e37fe1a5a980d98a58b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:12:11 GMT
ADD file:db86ce5a1665b6d8ac734c54ac249a811c58484f569b935b14772445962428aa in / 
# Fri, 11 Dec 2020 02:12:15 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 03:22:28 GMT
ENV HAPROXY_VERSION=2.0.19
# Fri, 11 Dec 2020 03:22:29 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.19.tar.gz
# Fri, 11 Dec 2020 03:22:29 GMT
ENV HAPROXY_SHA256=dcc444ac0aca0917e289653134333f7c29d05d844e6cd60dd04e23b5ff80c92d
# Fri, 11 Dec 2020 03:23:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 03:23:16 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 03:23:16 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 03:23:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:23:16 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:f4cf10ca9f31aab0854647d7878dc4db838e93b892b843dde3db24f2e909a106`  
		Last Modified: Fri, 11 Dec 2020 02:17:07 GMT  
		Size: 25.7 MB (25713957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d49688e932cfd1172e54b89f394b4808b410211cb9e130e48d70154edccaede`  
		Last Modified: Fri, 11 Dec 2020 03:28:53 GMT  
		Size: 8.2 MB (8221393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:323cbfdef2ecd0916ac4bf8fda513e65902e918d5c9dc0ace76fa03ef499fb8c`  
		Last Modified: Fri, 11 Dec 2020 03:28:52 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.0.19-alpine`

```console
$ docker pull haproxy@sha256:b458075c95e83922002d5235d1cd54c7f016a206c6449b2b3f13a6953e6d7a2a
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

### `haproxy:2.0.19-alpine` - linux; amd64

```console
$ docker pull haproxy@sha256:514f8fb884fe147c6ead1000a71c98a2ddc5c3b666a3504604b5dfc2f9a73a6d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.2 MB (9198244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3072e06472f379c4071e76317353e1b8310501ad818c754783ffa169361842f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:34:23 GMT
ENV HAPROXY_VERSION=2.0.19
# Thu, 17 Dec 2020 13:34:23 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.19.tar.gz
# Thu, 17 Dec 2020 13:34:24 GMT
ENV HAPROXY_SHA256=dcc444ac0aca0917e289653134333f7c29d05d844e6cd60dd04e23b5ff80c92d
# Thu, 17 Dec 2020 13:35:31 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 13:35:32 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 13:35:32 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 13:35:32 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 13:35:32 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc84968de80783403ccf06b01eaeb12b4a06c45595a61d0aff768f92b646ae6`  
		Last Modified: Thu, 17 Dec 2020 13:38:36 GMT  
		Size: 6.4 MB (6398797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0570ea965cd68fbdcb7944d76dadf1fb4d98425feb08badd34c3bc7576f06bee`  
		Last Modified: Thu, 17 Dec 2020 13:38:35 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0.19-alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:f9a72b57ac7366db4fbfe77eb0b3e8a7109c05e59a9208884fcfaae5017e808e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8683580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbd99ed027206d94ec4caa82d95145d41d78af8e9dbb79af82b20daebf402c65`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:38:53 GMT
ENV HAPROXY_VERSION=2.0.19
# Thu, 17 Dec 2020 01:38:54 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.19.tar.gz
# Thu, 17 Dec 2020 01:38:55 GMT
ENV HAPROXY_SHA256=dcc444ac0aca0917e289653134333f7c29d05d844e6cd60dd04e23b5ff80c92d
# Thu, 17 Dec 2020 01:39:23 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:39:24 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:39:24 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 01:39:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:39:26 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:826ffc551b22fa32d64442d34e38c0c0e8fc6b34c66d6ff5b02cc58ec58e3a8e`  
		Last Modified: Thu, 17 Dec 2020 01:41:57 GMT  
		Size: 6.1 MB (6079037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5901058f4053e307c9174eb7e2d1492e0c87da8ce32167f839f04abafb076fff`  
		Last Modified: Thu, 17 Dec 2020 01:41:55 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0.19-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:fbc5619ef23da7ba104522b46450f67ccd04f802d9e5b208f415983033211fe2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8611173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3705c20727b6a51457b1f1a4f4ab4ba5157f597764c64b8a8f1f013df818ed4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:40:54 GMT
ENV HAPROXY_VERSION=2.0.19
# Thu, 17 Dec 2020 01:40:55 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.19.tar.gz
# Thu, 17 Dec 2020 01:40:56 GMT
ENV HAPROXY_SHA256=dcc444ac0aca0917e289653134333f7c29d05d844e6cd60dd04e23b5ff80c92d
# Thu, 17 Dec 2020 01:41:15 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:41:16 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:41:17 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 01:41:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:41:18 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e8dcb1f221e30464e2e0746293cc062e3cb08c001dc4bdb406b222521c45bea`  
		Last Modified: Thu, 17 Dec 2020 01:44:00 GMT  
		Size: 6.2 MB (6203237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a89aa60a0d5060086b0ff92d4220d43dd0de5a23527bde6ba01cc14902bd77`  
		Last Modified: Thu, 17 Dec 2020 01:43:58 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0.19-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:2d613e1fa7d509fb094b2e56516943bfddfed95b5539dae0a21a8efd586ce7b5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.1 MB (9055672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e906dca2dbba673c35a61f5b95f1b64bfc3fc0dd22f24f264916b5d15226442`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:26:47 GMT
ENV HAPROXY_VERSION=2.0.19
# Thu, 17 Dec 2020 01:26:48 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.19.tar.gz
# Thu, 17 Dec 2020 01:26:50 GMT
ENV HAPROXY_SHA256=dcc444ac0aca0917e289653134333f7c29d05d844e6cd60dd04e23b5ff80c92d
# Thu, 17 Dec 2020 01:27:15 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:27:15 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:27:16 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 01:27:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:27:18 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f68ece70f0e70a22c9a91ebffa831c2cba8635f86d64167505db355d158698bd`  
		Last Modified: Thu, 17 Dec 2020 01:31:00 GMT  
		Size: 6.3 MB (6346244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ddac09a3364cd18e9546dab48988a6386c860cc75a13502fe56f2fb2ba28877`  
		Last Modified: Thu, 17 Dec 2020 01:30:58 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0.19-alpine` - linux; 386

```console
$ docker pull haproxy@sha256:8e3ca95461af242a2ca2cd545c47d7fcf126c8c0382e37be939a4b6042bd96c8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8988865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22387c1d190770f9605b8bb9c12c730d608b58dfe12d0ae2cc2dc4ecc0cedd80`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 17 Dec 2020 00:38:32 GMT
ADD file:de33fda50a142403e842620d20bc4404e66fc4ace16edc6946c4539e8a797458 in / 
# Thu, 17 Dec 2020 00:38:32 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:31:08 GMT
ENV HAPROXY_VERSION=2.0.19
# Thu, 17 Dec 2020 02:31:08 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.19.tar.gz
# Thu, 17 Dec 2020 02:31:08 GMT
ENV HAPROXY_SHA256=dcc444ac0aca0917e289653134333f7c29d05d844e6cd60dd04e23b5ff80c92d
# Thu, 17 Dec 2020 02:32:10 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 02:32:11 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 02:32:11 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 02:32:11 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 02:32:11 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:455793c72b878001f0905634ed52a2524ba51796e7377bf00683a85123f7dce9`  
		Last Modified: Thu, 17 Dec 2020 00:39:18 GMT  
		Size: 2.8 MB (2794130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ddbcfeaf3ec6c646f89ce2bc2a64f52784ea08d348992d0a5336d88796824e4`  
		Last Modified: Thu, 17 Dec 2020 02:35:13 GMT  
		Size: 6.2 MB (6194354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d66307ef763090ffce68cb51f67d6694f98f637efd1d87c8664eca5d679e0ec9`  
		Last Modified: Thu, 17 Dec 2020 02:35:12 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0.19-alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:2485ae7ac6db8fa98414583891f8ef1ef04008f3a627eae09a2c13512c46cfce
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9301129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89f910d7639b3f61b281f53e18a9b7f8861286a1e156a1bb60af2a62002e2190`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 17 Dec 2020 00:20:42 GMT
ADD file:0a38c9b4955f8faa79627c166fca80ef342e443a16ce2925a30eeae317bbd786 in / 
# Thu, 17 Dec 2020 00:20:48 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:45:20 GMT
ENV HAPROXY_VERSION=2.0.19
# Thu, 17 Dec 2020 02:45:25 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.19.tar.gz
# Thu, 17 Dec 2020 02:45:28 GMT
ENV HAPROXY_SHA256=dcc444ac0aca0917e289653134333f7c29d05d844e6cd60dd04e23b5ff80c92d
# Thu, 17 Dec 2020 02:46:03 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 02:46:07 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 02:46:10 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 02:46:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 02:46:16 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:a9d343b7bcc225fe7ac17d96a81329510ab7f31a50472311cafe7168d3107317`  
		Last Modified: Thu, 17 Dec 2020 00:21:33 GMT  
		Size: 2.8 MB (2805226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:197a32b5de93de45853083ed4b5d65027ce7fc2118bcf6e1f4ce70025e4f8a0d`  
		Last Modified: Thu, 17 Dec 2020 02:50:45 GMT  
		Size: 6.5 MB (6495523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3375a45376e9264b77cc6c08d3a998e2d38a58a0b6eced6f0f8092efc2ae3dfd`  
		Last Modified: Thu, 17 Dec 2020 02:50:44 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0.19-alpine` - linux; s390x

```console
$ docker pull haproxy@sha256:4b7587e7275ca7497d55b0832a865a5b2da092cdef536194d0c5d1c808a2f9af
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8815862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ba5a4acfadfe99372f6fdf44613bcf5602f6396b15ec82a3e12dbf4e0391eb6`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:41:37 GMT
ADD file:3ad3856d165e8760af85574a8ffa75ca44b7e1b97b64d1d6d4608445efa4b860 in / 
# Wed, 16 Dec 2020 23:41:37 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:28:22 GMT
ENV HAPROXY_VERSION=2.0.19
# Thu, 17 Dec 2020 01:28:23 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.19.tar.gz
# Thu, 17 Dec 2020 01:28:23 GMT
ENV HAPROXY_SHA256=dcc444ac0aca0917e289653134333f7c29d05d844e6cd60dd04e23b5ff80c92d
# Thu, 17 Dec 2020 01:29:04 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:29:06 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:29:06 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 01:29:07 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:29:07 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:ee52640a49e15b8b7c8edb66c2d048b26abdee8d828d6e5ef4e10a28cb15a84f`  
		Last Modified: Wed, 16 Dec 2020 23:42:15 GMT  
		Size: 2.6 MB (2567018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17db2719e0c0d7ac7e4a014cbadc69063869425954f8bff5df96f820b12abb88`  
		Last Modified: Thu, 17 Dec 2020 01:32:05 GMT  
		Size: 6.2 MB (6248464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b2f937e43b0f694e6a4b8faafef451120139c2ce510c7cf34c329facdba594`  
		Last Modified: Thu, 17 Dec 2020 01:32:04 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.0-alpine`

```console
$ docker pull haproxy@sha256:b458075c95e83922002d5235d1cd54c7f016a206c6449b2b3f13a6953e6d7a2a
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
$ docker pull haproxy@sha256:514f8fb884fe147c6ead1000a71c98a2ddc5c3b666a3504604b5dfc2f9a73a6d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.2 MB (9198244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3072e06472f379c4071e76317353e1b8310501ad818c754783ffa169361842f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:34:23 GMT
ENV HAPROXY_VERSION=2.0.19
# Thu, 17 Dec 2020 13:34:23 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.19.tar.gz
# Thu, 17 Dec 2020 13:34:24 GMT
ENV HAPROXY_SHA256=dcc444ac0aca0917e289653134333f7c29d05d844e6cd60dd04e23b5ff80c92d
# Thu, 17 Dec 2020 13:35:31 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 13:35:32 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 13:35:32 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 13:35:32 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 13:35:32 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc84968de80783403ccf06b01eaeb12b4a06c45595a61d0aff768f92b646ae6`  
		Last Modified: Thu, 17 Dec 2020 13:38:36 GMT  
		Size: 6.4 MB (6398797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0570ea965cd68fbdcb7944d76dadf1fb4d98425feb08badd34c3bc7576f06bee`  
		Last Modified: Thu, 17 Dec 2020 13:38:35 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0-alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:f9a72b57ac7366db4fbfe77eb0b3e8a7109c05e59a9208884fcfaae5017e808e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8683580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbd99ed027206d94ec4caa82d95145d41d78af8e9dbb79af82b20daebf402c65`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:38:53 GMT
ENV HAPROXY_VERSION=2.0.19
# Thu, 17 Dec 2020 01:38:54 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.19.tar.gz
# Thu, 17 Dec 2020 01:38:55 GMT
ENV HAPROXY_SHA256=dcc444ac0aca0917e289653134333f7c29d05d844e6cd60dd04e23b5ff80c92d
# Thu, 17 Dec 2020 01:39:23 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:39:24 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:39:24 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 01:39:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:39:26 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:826ffc551b22fa32d64442d34e38c0c0e8fc6b34c66d6ff5b02cc58ec58e3a8e`  
		Last Modified: Thu, 17 Dec 2020 01:41:57 GMT  
		Size: 6.1 MB (6079037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5901058f4053e307c9174eb7e2d1492e0c87da8ce32167f839f04abafb076fff`  
		Last Modified: Thu, 17 Dec 2020 01:41:55 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:fbc5619ef23da7ba104522b46450f67ccd04f802d9e5b208f415983033211fe2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.6 MB (8611173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3705c20727b6a51457b1f1a4f4ab4ba5157f597764c64b8a8f1f013df818ed4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:40:54 GMT
ENV HAPROXY_VERSION=2.0.19
# Thu, 17 Dec 2020 01:40:55 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.19.tar.gz
# Thu, 17 Dec 2020 01:40:56 GMT
ENV HAPROXY_SHA256=dcc444ac0aca0917e289653134333f7c29d05d844e6cd60dd04e23b5ff80c92d
# Thu, 17 Dec 2020 01:41:15 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:41:16 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:41:17 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 01:41:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:41:18 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e8dcb1f221e30464e2e0746293cc062e3cb08c001dc4bdb406b222521c45bea`  
		Last Modified: Thu, 17 Dec 2020 01:44:00 GMT  
		Size: 6.2 MB (6203237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a89aa60a0d5060086b0ff92d4220d43dd0de5a23527bde6ba01cc14902bd77`  
		Last Modified: Thu, 17 Dec 2020 01:43:58 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:2d613e1fa7d509fb094b2e56516943bfddfed95b5539dae0a21a8efd586ce7b5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.1 MB (9055672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e906dca2dbba673c35a61f5b95f1b64bfc3fc0dd22f24f264916b5d15226442`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:26:47 GMT
ENV HAPROXY_VERSION=2.0.19
# Thu, 17 Dec 2020 01:26:48 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.19.tar.gz
# Thu, 17 Dec 2020 01:26:50 GMT
ENV HAPROXY_SHA256=dcc444ac0aca0917e289653134333f7c29d05d844e6cd60dd04e23b5ff80c92d
# Thu, 17 Dec 2020 01:27:15 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:27:15 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:27:16 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 01:27:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:27:18 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f68ece70f0e70a22c9a91ebffa831c2cba8635f86d64167505db355d158698bd`  
		Last Modified: Thu, 17 Dec 2020 01:31:00 GMT  
		Size: 6.3 MB (6346244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ddac09a3364cd18e9546dab48988a6386c860cc75a13502fe56f2fb2ba28877`  
		Last Modified: Thu, 17 Dec 2020 01:30:58 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0-alpine` - linux; 386

```console
$ docker pull haproxy@sha256:8e3ca95461af242a2ca2cd545c47d7fcf126c8c0382e37be939a4b6042bd96c8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8988865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22387c1d190770f9605b8bb9c12c730d608b58dfe12d0ae2cc2dc4ecc0cedd80`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 17 Dec 2020 00:38:32 GMT
ADD file:de33fda50a142403e842620d20bc4404e66fc4ace16edc6946c4539e8a797458 in / 
# Thu, 17 Dec 2020 00:38:32 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:31:08 GMT
ENV HAPROXY_VERSION=2.0.19
# Thu, 17 Dec 2020 02:31:08 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.19.tar.gz
# Thu, 17 Dec 2020 02:31:08 GMT
ENV HAPROXY_SHA256=dcc444ac0aca0917e289653134333f7c29d05d844e6cd60dd04e23b5ff80c92d
# Thu, 17 Dec 2020 02:32:10 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 02:32:11 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 02:32:11 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 02:32:11 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 02:32:11 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:455793c72b878001f0905634ed52a2524ba51796e7377bf00683a85123f7dce9`  
		Last Modified: Thu, 17 Dec 2020 00:39:18 GMT  
		Size: 2.8 MB (2794130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ddbcfeaf3ec6c646f89ce2bc2a64f52784ea08d348992d0a5336d88796824e4`  
		Last Modified: Thu, 17 Dec 2020 02:35:13 GMT  
		Size: 6.2 MB (6194354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d66307ef763090ffce68cb51f67d6694f98f637efd1d87c8664eca5d679e0ec9`  
		Last Modified: Thu, 17 Dec 2020 02:35:12 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0-alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:2485ae7ac6db8fa98414583891f8ef1ef04008f3a627eae09a2c13512c46cfce
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9301129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89f910d7639b3f61b281f53e18a9b7f8861286a1e156a1bb60af2a62002e2190`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 17 Dec 2020 00:20:42 GMT
ADD file:0a38c9b4955f8faa79627c166fca80ef342e443a16ce2925a30eeae317bbd786 in / 
# Thu, 17 Dec 2020 00:20:48 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:45:20 GMT
ENV HAPROXY_VERSION=2.0.19
# Thu, 17 Dec 2020 02:45:25 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.19.tar.gz
# Thu, 17 Dec 2020 02:45:28 GMT
ENV HAPROXY_SHA256=dcc444ac0aca0917e289653134333f7c29d05d844e6cd60dd04e23b5ff80c92d
# Thu, 17 Dec 2020 02:46:03 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 02:46:07 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 02:46:10 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 02:46:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 02:46:16 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:a9d343b7bcc225fe7ac17d96a81329510ab7f31a50472311cafe7168d3107317`  
		Last Modified: Thu, 17 Dec 2020 00:21:33 GMT  
		Size: 2.8 MB (2805226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:197a32b5de93de45853083ed4b5d65027ce7fc2118bcf6e1f4ce70025e4f8a0d`  
		Last Modified: Thu, 17 Dec 2020 02:50:45 GMT  
		Size: 6.5 MB (6495523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3375a45376e9264b77cc6c08d3a998e2d38a58a0b6eced6f0f8092efc2ae3dfd`  
		Last Modified: Thu, 17 Dec 2020 02:50:44 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0-alpine` - linux; s390x

```console
$ docker pull haproxy@sha256:4b7587e7275ca7497d55b0832a865a5b2da092cdef536194d0c5d1c808a2f9af
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.8 MB (8815862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ba5a4acfadfe99372f6fdf44613bcf5602f6396b15ec82a3e12dbf4e0391eb6`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:41:37 GMT
ADD file:3ad3856d165e8760af85574a8ffa75ca44b7e1b97b64d1d6d4608445efa4b860 in / 
# Wed, 16 Dec 2020 23:41:37 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:28:22 GMT
ENV HAPROXY_VERSION=2.0.19
# Thu, 17 Dec 2020 01:28:23 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.19.tar.gz
# Thu, 17 Dec 2020 01:28:23 GMT
ENV HAPROXY_SHA256=dcc444ac0aca0917e289653134333f7c29d05d844e6cd60dd04e23b5ff80c92d
# Thu, 17 Dec 2020 01:29:04 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:29:06 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:29:06 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 01:29:07 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:29:07 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:ee52640a49e15b8b7c8edb66c2d048b26abdee8d828d6e5ef4e10a28cb15a84f`  
		Last Modified: Wed, 16 Dec 2020 23:42:15 GMT  
		Size: 2.6 MB (2567018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17db2719e0c0d7ac7e4a014cbadc69063869425954f8bff5df96f820b12abb88`  
		Last Modified: Thu, 17 Dec 2020 01:32:05 GMT  
		Size: 6.2 MB (6248464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b2f937e43b0f694e6a4b8faafef451120139c2ce510c7cf34c329facdba594`  
		Last Modified: Thu, 17 Dec 2020 01:32:04 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.1`

```console
$ docker pull haproxy@sha256:7ae9822295f310103e985cadf00d151de18e79b4dec058bc958bc7226f203b39
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

### `haproxy:2.1` - linux; amd64

```console
$ docker pull haproxy@sha256:f9a128941e55f38202c93f0cfa8f70f7eda232471d4330908132bd7a7bc68dd3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.1 MB (36148528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d02f71bf5a6ef11843e131ff4deda2ecea42e52799845277091974962a6ede5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:06:10 GMT
ADD file:3a7bff4e139bcacc5831fd70a035c130a91b5da001dd91c08b2acd635c7064e8 in / 
# Fri, 11 Dec 2020 02:06:10 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 06:36:18 GMT
ENV HAPROXY_VERSION=2.1.10
# Fri, 11 Dec 2020 06:36:18 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.1/src/haproxy-2.1.10.tar.gz
# Fri, 11 Dec 2020 06:36:18 GMT
ENV HAPROXY_SHA256=d245a06145d1d0cbe62681de84bc23dfc98afe10f8cc5c1422a447722a142a41
# Fri, 11 Dec 2020 06:37:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 06:37:22 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 06:37:22 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 06:37:23 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 06:37:23 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:6ec7b7d162b24bd6df88abde89ceb6d7bbc2be927f025c9dd061af2b0c328cfe`  
		Last Modified: Fri, 11 Dec 2020 02:12:26 GMT  
		Size: 27.1 MB (27099295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd121080b800e7504f825dde7f0d7f8cc09b6631ad5211f55cda4d590703e780`  
		Last Modified: Fri, 11 Dec 2020 06:48:35 GMT  
		Size: 9.0 MB (9048853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44434ccc257b5ae93eb41870abee4cb571e5ff482484d8993b6913f1ed8cd082`  
		Last Modified: Fri, 11 Dec 2020 06:48:32 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.1` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:d3591491ecd6c72f5d589f3cf4fbda99ce08f30f9e37de8538516e26cce202c0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.3 MB (33336706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa49159a13d579955fabccf8be204e6e1d8ba8f68ba71c0a92a43725e111567d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:49 GMT
ADD file:58ebb3ffaf26d9b7621efba5f109ae9d22832f2f22865cda36604b138cbdb7b8 in / 
# Fri, 11 Dec 2020 02:04:56 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 03:28:44 GMT
ENV HAPROXY_VERSION=2.1.10
# Fri, 11 Dec 2020 03:28:45 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.1/src/haproxy-2.1.10.tar.gz
# Fri, 11 Dec 2020 03:28:46 GMT
ENV HAPROXY_SHA256=d245a06145d1d0cbe62681de84bc23dfc98afe10f8cc5c1422a447722a142a41
# Fri, 11 Dec 2020 03:29:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 03:29:42 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 03:29:43 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 03:29:44 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:29:45 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:8cbd1f790d64c77fcac6c9dbfe4d4c82f0365de9438f1a42b0560dc88f9e6a55`  
		Last Modified: Fri, 11 Dec 2020 02:14:44 GMT  
		Size: 24.8 MB (24843461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1df6f05e8f3eee4db2c2d257efad01ff6afa4008158ec6946b3f9caa8c70d1f8`  
		Last Modified: Fri, 11 Dec 2020 03:35:38 GMT  
		Size: 8.5 MB (8492864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a293ecca8887fa8e5e7fd12e7fd1461f2176577798b1fc2b8d14a4d15c9353`  
		Last Modified: Fri, 11 Dec 2020 03:35:35 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.1` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:f49fea3222ab2d67ca0cd05e2ac68ec5d3b22792972acdf3ac42eef7b872cd27
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31151245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f8b64439f41d5bc68f9f02fceecf0227f850d0bb1d1c5cbf103cde0d7c33594`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:23:37 GMT
ADD file:75ca842ac2d6e9f6617bb3df280af1e4c9619c9805fd5e00c1c3d6b8b4e3d802 in / 
# Fri, 11 Dec 2020 02:23:39 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 04:57:16 GMT
ENV HAPROXY_VERSION=2.1.10
# Fri, 11 Dec 2020 04:57:18 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.1/src/haproxy-2.1.10.tar.gz
# Fri, 11 Dec 2020 04:57:19 GMT
ENV HAPROXY_SHA256=d245a06145d1d0cbe62681de84bc23dfc98afe10f8cc5c1422a447722a142a41
# Fri, 11 Dec 2020 04:58:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 04:58:05 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 04:58:06 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 04:58:06 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 04:58:08 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c06905228d4fc5a5c840a70e2e6ced56596a8bc73abc69e6a1867bbb6f7ae7e7`  
		Last Modified: Fri, 11 Dec 2020 02:33:07 GMT  
		Size: 22.7 MB (22707662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2101fd1a9e98fb2cec91707c2235003d0174ed96ce5ae155ce87cadec11c66d`  
		Last Modified: Fri, 11 Dec 2020 05:05:51 GMT  
		Size: 8.4 MB (8443203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4307042e2e77c0fffe81940d556fc944d0e90707e51608fb37e9d0bc75caafb6`  
		Last Modified: Fri, 11 Dec 2020 05:05:48 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.1` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:3907f2291bae4145295c5ed1049ab05f82427976f47f93530f3fe3e21b456c65
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34710129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f62798d9249f44e24484ae06c024b3a03e53011fd6207a7d24ab4d290a69dfe`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:45:53 GMT
ADD file:a5a2f039c00bc638b88cefdff4c3cd1865b4d415bf80c4fe6b496d975af7cc1f in / 
# Fri, 11 Dec 2020 02:45:57 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 05:35:57 GMT
ENV HAPROXY_VERSION=2.1.10
# Fri, 11 Dec 2020 05:35:58 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.1/src/haproxy-2.1.10.tar.gz
# Fri, 11 Dec 2020 05:35:59 GMT
ENV HAPROXY_SHA256=d245a06145d1d0cbe62681de84bc23dfc98afe10f8cc5c1422a447722a142a41
# Fri, 11 Dec 2020 05:36:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 05:36:50 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 05:36:51 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 05:36:52 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:36:53 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c9648d7fcbb6d597cf33916d8fcd207fde8ec05d764b4480d4f3e884e142a902`  
		Last Modified: Fri, 11 Dec 2020 02:53:14 GMT  
		Size: 25.9 MB (25856191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5930ba69bd091a78072ccf739f85bce9624286d05b4951ed41b6d888c3392d70`  
		Last Modified: Fri, 11 Dec 2020 05:44:41 GMT  
		Size: 8.9 MB (8853558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be43e6387d26cc00de8bc44e5ca41e656f652bd31d5945b12577a547bfdb2da3`  
		Last Modified: Fri, 11 Dec 2020 05:44:38 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.1` - linux; 386

```console
$ docker pull haproxy@sha256:e42c4428895c4a35d79af31782475ef0e98aa59687c8b080fde135f453198013
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.6 MB (36561694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01d71445be735df4f13a67c519bc8209123dca33bbd9f43acf17f5cbbabd7c69`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:07 GMT
ADD file:a0879774b23f70c4db7f7b04736cca142beb0b22e93f5952364ca990a1675552 in / 
# Fri, 11 Dec 2020 02:03:08 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 05:14:47 GMT
ENV HAPROXY_VERSION=2.1.10
# Fri, 11 Dec 2020 05:14:47 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.1/src/haproxy-2.1.10.tar.gz
# Fri, 11 Dec 2020 05:14:48 GMT
ENV HAPROXY_SHA256=d245a06145d1d0cbe62681de84bc23dfc98afe10f8cc5c1422a447722a142a41
# Fri, 11 Dec 2020 05:15:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 05:15:52 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 05:15:53 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 05:15:53 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:15:53 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:cfec07a090788e68b692f30d34e11dc7af0f1c8112fbc846e8e40e24faf882d7`  
		Last Modified: Fri, 11 Dec 2020 02:09:41 GMT  
		Size: 27.8 MB (27757584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a2412accca223e452c249003bd08cbcce351df3509e4b2cfd989aa683d873f2`  
		Last Modified: Fri, 11 Dec 2020 05:26:07 GMT  
		Size: 8.8 MB (8803730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07f544f0877b8499a45c0ec76778d853df39df3c9d200125b5877422442d0a5`  
		Last Modified: Fri, 11 Dec 2020 05:26:03 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.1` - linux; mips64le

```console
$ docker pull haproxy@sha256:f9bf4f4d759dff7c7ed8e5af2cbe8cda6f0a8134c5167c242aad6be99824331a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.2 MB (34217523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:641c90a03b5dd34c89f47b2b918264fd544513e36faf71770ab21918a2bae82a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:30 GMT
ADD file:edb758d587972f30ef28b162dcabf79f61b685afa3c6066cb611c61abea124f3 in / 
# Fri, 11 Dec 2020 02:03:30 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 03:23:47 GMT
ENV HAPROXY_VERSION=2.1.10
# Fri, 11 Dec 2020 03:23:47 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.1/src/haproxy-2.1.10.tar.gz
# Fri, 11 Dec 2020 03:23:47 GMT
ENV HAPROXY_SHA256=d245a06145d1d0cbe62681de84bc23dfc98afe10f8cc5c1422a447722a142a41
# Fri, 11 Dec 2020 03:25:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 03:25:59 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 03:25:59 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 03:25:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:26:00 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:bed35f8e8e003f268bd91c8bc28d93f0b1463296add14ab3ec84c3d3d30e9025`  
		Last Modified: Fri, 11 Dec 2020 02:10:15 GMT  
		Size: 25.8 MB (25769881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d268ddc589a11deacda07262138da0b40cf3ea02c6e19329b443b8a3872725`  
		Last Modified: Fri, 11 Dec 2020 03:33:44 GMT  
		Size: 8.4 MB (8447262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399ed9630a6c4c0697215c3725d0bc702454d326621dc688db9d829b41ac5271`  
		Last Modified: Fri, 11 Dec 2020 03:33:42 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.1` - linux; ppc64le

```console
$ docker pull haproxy@sha256:381381307939f1b8e21a73c5f76f7a74dd5ae2f983b5ddf3d02d65103d51f696
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.8 MB (39813441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:641310f8f3eecbbf328efe443fa0316fba78ab2169fa6b00fba2a7191190aaf3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 03:34:02 GMT
ADD file:eca1a7737bd5e84ff883c4c284c0cd22492145d9cd7ae3b8e7b490e3d8e5aefb in / 
# Fri, 11 Dec 2020 03:34:11 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 05:35:28 GMT
ENV HAPROXY_VERSION=2.1.10
# Fri, 11 Dec 2020 05:35:34 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.1/src/haproxy-2.1.10.tar.gz
# Fri, 11 Dec 2020 05:35:39 GMT
ENV HAPROXY_SHA256=d245a06145d1d0cbe62681de84bc23dfc98afe10f8cc5c1422a447722a142a41
# Fri, 11 Dec 2020 05:38:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 05:38:17 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 05:38:18 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 05:38:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:38:28 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c0f0648876332890be87a9f32ec4ad2a939e805be3152ab991a923f7dec2b35d`  
		Last Modified: Fri, 11 Dec 2020 03:41:39 GMT  
		Size: 30.5 MB (30524717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60d6e223866f2100cfd897121254a9e891b7295f34cf2cd2c498f70059aed5f1`  
		Last Modified: Fri, 11 Dec 2020 05:54:40 GMT  
		Size: 9.3 MB (9288344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a947cfed018c6b91a6ee5afc505779ca8bf38cd819ebeb9934818f5b1f50e24`  
		Last Modified: Fri, 11 Dec 2020 05:54:38 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.1` - linux; s390x

```console
$ docker pull haproxy@sha256:f3418a28722e30a57fa899617a567493261fa7cdc2b4561e919e551586cfedda
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34260946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b6afb7646fce1ff7fc22aa6a445c3afc19c32be974a884f1f623afed4653f40`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:12:11 GMT
ADD file:db86ce5a1665b6d8ac734c54ac249a811c58484f569b935b14772445962428aa in / 
# Fri, 11 Dec 2020 02:12:15 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 03:20:49 GMT
ENV HAPROXY_VERSION=2.1.10
# Fri, 11 Dec 2020 03:20:49 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.1/src/haproxy-2.1.10.tar.gz
# Fri, 11 Dec 2020 03:20:49 GMT
ENV HAPROXY_SHA256=d245a06145d1d0cbe62681de84bc23dfc98afe10f8cc5c1422a447722a142a41
# Fri, 11 Dec 2020 03:21:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 03:21:37 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 03:21:37 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 03:21:38 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:21:38 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:f4cf10ca9f31aab0854647d7878dc4db838e93b892b843dde3db24f2e909a106`  
		Last Modified: Fri, 11 Dec 2020 02:17:07 GMT  
		Size: 25.7 MB (25713957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6415ac38778210c6bd9d7b3bbaae09b247bb75bb1ab5957dbd281013c713f34d`  
		Last Modified: Fri, 11 Dec 2020 03:28:36 GMT  
		Size: 8.5 MB (8546609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b0b8eb8086a8249ed1c0ff85071020e1fd1f4fae65c5b8306f359ee6d06f0c6`  
		Last Modified: Fri, 11 Dec 2020 03:28:35 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.1.10`

```console
$ docker pull haproxy@sha256:7ae9822295f310103e985cadf00d151de18e79b4dec058bc958bc7226f203b39
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

### `haproxy:2.1.10` - linux; amd64

```console
$ docker pull haproxy@sha256:f9a128941e55f38202c93f0cfa8f70f7eda232471d4330908132bd7a7bc68dd3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.1 MB (36148528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d02f71bf5a6ef11843e131ff4deda2ecea42e52799845277091974962a6ede5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:06:10 GMT
ADD file:3a7bff4e139bcacc5831fd70a035c130a91b5da001dd91c08b2acd635c7064e8 in / 
# Fri, 11 Dec 2020 02:06:10 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 06:36:18 GMT
ENV HAPROXY_VERSION=2.1.10
# Fri, 11 Dec 2020 06:36:18 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.1/src/haproxy-2.1.10.tar.gz
# Fri, 11 Dec 2020 06:36:18 GMT
ENV HAPROXY_SHA256=d245a06145d1d0cbe62681de84bc23dfc98afe10f8cc5c1422a447722a142a41
# Fri, 11 Dec 2020 06:37:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 06:37:22 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 06:37:22 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 06:37:23 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 06:37:23 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:6ec7b7d162b24bd6df88abde89ceb6d7bbc2be927f025c9dd061af2b0c328cfe`  
		Last Modified: Fri, 11 Dec 2020 02:12:26 GMT  
		Size: 27.1 MB (27099295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd121080b800e7504f825dde7f0d7f8cc09b6631ad5211f55cda4d590703e780`  
		Last Modified: Fri, 11 Dec 2020 06:48:35 GMT  
		Size: 9.0 MB (9048853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44434ccc257b5ae93eb41870abee4cb571e5ff482484d8993b6913f1ed8cd082`  
		Last Modified: Fri, 11 Dec 2020 06:48:32 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.1.10` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:d3591491ecd6c72f5d589f3cf4fbda99ce08f30f9e37de8538516e26cce202c0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.3 MB (33336706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa49159a13d579955fabccf8be204e6e1d8ba8f68ba71c0a92a43725e111567d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:49 GMT
ADD file:58ebb3ffaf26d9b7621efba5f109ae9d22832f2f22865cda36604b138cbdb7b8 in / 
# Fri, 11 Dec 2020 02:04:56 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 03:28:44 GMT
ENV HAPROXY_VERSION=2.1.10
# Fri, 11 Dec 2020 03:28:45 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.1/src/haproxy-2.1.10.tar.gz
# Fri, 11 Dec 2020 03:28:46 GMT
ENV HAPROXY_SHA256=d245a06145d1d0cbe62681de84bc23dfc98afe10f8cc5c1422a447722a142a41
# Fri, 11 Dec 2020 03:29:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 03:29:42 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 03:29:43 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 03:29:44 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:29:45 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:8cbd1f790d64c77fcac6c9dbfe4d4c82f0365de9438f1a42b0560dc88f9e6a55`  
		Last Modified: Fri, 11 Dec 2020 02:14:44 GMT  
		Size: 24.8 MB (24843461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1df6f05e8f3eee4db2c2d257efad01ff6afa4008158ec6946b3f9caa8c70d1f8`  
		Last Modified: Fri, 11 Dec 2020 03:35:38 GMT  
		Size: 8.5 MB (8492864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a293ecca8887fa8e5e7fd12e7fd1461f2176577798b1fc2b8d14a4d15c9353`  
		Last Modified: Fri, 11 Dec 2020 03:35:35 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.1.10` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:f49fea3222ab2d67ca0cd05e2ac68ec5d3b22792972acdf3ac42eef7b872cd27
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31151245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f8b64439f41d5bc68f9f02fceecf0227f850d0bb1d1c5cbf103cde0d7c33594`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:23:37 GMT
ADD file:75ca842ac2d6e9f6617bb3df280af1e4c9619c9805fd5e00c1c3d6b8b4e3d802 in / 
# Fri, 11 Dec 2020 02:23:39 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 04:57:16 GMT
ENV HAPROXY_VERSION=2.1.10
# Fri, 11 Dec 2020 04:57:18 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.1/src/haproxy-2.1.10.tar.gz
# Fri, 11 Dec 2020 04:57:19 GMT
ENV HAPROXY_SHA256=d245a06145d1d0cbe62681de84bc23dfc98afe10f8cc5c1422a447722a142a41
# Fri, 11 Dec 2020 04:58:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 04:58:05 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 04:58:06 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 04:58:06 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 04:58:08 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c06905228d4fc5a5c840a70e2e6ced56596a8bc73abc69e6a1867bbb6f7ae7e7`  
		Last Modified: Fri, 11 Dec 2020 02:33:07 GMT  
		Size: 22.7 MB (22707662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2101fd1a9e98fb2cec91707c2235003d0174ed96ce5ae155ce87cadec11c66d`  
		Last Modified: Fri, 11 Dec 2020 05:05:51 GMT  
		Size: 8.4 MB (8443203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4307042e2e77c0fffe81940d556fc944d0e90707e51608fb37e9d0bc75caafb6`  
		Last Modified: Fri, 11 Dec 2020 05:05:48 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.1.10` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:3907f2291bae4145295c5ed1049ab05f82427976f47f93530f3fe3e21b456c65
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34710129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f62798d9249f44e24484ae06c024b3a03e53011fd6207a7d24ab4d290a69dfe`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:45:53 GMT
ADD file:a5a2f039c00bc638b88cefdff4c3cd1865b4d415bf80c4fe6b496d975af7cc1f in / 
# Fri, 11 Dec 2020 02:45:57 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 05:35:57 GMT
ENV HAPROXY_VERSION=2.1.10
# Fri, 11 Dec 2020 05:35:58 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.1/src/haproxy-2.1.10.tar.gz
# Fri, 11 Dec 2020 05:35:59 GMT
ENV HAPROXY_SHA256=d245a06145d1d0cbe62681de84bc23dfc98afe10f8cc5c1422a447722a142a41
# Fri, 11 Dec 2020 05:36:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 05:36:50 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 05:36:51 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 05:36:52 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:36:53 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c9648d7fcbb6d597cf33916d8fcd207fde8ec05d764b4480d4f3e884e142a902`  
		Last Modified: Fri, 11 Dec 2020 02:53:14 GMT  
		Size: 25.9 MB (25856191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5930ba69bd091a78072ccf739f85bce9624286d05b4951ed41b6d888c3392d70`  
		Last Modified: Fri, 11 Dec 2020 05:44:41 GMT  
		Size: 8.9 MB (8853558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be43e6387d26cc00de8bc44e5ca41e656f652bd31d5945b12577a547bfdb2da3`  
		Last Modified: Fri, 11 Dec 2020 05:44:38 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.1.10` - linux; 386

```console
$ docker pull haproxy@sha256:e42c4428895c4a35d79af31782475ef0e98aa59687c8b080fde135f453198013
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.6 MB (36561694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01d71445be735df4f13a67c519bc8209123dca33bbd9f43acf17f5cbbabd7c69`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:07 GMT
ADD file:a0879774b23f70c4db7f7b04736cca142beb0b22e93f5952364ca990a1675552 in / 
# Fri, 11 Dec 2020 02:03:08 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 05:14:47 GMT
ENV HAPROXY_VERSION=2.1.10
# Fri, 11 Dec 2020 05:14:47 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.1/src/haproxy-2.1.10.tar.gz
# Fri, 11 Dec 2020 05:14:48 GMT
ENV HAPROXY_SHA256=d245a06145d1d0cbe62681de84bc23dfc98afe10f8cc5c1422a447722a142a41
# Fri, 11 Dec 2020 05:15:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 05:15:52 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 05:15:53 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 05:15:53 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:15:53 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:cfec07a090788e68b692f30d34e11dc7af0f1c8112fbc846e8e40e24faf882d7`  
		Last Modified: Fri, 11 Dec 2020 02:09:41 GMT  
		Size: 27.8 MB (27757584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a2412accca223e452c249003bd08cbcce351df3509e4b2cfd989aa683d873f2`  
		Last Modified: Fri, 11 Dec 2020 05:26:07 GMT  
		Size: 8.8 MB (8803730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07f544f0877b8499a45c0ec76778d853df39df3c9d200125b5877422442d0a5`  
		Last Modified: Fri, 11 Dec 2020 05:26:03 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.1.10` - linux; mips64le

```console
$ docker pull haproxy@sha256:f9bf4f4d759dff7c7ed8e5af2cbe8cda6f0a8134c5167c242aad6be99824331a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.2 MB (34217523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:641c90a03b5dd34c89f47b2b918264fd544513e36faf71770ab21918a2bae82a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:30 GMT
ADD file:edb758d587972f30ef28b162dcabf79f61b685afa3c6066cb611c61abea124f3 in / 
# Fri, 11 Dec 2020 02:03:30 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 03:23:47 GMT
ENV HAPROXY_VERSION=2.1.10
# Fri, 11 Dec 2020 03:23:47 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.1/src/haproxy-2.1.10.tar.gz
# Fri, 11 Dec 2020 03:23:47 GMT
ENV HAPROXY_SHA256=d245a06145d1d0cbe62681de84bc23dfc98afe10f8cc5c1422a447722a142a41
# Fri, 11 Dec 2020 03:25:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 03:25:59 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 03:25:59 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 03:25:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:26:00 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:bed35f8e8e003f268bd91c8bc28d93f0b1463296add14ab3ec84c3d3d30e9025`  
		Last Modified: Fri, 11 Dec 2020 02:10:15 GMT  
		Size: 25.8 MB (25769881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d268ddc589a11deacda07262138da0b40cf3ea02c6e19329b443b8a3872725`  
		Last Modified: Fri, 11 Dec 2020 03:33:44 GMT  
		Size: 8.4 MB (8447262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399ed9630a6c4c0697215c3725d0bc702454d326621dc688db9d829b41ac5271`  
		Last Modified: Fri, 11 Dec 2020 03:33:42 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.1.10` - linux; ppc64le

```console
$ docker pull haproxy@sha256:381381307939f1b8e21a73c5f76f7a74dd5ae2f983b5ddf3d02d65103d51f696
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.8 MB (39813441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:641310f8f3eecbbf328efe443fa0316fba78ab2169fa6b00fba2a7191190aaf3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 03:34:02 GMT
ADD file:eca1a7737bd5e84ff883c4c284c0cd22492145d9cd7ae3b8e7b490e3d8e5aefb in / 
# Fri, 11 Dec 2020 03:34:11 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 05:35:28 GMT
ENV HAPROXY_VERSION=2.1.10
# Fri, 11 Dec 2020 05:35:34 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.1/src/haproxy-2.1.10.tar.gz
# Fri, 11 Dec 2020 05:35:39 GMT
ENV HAPROXY_SHA256=d245a06145d1d0cbe62681de84bc23dfc98afe10f8cc5c1422a447722a142a41
# Fri, 11 Dec 2020 05:38:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 05:38:17 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 05:38:18 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 05:38:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:38:28 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c0f0648876332890be87a9f32ec4ad2a939e805be3152ab991a923f7dec2b35d`  
		Last Modified: Fri, 11 Dec 2020 03:41:39 GMT  
		Size: 30.5 MB (30524717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60d6e223866f2100cfd897121254a9e891b7295f34cf2cd2c498f70059aed5f1`  
		Last Modified: Fri, 11 Dec 2020 05:54:40 GMT  
		Size: 9.3 MB (9288344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a947cfed018c6b91a6ee5afc505779ca8bf38cd819ebeb9934818f5b1f50e24`  
		Last Modified: Fri, 11 Dec 2020 05:54:38 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.1.10` - linux; s390x

```console
$ docker pull haproxy@sha256:f3418a28722e30a57fa899617a567493261fa7cdc2b4561e919e551586cfedda
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34260946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b6afb7646fce1ff7fc22aa6a445c3afc19c32be974a884f1f623afed4653f40`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:12:11 GMT
ADD file:db86ce5a1665b6d8ac734c54ac249a811c58484f569b935b14772445962428aa in / 
# Fri, 11 Dec 2020 02:12:15 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 03:20:49 GMT
ENV HAPROXY_VERSION=2.1.10
# Fri, 11 Dec 2020 03:20:49 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.1/src/haproxy-2.1.10.tar.gz
# Fri, 11 Dec 2020 03:20:49 GMT
ENV HAPROXY_SHA256=d245a06145d1d0cbe62681de84bc23dfc98afe10f8cc5c1422a447722a142a41
# Fri, 11 Dec 2020 03:21:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 03:21:37 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 03:21:37 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 03:21:38 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:21:38 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:f4cf10ca9f31aab0854647d7878dc4db838e93b892b843dde3db24f2e909a106`  
		Last Modified: Fri, 11 Dec 2020 02:17:07 GMT  
		Size: 25.7 MB (25713957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6415ac38778210c6bd9d7b3bbaae09b247bb75bb1ab5957dbd281013c713f34d`  
		Last Modified: Fri, 11 Dec 2020 03:28:36 GMT  
		Size: 8.5 MB (8546609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b0b8eb8086a8249ed1c0ff85071020e1fd1f4fae65c5b8306f359ee6d06f0c6`  
		Last Modified: Fri, 11 Dec 2020 03:28:35 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.1.10-alpine`

```console
$ docker pull haproxy@sha256:0ed5f487e1700fad0751001cde75c7641c0b5251a82911eac690778215af11e3
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

### `haproxy:2.1.10-alpine` - linux; amd64

```console
$ docker pull haproxy@sha256:cd5261756a3b294bf4d96e4d0e57723aadce2c913b12487dc2c521bb1c358c16
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9573449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4281c14b9af1cab8fb9936f63edda5c9e105c3a2e345fa829c5fc258cf61bf2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:33:03 GMT
ENV HAPROXY_VERSION=2.1.10
# Thu, 17 Dec 2020 13:33:03 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.1/src/haproxy-2.1.10.tar.gz
# Thu, 17 Dec 2020 13:33:03 GMT
ENV HAPROXY_SHA256=d245a06145d1d0cbe62681de84bc23dfc98afe10f8cc5c1422a447722a142a41
# Thu, 17 Dec 2020 13:34:14 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 13:34:14 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 13:34:14 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 13:34:14 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 13:34:14 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3de298fec6517641fd0d0138d49584e59429c8eb55b2491766752021713db09e`  
		Last Modified: Thu, 17 Dec 2020 13:38:24 GMT  
		Size: 6.8 MB (6774003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78ba3b9eee947c65bede4d4c31614c044cd8b8426d7991bbe481ff40ab78d103`  
		Last Modified: Thu, 17 Dec 2020 13:38:23 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.1.10-alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:c09d078ce73d0f788e647806698f3ec85c54e7a8a39b621c8b9b32dc414339f7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9033962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb5f3af3206358a62c39808aa8222b110d2c3453b7c9748ef001321168ace6a8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:38:10 GMT
ENV HAPROXY_VERSION=2.1.10
# Thu, 17 Dec 2020 01:38:10 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.1/src/haproxy-2.1.10.tar.gz
# Thu, 17 Dec 2020 01:38:11 GMT
ENV HAPROXY_SHA256=d245a06145d1d0cbe62681de84bc23dfc98afe10f8cc5c1422a447722a142a41
# Thu, 17 Dec 2020 01:38:39 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:38:40 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:38:40 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 01:38:41 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:38:41 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782df5c5356bdfb6354b9bd7b6ac2106b417aa4ce000bfe0aea7f3bc41f6588f`  
		Last Modified: Thu, 17 Dec 2020 01:41:42 GMT  
		Size: 6.4 MB (6429419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec63a4db82395714ae7bb43490ea0f1eeec2f7d4f65639f5737870d734ae0b89`  
		Last Modified: Thu, 17 Dec 2020 01:41:41 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.1.10-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:32d5bada42549851b867de06a19b2d46d93696432d1e4ee4cb129e0f4fb3b919
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8994867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:937d557dd697978ab33cd0a84519a06facfc81512a08a56bbc8b13bc2386e242`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:40:18 GMT
ENV HAPROXY_VERSION=2.1.10
# Thu, 17 Dec 2020 01:40:18 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.1/src/haproxy-2.1.10.tar.gz
# Thu, 17 Dec 2020 01:40:19 GMT
ENV HAPROXY_SHA256=d245a06145d1d0cbe62681de84bc23dfc98afe10f8cc5c1422a447722a142a41
# Thu, 17 Dec 2020 01:40:41 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:40:41 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:40:42 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 01:40:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:40:43 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b583511479fb3d9e137e5dfb7083dd8db807823941c9d36bd42c72444ab2e21`  
		Last Modified: Thu, 17 Dec 2020 01:43:48 GMT  
		Size: 6.6 MB (6586932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c5ff94de08f7e709bb5a04a14155635cf15edce4612fa640bb86c734a32bac5`  
		Last Modified: Thu, 17 Dec 2020 01:43:46 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.1.10-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:261aa3912a82e724ea30e21df70fe4e7910bf1e1188ad9c7794f8d2836e8820e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9424051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bdc76aa0182f475079f76fbd9162edb4eaafbf8176e2c24a536f67bb5a10b86`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:25:45 GMT
ENV HAPROXY_VERSION=2.1.10
# Thu, 17 Dec 2020 01:25:49 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.1/src/haproxy-2.1.10.tar.gz
# Thu, 17 Dec 2020 01:25:57 GMT
ENV HAPROXY_SHA256=d245a06145d1d0cbe62681de84bc23dfc98afe10f8cc5c1422a447722a142a41
# Thu, 17 Dec 2020 01:26:25 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:26:26 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:26:27 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 01:26:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:26:28 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e432de3863f504eff61cd3c5245d2de4970c16a31ee1cc401826d75c78f66025`  
		Last Modified: Thu, 17 Dec 2020 01:30:45 GMT  
		Size: 6.7 MB (6714623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e6e377054d2cb2b5b9ac5bb5910ed4e96a156c5f86699d3cf4827d05e5c0f77`  
		Last Modified: Thu, 17 Dec 2020 01:30:42 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.1.10-alpine` - linux; 386

```console
$ docker pull haproxy@sha256:1fceb8b102148a4deee4c7750af67bdc1a23a96b9ca9fe3a8d79efdaf9a4b93d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9336248 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:809ba0b76890128cd9bf13363286cfb0fa7fd662c0affe9dcb742ecaeaadaa48`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 17 Dec 2020 00:38:32 GMT
ADD file:de33fda50a142403e842620d20bc4404e66fc4ace16edc6946c4539e8a797458 in / 
# Thu, 17 Dec 2020 00:38:32 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:29:48 GMT
ENV HAPROXY_VERSION=2.1.10
# Thu, 17 Dec 2020 02:29:48 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.1/src/haproxy-2.1.10.tar.gz
# Thu, 17 Dec 2020 02:29:48 GMT
ENV HAPROXY_SHA256=d245a06145d1d0cbe62681de84bc23dfc98afe10f8cc5c1422a447722a142a41
# Thu, 17 Dec 2020 02:30:52 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 02:30:52 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 02:30:52 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 02:30:53 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 02:30:53 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:455793c72b878001f0905634ed52a2524ba51796e7377bf00683a85123f7dce9`  
		Last Modified: Thu, 17 Dec 2020 00:39:18 GMT  
		Size: 2.8 MB (2794130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:916cc9321dc75b7e60e9a29dcdffab88ee62c09b0aca7db4bc1180208e158dea`  
		Last Modified: Thu, 17 Dec 2020 02:35:04 GMT  
		Size: 6.5 MB (6541738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26f1291da0d685cdd6d0c3f98fba5483cd653af0a767b40b859494fd2396a4d0`  
		Last Modified: Thu, 17 Dec 2020 02:35:02 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.1.10-alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:c34d7f54c9187e121599ee5ed61d989ea4b0f74efc69ddbc5b495ba208b95ced
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9659260 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7b40011db63e5c1fff728281c4663c7ddb3663db180fa7ef462293b38f9a539`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 17 Dec 2020 00:20:42 GMT
ADD file:0a38c9b4955f8faa79627c166fca80ef342e443a16ce2925a30eeae317bbd786 in / 
# Thu, 17 Dec 2020 00:20:48 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:43:51 GMT
ENV HAPROXY_VERSION=2.1.10
# Thu, 17 Dec 2020 02:43:57 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.1/src/haproxy-2.1.10.tar.gz
# Thu, 17 Dec 2020 02:44:02 GMT
ENV HAPROXY_SHA256=d245a06145d1d0cbe62681de84bc23dfc98afe10f8cc5c1422a447722a142a41
# Thu, 17 Dec 2020 02:44:43 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 02:44:45 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 02:44:47 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 02:44:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 02:45:02 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:a9d343b7bcc225fe7ac17d96a81329510ab7f31a50472311cafe7168d3107317`  
		Last Modified: Thu, 17 Dec 2020 00:21:33 GMT  
		Size: 2.8 MB (2805226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b88e22133859a2b92c3ee5c190970eceeda72edddc87941042b560dd07b7a31`  
		Last Modified: Thu, 17 Dec 2020 02:50:30 GMT  
		Size: 6.9 MB (6853653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b398b57effc53a801ae6746f66c00610cd6d20db93e0a8d485e7365fe7e9c45b`  
		Last Modified: Thu, 17 Dec 2020 02:50:28 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.1.10-alpine` - linux; s390x

```console
$ docker pull haproxy@sha256:cf557feb8f0aaf0596d0e35620ff29dd4d08aeb5e28e193a7475462a4861f446
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.1 MB (9137591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e5021215af7e2bc542b7e45fee33690e4c587e1798823a357bc35129f727a25`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:41:37 GMT
ADD file:3ad3856d165e8760af85574a8ffa75ca44b7e1b97b64d1d6d4608445efa4b860 in / 
# Wed, 16 Dec 2020 23:41:37 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:27:20 GMT
ENV HAPROXY_VERSION=2.1.10
# Thu, 17 Dec 2020 01:27:21 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.1/src/haproxy-2.1.10.tar.gz
# Thu, 17 Dec 2020 01:27:21 GMT
ENV HAPROXY_SHA256=d245a06145d1d0cbe62681de84bc23dfc98afe10f8cc5c1422a447722a142a41
# Thu, 17 Dec 2020 01:28:03 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:28:04 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:28:04 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 01:28:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:28:05 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:ee52640a49e15b8b7c8edb66c2d048b26abdee8d828d6e5ef4e10a28cb15a84f`  
		Last Modified: Wed, 16 Dec 2020 23:42:15 GMT  
		Size: 2.6 MB (2567018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5009923e9e4c845bb9e500bc79e16cb623608f382b595714b1ce18f8e783d90a`  
		Last Modified: Thu, 17 Dec 2020 01:31:51 GMT  
		Size: 6.6 MB (6570192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ebc4a4860c73d205917736309b89885fa1e99dec5e49c8c728c9d437d26527c`  
		Last Modified: Thu, 17 Dec 2020 01:31:51 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.1-alpine`

```console
$ docker pull haproxy@sha256:0ed5f487e1700fad0751001cde75c7641c0b5251a82911eac690778215af11e3
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

### `haproxy:2.1-alpine` - linux; amd64

```console
$ docker pull haproxy@sha256:cd5261756a3b294bf4d96e4d0e57723aadce2c913b12487dc2c521bb1c358c16
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9573449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4281c14b9af1cab8fb9936f63edda5c9e105c3a2e345fa829c5fc258cf61bf2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:33:03 GMT
ENV HAPROXY_VERSION=2.1.10
# Thu, 17 Dec 2020 13:33:03 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.1/src/haproxy-2.1.10.tar.gz
# Thu, 17 Dec 2020 13:33:03 GMT
ENV HAPROXY_SHA256=d245a06145d1d0cbe62681de84bc23dfc98afe10f8cc5c1422a447722a142a41
# Thu, 17 Dec 2020 13:34:14 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 13:34:14 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 13:34:14 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 13:34:14 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 13:34:14 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3de298fec6517641fd0d0138d49584e59429c8eb55b2491766752021713db09e`  
		Last Modified: Thu, 17 Dec 2020 13:38:24 GMT  
		Size: 6.8 MB (6774003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78ba3b9eee947c65bede4d4c31614c044cd8b8426d7991bbe481ff40ab78d103`  
		Last Modified: Thu, 17 Dec 2020 13:38:23 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.1-alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:c09d078ce73d0f788e647806698f3ec85c54e7a8a39b621c8b9b32dc414339f7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9033962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb5f3af3206358a62c39808aa8222b110d2c3453b7c9748ef001321168ace6a8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:38:10 GMT
ENV HAPROXY_VERSION=2.1.10
# Thu, 17 Dec 2020 01:38:10 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.1/src/haproxy-2.1.10.tar.gz
# Thu, 17 Dec 2020 01:38:11 GMT
ENV HAPROXY_SHA256=d245a06145d1d0cbe62681de84bc23dfc98afe10f8cc5c1422a447722a142a41
# Thu, 17 Dec 2020 01:38:39 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:38:40 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:38:40 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 01:38:41 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:38:41 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782df5c5356bdfb6354b9bd7b6ac2106b417aa4ce000bfe0aea7f3bc41f6588f`  
		Last Modified: Thu, 17 Dec 2020 01:41:42 GMT  
		Size: 6.4 MB (6429419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec63a4db82395714ae7bb43490ea0f1eeec2f7d4f65639f5737870d734ae0b89`  
		Last Modified: Thu, 17 Dec 2020 01:41:41 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.1-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:32d5bada42549851b867de06a19b2d46d93696432d1e4ee4cb129e0f4fb3b919
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8994867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:937d557dd697978ab33cd0a84519a06facfc81512a08a56bbc8b13bc2386e242`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:40:18 GMT
ENV HAPROXY_VERSION=2.1.10
# Thu, 17 Dec 2020 01:40:18 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.1/src/haproxy-2.1.10.tar.gz
# Thu, 17 Dec 2020 01:40:19 GMT
ENV HAPROXY_SHA256=d245a06145d1d0cbe62681de84bc23dfc98afe10f8cc5c1422a447722a142a41
# Thu, 17 Dec 2020 01:40:41 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:40:41 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:40:42 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 01:40:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:40:43 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b583511479fb3d9e137e5dfb7083dd8db807823941c9d36bd42c72444ab2e21`  
		Last Modified: Thu, 17 Dec 2020 01:43:48 GMT  
		Size: 6.6 MB (6586932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c5ff94de08f7e709bb5a04a14155635cf15edce4612fa640bb86c734a32bac5`  
		Last Modified: Thu, 17 Dec 2020 01:43:46 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.1-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:261aa3912a82e724ea30e21df70fe4e7910bf1e1188ad9c7794f8d2836e8820e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9424051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bdc76aa0182f475079f76fbd9162edb4eaafbf8176e2c24a536f67bb5a10b86`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:25:45 GMT
ENV HAPROXY_VERSION=2.1.10
# Thu, 17 Dec 2020 01:25:49 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.1/src/haproxy-2.1.10.tar.gz
# Thu, 17 Dec 2020 01:25:57 GMT
ENV HAPROXY_SHA256=d245a06145d1d0cbe62681de84bc23dfc98afe10f8cc5c1422a447722a142a41
# Thu, 17 Dec 2020 01:26:25 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:26:26 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:26:27 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 01:26:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:26:28 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e432de3863f504eff61cd3c5245d2de4970c16a31ee1cc401826d75c78f66025`  
		Last Modified: Thu, 17 Dec 2020 01:30:45 GMT  
		Size: 6.7 MB (6714623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e6e377054d2cb2b5b9ac5bb5910ed4e96a156c5f86699d3cf4827d05e5c0f77`  
		Last Modified: Thu, 17 Dec 2020 01:30:42 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.1-alpine` - linux; 386

```console
$ docker pull haproxy@sha256:1fceb8b102148a4deee4c7750af67bdc1a23a96b9ca9fe3a8d79efdaf9a4b93d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9336248 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:809ba0b76890128cd9bf13363286cfb0fa7fd662c0affe9dcb742ecaeaadaa48`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 17 Dec 2020 00:38:32 GMT
ADD file:de33fda50a142403e842620d20bc4404e66fc4ace16edc6946c4539e8a797458 in / 
# Thu, 17 Dec 2020 00:38:32 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:29:48 GMT
ENV HAPROXY_VERSION=2.1.10
# Thu, 17 Dec 2020 02:29:48 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.1/src/haproxy-2.1.10.tar.gz
# Thu, 17 Dec 2020 02:29:48 GMT
ENV HAPROXY_SHA256=d245a06145d1d0cbe62681de84bc23dfc98afe10f8cc5c1422a447722a142a41
# Thu, 17 Dec 2020 02:30:52 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 02:30:52 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 02:30:52 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 02:30:53 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 02:30:53 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:455793c72b878001f0905634ed52a2524ba51796e7377bf00683a85123f7dce9`  
		Last Modified: Thu, 17 Dec 2020 00:39:18 GMT  
		Size: 2.8 MB (2794130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:916cc9321dc75b7e60e9a29dcdffab88ee62c09b0aca7db4bc1180208e158dea`  
		Last Modified: Thu, 17 Dec 2020 02:35:04 GMT  
		Size: 6.5 MB (6541738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26f1291da0d685cdd6d0c3f98fba5483cd653af0a767b40b859494fd2396a4d0`  
		Last Modified: Thu, 17 Dec 2020 02:35:02 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.1-alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:c34d7f54c9187e121599ee5ed61d989ea4b0f74efc69ddbc5b495ba208b95ced
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9659260 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7b40011db63e5c1fff728281c4663c7ddb3663db180fa7ef462293b38f9a539`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 17 Dec 2020 00:20:42 GMT
ADD file:0a38c9b4955f8faa79627c166fca80ef342e443a16ce2925a30eeae317bbd786 in / 
# Thu, 17 Dec 2020 00:20:48 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:43:51 GMT
ENV HAPROXY_VERSION=2.1.10
# Thu, 17 Dec 2020 02:43:57 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.1/src/haproxy-2.1.10.tar.gz
# Thu, 17 Dec 2020 02:44:02 GMT
ENV HAPROXY_SHA256=d245a06145d1d0cbe62681de84bc23dfc98afe10f8cc5c1422a447722a142a41
# Thu, 17 Dec 2020 02:44:43 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 02:44:45 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 02:44:47 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 02:44:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 02:45:02 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:a9d343b7bcc225fe7ac17d96a81329510ab7f31a50472311cafe7168d3107317`  
		Last Modified: Thu, 17 Dec 2020 00:21:33 GMT  
		Size: 2.8 MB (2805226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b88e22133859a2b92c3ee5c190970eceeda72edddc87941042b560dd07b7a31`  
		Last Modified: Thu, 17 Dec 2020 02:50:30 GMT  
		Size: 6.9 MB (6853653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b398b57effc53a801ae6746f66c00610cd6d20db93e0a8d485e7365fe7e9c45b`  
		Last Modified: Thu, 17 Dec 2020 02:50:28 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.1-alpine` - linux; s390x

```console
$ docker pull haproxy@sha256:cf557feb8f0aaf0596d0e35620ff29dd4d08aeb5e28e193a7475462a4861f446
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.1 MB (9137591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e5021215af7e2bc542b7e45fee33690e4c587e1798823a357bc35129f727a25`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:41:37 GMT
ADD file:3ad3856d165e8760af85574a8ffa75ca44b7e1b97b64d1d6d4608445efa4b860 in / 
# Wed, 16 Dec 2020 23:41:37 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:27:20 GMT
ENV HAPROXY_VERSION=2.1.10
# Thu, 17 Dec 2020 01:27:21 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.1/src/haproxy-2.1.10.tar.gz
# Thu, 17 Dec 2020 01:27:21 GMT
ENV HAPROXY_SHA256=d245a06145d1d0cbe62681de84bc23dfc98afe10f8cc5c1422a447722a142a41
# Thu, 17 Dec 2020 01:28:03 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:28:04 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:28:04 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 01:28:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:28:05 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:ee52640a49e15b8b7c8edb66c2d048b26abdee8d828d6e5ef4e10a28cb15a84f`  
		Last Modified: Wed, 16 Dec 2020 23:42:15 GMT  
		Size: 2.6 MB (2567018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5009923e9e4c845bb9e500bc79e16cb623608f382b595714b1ce18f8e783d90a`  
		Last Modified: Thu, 17 Dec 2020 01:31:51 GMT  
		Size: 6.6 MB (6570192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ebc4a4860c73d205917736309b89885fa1e99dec5e49c8c728c9d437d26527c`  
		Last Modified: Thu, 17 Dec 2020 01:31:51 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.2`

```console
$ docker pull haproxy@sha256:09bdec22b056a76eb6186125206eafb2cebca84d054bc7f34fbfb3a6ecc808bf
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
$ docker pull haproxy@sha256:8d256391453d747a976fc2981ac618686650d5b269c4adb0d4a3fa12b4135f05
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.4 MB (36361780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5cf79a9a418029a83d802f592e7af8c7b86e63fe965984432ed4a46f512706c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:06:10 GMT
ADD file:3a7bff4e139bcacc5831fd70a035c130a91b5da001dd91c08b2acd635c7064e8 in / 
# Fri, 11 Dec 2020 02:06:10 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 06:32:14 GMT
ENV HAPROXY_VERSION=2.2.6
# Fri, 11 Dec 2020 06:32:14 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.6.tar.gz
# Fri, 11 Dec 2020 06:32:15 GMT
ENV HAPROXY_SHA256=be1c6754cbaceafc4837e0c6036c7f81027a3992516435cbbbc5dc749bf5a087
# Fri, 11 Dec 2020 06:33:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 06:33:57 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 06:33:58 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 06:33:58 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 06:33:58 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:6ec7b7d162b24bd6df88abde89ceb6d7bbc2be927f025c9dd061af2b0c328cfe`  
		Last Modified: Fri, 11 Dec 2020 02:12:26 GMT  
		Size: 27.1 MB (27099295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec8cba38ca5dd282c67ba27b309ce8ac7ed06c07962c2c3c556979cd4aef595`  
		Last Modified: Fri, 11 Dec 2020 06:48:17 GMT  
		Size: 9.3 MB (9262105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f769eb67a743777a835e601828829fe93fab0c4a8aeba36631702dd503565f1f`  
		Last Modified: Fri, 11 Dec 2020 06:48:14 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:63132c4d6f537017f665eadc3498ac659596f62dad4497376bff9f68ef41967b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.7 MB (33712088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7379ce9c6013e5f08258df1958d56349c25821e28de8fad2b6ef4c49c716525`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:49 GMT
ADD file:58ebb3ffaf26d9b7621efba5f109ae9d22832f2f22865cda36604b138cbdb7b8 in / 
# Fri, 11 Dec 2020 02:04:56 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 03:27:36 GMT
ENV HAPROXY_VERSION=2.2.6
# Fri, 11 Dec 2020 03:27:37 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.6.tar.gz
# Fri, 11 Dec 2020 03:27:37 GMT
ENV HAPROXY_SHA256=be1c6754cbaceafc4837e0c6036c7f81027a3992516435cbbbc5dc749bf5a087
# Fri, 11 Dec 2020 03:28:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 03:28:25 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 03:28:26 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 03:28:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:28:28 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:8cbd1f790d64c77fcac6c9dbfe4d4c82f0365de9438f1a42b0560dc88f9e6a55`  
		Last Modified: Fri, 11 Dec 2020 02:14:44 GMT  
		Size: 24.8 MB (24843461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bbc3be8af28f619ffcbaf075fa11239304fd31314feac5bab52a950a53fec09`  
		Last Modified: Fri, 11 Dec 2020 03:35:25 GMT  
		Size: 8.9 MB (8868246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c87b4e1920b700942381841e8dda8cbd8348bbdb4c3954bbf205ef55c21eaaf5`  
		Last Modified: Fri, 11 Dec 2020 03:35:22 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:bfb727159cb18123ffe505ce5378158b3d39f733c16c50c4e0510322d2a68ef5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31385471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e846073708d57e8a4ccea6bc82f7c5f5a0478ede7cf5a1b2a00104ed74cdbb38`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:23:37 GMT
ADD file:75ca842ac2d6e9f6617bb3df280af1e4c9619c9805fd5e00c1c3d6b8b4e3d802 in / 
# Fri, 11 Dec 2020 02:23:39 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 04:55:36 GMT
ENV HAPROXY_VERSION=2.2.6
# Fri, 11 Dec 2020 04:55:37 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.6.tar.gz
# Fri, 11 Dec 2020 04:55:37 GMT
ENV HAPROXY_SHA256=be1c6754cbaceafc4837e0c6036c7f81027a3992516435cbbbc5dc749bf5a087
# Fri, 11 Dec 2020 04:56:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 04:56:22 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 04:56:23 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 04:56:23 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 04:56:24 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c06905228d4fc5a5c840a70e2e6ced56596a8bc73abc69e6a1867bbb6f7ae7e7`  
		Last Modified: Fri, 11 Dec 2020 02:33:07 GMT  
		Size: 22.7 MB (22707662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c7ae28f106557ec472cc950af6eeda82b3a0dd7783c1dac977b40d916f4fda`  
		Last Modified: Fri, 11 Dec 2020 05:05:27 GMT  
		Size: 8.7 MB (8677429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1905cfd88afb156e0ea86b3b5bccd788096b16684660928f90fff8fde968989`  
		Last Modified: Fri, 11 Dec 2020 05:05:25 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:35eeeed1ab0350d953a6fecebb8bb7d37929b15b1380f730f4a79251a23814cc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.9 MB (34938817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9431c867864058dea4ec59609fcd43b6302908aca8f0b3d18be96f688aec51ee`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:45:53 GMT
ADD file:a5a2f039c00bc638b88cefdff4c3cd1865b4d415bf80c4fe6b496d975af7cc1f in / 
# Fri, 11 Dec 2020 02:45:57 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 05:33:26 GMT
ENV HAPROXY_VERSION=2.2.6
# Fri, 11 Dec 2020 05:33:27 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.6.tar.gz
# Fri, 11 Dec 2020 05:33:28 GMT
ENV HAPROXY_SHA256=be1c6754cbaceafc4837e0c6036c7f81027a3992516435cbbbc5dc749bf5a087
# Fri, 11 Dec 2020 05:34:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 05:34:32 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 05:34:33 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 05:34:36 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:34:39 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c9648d7fcbb6d597cf33916d8fcd207fde8ec05d764b4480d4f3e884e142a902`  
		Last Modified: Fri, 11 Dec 2020 02:53:14 GMT  
		Size: 25.9 MB (25856191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1add3f9207b5ef098d2aafd4a2e15d79ca7abe80a71e060e771f2dfe4ec8f9b5`  
		Last Modified: Fri, 11 Dec 2020 05:44:16 GMT  
		Size: 9.1 MB (9082245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5a7da4f421bf47a867df37a1fa1e7a758d1464a7268d2289c0e1c300322eff4`  
		Last Modified: Fri, 11 Dec 2020 05:44:13 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2` - linux; 386

```console
$ docker pull haproxy@sha256:d87b7f3d94a73cc2d813ace1731a23ee4160bb5e16a510a282d22a2c72768923
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.9 MB (36898031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7c1b93169b077d16b58324f9d72e7b4bc73a701ca1c17bcd95fd6b7fa5655e0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:07 GMT
ADD file:a0879774b23f70c4db7f7b04736cca142beb0b22e93f5952364ca990a1675552 in / 
# Fri, 11 Dec 2020 02:03:08 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 05:10:44 GMT
ENV HAPROXY_VERSION=2.2.6
# Fri, 11 Dec 2020 05:10:44 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.6.tar.gz
# Fri, 11 Dec 2020 05:10:44 GMT
ENV HAPROXY_SHA256=be1c6754cbaceafc4837e0c6036c7f81027a3992516435cbbbc5dc749bf5a087
# Fri, 11 Dec 2020 05:12:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 05:12:23 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 05:12:23 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 05:12:23 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:12:23 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:cfec07a090788e68b692f30d34e11dc7af0f1c8112fbc846e8e40e24faf882d7`  
		Last Modified: Fri, 11 Dec 2020 02:09:41 GMT  
		Size: 27.8 MB (27757584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:081e978aa8c309ca75402a34a8e617d85ad6e185cf19fb056864296178948ae0`  
		Last Modified: Fri, 11 Dec 2020 05:25:45 GMT  
		Size: 9.1 MB (9140066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5178ce4deb6b15b8657bb5b2e232df5606ea097853a30df0d4943b6ebb8ffc`  
		Last Modified: Fri, 11 Dec 2020 05:25:42 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2` - linux; mips64le

```console
$ docker pull haproxy@sha256:1693fdc275c879fb7436b059c1a506ec7287c117479ed39dac7db7588abae3e5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.6 MB (34602107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9c743e757ccc7273b9f380196c105abd0ea2b5530b2fb5a065b5997defd61c0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:30 GMT
ADD file:edb758d587972f30ef28b162dcabf79f61b685afa3c6066cb611c61abea124f3 in / 
# Fri, 11 Dec 2020 02:03:30 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 03:21:20 GMT
ENV HAPROXY_VERSION=2.2.6
# Fri, 11 Dec 2020 03:21:21 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.6.tar.gz
# Fri, 11 Dec 2020 03:21:21 GMT
ENV HAPROXY_SHA256=be1c6754cbaceafc4837e0c6036c7f81027a3992516435cbbbc5dc749bf5a087
# Fri, 11 Dec 2020 03:23:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 03:23:42 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 03:23:42 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 03:23:42 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:23:43 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:bed35f8e8e003f268bd91c8bc28d93f0b1463296add14ab3ec84c3d3d30e9025`  
		Last Modified: Fri, 11 Dec 2020 02:10:15 GMT  
		Size: 25.8 MB (25769881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c5f65a386c1ed85efa2abfe435e79442cf5db1892acfe55e0d9db56e3148905`  
		Last Modified: Fri, 11 Dec 2020 03:33:24 GMT  
		Size: 8.8 MB (8831846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9539bf3bf1abc25ce84fdec18ef846805479679554d31d61ca022f443eac5c15`  
		Last Modified: Fri, 11 Dec 2020 03:33:18 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2` - linux; ppc64le

```console
$ docker pull haproxy@sha256:3312f227706a464629651ea9a5b0707c1bf6679d957df5c2560f66b6b2745cb6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40252016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d85fd237b4c4712e373ae95f36cfe3f5ae604d1cd847f83c57dc824008d24ffa`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 03:34:02 GMT
ADD file:eca1a7737bd5e84ff883c4c284c0cd22492145d9cd7ae3b8e7b490e3d8e5aefb in / 
# Fri, 11 Dec 2020 03:34:11 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 05:29:57 GMT
ENV HAPROXY_VERSION=2.2.6
# Fri, 11 Dec 2020 05:30:00 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.6.tar.gz
# Fri, 11 Dec 2020 05:30:03 GMT
ENV HAPROXY_SHA256=be1c6754cbaceafc4837e0c6036c7f81027a3992516435cbbbc5dc749bf5a087
# Fri, 11 Dec 2020 05:33:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 05:33:30 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 05:33:31 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 05:33:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:33:40 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c0f0648876332890be87a9f32ec4ad2a939e805be3152ab991a923f7dec2b35d`  
		Last Modified: Fri, 11 Dec 2020 03:41:39 GMT  
		Size: 30.5 MB (30524717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:477fcdb8fd9422a6d91a0b51b4a556ededd7ad2a1e2f89b36a11a751938c739c`  
		Last Modified: Fri, 11 Dec 2020 05:54:08 GMT  
		Size: 9.7 MB (9726919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1528107bda347188426c219b16ea67b373659dec38137713456ea09c7a010e`  
		Last Modified: Fri, 11 Dec 2020 05:54:06 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2` - linux; s390x

```console
$ docker pull haproxy@sha256:a591d35c15413d1a3e1e9b23e2c722e673a6f31d6e3df6bbb08d2e5f78babef5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34675346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:582fe644d7a4d5b108df1cbf93e36b3e9734da0f3cc338828c268022ebb6c0e5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:12:11 GMT
ADD file:db86ce5a1665b6d8ac734c54ac249a811c58484f569b935b14772445962428aa in / 
# Fri, 11 Dec 2020 02:12:15 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 03:18:54 GMT
ENV HAPROXY_VERSION=2.2.6
# Fri, 11 Dec 2020 03:18:54 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.6.tar.gz
# Fri, 11 Dec 2020 03:18:55 GMT
ENV HAPROXY_SHA256=be1c6754cbaceafc4837e0c6036c7f81027a3992516435cbbbc5dc749bf5a087
# Fri, 11 Dec 2020 03:19:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 03:19:50 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 03:19:50 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 03:19:51 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:19:51 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:f4cf10ca9f31aab0854647d7878dc4db838e93b892b843dde3db24f2e909a106`  
		Last Modified: Fri, 11 Dec 2020 02:17:07 GMT  
		Size: 25.7 MB (25713957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fb580d8c3a873086ed2fa8f054f0b2f3b10607a065695564201de95b7086b30`  
		Last Modified: Fri, 11 Dec 2020 03:28:12 GMT  
		Size: 9.0 MB (8961008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f34dafa5401bd4ca0f465d6a4c19fb8caeac5cdc0c00820cc720ff4b7d93f8`  
		Last Modified: Fri, 11 Dec 2020 03:28:11 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.2.6`

```console
$ docker pull haproxy@sha256:09bdec22b056a76eb6186125206eafb2cebca84d054bc7f34fbfb3a6ecc808bf
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

### `haproxy:2.2.6` - linux; amd64

```console
$ docker pull haproxy@sha256:8d256391453d747a976fc2981ac618686650d5b269c4adb0d4a3fa12b4135f05
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.4 MB (36361780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5cf79a9a418029a83d802f592e7af8c7b86e63fe965984432ed4a46f512706c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:06:10 GMT
ADD file:3a7bff4e139bcacc5831fd70a035c130a91b5da001dd91c08b2acd635c7064e8 in / 
# Fri, 11 Dec 2020 02:06:10 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 06:32:14 GMT
ENV HAPROXY_VERSION=2.2.6
# Fri, 11 Dec 2020 06:32:14 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.6.tar.gz
# Fri, 11 Dec 2020 06:32:15 GMT
ENV HAPROXY_SHA256=be1c6754cbaceafc4837e0c6036c7f81027a3992516435cbbbc5dc749bf5a087
# Fri, 11 Dec 2020 06:33:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 06:33:57 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 06:33:58 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 06:33:58 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 06:33:58 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:6ec7b7d162b24bd6df88abde89ceb6d7bbc2be927f025c9dd061af2b0c328cfe`  
		Last Modified: Fri, 11 Dec 2020 02:12:26 GMT  
		Size: 27.1 MB (27099295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec8cba38ca5dd282c67ba27b309ce8ac7ed06c07962c2c3c556979cd4aef595`  
		Last Modified: Fri, 11 Dec 2020 06:48:17 GMT  
		Size: 9.3 MB (9262105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f769eb67a743777a835e601828829fe93fab0c4a8aeba36631702dd503565f1f`  
		Last Modified: Fri, 11 Dec 2020 06:48:14 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.6` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:63132c4d6f537017f665eadc3498ac659596f62dad4497376bff9f68ef41967b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.7 MB (33712088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7379ce9c6013e5f08258df1958d56349c25821e28de8fad2b6ef4c49c716525`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:49 GMT
ADD file:58ebb3ffaf26d9b7621efba5f109ae9d22832f2f22865cda36604b138cbdb7b8 in / 
# Fri, 11 Dec 2020 02:04:56 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 03:27:36 GMT
ENV HAPROXY_VERSION=2.2.6
# Fri, 11 Dec 2020 03:27:37 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.6.tar.gz
# Fri, 11 Dec 2020 03:27:37 GMT
ENV HAPROXY_SHA256=be1c6754cbaceafc4837e0c6036c7f81027a3992516435cbbbc5dc749bf5a087
# Fri, 11 Dec 2020 03:28:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 03:28:25 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 03:28:26 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 03:28:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:28:28 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:8cbd1f790d64c77fcac6c9dbfe4d4c82f0365de9438f1a42b0560dc88f9e6a55`  
		Last Modified: Fri, 11 Dec 2020 02:14:44 GMT  
		Size: 24.8 MB (24843461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bbc3be8af28f619ffcbaf075fa11239304fd31314feac5bab52a950a53fec09`  
		Last Modified: Fri, 11 Dec 2020 03:35:25 GMT  
		Size: 8.9 MB (8868246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c87b4e1920b700942381841e8dda8cbd8348bbdb4c3954bbf205ef55c21eaaf5`  
		Last Modified: Fri, 11 Dec 2020 03:35:22 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.6` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:bfb727159cb18123ffe505ce5378158b3d39f733c16c50c4e0510322d2a68ef5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31385471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e846073708d57e8a4ccea6bc82f7c5f5a0478ede7cf5a1b2a00104ed74cdbb38`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:23:37 GMT
ADD file:75ca842ac2d6e9f6617bb3df280af1e4c9619c9805fd5e00c1c3d6b8b4e3d802 in / 
# Fri, 11 Dec 2020 02:23:39 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 04:55:36 GMT
ENV HAPROXY_VERSION=2.2.6
# Fri, 11 Dec 2020 04:55:37 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.6.tar.gz
# Fri, 11 Dec 2020 04:55:37 GMT
ENV HAPROXY_SHA256=be1c6754cbaceafc4837e0c6036c7f81027a3992516435cbbbc5dc749bf5a087
# Fri, 11 Dec 2020 04:56:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 04:56:22 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 04:56:23 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 04:56:23 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 04:56:24 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c06905228d4fc5a5c840a70e2e6ced56596a8bc73abc69e6a1867bbb6f7ae7e7`  
		Last Modified: Fri, 11 Dec 2020 02:33:07 GMT  
		Size: 22.7 MB (22707662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c7ae28f106557ec472cc950af6eeda82b3a0dd7783c1dac977b40d916f4fda`  
		Last Modified: Fri, 11 Dec 2020 05:05:27 GMT  
		Size: 8.7 MB (8677429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1905cfd88afb156e0ea86b3b5bccd788096b16684660928f90fff8fde968989`  
		Last Modified: Fri, 11 Dec 2020 05:05:25 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.6` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:35eeeed1ab0350d953a6fecebb8bb7d37929b15b1380f730f4a79251a23814cc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.9 MB (34938817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9431c867864058dea4ec59609fcd43b6302908aca8f0b3d18be96f688aec51ee`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:45:53 GMT
ADD file:a5a2f039c00bc638b88cefdff4c3cd1865b4d415bf80c4fe6b496d975af7cc1f in / 
# Fri, 11 Dec 2020 02:45:57 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 05:33:26 GMT
ENV HAPROXY_VERSION=2.2.6
# Fri, 11 Dec 2020 05:33:27 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.6.tar.gz
# Fri, 11 Dec 2020 05:33:28 GMT
ENV HAPROXY_SHA256=be1c6754cbaceafc4837e0c6036c7f81027a3992516435cbbbc5dc749bf5a087
# Fri, 11 Dec 2020 05:34:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 05:34:32 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 05:34:33 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 05:34:36 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:34:39 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c9648d7fcbb6d597cf33916d8fcd207fde8ec05d764b4480d4f3e884e142a902`  
		Last Modified: Fri, 11 Dec 2020 02:53:14 GMT  
		Size: 25.9 MB (25856191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1add3f9207b5ef098d2aafd4a2e15d79ca7abe80a71e060e771f2dfe4ec8f9b5`  
		Last Modified: Fri, 11 Dec 2020 05:44:16 GMT  
		Size: 9.1 MB (9082245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5a7da4f421bf47a867df37a1fa1e7a758d1464a7268d2289c0e1c300322eff4`  
		Last Modified: Fri, 11 Dec 2020 05:44:13 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.6` - linux; 386

```console
$ docker pull haproxy@sha256:d87b7f3d94a73cc2d813ace1731a23ee4160bb5e16a510a282d22a2c72768923
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.9 MB (36898031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7c1b93169b077d16b58324f9d72e7b4bc73a701ca1c17bcd95fd6b7fa5655e0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:07 GMT
ADD file:a0879774b23f70c4db7f7b04736cca142beb0b22e93f5952364ca990a1675552 in / 
# Fri, 11 Dec 2020 02:03:08 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 05:10:44 GMT
ENV HAPROXY_VERSION=2.2.6
# Fri, 11 Dec 2020 05:10:44 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.6.tar.gz
# Fri, 11 Dec 2020 05:10:44 GMT
ENV HAPROXY_SHA256=be1c6754cbaceafc4837e0c6036c7f81027a3992516435cbbbc5dc749bf5a087
# Fri, 11 Dec 2020 05:12:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 05:12:23 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 05:12:23 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 05:12:23 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:12:23 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:cfec07a090788e68b692f30d34e11dc7af0f1c8112fbc846e8e40e24faf882d7`  
		Last Modified: Fri, 11 Dec 2020 02:09:41 GMT  
		Size: 27.8 MB (27757584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:081e978aa8c309ca75402a34a8e617d85ad6e185cf19fb056864296178948ae0`  
		Last Modified: Fri, 11 Dec 2020 05:25:45 GMT  
		Size: 9.1 MB (9140066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5178ce4deb6b15b8657bb5b2e232df5606ea097853a30df0d4943b6ebb8ffc`  
		Last Modified: Fri, 11 Dec 2020 05:25:42 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.6` - linux; mips64le

```console
$ docker pull haproxy@sha256:1693fdc275c879fb7436b059c1a506ec7287c117479ed39dac7db7588abae3e5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.6 MB (34602107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9c743e757ccc7273b9f380196c105abd0ea2b5530b2fb5a065b5997defd61c0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:30 GMT
ADD file:edb758d587972f30ef28b162dcabf79f61b685afa3c6066cb611c61abea124f3 in / 
# Fri, 11 Dec 2020 02:03:30 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 03:21:20 GMT
ENV HAPROXY_VERSION=2.2.6
# Fri, 11 Dec 2020 03:21:21 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.6.tar.gz
# Fri, 11 Dec 2020 03:21:21 GMT
ENV HAPROXY_SHA256=be1c6754cbaceafc4837e0c6036c7f81027a3992516435cbbbc5dc749bf5a087
# Fri, 11 Dec 2020 03:23:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 03:23:42 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 03:23:42 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 03:23:42 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:23:43 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:bed35f8e8e003f268bd91c8bc28d93f0b1463296add14ab3ec84c3d3d30e9025`  
		Last Modified: Fri, 11 Dec 2020 02:10:15 GMT  
		Size: 25.8 MB (25769881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c5f65a386c1ed85efa2abfe435e79442cf5db1892acfe55e0d9db56e3148905`  
		Last Modified: Fri, 11 Dec 2020 03:33:24 GMT  
		Size: 8.8 MB (8831846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9539bf3bf1abc25ce84fdec18ef846805479679554d31d61ca022f443eac5c15`  
		Last Modified: Fri, 11 Dec 2020 03:33:18 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.6` - linux; ppc64le

```console
$ docker pull haproxy@sha256:3312f227706a464629651ea9a5b0707c1bf6679d957df5c2560f66b6b2745cb6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40252016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d85fd237b4c4712e373ae95f36cfe3f5ae604d1cd847f83c57dc824008d24ffa`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 03:34:02 GMT
ADD file:eca1a7737bd5e84ff883c4c284c0cd22492145d9cd7ae3b8e7b490e3d8e5aefb in / 
# Fri, 11 Dec 2020 03:34:11 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 05:29:57 GMT
ENV HAPROXY_VERSION=2.2.6
# Fri, 11 Dec 2020 05:30:00 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.6.tar.gz
# Fri, 11 Dec 2020 05:30:03 GMT
ENV HAPROXY_SHA256=be1c6754cbaceafc4837e0c6036c7f81027a3992516435cbbbc5dc749bf5a087
# Fri, 11 Dec 2020 05:33:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 05:33:30 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 05:33:31 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 05:33:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:33:40 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c0f0648876332890be87a9f32ec4ad2a939e805be3152ab991a923f7dec2b35d`  
		Last Modified: Fri, 11 Dec 2020 03:41:39 GMT  
		Size: 30.5 MB (30524717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:477fcdb8fd9422a6d91a0b51b4a556ededd7ad2a1e2f89b36a11a751938c739c`  
		Last Modified: Fri, 11 Dec 2020 05:54:08 GMT  
		Size: 9.7 MB (9726919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1528107bda347188426c219b16ea67b373659dec38137713456ea09c7a010e`  
		Last Modified: Fri, 11 Dec 2020 05:54:06 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.6` - linux; s390x

```console
$ docker pull haproxy@sha256:a591d35c15413d1a3e1e9b23e2c722e673a6f31d6e3df6bbb08d2e5f78babef5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34675346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:582fe644d7a4d5b108df1cbf93e36b3e9734da0f3cc338828c268022ebb6c0e5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:12:11 GMT
ADD file:db86ce5a1665b6d8ac734c54ac249a811c58484f569b935b14772445962428aa in / 
# Fri, 11 Dec 2020 02:12:15 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 03:18:54 GMT
ENV HAPROXY_VERSION=2.2.6
# Fri, 11 Dec 2020 03:18:54 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.6.tar.gz
# Fri, 11 Dec 2020 03:18:55 GMT
ENV HAPROXY_SHA256=be1c6754cbaceafc4837e0c6036c7f81027a3992516435cbbbc5dc749bf5a087
# Fri, 11 Dec 2020 03:19:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 03:19:50 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 03:19:50 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 03:19:51 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:19:51 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:f4cf10ca9f31aab0854647d7878dc4db838e93b892b843dde3db24f2e909a106`  
		Last Modified: Fri, 11 Dec 2020 02:17:07 GMT  
		Size: 25.7 MB (25713957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fb580d8c3a873086ed2fa8f054f0b2f3b10607a065695564201de95b7086b30`  
		Last Modified: Fri, 11 Dec 2020 03:28:12 GMT  
		Size: 9.0 MB (8961008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f34dafa5401bd4ca0f465d6a4c19fb8caeac5cdc0c00820cc720ff4b7d93f8`  
		Last Modified: Fri, 11 Dec 2020 03:28:11 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.2.6-alpine`

```console
$ docker pull haproxy@sha256:9bc2f658ba59c0bf73cf5ead746088fb3538c62b6ae04fa243b9a6e0e93fc276
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

### `haproxy:2.2.6-alpine` - linux; amd64

```console
$ docker pull haproxy@sha256:526dee11e5d239cff7277e614050859fc31b2c2defceb086c2b566b990f58153
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.8 MB (9840056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d6dea3f03bbca57a5827517780f65ab2ed5951a9e3e35ec438d27703daf3ebd`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:30:59 GMT
ENV HAPROXY_VERSION=2.2.6
# Thu, 17 Dec 2020 13:30:59 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.6.tar.gz
# Thu, 17 Dec 2020 13:31:00 GMT
ENV HAPROXY_SHA256=be1c6754cbaceafc4837e0c6036c7f81027a3992516435cbbbc5dc749bf5a087
# Thu, 17 Dec 2020 13:32:52 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 13:32:52 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 13:32:52 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 13:32:52 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 13:32:53 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759eb7f81a327bc1a3d612ac3a50b3b84b78a3516fcc3aabcc01e8dbfd5b9e40`  
		Last Modified: Thu, 17 Dec 2020 13:38:14 GMT  
		Size: 7.0 MB (7040609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85c4cdd2faa6bed3ca9ba8bed31b1e2574744ac8cfdc1c7108e30e5e4fd72565`  
		Last Modified: Thu, 17 Dec 2020 13:38:13 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.6-alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:2719f3b4fcb4af0feb5a5edf06c49e8a56653644170a7486ea333a5b835bd42d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9506086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0e394b8272efd1126be17e7b53d6b303ca7a952d8cd36247fc1d447090b13fc`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:37:18 GMT
ENV HAPROXY_VERSION=2.2.6
# Thu, 17 Dec 2020 01:37:19 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.6.tar.gz
# Thu, 17 Dec 2020 01:37:21 GMT
ENV HAPROXY_SHA256=be1c6754cbaceafc4837e0c6036c7f81027a3992516435cbbbc5dc749bf5a087
# Thu, 17 Dec 2020 01:37:54 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:37:55 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:37:55 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 01:37:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:37:57 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85db562c8ad7ba86d9e7b120b60063560d79bfa30565b71dfe8a474e25d730f6`  
		Last Modified: Thu, 17 Dec 2020 01:41:30 GMT  
		Size: 6.9 MB (6901544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:232105dd31bf2e77869f401d6d599b724067ac9f2142a6bef35c760ccbfc8940`  
		Last Modified: Thu, 17 Dec 2020 01:41:27 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.6-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:daa8862e7c0f0b79f9c2ea2eb57a3788c86f9e0933de00610975716d73c4ebb0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9269715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3641a5ac74cfeb1efef1023f9b65091f0d0ddf47e5f2a930029b78565b59573c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:39:30 GMT
ENV HAPROXY_VERSION=2.2.6
# Thu, 17 Dec 2020 01:39:31 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.6.tar.gz
# Thu, 17 Dec 2020 01:39:32 GMT
ENV HAPROXY_SHA256=be1c6754cbaceafc4837e0c6036c7f81027a3992516435cbbbc5dc749bf5a087
# Thu, 17 Dec 2020 01:39:59 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:40:00 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:40:01 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 01:40:02 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:40:02 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b6e463615171e2a31179dd5ff1429d294d7ab17460f19303a0d5adcdce81757`  
		Last Modified: Thu, 17 Dec 2020 01:43:35 GMT  
		Size: 6.9 MB (6861780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7962c64ebb536fd12e3b688fcd64bd1df74149b49fd9b0520993e274c6e174`  
		Last Modified: Thu, 17 Dec 2020 01:43:32 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.6-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:30f8dd480c7bc2d7e8272f78dbb1e4d041de19e06298f26cd7503208692c8d80
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9709280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d600a937a50a5d5ace5d635075a67ffeed8714c9cd6cce90cccf68d4c6326b0c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:24:58 GMT
ENV HAPROXY_VERSION=2.2.6
# Thu, 17 Dec 2020 01:25:00 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.6.tar.gz
# Thu, 17 Dec 2020 01:25:01 GMT
ENV HAPROXY_SHA256=be1c6754cbaceafc4837e0c6036c7f81027a3992516435cbbbc5dc749bf5a087
# Thu, 17 Dec 2020 01:25:24 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:25:25 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:25:26 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 01:25:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:25:27 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5bed8e0c2754d35b1f66e5672f12caaccc4ccdd8586e63ab1890e73ba592f42`  
		Last Modified: Thu, 17 Dec 2020 01:30:31 GMT  
		Size: 7.0 MB (6999852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f29e8e256e27e16150bcdfc08f5158e053ff5b588556906ff5accd0943a7d1`  
		Last Modified: Thu, 17 Dec 2020 01:30:30 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.6-alpine` - linux; 386

```console
$ docker pull haproxy@sha256:72f2efb3ad6b3004c443030e00d357f061958441d278a361537fb72656f3d907
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.8 MB (9773186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41212fb3cc8f9751506f26530dc2286344e63bb880d8a9ad4ef56025ab2d9814`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 17 Dec 2020 00:38:32 GMT
ADD file:de33fda50a142403e842620d20bc4404e66fc4ace16edc6946c4539e8a797458 in / 
# Thu, 17 Dec 2020 00:38:32 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:28:14 GMT
ENV HAPROXY_VERSION=2.2.6
# Thu, 17 Dec 2020 02:28:14 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.6.tar.gz
# Thu, 17 Dec 2020 02:28:14 GMT
ENV HAPROXY_SHA256=be1c6754cbaceafc4837e0c6036c7f81027a3992516435cbbbc5dc749bf5a087
# Thu, 17 Dec 2020 02:29:36 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 02:29:36 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 02:29:37 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 02:29:37 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 02:29:37 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:455793c72b878001f0905634ed52a2524ba51796e7377bf00683a85123f7dce9`  
		Last Modified: Thu, 17 Dec 2020 00:39:18 GMT  
		Size: 2.8 MB (2794130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d138995e356aece6ca41b32bb307e0afaa434035ffc74910401a28f9eeea344`  
		Last Modified: Thu, 17 Dec 2020 02:34:56 GMT  
		Size: 7.0 MB (6978676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0fb3a312dbd21c06c01bb58d7da51e9321383895092ed35a567a9fed213c114`  
		Last Modified: Thu, 17 Dec 2020 02:34:54 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.6-alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:bec2a820948b8188b294d1bcd1ac7394cdd3c6031285be0c10940ca2a469e655
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.2 MB (10187069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6ad91eb8f93d270fd69f9895dc48452bc82037af79cfc72117b61b4b47184d7`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 17 Dec 2020 00:20:42 GMT
ADD file:0a38c9b4955f8faa79627c166fca80ef342e443a16ce2925a30eeae317bbd786 in / 
# Thu, 17 Dec 2020 00:20:48 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:42:08 GMT
ENV HAPROXY_VERSION=2.2.6
# Thu, 17 Dec 2020 02:42:16 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.6.tar.gz
# Thu, 17 Dec 2020 02:42:26 GMT
ENV HAPROXY_SHA256=be1c6754cbaceafc4837e0c6036c7f81027a3992516435cbbbc5dc749bf5a087
# Thu, 17 Dec 2020 02:43:07 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 02:43:16 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 02:43:22 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 02:43:28 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 02:43:33 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:a9d343b7bcc225fe7ac17d96a81329510ab7f31a50472311cafe7168d3107317`  
		Last Modified: Thu, 17 Dec 2020 00:21:33 GMT  
		Size: 2.8 MB (2805226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77cd771ed6b5e28c4a26cf193ce198e156b11fc7f6f673db8150a9d3120daefc`  
		Last Modified: Thu, 17 Dec 2020 02:50:13 GMT  
		Size: 7.4 MB (7381462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8848329b6093e7e582622ed4c4addc36d9fc50bb4643bf47f01440775e10773`  
		Last Modified: Thu, 17 Dec 2020 02:50:12 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.6-alpine` - linux; s390x

```console
$ docker pull haproxy@sha256:62f9c9c476998bc0d23607d30d909c35fc5c89640982ed8b6cf21f74eaef2e9d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9653023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b66e3eb0a0d2ba561a17f668ee34c3254f2f3d409dca460dca0ec86b8f4f1a51`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:41:37 GMT
ADD file:3ad3856d165e8760af85574a8ffa75ca44b7e1b97b64d1d6d4608445efa4b860 in / 
# Wed, 16 Dec 2020 23:41:37 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:26:18 GMT
ENV HAPROXY_VERSION=2.2.6
# Thu, 17 Dec 2020 01:26:18 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.6.tar.gz
# Thu, 17 Dec 2020 01:26:19 GMT
ENV HAPROXY_SHA256=be1c6754cbaceafc4837e0c6036c7f81027a3992516435cbbbc5dc749bf5a087
# Thu, 17 Dec 2020 01:27:05 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:27:06 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:27:07 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 01:27:07 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:27:08 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:ee52640a49e15b8b7c8edb66c2d048b26abdee8d828d6e5ef4e10a28cb15a84f`  
		Last Modified: Wed, 16 Dec 2020 23:42:15 GMT  
		Size: 2.6 MB (2567018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9ec00b782bf6a7bcf6d4c23d67da618049c965a58a5f25bac4ded1c3db27b4`  
		Last Modified: Thu, 17 Dec 2020 01:31:34 GMT  
		Size: 7.1 MB (7085625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a55622d8f9ba26c780c474e60ce94e0755d30d28639d58ab1fbd7f129d4e30d`  
		Last Modified: Thu, 17 Dec 2020 01:31:33 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.2-alpine`

```console
$ docker pull haproxy@sha256:9bc2f658ba59c0bf73cf5ead746088fb3538c62b6ae04fa243b9a6e0e93fc276
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
$ docker pull haproxy@sha256:526dee11e5d239cff7277e614050859fc31b2c2defceb086c2b566b990f58153
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.8 MB (9840056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d6dea3f03bbca57a5827517780f65ab2ed5951a9e3e35ec438d27703daf3ebd`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:30:59 GMT
ENV HAPROXY_VERSION=2.2.6
# Thu, 17 Dec 2020 13:30:59 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.6.tar.gz
# Thu, 17 Dec 2020 13:31:00 GMT
ENV HAPROXY_SHA256=be1c6754cbaceafc4837e0c6036c7f81027a3992516435cbbbc5dc749bf5a087
# Thu, 17 Dec 2020 13:32:52 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 13:32:52 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 13:32:52 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 13:32:52 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 13:32:53 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759eb7f81a327bc1a3d612ac3a50b3b84b78a3516fcc3aabcc01e8dbfd5b9e40`  
		Last Modified: Thu, 17 Dec 2020 13:38:14 GMT  
		Size: 7.0 MB (7040609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85c4cdd2faa6bed3ca9ba8bed31b1e2574744ac8cfdc1c7108e30e5e4fd72565`  
		Last Modified: Thu, 17 Dec 2020 13:38:13 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2-alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:2719f3b4fcb4af0feb5a5edf06c49e8a56653644170a7486ea333a5b835bd42d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9506086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0e394b8272efd1126be17e7b53d6b303ca7a952d8cd36247fc1d447090b13fc`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:37:18 GMT
ENV HAPROXY_VERSION=2.2.6
# Thu, 17 Dec 2020 01:37:19 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.6.tar.gz
# Thu, 17 Dec 2020 01:37:21 GMT
ENV HAPROXY_SHA256=be1c6754cbaceafc4837e0c6036c7f81027a3992516435cbbbc5dc749bf5a087
# Thu, 17 Dec 2020 01:37:54 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:37:55 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:37:55 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 01:37:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:37:57 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85db562c8ad7ba86d9e7b120b60063560d79bfa30565b71dfe8a474e25d730f6`  
		Last Modified: Thu, 17 Dec 2020 01:41:30 GMT  
		Size: 6.9 MB (6901544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:232105dd31bf2e77869f401d6d599b724067ac9f2142a6bef35c760ccbfc8940`  
		Last Modified: Thu, 17 Dec 2020 01:41:27 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:daa8862e7c0f0b79f9c2ea2eb57a3788c86f9e0933de00610975716d73c4ebb0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9269715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3641a5ac74cfeb1efef1023f9b65091f0d0ddf47e5f2a930029b78565b59573c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:39:30 GMT
ENV HAPROXY_VERSION=2.2.6
# Thu, 17 Dec 2020 01:39:31 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.6.tar.gz
# Thu, 17 Dec 2020 01:39:32 GMT
ENV HAPROXY_SHA256=be1c6754cbaceafc4837e0c6036c7f81027a3992516435cbbbc5dc749bf5a087
# Thu, 17 Dec 2020 01:39:59 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:40:00 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:40:01 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 01:40:02 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:40:02 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b6e463615171e2a31179dd5ff1429d294d7ab17460f19303a0d5adcdce81757`  
		Last Modified: Thu, 17 Dec 2020 01:43:35 GMT  
		Size: 6.9 MB (6861780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7962c64ebb536fd12e3b688fcd64bd1df74149b49fd9b0520993e274c6e174`  
		Last Modified: Thu, 17 Dec 2020 01:43:32 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:30f8dd480c7bc2d7e8272f78dbb1e4d041de19e06298f26cd7503208692c8d80
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9709280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d600a937a50a5d5ace5d635075a67ffeed8714c9cd6cce90cccf68d4c6326b0c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:24:58 GMT
ENV HAPROXY_VERSION=2.2.6
# Thu, 17 Dec 2020 01:25:00 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.6.tar.gz
# Thu, 17 Dec 2020 01:25:01 GMT
ENV HAPROXY_SHA256=be1c6754cbaceafc4837e0c6036c7f81027a3992516435cbbbc5dc749bf5a087
# Thu, 17 Dec 2020 01:25:24 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:25:25 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:25:26 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 01:25:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:25:27 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5bed8e0c2754d35b1f66e5672f12caaccc4ccdd8586e63ab1890e73ba592f42`  
		Last Modified: Thu, 17 Dec 2020 01:30:31 GMT  
		Size: 7.0 MB (6999852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f29e8e256e27e16150bcdfc08f5158e053ff5b588556906ff5accd0943a7d1`  
		Last Modified: Thu, 17 Dec 2020 01:30:30 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2-alpine` - linux; 386

```console
$ docker pull haproxy@sha256:72f2efb3ad6b3004c443030e00d357f061958441d278a361537fb72656f3d907
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.8 MB (9773186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41212fb3cc8f9751506f26530dc2286344e63bb880d8a9ad4ef56025ab2d9814`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 17 Dec 2020 00:38:32 GMT
ADD file:de33fda50a142403e842620d20bc4404e66fc4ace16edc6946c4539e8a797458 in / 
# Thu, 17 Dec 2020 00:38:32 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:28:14 GMT
ENV HAPROXY_VERSION=2.2.6
# Thu, 17 Dec 2020 02:28:14 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.6.tar.gz
# Thu, 17 Dec 2020 02:28:14 GMT
ENV HAPROXY_SHA256=be1c6754cbaceafc4837e0c6036c7f81027a3992516435cbbbc5dc749bf5a087
# Thu, 17 Dec 2020 02:29:36 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 02:29:36 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 02:29:37 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 02:29:37 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 02:29:37 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:455793c72b878001f0905634ed52a2524ba51796e7377bf00683a85123f7dce9`  
		Last Modified: Thu, 17 Dec 2020 00:39:18 GMT  
		Size: 2.8 MB (2794130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d138995e356aece6ca41b32bb307e0afaa434035ffc74910401a28f9eeea344`  
		Last Modified: Thu, 17 Dec 2020 02:34:56 GMT  
		Size: 7.0 MB (6978676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0fb3a312dbd21c06c01bb58d7da51e9321383895092ed35a567a9fed213c114`  
		Last Modified: Thu, 17 Dec 2020 02:34:54 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2-alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:bec2a820948b8188b294d1bcd1ac7394cdd3c6031285be0c10940ca2a469e655
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.2 MB (10187069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6ad91eb8f93d270fd69f9895dc48452bc82037af79cfc72117b61b4b47184d7`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 17 Dec 2020 00:20:42 GMT
ADD file:0a38c9b4955f8faa79627c166fca80ef342e443a16ce2925a30eeae317bbd786 in / 
# Thu, 17 Dec 2020 00:20:48 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:42:08 GMT
ENV HAPROXY_VERSION=2.2.6
# Thu, 17 Dec 2020 02:42:16 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.6.tar.gz
# Thu, 17 Dec 2020 02:42:26 GMT
ENV HAPROXY_SHA256=be1c6754cbaceafc4837e0c6036c7f81027a3992516435cbbbc5dc749bf5a087
# Thu, 17 Dec 2020 02:43:07 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 02:43:16 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 02:43:22 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 02:43:28 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 02:43:33 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:a9d343b7bcc225fe7ac17d96a81329510ab7f31a50472311cafe7168d3107317`  
		Last Modified: Thu, 17 Dec 2020 00:21:33 GMT  
		Size: 2.8 MB (2805226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77cd771ed6b5e28c4a26cf193ce198e156b11fc7f6f673db8150a9d3120daefc`  
		Last Modified: Thu, 17 Dec 2020 02:50:13 GMT  
		Size: 7.4 MB (7381462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8848329b6093e7e582622ed4c4addc36d9fc50bb4643bf47f01440775e10773`  
		Last Modified: Thu, 17 Dec 2020 02:50:12 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2-alpine` - linux; s390x

```console
$ docker pull haproxy@sha256:62f9c9c476998bc0d23607d30d909c35fc5c89640982ed8b6cf21f74eaef2e9d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9653023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b66e3eb0a0d2ba561a17f668ee34c3254f2f3d409dca460dca0ec86b8f4f1a51`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:41:37 GMT
ADD file:3ad3856d165e8760af85574a8ffa75ca44b7e1b97b64d1d6d4608445efa4b860 in / 
# Wed, 16 Dec 2020 23:41:37 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:26:18 GMT
ENV HAPROXY_VERSION=2.2.6
# Thu, 17 Dec 2020 01:26:18 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.6.tar.gz
# Thu, 17 Dec 2020 01:26:19 GMT
ENV HAPROXY_SHA256=be1c6754cbaceafc4837e0c6036c7f81027a3992516435cbbbc5dc749bf5a087
# Thu, 17 Dec 2020 01:27:05 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:27:06 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:27:07 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 01:27:07 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:27:08 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:ee52640a49e15b8b7c8edb66c2d048b26abdee8d828d6e5ef4e10a28cb15a84f`  
		Last Modified: Wed, 16 Dec 2020 23:42:15 GMT  
		Size: 2.6 MB (2567018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9ec00b782bf6a7bcf6d4c23d67da618049c965a58a5f25bac4ded1c3db27b4`  
		Last Modified: Thu, 17 Dec 2020 01:31:34 GMT  
		Size: 7.1 MB (7085625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a55622d8f9ba26c780c474e60ce94e0755d30d28639d58ab1fbd7f129d4e30d`  
		Last Modified: Thu, 17 Dec 2020 01:31:33 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.3`

```console
$ docker pull haproxy@sha256:889b4c9d7fc1bc96de9003dbd7032e4fc43ec75194b69d4a2ac401f1f24f4e16
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
$ docker pull haproxy@sha256:4860d9794eda9fb82255fc89d6dce85ad5a9ef14b47b9ebeec6539e6179eb99c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.7 MB (36738634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecf07e33b5c4bbb59188bf77781c047d9ff8accdf21b1902212b4c04864982a8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:06:10 GMT
ADD file:3a7bff4e139bcacc5831fd70a035c130a91b5da001dd91c08b2acd635c7064e8 in / 
# Fri, 11 Dec 2020 02:06:10 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 06:28:09 GMT
ENV HAPROXY_VERSION=2.3.2
# Fri, 11 Dec 2020 06:28:09 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.2.tar.gz
# Fri, 11 Dec 2020 06:28:09 GMT
ENV HAPROXY_SHA256=99cb73bb791a2cd18898d0595e14fdc820a6cbd622c762f4ed83f2884d038fd5
# Fri, 11 Dec 2020 06:29:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 06:29:46 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 06:29:47 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 06:29:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 06:29:47 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:6ec7b7d162b24bd6df88abde89ceb6d7bbc2be927f025c9dd061af2b0c328cfe`  
		Last Modified: Fri, 11 Dec 2020 02:12:26 GMT  
		Size: 27.1 MB (27099295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:babde0d7067ce5bb18c684bf031cfae2b1347e9c1b33dcd28534e777e3be722f`  
		Last Modified: Fri, 11 Dec 2020 06:48:01 GMT  
		Size: 9.6 MB (9638959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5481c8a4effb2e57ba600574d8f3d55527251112fad63bde55889ef48e2aa889`  
		Last Modified: Fri, 11 Dec 2020 06:47:51 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:ce1efa598867b2b6bdc23e8939cf570bd497ca50cf89cbd5cf47df73f4455d5c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34094439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e4360389b6e24cf55fe8b4f15e16bb3de800395360213a6e196e51383e33272`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:49 GMT
ADD file:58ebb3ffaf26d9b7621efba5f109ae9d22832f2f22865cda36604b138cbdb7b8 in / 
# Fri, 11 Dec 2020 02:04:56 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 03:26:28 GMT
ENV HAPROXY_VERSION=2.3.2
# Fri, 11 Dec 2020 03:26:30 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.2.tar.gz
# Fri, 11 Dec 2020 03:26:32 GMT
ENV HAPROXY_SHA256=99cb73bb791a2cd18898d0595e14fdc820a6cbd622c762f4ed83f2884d038fd5
# Fri, 11 Dec 2020 03:27:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 03:27:26 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 03:27:27 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 03:27:28 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:27:29 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:8cbd1f790d64c77fcac6c9dbfe4d4c82f0365de9438f1a42b0560dc88f9e6a55`  
		Last Modified: Fri, 11 Dec 2020 02:14:44 GMT  
		Size: 24.8 MB (24843461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8201a0540f14f83cebd166f9eb8b2e6868ae479bb9d88db3782b27f4475f6115`  
		Last Modified: Fri, 11 Dec 2020 03:35:10 GMT  
		Size: 9.3 MB (9250597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f414bb6e55af4c969210ca000a4e3db02adcdc632ce2fa733d23c23f4cee46d`  
		Last Modified: Fri, 11 Dec 2020 03:35:06 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:799c4cf3d5511ec7a381d76d624bfda090da64f0f7a570ebea7f7fb2492c2b08
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31774902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34a16b900cd9c658ddc60b921684ffb64fdc25dccbc6cb2d0ba445fa99c76cb1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:23:37 GMT
ADD file:75ca842ac2d6e9f6617bb3df280af1e4c9619c9805fd5e00c1c3d6b8b4e3d802 in / 
# Fri, 11 Dec 2020 02:23:39 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 04:53:56 GMT
ENV HAPROXY_VERSION=2.3.2
# Fri, 11 Dec 2020 04:53:57 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.2.tar.gz
# Fri, 11 Dec 2020 04:53:58 GMT
ENV HAPROXY_SHA256=99cb73bb791a2cd18898d0595e14fdc820a6cbd622c762f4ed83f2884d038fd5
# Fri, 11 Dec 2020 04:54:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 04:54:42 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 04:54:44 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 04:54:44 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 04:54:46 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c06905228d4fc5a5c840a70e2e6ced56596a8bc73abc69e6a1867bbb6f7ae7e7`  
		Last Modified: Fri, 11 Dec 2020 02:33:07 GMT  
		Size: 22.7 MB (22707662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b18920727745d1198efa252a298135ebb3e0cee3f2be2ec4aed8608d42e8c7c`  
		Last Modified: Fri, 11 Dec 2020 05:04:59 GMT  
		Size: 9.1 MB (9066859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:503a299b85cfeda421f53031cf13ae1d8f2328cf24410ca507aa257db3a584e8`  
		Last Modified: Fri, 11 Dec 2020 05:04:57 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:4797dffb4de987894cd0d7e3fddf97dd39e17fd34f409630724501d5d54f3375
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35320778 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1073c1f4bbe1be3699a00df24887f2b7b22c658b160f8e69caeaed50a856a06d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:45:53 GMT
ADD file:a5a2f039c00bc638b88cefdff4c3cd1865b4d415bf80c4fe6b496d975af7cc1f in / 
# Fri, 11 Dec 2020 02:45:57 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 05:31:27 GMT
ENV HAPROXY_VERSION=2.3.2
# Fri, 11 Dec 2020 05:31:28 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.2.tar.gz
# Fri, 11 Dec 2020 05:31:29 GMT
ENV HAPROXY_SHA256=99cb73bb791a2cd18898d0595e14fdc820a6cbd622c762f4ed83f2884d038fd5
# Fri, 11 Dec 2020 05:32:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 05:32:23 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 05:32:24 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 05:32:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:32:26 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c9648d7fcbb6d597cf33916d8fcd207fde8ec05d764b4480d4f3e884e142a902`  
		Last Modified: Fri, 11 Dec 2020 02:53:14 GMT  
		Size: 25.9 MB (25856191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a03032109a3408c7f6452a59eba9ff651f3be467ace9c735b2c151cb7b9cb31`  
		Last Modified: Fri, 11 Dec 2020 05:43:52 GMT  
		Size: 9.5 MB (9464207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780c192d356a56d112c0bff8106c349e11329c5e23d76dd868a996bf09dd50f9`  
		Last Modified: Fri, 11 Dec 2020 05:43:50 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3` - linux; 386

```console
$ docker pull haproxy@sha256:3b84c007b2fb56ce5380065119d78475dba59a3bfeb417be3edb6c2bdda80d60
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37287145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1fd13752edbb99935735f761ee08efa7ec780f27a6f8d7026ea8b5086d9c332`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:07 GMT
ADD file:a0879774b23f70c4db7f7b04736cca142beb0b22e93f5952364ca990a1675552 in / 
# Fri, 11 Dec 2020 02:03:08 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 05:06:25 GMT
ENV HAPROXY_VERSION=2.3.2
# Fri, 11 Dec 2020 05:06:25 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.2.tar.gz
# Fri, 11 Dec 2020 05:06:26 GMT
ENV HAPROXY_SHA256=99cb73bb791a2cd18898d0595e14fdc820a6cbd622c762f4ed83f2884d038fd5
# Fri, 11 Dec 2020 05:08:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 05:08:06 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 05:08:07 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 05:08:07 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:08:08 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:cfec07a090788e68b692f30d34e11dc7af0f1c8112fbc846e8e40e24faf882d7`  
		Last Modified: Fri, 11 Dec 2020 02:09:41 GMT  
		Size: 27.8 MB (27757584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d24160835d3ce6cd6a891511665f008d92aa7b2785ad76b373c67d9e555158af`  
		Last Modified: Fri, 11 Dec 2020 05:25:25 GMT  
		Size: 9.5 MB (9529181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c720f841b372f39c960735d688b1a090f8287dd22c78278da10850ed3675fd9`  
		Last Modified: Fri, 11 Dec 2020 05:25:22 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3` - linux; mips64le

```console
$ docker pull haproxy@sha256:47fe68bf4ccd8b76178f984ee18686fc7618231049db8d91d3b31ab017a7d93c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.0 MB (34986193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b7bee85f1b7b1ba34fa6c15d4003eb40217a24da9445980254f2f8cf07239f2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:30 GMT
ADD file:edb758d587972f30ef28b162dcabf79f61b685afa3c6066cb611c61abea124f3 in / 
# Fri, 11 Dec 2020 02:03:30 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 03:18:39 GMT
ENV HAPROXY_VERSION=2.3.2
# Fri, 11 Dec 2020 03:18:39 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.2.tar.gz
# Fri, 11 Dec 2020 03:18:39 GMT
ENV HAPROXY_SHA256=99cb73bb791a2cd18898d0595e14fdc820a6cbd622c762f4ed83f2884d038fd5
# Fri, 11 Dec 2020 03:21:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 03:21:02 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 03:21:02 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 03:21:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:21:03 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:bed35f8e8e003f268bd91c8bc28d93f0b1463296add14ab3ec84c3d3d30e9025`  
		Last Modified: Fri, 11 Dec 2020 02:10:15 GMT  
		Size: 25.8 MB (25769881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56160242f2040d557d6d1772d02a223df3069a8367382e6a1e259b1196effe92`  
		Last Modified: Fri, 11 Dec 2020 03:33:03 GMT  
		Size: 9.2 MB (9215932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ccc4a11e34e39a69c2886e2edd20c1c5a156411ca4db70a665bfb097227c14`  
		Last Modified: Fri, 11 Dec 2020 03:32:56 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3` - linux; ppc64le

```console
$ docker pull haproxy@sha256:37819fd7b83a49c2986493f3be3d2183c638125f75688d202a861d4a97fec17d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40649597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e9b50a06cb8bcebb665437264710388e31be79f6c9b4b6da1f03f81369ecdaa`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 03:34:02 GMT
ADD file:eca1a7737bd5e84ff883c4c284c0cd22492145d9cd7ae3b8e7b490e3d8e5aefb in / 
# Fri, 11 Dec 2020 03:34:11 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 05:25:33 GMT
ENV HAPROXY_VERSION=2.3.2
# Fri, 11 Dec 2020 05:25:36 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.2.tar.gz
# Fri, 11 Dec 2020 05:25:40 GMT
ENV HAPROXY_SHA256=99cb73bb791a2cd18898d0595e14fdc820a6cbd622c762f4ed83f2884d038fd5
# Fri, 11 Dec 2020 05:28:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 05:28:25 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 05:28:27 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 05:28:32 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:28:34 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c0f0648876332890be87a9f32ec4ad2a939e805be3152ab991a923f7dec2b35d`  
		Last Modified: Fri, 11 Dec 2020 03:41:39 GMT  
		Size: 30.5 MB (30524717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19f0165c728ecb9e371716d3a364af6237f7d0bbaef67fba0be7aeee08ba4677`  
		Last Modified: Fri, 11 Dec 2020 05:53:36 GMT  
		Size: 10.1 MB (10124500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb3355b62bacf1809975a9c89f56412ce4e0bca80b083087057b7e3d425e420e`  
		Last Modified: Fri, 11 Dec 2020 05:53:34 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3` - linux; s390x

```console
$ docker pull haproxy@sha256:95130cc7eabcb463bf983aa7983a3aea1a424f8693893ecf23af0faf2e0b9dd5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35063292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42304927f097e7b29030c4c8a900826d39241b05fd329b83314d68ddfe39d491`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:12:11 GMT
ADD file:db86ce5a1665b6d8ac734c54ac249a811c58484f569b935b14772445962428aa in / 
# Fri, 11 Dec 2020 02:12:15 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 03:16:37 GMT
ENV HAPROXY_VERSION=2.3.2
# Fri, 11 Dec 2020 03:16:37 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.2.tar.gz
# Fri, 11 Dec 2020 03:16:38 GMT
ENV HAPROXY_SHA256=99cb73bb791a2cd18898d0595e14fdc820a6cbd622c762f4ed83f2884d038fd5
# Fri, 11 Dec 2020 03:17:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 03:17:50 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 03:17:50 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 03:17:50 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:17:51 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:f4cf10ca9f31aab0854647d7878dc4db838e93b892b843dde3db24f2e909a106`  
		Last Modified: Fri, 11 Dec 2020 02:17:07 GMT  
		Size: 25.7 MB (25713957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e1407baabb38f88b38bde51950dda870904b2cbb0781a1c2927cb795c59834f`  
		Last Modified: Fri, 11 Dec 2020 03:27:48 GMT  
		Size: 9.3 MB (9348954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:014aca4270aeead92d2682142602ba0bfb1a50c5869a2e05879a84d4af45c88c`  
		Last Modified: Fri, 11 Dec 2020 03:27:47 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.3.2`

```console
$ docker pull haproxy@sha256:889b4c9d7fc1bc96de9003dbd7032e4fc43ec75194b69d4a2ac401f1f24f4e16
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

### `haproxy:2.3.2` - linux; amd64

```console
$ docker pull haproxy@sha256:4860d9794eda9fb82255fc89d6dce85ad5a9ef14b47b9ebeec6539e6179eb99c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.7 MB (36738634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecf07e33b5c4bbb59188bf77781c047d9ff8accdf21b1902212b4c04864982a8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:06:10 GMT
ADD file:3a7bff4e139bcacc5831fd70a035c130a91b5da001dd91c08b2acd635c7064e8 in / 
# Fri, 11 Dec 2020 02:06:10 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 06:28:09 GMT
ENV HAPROXY_VERSION=2.3.2
# Fri, 11 Dec 2020 06:28:09 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.2.tar.gz
# Fri, 11 Dec 2020 06:28:09 GMT
ENV HAPROXY_SHA256=99cb73bb791a2cd18898d0595e14fdc820a6cbd622c762f4ed83f2884d038fd5
# Fri, 11 Dec 2020 06:29:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 06:29:46 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 06:29:47 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 06:29:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 06:29:47 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:6ec7b7d162b24bd6df88abde89ceb6d7bbc2be927f025c9dd061af2b0c328cfe`  
		Last Modified: Fri, 11 Dec 2020 02:12:26 GMT  
		Size: 27.1 MB (27099295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:babde0d7067ce5bb18c684bf031cfae2b1347e9c1b33dcd28534e777e3be722f`  
		Last Modified: Fri, 11 Dec 2020 06:48:01 GMT  
		Size: 9.6 MB (9638959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5481c8a4effb2e57ba600574d8f3d55527251112fad63bde55889ef48e2aa889`  
		Last Modified: Fri, 11 Dec 2020 06:47:51 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.2` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:ce1efa598867b2b6bdc23e8939cf570bd497ca50cf89cbd5cf47df73f4455d5c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34094439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e4360389b6e24cf55fe8b4f15e16bb3de800395360213a6e196e51383e33272`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:49 GMT
ADD file:58ebb3ffaf26d9b7621efba5f109ae9d22832f2f22865cda36604b138cbdb7b8 in / 
# Fri, 11 Dec 2020 02:04:56 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 03:26:28 GMT
ENV HAPROXY_VERSION=2.3.2
# Fri, 11 Dec 2020 03:26:30 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.2.tar.gz
# Fri, 11 Dec 2020 03:26:32 GMT
ENV HAPROXY_SHA256=99cb73bb791a2cd18898d0595e14fdc820a6cbd622c762f4ed83f2884d038fd5
# Fri, 11 Dec 2020 03:27:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 03:27:26 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 03:27:27 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 03:27:28 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:27:29 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:8cbd1f790d64c77fcac6c9dbfe4d4c82f0365de9438f1a42b0560dc88f9e6a55`  
		Last Modified: Fri, 11 Dec 2020 02:14:44 GMT  
		Size: 24.8 MB (24843461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8201a0540f14f83cebd166f9eb8b2e6868ae479bb9d88db3782b27f4475f6115`  
		Last Modified: Fri, 11 Dec 2020 03:35:10 GMT  
		Size: 9.3 MB (9250597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f414bb6e55af4c969210ca000a4e3db02adcdc632ce2fa733d23c23f4cee46d`  
		Last Modified: Fri, 11 Dec 2020 03:35:06 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.2` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:799c4cf3d5511ec7a381d76d624bfda090da64f0f7a570ebea7f7fb2492c2b08
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31774902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34a16b900cd9c658ddc60b921684ffb64fdc25dccbc6cb2d0ba445fa99c76cb1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:23:37 GMT
ADD file:75ca842ac2d6e9f6617bb3df280af1e4c9619c9805fd5e00c1c3d6b8b4e3d802 in / 
# Fri, 11 Dec 2020 02:23:39 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 04:53:56 GMT
ENV HAPROXY_VERSION=2.3.2
# Fri, 11 Dec 2020 04:53:57 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.2.tar.gz
# Fri, 11 Dec 2020 04:53:58 GMT
ENV HAPROXY_SHA256=99cb73bb791a2cd18898d0595e14fdc820a6cbd622c762f4ed83f2884d038fd5
# Fri, 11 Dec 2020 04:54:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 04:54:42 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 04:54:44 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 04:54:44 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 04:54:46 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c06905228d4fc5a5c840a70e2e6ced56596a8bc73abc69e6a1867bbb6f7ae7e7`  
		Last Modified: Fri, 11 Dec 2020 02:33:07 GMT  
		Size: 22.7 MB (22707662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b18920727745d1198efa252a298135ebb3e0cee3f2be2ec4aed8608d42e8c7c`  
		Last Modified: Fri, 11 Dec 2020 05:04:59 GMT  
		Size: 9.1 MB (9066859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:503a299b85cfeda421f53031cf13ae1d8f2328cf24410ca507aa257db3a584e8`  
		Last Modified: Fri, 11 Dec 2020 05:04:57 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.2` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:4797dffb4de987894cd0d7e3fddf97dd39e17fd34f409630724501d5d54f3375
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35320778 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1073c1f4bbe1be3699a00df24887f2b7b22c658b160f8e69caeaed50a856a06d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:45:53 GMT
ADD file:a5a2f039c00bc638b88cefdff4c3cd1865b4d415bf80c4fe6b496d975af7cc1f in / 
# Fri, 11 Dec 2020 02:45:57 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 05:31:27 GMT
ENV HAPROXY_VERSION=2.3.2
# Fri, 11 Dec 2020 05:31:28 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.2.tar.gz
# Fri, 11 Dec 2020 05:31:29 GMT
ENV HAPROXY_SHA256=99cb73bb791a2cd18898d0595e14fdc820a6cbd622c762f4ed83f2884d038fd5
# Fri, 11 Dec 2020 05:32:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 05:32:23 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 05:32:24 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 05:32:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:32:26 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c9648d7fcbb6d597cf33916d8fcd207fde8ec05d764b4480d4f3e884e142a902`  
		Last Modified: Fri, 11 Dec 2020 02:53:14 GMT  
		Size: 25.9 MB (25856191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a03032109a3408c7f6452a59eba9ff651f3be467ace9c735b2c151cb7b9cb31`  
		Last Modified: Fri, 11 Dec 2020 05:43:52 GMT  
		Size: 9.5 MB (9464207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780c192d356a56d112c0bff8106c349e11329c5e23d76dd868a996bf09dd50f9`  
		Last Modified: Fri, 11 Dec 2020 05:43:50 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.2` - linux; 386

```console
$ docker pull haproxy@sha256:3b84c007b2fb56ce5380065119d78475dba59a3bfeb417be3edb6c2bdda80d60
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37287145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1fd13752edbb99935735f761ee08efa7ec780f27a6f8d7026ea8b5086d9c332`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:07 GMT
ADD file:a0879774b23f70c4db7f7b04736cca142beb0b22e93f5952364ca990a1675552 in / 
# Fri, 11 Dec 2020 02:03:08 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 05:06:25 GMT
ENV HAPROXY_VERSION=2.3.2
# Fri, 11 Dec 2020 05:06:25 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.2.tar.gz
# Fri, 11 Dec 2020 05:06:26 GMT
ENV HAPROXY_SHA256=99cb73bb791a2cd18898d0595e14fdc820a6cbd622c762f4ed83f2884d038fd5
# Fri, 11 Dec 2020 05:08:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 05:08:06 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 05:08:07 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 05:08:07 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:08:08 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:cfec07a090788e68b692f30d34e11dc7af0f1c8112fbc846e8e40e24faf882d7`  
		Last Modified: Fri, 11 Dec 2020 02:09:41 GMT  
		Size: 27.8 MB (27757584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d24160835d3ce6cd6a891511665f008d92aa7b2785ad76b373c67d9e555158af`  
		Last Modified: Fri, 11 Dec 2020 05:25:25 GMT  
		Size: 9.5 MB (9529181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c720f841b372f39c960735d688b1a090f8287dd22c78278da10850ed3675fd9`  
		Last Modified: Fri, 11 Dec 2020 05:25:22 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.2` - linux; mips64le

```console
$ docker pull haproxy@sha256:47fe68bf4ccd8b76178f984ee18686fc7618231049db8d91d3b31ab017a7d93c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.0 MB (34986193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b7bee85f1b7b1ba34fa6c15d4003eb40217a24da9445980254f2f8cf07239f2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:30 GMT
ADD file:edb758d587972f30ef28b162dcabf79f61b685afa3c6066cb611c61abea124f3 in / 
# Fri, 11 Dec 2020 02:03:30 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 03:18:39 GMT
ENV HAPROXY_VERSION=2.3.2
# Fri, 11 Dec 2020 03:18:39 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.2.tar.gz
# Fri, 11 Dec 2020 03:18:39 GMT
ENV HAPROXY_SHA256=99cb73bb791a2cd18898d0595e14fdc820a6cbd622c762f4ed83f2884d038fd5
# Fri, 11 Dec 2020 03:21:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 03:21:02 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 03:21:02 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 03:21:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:21:03 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:bed35f8e8e003f268bd91c8bc28d93f0b1463296add14ab3ec84c3d3d30e9025`  
		Last Modified: Fri, 11 Dec 2020 02:10:15 GMT  
		Size: 25.8 MB (25769881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56160242f2040d557d6d1772d02a223df3069a8367382e6a1e259b1196effe92`  
		Last Modified: Fri, 11 Dec 2020 03:33:03 GMT  
		Size: 9.2 MB (9215932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ccc4a11e34e39a69c2886e2edd20c1c5a156411ca4db70a665bfb097227c14`  
		Last Modified: Fri, 11 Dec 2020 03:32:56 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.2` - linux; ppc64le

```console
$ docker pull haproxy@sha256:37819fd7b83a49c2986493f3be3d2183c638125f75688d202a861d4a97fec17d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40649597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e9b50a06cb8bcebb665437264710388e31be79f6c9b4b6da1f03f81369ecdaa`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 03:34:02 GMT
ADD file:eca1a7737bd5e84ff883c4c284c0cd22492145d9cd7ae3b8e7b490e3d8e5aefb in / 
# Fri, 11 Dec 2020 03:34:11 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 05:25:33 GMT
ENV HAPROXY_VERSION=2.3.2
# Fri, 11 Dec 2020 05:25:36 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.2.tar.gz
# Fri, 11 Dec 2020 05:25:40 GMT
ENV HAPROXY_SHA256=99cb73bb791a2cd18898d0595e14fdc820a6cbd622c762f4ed83f2884d038fd5
# Fri, 11 Dec 2020 05:28:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 05:28:25 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 05:28:27 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 05:28:32 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:28:34 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c0f0648876332890be87a9f32ec4ad2a939e805be3152ab991a923f7dec2b35d`  
		Last Modified: Fri, 11 Dec 2020 03:41:39 GMT  
		Size: 30.5 MB (30524717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19f0165c728ecb9e371716d3a364af6237f7d0bbaef67fba0be7aeee08ba4677`  
		Last Modified: Fri, 11 Dec 2020 05:53:36 GMT  
		Size: 10.1 MB (10124500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb3355b62bacf1809975a9c89f56412ce4e0bca80b083087057b7e3d425e420e`  
		Last Modified: Fri, 11 Dec 2020 05:53:34 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.2` - linux; s390x

```console
$ docker pull haproxy@sha256:95130cc7eabcb463bf983aa7983a3aea1a424f8693893ecf23af0faf2e0b9dd5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35063292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42304927f097e7b29030c4c8a900826d39241b05fd329b83314d68ddfe39d491`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:12:11 GMT
ADD file:db86ce5a1665b6d8ac734c54ac249a811c58484f569b935b14772445962428aa in / 
# Fri, 11 Dec 2020 02:12:15 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 03:16:37 GMT
ENV HAPROXY_VERSION=2.3.2
# Fri, 11 Dec 2020 03:16:37 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.2.tar.gz
# Fri, 11 Dec 2020 03:16:38 GMT
ENV HAPROXY_SHA256=99cb73bb791a2cd18898d0595e14fdc820a6cbd622c762f4ed83f2884d038fd5
# Fri, 11 Dec 2020 03:17:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 03:17:50 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 03:17:50 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 03:17:50 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:17:51 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:f4cf10ca9f31aab0854647d7878dc4db838e93b892b843dde3db24f2e909a106`  
		Last Modified: Fri, 11 Dec 2020 02:17:07 GMT  
		Size: 25.7 MB (25713957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e1407baabb38f88b38bde51950dda870904b2cbb0781a1c2927cb795c59834f`  
		Last Modified: Fri, 11 Dec 2020 03:27:48 GMT  
		Size: 9.3 MB (9348954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:014aca4270aeead92d2682142602ba0bfb1a50c5869a2e05879a84d4af45c88c`  
		Last Modified: Fri, 11 Dec 2020 03:27:47 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.3.2-alpine`

```console
$ docker pull haproxy@sha256:a4b532622824aa6421c107dcadaee692e48ebedd9b5bbb8c6ac612a89c66798c
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

### `haproxy:2.3.2-alpine` - linux; amd64

```console
$ docker pull haproxy@sha256:497f197a318f09642c09cacf4c3625978e83cca29bfa3dde2dacd9be893163ca
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.2 MB (10203759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a1001ef82706917ec78b526c93dfcf5e6263b0dc4eecc8631abaf9b685f8659`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:28:35 GMT
ENV HAPROXY_VERSION=2.3.2
# Thu, 17 Dec 2020 13:28:35 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.2.tar.gz
# Thu, 17 Dec 2020 13:28:36 GMT
ENV HAPROXY_SHA256=99cb73bb791a2cd18898d0595e14fdc820a6cbd622c762f4ed83f2884d038fd5
# Thu, 17 Dec 2020 13:30:35 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 13:30:36 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 13:30:36 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 13:30:37 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 13:30:37 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca683bcd5723099a7c129a2a93f01f05bceeedc9db28a5f533741450b4e65cb`  
		Last Modified: Thu, 17 Dec 2020 13:38:02 GMT  
		Size: 7.4 MB (7404313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9b048041f14ac7dc9e1866c7185833d10ed665e5cd25b2f29dba5905a1ab2f`  
		Last Modified: Thu, 17 Dec 2020 13:38:00 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.2-alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:65ef8a4ed34778a5b768c4caa6dacd7524c412b75b4a3fb621cfb33808142d7b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9859894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:644556767ede8d9f4e94615aa163bf7ad16beb93c44bfecc7e7ecbc65cbfa18d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:36:29 GMT
ENV HAPROXY_VERSION=2.3.2
# Thu, 17 Dec 2020 01:36:29 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.2.tar.gz
# Thu, 17 Dec 2020 01:36:30 GMT
ENV HAPROXY_SHA256=99cb73bb791a2cd18898d0595e14fdc820a6cbd622c762f4ed83f2884d038fd5
# Thu, 17 Dec 2020 01:37:03 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:37:04 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:37:04 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 01:37:06 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:37:06 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6776e0a3544c93d9c3ce724a749c0386c4e5f879573dfa081a51e93e145cbf13`  
		Last Modified: Thu, 17 Dec 2020 01:41:17 GMT  
		Size: 7.3 MB (7255351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbf020734cc589411856a09679f990f60b5c80673fbe47f54599b3c8b06c44ac`  
		Last Modified: Thu, 17 Dec 2020 01:41:14 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.2-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:f6dc03525659ac0fb9fa9389b4ea80bc23226b720c3062003b725cf2860a6d66
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9617506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e94d22c496a979d2a87129121fd7cb23d1a5afc881ee21ffcd4ad9ce2030b24`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:38:43 GMT
ENV HAPROXY_VERSION=2.3.2
# Thu, 17 Dec 2020 01:38:44 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.2.tar.gz
# Thu, 17 Dec 2020 01:38:45 GMT
ENV HAPROXY_SHA256=99cb73bb791a2cd18898d0595e14fdc820a6cbd622c762f4ed83f2884d038fd5
# Thu, 17 Dec 2020 01:39:11 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:39:12 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:39:13 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 01:39:14 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:39:15 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef8ff9670f7a5023ba54df386ffccedb014f1e72bb95c20ff50a8bc703b00846`  
		Last Modified: Thu, 17 Dec 2020 01:43:19 GMT  
		Size: 7.2 MB (7209570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4541c3937c06cd84646da87a798a822082f7d4dbb187989a9b60f002585f4bb9`  
		Last Modified: Thu, 17 Dec 2020 01:43:17 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.2-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:4e20f7e25d2b0f281125d57b0b2d86df68d8ab063382c4bb9ebad18bf1fb7388
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.1 MB (10077526 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:405dfdce2795fb2b2cef8a6d78fbd610877e9d667ebdb03723e6625586a3e83e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:24:10 GMT
ENV HAPROXY_VERSION=2.3.2
# Thu, 17 Dec 2020 01:24:11 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.2.tar.gz
# Thu, 17 Dec 2020 01:24:13 GMT
ENV HAPROXY_SHA256=99cb73bb791a2cd18898d0595e14fdc820a6cbd622c762f4ed83f2884d038fd5
# Thu, 17 Dec 2020 01:24:38 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:24:39 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:24:40 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 01:24:41 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:24:42 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bef0c4aa00924d2cd300bd631a261a142299e072a13e8621d7d11b3cd208494`  
		Last Modified: Thu, 17 Dec 2020 01:30:18 GMT  
		Size: 7.4 MB (7368098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb9470f170e025b1fd1dd58d461a21682de90e83c63d0178dc7218e4f8dbf43`  
		Last Modified: Thu, 17 Dec 2020 01:30:15 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.2-alpine` - linux; 386

```console
$ docker pull haproxy@sha256:092422718ce95ec83ae9cea7ac7b86bb213a849e20e88ac5f3277ca890cac479
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.1 MB (10138880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd732a59bde146f31bc8514ec3cce5774631f523534edca54a2aedaf03218308`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 17 Dec 2020 00:38:32 GMT
ADD file:de33fda50a142403e842620d20bc4404e66fc4ace16edc6946c4539e8a797458 in / 
# Thu, 17 Dec 2020 00:38:32 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:26:24 GMT
ENV HAPROXY_VERSION=2.3.2
# Thu, 17 Dec 2020 02:26:24 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.2.tar.gz
# Thu, 17 Dec 2020 02:26:25 GMT
ENV HAPROXY_SHA256=99cb73bb791a2cd18898d0595e14fdc820a6cbd622c762f4ed83f2884d038fd5
# Thu, 17 Dec 2020 02:27:54 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 02:27:54 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 02:27:55 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 02:27:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 02:27:55 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:455793c72b878001f0905634ed52a2524ba51796e7377bf00683a85123f7dce9`  
		Last Modified: Thu, 17 Dec 2020 00:39:18 GMT  
		Size: 2.8 MB (2794130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3e70eb052ff09369f2e1424ad47ba6b4a21af58719dc96aaa4aaafa72e7e070`  
		Last Modified: Thu, 17 Dec 2020 02:34:47 GMT  
		Size: 7.3 MB (7344370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244af8e13011e1cbccf7467e84202b44ba3ac0e2f880fb76d6b68816b7f5876d`  
		Last Modified: Thu, 17 Dec 2020 02:34:35 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.2-alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:c61f9595bd2d242786faef3608ac945b53ca84c812e2d24badadf4c29e8b93bf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.6 MB (10560399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6119c04ca1f959d866145f912434d0f905b783cbbe369b992d80546bcde463f0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 17 Dec 2020 00:20:42 GMT
ADD file:0a38c9b4955f8faa79627c166fca80ef342e443a16ce2925a30eeae317bbd786 in / 
# Thu, 17 Dec 2020 00:20:48 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:40:24 GMT
ENV HAPROXY_VERSION=2.3.2
# Thu, 17 Dec 2020 02:40:30 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.2.tar.gz
# Thu, 17 Dec 2020 02:40:38 GMT
ENV HAPROXY_SHA256=99cb73bb791a2cd18898d0595e14fdc820a6cbd622c762f4ed83f2884d038fd5
# Thu, 17 Dec 2020 02:41:25 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 02:41:31 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 02:41:34 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 02:41:40 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 02:41:45 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:a9d343b7bcc225fe7ac17d96a81329510ab7f31a50472311cafe7168d3107317`  
		Last Modified: Thu, 17 Dec 2020 00:21:33 GMT  
		Size: 2.8 MB (2805226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a36c2bce9570afb3b4542d019f7bf4931dc2abb64cd8133014a2f4960b5ccb`  
		Last Modified: Thu, 17 Dec 2020 02:49:54 GMT  
		Size: 7.8 MB (7754792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fce22188bda157976ae629c97e6d917919a5d010dbe11711e9c573c3917dc287`  
		Last Modified: Thu, 17 Dec 2020 02:49:51 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.2-alpine` - linux; s390x

```console
$ docker pull haproxy@sha256:e32e50f1720d8d74347be1d08c53060b121f5d33cf8dfe1c78e2b6673b5e4e01
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (10004227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85bf20b1ba112bcb2e39f297e7cda027a40971e4f4e077b9325806262e9f6b93`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:41:37 GMT
ADD file:3ad3856d165e8760af85574a8ffa75ca44b7e1b97b64d1d6d4608445efa4b860 in / 
# Wed, 16 Dec 2020 23:41:37 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:25:15 GMT
ENV HAPROXY_VERSION=2.3.2
# Thu, 17 Dec 2020 01:25:16 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.2.tar.gz
# Thu, 17 Dec 2020 01:25:16 GMT
ENV HAPROXY_SHA256=99cb73bb791a2cd18898d0595e14fdc820a6cbd622c762f4ed83f2884d038fd5
# Thu, 17 Dec 2020 01:26:02 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:26:03 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:26:03 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 01:26:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:26:04 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:ee52640a49e15b8b7c8edb66c2d048b26abdee8d828d6e5ef4e10a28cb15a84f`  
		Last Modified: Wed, 16 Dec 2020 23:42:15 GMT  
		Size: 2.6 MB (2567018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be334f2af5c8c1dc2046c3bb58d2969ce6e9e13d6c37a60c5d5facc7519b387`  
		Last Modified: Thu, 17 Dec 2020 01:31:21 GMT  
		Size: 7.4 MB (7436829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53baf298aad5720b3f2d0ebd9a6ea91ba7aee6a1038fc638434af786da52d4ec`  
		Last Modified: Thu, 17 Dec 2020 01:31:20 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.3-alpine`

```console
$ docker pull haproxy@sha256:a4b532622824aa6421c107dcadaee692e48ebedd9b5bbb8c6ac612a89c66798c
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
$ docker pull haproxy@sha256:497f197a318f09642c09cacf4c3625978e83cca29bfa3dde2dacd9be893163ca
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.2 MB (10203759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a1001ef82706917ec78b526c93dfcf5e6263b0dc4eecc8631abaf9b685f8659`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:28:35 GMT
ENV HAPROXY_VERSION=2.3.2
# Thu, 17 Dec 2020 13:28:35 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.2.tar.gz
# Thu, 17 Dec 2020 13:28:36 GMT
ENV HAPROXY_SHA256=99cb73bb791a2cd18898d0595e14fdc820a6cbd622c762f4ed83f2884d038fd5
# Thu, 17 Dec 2020 13:30:35 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 13:30:36 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 13:30:36 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 13:30:37 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 13:30:37 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca683bcd5723099a7c129a2a93f01f05bceeedc9db28a5f533741450b4e65cb`  
		Last Modified: Thu, 17 Dec 2020 13:38:02 GMT  
		Size: 7.4 MB (7404313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9b048041f14ac7dc9e1866c7185833d10ed665e5cd25b2f29dba5905a1ab2f`  
		Last Modified: Thu, 17 Dec 2020 13:38:00 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3-alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:65ef8a4ed34778a5b768c4caa6dacd7524c412b75b4a3fb621cfb33808142d7b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9859894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:644556767ede8d9f4e94615aa163bf7ad16beb93c44bfecc7e7ecbc65cbfa18d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:36:29 GMT
ENV HAPROXY_VERSION=2.3.2
# Thu, 17 Dec 2020 01:36:29 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.2.tar.gz
# Thu, 17 Dec 2020 01:36:30 GMT
ENV HAPROXY_SHA256=99cb73bb791a2cd18898d0595e14fdc820a6cbd622c762f4ed83f2884d038fd5
# Thu, 17 Dec 2020 01:37:03 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:37:04 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:37:04 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 01:37:06 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:37:06 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6776e0a3544c93d9c3ce724a749c0386c4e5f879573dfa081a51e93e145cbf13`  
		Last Modified: Thu, 17 Dec 2020 01:41:17 GMT  
		Size: 7.3 MB (7255351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbf020734cc589411856a09679f990f60b5c80673fbe47f54599b3c8b06c44ac`  
		Last Modified: Thu, 17 Dec 2020 01:41:14 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:f6dc03525659ac0fb9fa9389b4ea80bc23226b720c3062003b725cf2860a6d66
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9617506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e94d22c496a979d2a87129121fd7cb23d1a5afc881ee21ffcd4ad9ce2030b24`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:38:43 GMT
ENV HAPROXY_VERSION=2.3.2
# Thu, 17 Dec 2020 01:38:44 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.2.tar.gz
# Thu, 17 Dec 2020 01:38:45 GMT
ENV HAPROXY_SHA256=99cb73bb791a2cd18898d0595e14fdc820a6cbd622c762f4ed83f2884d038fd5
# Thu, 17 Dec 2020 01:39:11 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:39:12 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:39:13 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 01:39:14 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:39:15 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef8ff9670f7a5023ba54df386ffccedb014f1e72bb95c20ff50a8bc703b00846`  
		Last Modified: Thu, 17 Dec 2020 01:43:19 GMT  
		Size: 7.2 MB (7209570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4541c3937c06cd84646da87a798a822082f7d4dbb187989a9b60f002585f4bb9`  
		Last Modified: Thu, 17 Dec 2020 01:43:17 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:4e20f7e25d2b0f281125d57b0b2d86df68d8ab063382c4bb9ebad18bf1fb7388
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.1 MB (10077526 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:405dfdce2795fb2b2cef8a6d78fbd610877e9d667ebdb03723e6625586a3e83e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:24:10 GMT
ENV HAPROXY_VERSION=2.3.2
# Thu, 17 Dec 2020 01:24:11 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.2.tar.gz
# Thu, 17 Dec 2020 01:24:13 GMT
ENV HAPROXY_SHA256=99cb73bb791a2cd18898d0595e14fdc820a6cbd622c762f4ed83f2884d038fd5
# Thu, 17 Dec 2020 01:24:38 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:24:39 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:24:40 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 01:24:41 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:24:42 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bef0c4aa00924d2cd300bd631a261a142299e072a13e8621d7d11b3cd208494`  
		Last Modified: Thu, 17 Dec 2020 01:30:18 GMT  
		Size: 7.4 MB (7368098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb9470f170e025b1fd1dd58d461a21682de90e83c63d0178dc7218e4f8dbf43`  
		Last Modified: Thu, 17 Dec 2020 01:30:15 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3-alpine` - linux; 386

```console
$ docker pull haproxy@sha256:092422718ce95ec83ae9cea7ac7b86bb213a849e20e88ac5f3277ca890cac479
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.1 MB (10138880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd732a59bde146f31bc8514ec3cce5774631f523534edca54a2aedaf03218308`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 17 Dec 2020 00:38:32 GMT
ADD file:de33fda50a142403e842620d20bc4404e66fc4ace16edc6946c4539e8a797458 in / 
# Thu, 17 Dec 2020 00:38:32 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:26:24 GMT
ENV HAPROXY_VERSION=2.3.2
# Thu, 17 Dec 2020 02:26:24 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.2.tar.gz
# Thu, 17 Dec 2020 02:26:25 GMT
ENV HAPROXY_SHA256=99cb73bb791a2cd18898d0595e14fdc820a6cbd622c762f4ed83f2884d038fd5
# Thu, 17 Dec 2020 02:27:54 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 02:27:54 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 02:27:55 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 02:27:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 02:27:55 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:455793c72b878001f0905634ed52a2524ba51796e7377bf00683a85123f7dce9`  
		Last Modified: Thu, 17 Dec 2020 00:39:18 GMT  
		Size: 2.8 MB (2794130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3e70eb052ff09369f2e1424ad47ba6b4a21af58719dc96aaa4aaafa72e7e070`  
		Last Modified: Thu, 17 Dec 2020 02:34:47 GMT  
		Size: 7.3 MB (7344370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244af8e13011e1cbccf7467e84202b44ba3ac0e2f880fb76d6b68816b7f5876d`  
		Last Modified: Thu, 17 Dec 2020 02:34:35 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3-alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:c61f9595bd2d242786faef3608ac945b53ca84c812e2d24badadf4c29e8b93bf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.6 MB (10560399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6119c04ca1f959d866145f912434d0f905b783cbbe369b992d80546bcde463f0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 17 Dec 2020 00:20:42 GMT
ADD file:0a38c9b4955f8faa79627c166fca80ef342e443a16ce2925a30eeae317bbd786 in / 
# Thu, 17 Dec 2020 00:20:48 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:40:24 GMT
ENV HAPROXY_VERSION=2.3.2
# Thu, 17 Dec 2020 02:40:30 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.2.tar.gz
# Thu, 17 Dec 2020 02:40:38 GMT
ENV HAPROXY_SHA256=99cb73bb791a2cd18898d0595e14fdc820a6cbd622c762f4ed83f2884d038fd5
# Thu, 17 Dec 2020 02:41:25 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 02:41:31 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 02:41:34 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 02:41:40 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 02:41:45 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:a9d343b7bcc225fe7ac17d96a81329510ab7f31a50472311cafe7168d3107317`  
		Last Modified: Thu, 17 Dec 2020 00:21:33 GMT  
		Size: 2.8 MB (2805226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a36c2bce9570afb3b4542d019f7bf4931dc2abb64cd8133014a2f4960b5ccb`  
		Last Modified: Thu, 17 Dec 2020 02:49:54 GMT  
		Size: 7.8 MB (7754792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fce22188bda157976ae629c97e6d917919a5d010dbe11711e9c573c3917dc287`  
		Last Modified: Thu, 17 Dec 2020 02:49:51 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3-alpine` - linux; s390x

```console
$ docker pull haproxy@sha256:e32e50f1720d8d74347be1d08c53060b121f5d33cf8dfe1c78e2b6673b5e4e01
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (10004227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85bf20b1ba112bcb2e39f297e7cda027a40971e4f4e077b9325806262e9f6b93`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:41:37 GMT
ADD file:3ad3856d165e8760af85574a8ffa75ca44b7e1b97b64d1d6d4608445efa4b860 in / 
# Wed, 16 Dec 2020 23:41:37 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:25:15 GMT
ENV HAPROXY_VERSION=2.3.2
# Thu, 17 Dec 2020 01:25:16 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.2.tar.gz
# Thu, 17 Dec 2020 01:25:16 GMT
ENV HAPROXY_SHA256=99cb73bb791a2cd18898d0595e14fdc820a6cbd622c762f4ed83f2884d038fd5
# Thu, 17 Dec 2020 01:26:02 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:26:03 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:26:03 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 01:26:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:26:04 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:ee52640a49e15b8b7c8edb66c2d048b26abdee8d828d6e5ef4e10a28cb15a84f`  
		Last Modified: Wed, 16 Dec 2020 23:42:15 GMT  
		Size: 2.6 MB (2567018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be334f2af5c8c1dc2046c3bb58d2969ce6e9e13d6c37a60c5d5facc7519b387`  
		Last Modified: Thu, 17 Dec 2020 01:31:21 GMT  
		Size: 7.4 MB (7436829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53baf298aad5720b3f2d0ebd9a6ea91ba7aee6a1038fc638434af786da52d4ec`  
		Last Modified: Thu, 17 Dec 2020 01:31:20 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.4-dev`

```console
$ docker pull haproxy@sha256:6c659c66aba4bbe3b4b8d37e77e0d907de21634207568c24a064f8dc2dd2d776
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
$ docker pull haproxy@sha256:39a5f7c6d8423f3cd31de4f7b557dfe0bc71f4cf7dbbd3d5fab6c48fb3ff67f4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.9 MB (36872153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c0054b724338af8652511b1d4c833784002a3cd4d7733dd668a0fa47bcb6c25`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:06:10 GMT
ADD file:3a7bff4e139bcacc5831fd70a035c130a91b5da001dd91c08b2acd635c7064e8 in / 
# Fri, 11 Dec 2020 02:06:10 GMT
CMD ["bash"]
# Sat, 12 Dec 2020 18:18:41 GMT
ENV HAPROXY_VERSION=2.4-dev3
# Sat, 12 Dec 2020 18:18:41 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev3.tar.gz
# Sat, 12 Dec 2020 18:18:41 GMT
ENV HAPROXY_SHA256=c5de469830a43ac34d84af3de480b070d357af6289d47df00396db05dd1f7918
# Sat, 12 Dec 2020 18:19:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 12 Dec 2020 18:19:38 GMT
STOPSIGNAL SIGUSR1
# Sat, 12 Dec 2020 18:19:38 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Sat, 12 Dec 2020 18:19:39 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 12 Dec 2020 18:19:39 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:6ec7b7d162b24bd6df88abde89ceb6d7bbc2be927f025c9dd061af2b0c328cfe`  
		Last Modified: Fri, 11 Dec 2020 02:12:26 GMT  
		Size: 27.1 MB (27099295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2863a2e6cd20b95599bff9889bfb39c9b9890d4a9544219585d4320c7b709471`  
		Last Modified: Sat, 12 Dec 2020 18:22:14 GMT  
		Size: 9.8 MB (9772478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afdda0fb03eb71fd4adaf16dc76b69970433ad6228d718628705da79232b0139`  
		Last Modified: Sat, 12 Dec 2020 18:22:13 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:93074b84aa2e3fccc4543f09a28be2243ff91081dcb2671fbf28677f8bd6c458
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.2 MB (34219078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7eb5d8cd10e74195f2a1d6fc8f092709930616fbad75cbdc3e40e77ce7f303f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:49 GMT
ADD file:58ebb3ffaf26d9b7621efba5f109ae9d22832f2f22865cda36604b138cbdb7b8 in / 
# Fri, 11 Dec 2020 02:04:56 GMT
CMD ["bash"]
# Sat, 12 Dec 2020 01:48:41 GMT
ENV HAPROXY_VERSION=2.4-dev3
# Sat, 12 Dec 2020 01:48:42 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev3.tar.gz
# Sat, 12 Dec 2020 01:48:43 GMT
ENV HAPROXY_SHA256=c5de469830a43ac34d84af3de480b070d357af6289d47df00396db05dd1f7918
# Sat, 12 Dec 2020 01:49:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 12 Dec 2020 01:49:35 GMT
STOPSIGNAL SIGUSR1
# Sat, 12 Dec 2020 01:49:36 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Sat, 12 Dec 2020 01:49:37 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 12 Dec 2020 01:49:39 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:8cbd1f790d64c77fcac6c9dbfe4d4c82f0365de9438f1a42b0560dc88f9e6a55`  
		Last Modified: Fri, 11 Dec 2020 02:14:44 GMT  
		Size: 24.8 MB (24843461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:742da06ed7bdebb6c50238dbce597159c81102461858ff32359a6c8d2d9a5c9f`  
		Last Modified: Sat, 12 Dec 2020 01:50:39 GMT  
		Size: 9.4 MB (9375237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f152f0c689bf5530c8f5453c12e10ff513c060d3bafd72c4e9f558ac4b56d0`  
		Last Modified: Sat, 12 Dec 2020 01:50:36 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:5c59d63c6767eb96e5d77c66e6f63516301ed8c94b33a5c4da0e7475fa764d7c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.9 MB (31903748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd66c95c0acf12ec519ce2bad2d3496a5c9f1fbb7be3ed638501158de86294c3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:23:37 GMT
ADD file:75ca842ac2d6e9f6617bb3df280af1e4c9619c9805fd5e00c1c3d6b8b4e3d802 in / 
# Fri, 11 Dec 2020 02:23:39 GMT
CMD ["bash"]
# Sat, 12 Dec 2020 11:19:29 GMT
ENV HAPROXY_VERSION=2.4-dev3
# Sat, 12 Dec 2020 11:19:30 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev3.tar.gz
# Sat, 12 Dec 2020 11:19:31 GMT
ENV HAPROXY_SHA256=c5de469830a43ac34d84af3de480b070d357af6289d47df00396db05dd1f7918
# Sat, 12 Dec 2020 11:20:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 12 Dec 2020 11:20:15 GMT
STOPSIGNAL SIGUSR1
# Sat, 12 Dec 2020 11:20:16 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Sat, 12 Dec 2020 11:20:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 12 Dec 2020 11:20:17 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c06905228d4fc5a5c840a70e2e6ced56596a8bc73abc69e6a1867bbb6f7ae7e7`  
		Last Modified: Fri, 11 Dec 2020 02:33:07 GMT  
		Size: 22.7 MB (22707662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea077673c59617032180d45e180a3e1d1f84cecaa2a49c40f639a8a6797bef5`  
		Last Modified: Sat, 12 Dec 2020 11:22:31 GMT  
		Size: 9.2 MB (9195705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1781de94fbbf59d888ea230caf4b49c52c84104f71f9d9542d28f5af97f60b69`  
		Last Modified: Sat, 12 Dec 2020 11:22:28 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:14d63ce9d087c635e0b2d30b1ae38d6e92c38042c4d8b1066478f751d0b3f38c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.5 MB (35458487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe25e7a9fe83585a75d6dd6abaef891e24a927596a890ff95dc9c573c9d0f725`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:45:53 GMT
ADD file:a5a2f039c00bc638b88cefdff4c3cd1865b4d415bf80c4fe6b496d975af7cc1f in / 
# Fri, 11 Dec 2020 02:45:57 GMT
CMD ["bash"]
# Sat, 12 Dec 2020 14:25:35 GMT
ENV HAPROXY_VERSION=2.4-dev3
# Sat, 12 Dec 2020 14:25:36 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev3.tar.gz
# Sat, 12 Dec 2020 14:25:37 GMT
ENV HAPROXY_SHA256=c5de469830a43ac34d84af3de480b070d357af6289d47df00396db05dd1f7918
# Sat, 12 Dec 2020 14:26:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 12 Dec 2020 14:26:28 GMT
STOPSIGNAL SIGUSR1
# Sat, 12 Dec 2020 14:26:29 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Sat, 12 Dec 2020 14:26:29 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 12 Dec 2020 14:26:30 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c9648d7fcbb6d597cf33916d8fcd207fde8ec05d764b4480d4f3e884e142a902`  
		Last Modified: Fri, 11 Dec 2020 02:53:14 GMT  
		Size: 25.9 MB (25856191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c744de7f903802790a8275a36cb04e419d5ef1be0523fc8ed2e010445999858`  
		Last Modified: Sat, 12 Dec 2020 14:28:48 GMT  
		Size: 9.6 MB (9601915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:489d4522af9d44f78172b9b865eedc72112ee9f9e79265e78ed35ea39319f61b`  
		Last Modified: Sat, 12 Dec 2020 14:28:46 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev` - linux; 386

```console
$ docker pull haproxy@sha256:21c4d574263cf1c2b5fe4c7adbf4c1aee4e2fa9ed64cc46ae7f7599746eeb7f1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37418077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6d4f0a54334cd9d18301d9e4bd55b8bdee135d51347aea6747d36e8155ef5a8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:07 GMT
ADD file:a0879774b23f70c4db7f7b04736cca142beb0b22e93f5952364ca990a1675552 in / 
# Fri, 11 Dec 2020 02:03:08 GMT
CMD ["bash"]
# Sat, 12 Dec 2020 16:23:58 GMT
ENV HAPROXY_VERSION=2.4-dev3
# Sat, 12 Dec 2020 16:23:59 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev3.tar.gz
# Sat, 12 Dec 2020 16:23:59 GMT
ENV HAPROXY_SHA256=c5de469830a43ac34d84af3de480b070d357af6289d47df00396db05dd1f7918
# Sat, 12 Dec 2020 16:25:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 12 Dec 2020 16:25:50 GMT
STOPSIGNAL SIGUSR1
# Sat, 12 Dec 2020 16:25:51 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Sat, 12 Dec 2020 16:25:51 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 12 Dec 2020 16:25:51 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:cfec07a090788e68b692f30d34e11dc7af0f1c8112fbc846e8e40e24faf882d7`  
		Last Modified: Fri, 11 Dec 2020 02:09:41 GMT  
		Size: 27.8 MB (27757584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c309a975b1c08ab7de265e3112ae48ed6fb035578b2dcc81b93c472934aba2`  
		Last Modified: Sat, 12 Dec 2020 16:29:29 GMT  
		Size: 9.7 MB (9660112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7d28b5eacccb5e4cb91557cac93d5b30464f28210a70956f352a862d417ea8`  
		Last Modified: Sat, 12 Dec 2020 16:29:26 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev` - linux; mips64le

```console
$ docker pull haproxy@sha256:3b6a5219490294703eec1f892d1a1985ef869699c2455e0b6245862b623ad38a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35119464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2989fc8df8205f12a97711aae9185b6fa39a81c140bc368f3ac236e31f99a89`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:30 GMT
ADD file:edb758d587972f30ef28b162dcabf79f61b685afa3c6066cb611c61abea124f3 in / 
# Fri, 11 Dec 2020 02:03:30 GMT
CMD ["bash"]
# Sat, 12 Dec 2020 01:07:22 GMT
ENV HAPROXY_VERSION=2.4-dev3
# Sat, 12 Dec 2020 01:07:23 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev3.tar.gz
# Sat, 12 Dec 2020 01:07:23 GMT
ENV HAPROXY_SHA256=c5de469830a43ac34d84af3de480b070d357af6289d47df00396db05dd1f7918
# Sat, 12 Dec 2020 01:09:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 12 Dec 2020 01:09:51 GMT
STOPSIGNAL SIGUSR1
# Sat, 12 Dec 2020 01:09:51 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Sat, 12 Dec 2020 01:09:51 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 12 Dec 2020 01:09:52 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:bed35f8e8e003f268bd91c8bc28d93f0b1463296add14ab3ec84c3d3d30e9025`  
		Last Modified: Fri, 11 Dec 2020 02:10:15 GMT  
		Size: 25.8 MB (25769881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09917d94a5949242ade4d8b9626387b51b7a69528cdca4da968c00174027d24e`  
		Last Modified: Sat, 12 Dec 2020 01:10:42 GMT  
		Size: 9.3 MB (9349203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c01c4aad2f452ac52baab7ec7535b3a9b96c18a88cd67efc16f31db9a266ff2`  
		Last Modified: Sat, 12 Dec 2020 01:10:35 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev` - linux; ppc64le

```console
$ docker pull haproxy@sha256:af68d29ea5ef14ed560870bb9a323a2825487e309abb2fdab529daa02a5170f0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.8 MB (40786809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:863dbeaf4a467771bf759e62830afb3efc3cd594d28ae5a59ba5edc7d646b211`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 03:34:02 GMT
ADD file:eca1a7737bd5e84ff883c4c284c0cd22492145d9cd7ae3b8e7b490e3d8e5aefb in / 
# Fri, 11 Dec 2020 03:34:11 GMT
CMD ["bash"]
# Sat, 12 Dec 2020 16:27:59 GMT
ENV HAPROXY_VERSION=2.4-dev3
# Sat, 12 Dec 2020 16:28:01 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev3.tar.gz
# Sat, 12 Dec 2020 16:28:04 GMT
ENV HAPROXY_SHA256=c5de469830a43ac34d84af3de480b070d357af6289d47df00396db05dd1f7918
# Sat, 12 Dec 2020 16:32:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 12 Dec 2020 16:32:28 GMT
STOPSIGNAL SIGUSR1
# Sat, 12 Dec 2020 16:32:34 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Sat, 12 Dec 2020 16:32:37 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 12 Dec 2020 16:32:40 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c0f0648876332890be87a9f32ec4ad2a939e805be3152ab991a923f7dec2b35d`  
		Last Modified: Fri, 11 Dec 2020 03:41:39 GMT  
		Size: 30.5 MB (30524717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8e34b843ee17b6a31857c8b9561fbd465619ccc8241c41aaa5832fd26a5aa9b`  
		Last Modified: Sat, 12 Dec 2020 16:35:52 GMT  
		Size: 10.3 MB (10261712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e0a33afa2560dccaaf156dae82944a8552069a43645011808b096a5441744b`  
		Last Modified: Sat, 12 Dec 2020 16:35:48 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev` - linux; s390x

```console
$ docker pull haproxy@sha256:4907443cc858240ac55bc17816703836547da222da93a9b1bbc207b865a96cc1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.2 MB (35194648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:562e5e3477ee5ca38e2d3e0304eec278be9fac474be827b1e78541114bc2c3fc`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:12:11 GMT
ADD file:db86ce5a1665b6d8ac734c54ac249a811c58484f569b935b14772445962428aa in / 
# Fri, 11 Dec 2020 02:12:15 GMT
CMD ["bash"]
# Sat, 12 Dec 2020 03:58:54 GMT
ENV HAPROXY_VERSION=2.4-dev3
# Sat, 12 Dec 2020 03:58:54 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev3.tar.gz
# Sat, 12 Dec 2020 03:58:55 GMT
ENV HAPROXY_SHA256=c5de469830a43ac34d84af3de480b070d357af6289d47df00396db05dd1f7918
# Sat, 12 Dec 2020 03:59:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 12 Dec 2020 03:59:51 GMT
STOPSIGNAL SIGUSR1
# Sat, 12 Dec 2020 03:59:52 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Sat, 12 Dec 2020 03:59:52 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 12 Dec 2020 03:59:53 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:f4cf10ca9f31aab0854647d7878dc4db838e93b892b843dde3db24f2e909a106`  
		Last Modified: Fri, 11 Dec 2020 02:17:07 GMT  
		Size: 25.7 MB (25713957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd921b604346406e9dd864887ebb05dd9c41c9d03c5998d9afa66aac0a93bf34`  
		Last Modified: Sat, 12 Dec 2020 04:02:42 GMT  
		Size: 9.5 MB (9480311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8672adc52443d061895a600d2d80c5297f6bd2b9c5daac447b5754e0931cfab6`  
		Last Modified: Sat, 12 Dec 2020 04:02:40 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.4-dev4`

**does not exist** (yet?)

## `haproxy:2.4-dev4-alpine`

**does not exist** (yet?)

## `haproxy:2.4-dev-alpine`

```console
$ docker pull haproxy@sha256:d0124cbd86599cbce938ad841241d45ee2d6c7d019419d602f49fd8502111c4a
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
$ docker pull haproxy@sha256:828ee45dc6ede1405b8adf67501ff0d6cecc64ec2c64d35996fced409b2c79fc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.3 MB (10321840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5364de45b3992e88e760dc273343c214549edcb5be1076da9bd8d125e79e83bb`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:26:59 GMT
ENV HAPROXY_VERSION=2.4-dev3
# Thu, 17 Dec 2020 13:27:00 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev3.tar.gz
# Thu, 17 Dec 2020 13:27:00 GMT
ENV HAPROXY_SHA256=c5de469830a43ac34d84af3de480b070d357af6289d47df00396db05dd1f7918
# Thu, 17 Dec 2020 13:28:11 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 13:28:12 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 13:28:12 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 13:28:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 13:28:12 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7e3959b3458c993b92dadb892426bfa46a4209d7c716e87ff6d2fad1d321bc`  
		Last Modified: Thu, 17 Dec 2020 13:37:54 GMT  
		Size: 7.5 MB (7522393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76574a53f0ed81f4a029522cab0d2a2a4b1421b7d92601636e709de896a0bcb1`  
		Last Modified: Thu, 17 Dec 2020 13:37:51 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev-alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:5f95b45f13308769ed068c85044853462da0af50f6b9891c41805674227eb615
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (9976797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b94057fe13da18cf4278388480e038d51e048bdb98d3e660ad62ef2cedc46ee`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:35:39 GMT
ENV HAPROXY_VERSION=2.4-dev3
# Thu, 17 Dec 2020 01:35:41 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev3.tar.gz
# Thu, 17 Dec 2020 01:35:42 GMT
ENV HAPROXY_SHA256=c5de469830a43ac34d84af3de480b070d357af6289d47df00396db05dd1f7918
# Thu, 17 Dec 2020 01:36:15 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:36:16 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:36:16 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 01:36:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:36:18 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82840efd1dfbcdac35b53bb205cdf013cc520fe6a33348b22da37c1adecb116c`  
		Last Modified: Thu, 17 Dec 2020 01:41:05 GMT  
		Size: 7.4 MB (7372253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37738336809ad1a545769a54f4f5fdc50a0205954f2ff164c0f8dd8df7fd6bbc`  
		Last Modified: Thu, 17 Dec 2020 01:41:02 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:49a9060f6d457d107324de9a4ce529351cedd036ddc5999183b80421b0f6fc00
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9736882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b92363139f4709d1cfbde620ef379ca5d8e1279e109198add1d568feb2663173`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:37:53 GMT
ENV HAPROXY_VERSION=2.4-dev3
# Thu, 17 Dec 2020 01:37:54 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev3.tar.gz
# Thu, 17 Dec 2020 01:37:55 GMT
ENV HAPROXY_SHA256=c5de469830a43ac34d84af3de480b070d357af6289d47df00396db05dd1f7918
# Thu, 17 Dec 2020 01:38:22 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:38:24 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:38:26 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 01:38:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:38:29 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e742713895b031dec4e02fb0df5e61897f49bd47b8d4818dc2612e1c59d74a3`  
		Last Modified: Thu, 17 Dec 2020 01:43:06 GMT  
		Size: 7.3 MB (7328946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7e5540774bad9ee701064cf7dfab0294bd765b28bdc72e47756c78cc462f609`  
		Last Modified: Thu, 17 Dec 2020 01:43:04 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:9c34f5806c0d61d6c6943662f718dcf7c3a6c8577ff266a9323be50805cdab89
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.2 MB (10194387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:476be8e03a016dd992910f2accfaf02aa21d8136c6a502a8c06d0d9b2c61a64f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:23:24 GMT
ENV HAPROXY_VERSION=2.4-dev3
# Thu, 17 Dec 2020 01:23:25 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev3.tar.gz
# Thu, 17 Dec 2020 01:23:26 GMT
ENV HAPROXY_SHA256=c5de469830a43ac34d84af3de480b070d357af6289d47df00396db05dd1f7918
# Thu, 17 Dec 2020 01:23:50 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:23:52 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:23:53 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 01:23:53 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:23:55 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10d9e452e2cfcb1be11d23b64aa13ebad50d8053b66d3561c2ae19676b80ea1`  
		Last Modified: Thu, 17 Dec 2020 01:30:04 GMT  
		Size: 7.5 MB (7484958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d4d317b5887d82ce21492b22cfe92cdec1c0f8ba21c514b124c12ea19c9f78a`  
		Last Modified: Thu, 17 Dec 2020 01:30:01 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev-alpine` - linux; 386

```console
$ docker pull haproxy@sha256:5979b779e15173a48a51f67783fd61962385a71e0b2b84e74825703af59572cb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.3 MB (10257703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32c9a815d11f3e86949802595e54f411a7821128e95415e54d7f616b1037feb7`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 17 Dec 2020 00:38:32 GMT
ADD file:de33fda50a142403e842620d20bc4404e66fc4ace16edc6946c4539e8a797458 in / 
# Thu, 17 Dec 2020 00:38:32 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:24:35 GMT
ENV HAPROXY_VERSION=2.4-dev3
# Thu, 17 Dec 2020 02:24:35 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev3.tar.gz
# Thu, 17 Dec 2020 02:24:35 GMT
ENV HAPROXY_SHA256=c5de469830a43ac34d84af3de480b070d357af6289d47df00396db05dd1f7918
# Thu, 17 Dec 2020 02:26:11 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 02:26:11 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 02:26:11 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 02:26:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 02:26:12 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:455793c72b878001f0905634ed52a2524ba51796e7377bf00683a85123f7dce9`  
		Last Modified: Thu, 17 Dec 2020 00:39:18 GMT  
		Size: 2.8 MB (2794130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2500aec61b0965866a7f7e3daa6f99353fda20cbcba4cffbda7fb7b38e2b446`  
		Last Modified: Thu, 17 Dec 2020 02:34:29 GMT  
		Size: 7.5 MB (7463193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8df09994cfdb6a8e1a414626b4157dbe8cff0306a592c6ce318a1b9fce7dd897`  
		Last Modified: Thu, 17 Dec 2020 02:34:27 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev-alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:2e790f1dc8502f654ee0147f34bbf80971fbf1cb85c69d05298c7a58265f06ee
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.7 MB (10677434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8894be8d48319fb50edaa897f5b2708cb18895e3e6b4e43ddffb38d66ac94f48`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 17 Dec 2020 00:20:42 GMT
ADD file:0a38c9b4955f8faa79627c166fca80ef342e443a16ce2925a30eeae317bbd786 in / 
# Thu, 17 Dec 2020 00:20:48 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:38:53 GMT
ENV HAPROXY_VERSION=2.4-dev3
# Thu, 17 Dec 2020 02:39:03 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev3.tar.gz
# Thu, 17 Dec 2020 02:39:08 GMT
ENV HAPROXY_SHA256=c5de469830a43ac34d84af3de480b070d357af6289d47df00396db05dd1f7918
# Thu, 17 Dec 2020 02:39:52 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 02:39:57 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 02:39:59 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 02:40:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 02:40:11 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:a9d343b7bcc225fe7ac17d96a81329510ab7f31a50472311cafe7168d3107317`  
		Last Modified: Thu, 17 Dec 2020 00:21:33 GMT  
		Size: 2.8 MB (2805226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:069fecdb4ea52c8fd2623ef74fa2170ab266cccf6d908dba6016842cabe15ce1`  
		Last Modified: Thu, 17 Dec 2020 02:49:39 GMT  
		Size: 7.9 MB (7871827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c510411dfe7f080ff3164aee327cd753516fbad8092c7f89ce3cc16668208ac1`  
		Last Modified: Thu, 17 Dec 2020 02:49:37 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-dev-alpine` - linux; s390x

```console
$ docker pull haproxy@sha256:64f946eeef14ff3a4bc4dcb4dda250f78fe8a95647e5588b34e11beaf944eee2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.1 MB (10122166 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b9c9c8a0b8554479e913ee297789b900d05bc8aff127cc35a2bf817bf2a4d9f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:41:37 GMT
ADD file:3ad3856d165e8760af85574a8ffa75ca44b7e1b97b64d1d6d4608445efa4b860 in / 
# Wed, 16 Dec 2020 23:41:37 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:24:14 GMT
ENV HAPROXY_VERSION=2.4-dev3
# Thu, 17 Dec 2020 01:24:14 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/devel/haproxy-2.4-dev3.tar.gz
# Thu, 17 Dec 2020 01:24:15 GMT
ENV HAPROXY_SHA256=c5de469830a43ac34d84af3de480b070d357af6289d47df00396db05dd1f7918
# Thu, 17 Dec 2020 01:25:03 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:25:04 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:25:04 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 01:25:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:25:05 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:ee52640a49e15b8b7c8edb66c2d048b26abdee8d828d6e5ef4e10a28cb15a84f`  
		Last Modified: Wed, 16 Dec 2020 23:42:15 GMT  
		Size: 2.6 MB (2567018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc23d3f37e2b8c652950ee2a8f20ad629076e762fb2f80becad47ae894799ee`  
		Last Modified: Thu, 17 Dec 2020 01:31:11 GMT  
		Size: 7.6 MB (7554769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4956e5db3c78c5f0dabd5505a00f48d48149037aaf572b30bdc35095e73e4433`  
		Last Modified: Thu, 17 Dec 2020 01:31:09 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:alpine`

```console
$ docker pull haproxy@sha256:a4b532622824aa6421c107dcadaee692e48ebedd9b5bbb8c6ac612a89c66798c
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
$ docker pull haproxy@sha256:497f197a318f09642c09cacf4c3625978e83cca29bfa3dde2dacd9be893163ca
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.2 MB (10203759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a1001ef82706917ec78b526c93dfcf5e6263b0dc4eecc8631abaf9b685f8659`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:28:35 GMT
ENV HAPROXY_VERSION=2.3.2
# Thu, 17 Dec 2020 13:28:35 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.2.tar.gz
# Thu, 17 Dec 2020 13:28:36 GMT
ENV HAPROXY_SHA256=99cb73bb791a2cd18898d0595e14fdc820a6cbd622c762f4ed83f2884d038fd5
# Thu, 17 Dec 2020 13:30:35 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 13:30:36 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 13:30:36 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 13:30:37 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 13:30:37 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca683bcd5723099a7c129a2a93f01f05bceeedc9db28a5f533741450b4e65cb`  
		Last Modified: Thu, 17 Dec 2020 13:38:02 GMT  
		Size: 7.4 MB (7404313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9b048041f14ac7dc9e1866c7185833d10ed665e5cd25b2f29dba5905a1ab2f`  
		Last Modified: Thu, 17 Dec 2020 13:38:00 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:65ef8a4ed34778a5b768c4caa6dacd7524c412b75b4a3fb621cfb33808142d7b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9859894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:644556767ede8d9f4e94615aa163bf7ad16beb93c44bfecc7e7ecbc65cbfa18d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:36:29 GMT
ENV HAPROXY_VERSION=2.3.2
# Thu, 17 Dec 2020 01:36:29 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.2.tar.gz
# Thu, 17 Dec 2020 01:36:30 GMT
ENV HAPROXY_SHA256=99cb73bb791a2cd18898d0595e14fdc820a6cbd622c762f4ed83f2884d038fd5
# Thu, 17 Dec 2020 01:37:03 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:37:04 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:37:04 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 01:37:06 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:37:06 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6776e0a3544c93d9c3ce724a749c0386c4e5f879573dfa081a51e93e145cbf13`  
		Last Modified: Thu, 17 Dec 2020 01:41:17 GMT  
		Size: 7.3 MB (7255351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbf020734cc589411856a09679f990f60b5c80673fbe47f54599b3c8b06c44ac`  
		Last Modified: Thu, 17 Dec 2020 01:41:14 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:f6dc03525659ac0fb9fa9389b4ea80bc23226b720c3062003b725cf2860a6d66
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9617506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e94d22c496a979d2a87129121fd7cb23d1a5afc881ee21ffcd4ad9ce2030b24`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:38:43 GMT
ENV HAPROXY_VERSION=2.3.2
# Thu, 17 Dec 2020 01:38:44 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.2.tar.gz
# Thu, 17 Dec 2020 01:38:45 GMT
ENV HAPROXY_SHA256=99cb73bb791a2cd18898d0595e14fdc820a6cbd622c762f4ed83f2884d038fd5
# Thu, 17 Dec 2020 01:39:11 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:39:12 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:39:13 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 01:39:14 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:39:15 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef8ff9670f7a5023ba54df386ffccedb014f1e72bb95c20ff50a8bc703b00846`  
		Last Modified: Thu, 17 Dec 2020 01:43:19 GMT  
		Size: 7.2 MB (7209570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4541c3937c06cd84646da87a798a822082f7d4dbb187989a9b60f002585f4bb9`  
		Last Modified: Thu, 17 Dec 2020 01:43:17 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:4e20f7e25d2b0f281125d57b0b2d86df68d8ab063382c4bb9ebad18bf1fb7388
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.1 MB (10077526 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:405dfdce2795fb2b2cef8a6d78fbd610877e9d667ebdb03723e6625586a3e83e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:24:10 GMT
ENV HAPROXY_VERSION=2.3.2
# Thu, 17 Dec 2020 01:24:11 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.2.tar.gz
# Thu, 17 Dec 2020 01:24:13 GMT
ENV HAPROXY_SHA256=99cb73bb791a2cd18898d0595e14fdc820a6cbd622c762f4ed83f2884d038fd5
# Thu, 17 Dec 2020 01:24:38 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:24:39 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:24:40 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 01:24:41 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:24:42 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bef0c4aa00924d2cd300bd631a261a142299e072a13e8621d7d11b3cd208494`  
		Last Modified: Thu, 17 Dec 2020 01:30:18 GMT  
		Size: 7.4 MB (7368098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb9470f170e025b1fd1dd58d461a21682de90e83c63d0178dc7218e4f8dbf43`  
		Last Modified: Thu, 17 Dec 2020 01:30:15 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:alpine` - linux; 386

```console
$ docker pull haproxy@sha256:092422718ce95ec83ae9cea7ac7b86bb213a849e20e88ac5f3277ca890cac479
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.1 MB (10138880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd732a59bde146f31bc8514ec3cce5774631f523534edca54a2aedaf03218308`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 17 Dec 2020 00:38:32 GMT
ADD file:de33fda50a142403e842620d20bc4404e66fc4ace16edc6946c4539e8a797458 in / 
# Thu, 17 Dec 2020 00:38:32 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:26:24 GMT
ENV HAPROXY_VERSION=2.3.2
# Thu, 17 Dec 2020 02:26:24 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.2.tar.gz
# Thu, 17 Dec 2020 02:26:25 GMT
ENV HAPROXY_SHA256=99cb73bb791a2cd18898d0595e14fdc820a6cbd622c762f4ed83f2884d038fd5
# Thu, 17 Dec 2020 02:27:54 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 02:27:54 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 02:27:55 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 02:27:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 02:27:55 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:455793c72b878001f0905634ed52a2524ba51796e7377bf00683a85123f7dce9`  
		Last Modified: Thu, 17 Dec 2020 00:39:18 GMT  
		Size: 2.8 MB (2794130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3e70eb052ff09369f2e1424ad47ba6b4a21af58719dc96aaa4aaafa72e7e070`  
		Last Modified: Thu, 17 Dec 2020 02:34:47 GMT  
		Size: 7.3 MB (7344370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244af8e13011e1cbccf7467e84202b44ba3ac0e2f880fb76d6b68816b7f5876d`  
		Last Modified: Thu, 17 Dec 2020 02:34:35 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:c61f9595bd2d242786faef3608ac945b53ca84c812e2d24badadf4c29e8b93bf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.6 MB (10560399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6119c04ca1f959d866145f912434d0f905b783cbbe369b992d80546bcde463f0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 17 Dec 2020 00:20:42 GMT
ADD file:0a38c9b4955f8faa79627c166fca80ef342e443a16ce2925a30eeae317bbd786 in / 
# Thu, 17 Dec 2020 00:20:48 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:40:24 GMT
ENV HAPROXY_VERSION=2.3.2
# Thu, 17 Dec 2020 02:40:30 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.2.tar.gz
# Thu, 17 Dec 2020 02:40:38 GMT
ENV HAPROXY_SHA256=99cb73bb791a2cd18898d0595e14fdc820a6cbd622c762f4ed83f2884d038fd5
# Thu, 17 Dec 2020 02:41:25 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 02:41:31 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 02:41:34 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 02:41:40 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 02:41:45 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:a9d343b7bcc225fe7ac17d96a81329510ab7f31a50472311cafe7168d3107317`  
		Last Modified: Thu, 17 Dec 2020 00:21:33 GMT  
		Size: 2.8 MB (2805226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a36c2bce9570afb3b4542d019f7bf4931dc2abb64cd8133014a2f4960b5ccb`  
		Last Modified: Thu, 17 Dec 2020 02:49:54 GMT  
		Size: 7.8 MB (7754792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fce22188bda157976ae629c97e6d917919a5d010dbe11711e9c573c3917dc287`  
		Last Modified: Thu, 17 Dec 2020 02:49:51 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:alpine` - linux; s390x

```console
$ docker pull haproxy@sha256:e32e50f1720d8d74347be1d08c53060b121f5d33cf8dfe1c78e2b6673b5e4e01
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (10004227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85bf20b1ba112bcb2e39f297e7cda027a40971e4f4e077b9325806262e9f6b93`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:41:37 GMT
ADD file:3ad3856d165e8760af85574a8ffa75ca44b7e1b97b64d1d6d4608445efa4b860 in / 
# Wed, 16 Dec 2020 23:41:37 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:25:15 GMT
ENV HAPROXY_VERSION=2.3.2
# Thu, 17 Dec 2020 01:25:16 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.2.tar.gz
# Thu, 17 Dec 2020 01:25:16 GMT
ENV HAPROXY_SHA256=99cb73bb791a2cd18898d0595e14fdc820a6cbd622c762f4ed83f2884d038fd5
# Thu, 17 Dec 2020 01:26:02 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:26:03 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:26:03 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 01:26:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:26:04 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:ee52640a49e15b8b7c8edb66c2d048b26abdee8d828d6e5ef4e10a28cb15a84f`  
		Last Modified: Wed, 16 Dec 2020 23:42:15 GMT  
		Size: 2.6 MB (2567018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be334f2af5c8c1dc2046c3bb58d2969ce6e9e13d6c37a60c5d5facc7519b387`  
		Last Modified: Thu, 17 Dec 2020 01:31:21 GMT  
		Size: 7.4 MB (7436829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53baf298aad5720b3f2d0ebd9a6ea91ba7aee6a1038fc638434af786da52d4ec`  
		Last Modified: Thu, 17 Dec 2020 01:31:20 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:latest`

```console
$ docker pull haproxy@sha256:889b4c9d7fc1bc96de9003dbd7032e4fc43ec75194b69d4a2ac401f1f24f4e16
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
$ docker pull haproxy@sha256:4860d9794eda9fb82255fc89d6dce85ad5a9ef14b47b9ebeec6539e6179eb99c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.7 MB (36738634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecf07e33b5c4bbb59188bf77781c047d9ff8accdf21b1902212b4c04864982a8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:06:10 GMT
ADD file:3a7bff4e139bcacc5831fd70a035c130a91b5da001dd91c08b2acd635c7064e8 in / 
# Fri, 11 Dec 2020 02:06:10 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 06:28:09 GMT
ENV HAPROXY_VERSION=2.3.2
# Fri, 11 Dec 2020 06:28:09 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.2.tar.gz
# Fri, 11 Dec 2020 06:28:09 GMT
ENV HAPROXY_SHA256=99cb73bb791a2cd18898d0595e14fdc820a6cbd622c762f4ed83f2884d038fd5
# Fri, 11 Dec 2020 06:29:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 06:29:46 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 06:29:47 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 06:29:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 06:29:47 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:6ec7b7d162b24bd6df88abde89ceb6d7bbc2be927f025c9dd061af2b0c328cfe`  
		Last Modified: Fri, 11 Dec 2020 02:12:26 GMT  
		Size: 27.1 MB (27099295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:babde0d7067ce5bb18c684bf031cfae2b1347e9c1b33dcd28534e777e3be722f`  
		Last Modified: Fri, 11 Dec 2020 06:48:01 GMT  
		Size: 9.6 MB (9638959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5481c8a4effb2e57ba600574d8f3d55527251112fad63bde55889ef48e2aa889`  
		Last Modified: Fri, 11 Dec 2020 06:47:51 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:latest` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:ce1efa598867b2b6bdc23e8939cf570bd497ca50cf89cbd5cf47df73f4455d5c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34094439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e4360389b6e24cf55fe8b4f15e16bb3de800395360213a6e196e51383e33272`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:49 GMT
ADD file:58ebb3ffaf26d9b7621efba5f109ae9d22832f2f22865cda36604b138cbdb7b8 in / 
# Fri, 11 Dec 2020 02:04:56 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 03:26:28 GMT
ENV HAPROXY_VERSION=2.3.2
# Fri, 11 Dec 2020 03:26:30 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.2.tar.gz
# Fri, 11 Dec 2020 03:26:32 GMT
ENV HAPROXY_SHA256=99cb73bb791a2cd18898d0595e14fdc820a6cbd622c762f4ed83f2884d038fd5
# Fri, 11 Dec 2020 03:27:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 03:27:26 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 03:27:27 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 03:27:28 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:27:29 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:8cbd1f790d64c77fcac6c9dbfe4d4c82f0365de9438f1a42b0560dc88f9e6a55`  
		Last Modified: Fri, 11 Dec 2020 02:14:44 GMT  
		Size: 24.8 MB (24843461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8201a0540f14f83cebd166f9eb8b2e6868ae479bb9d88db3782b27f4475f6115`  
		Last Modified: Fri, 11 Dec 2020 03:35:10 GMT  
		Size: 9.3 MB (9250597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f414bb6e55af4c969210ca000a4e3db02adcdc632ce2fa733d23c23f4cee46d`  
		Last Modified: Fri, 11 Dec 2020 03:35:06 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:latest` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:799c4cf3d5511ec7a381d76d624bfda090da64f0f7a570ebea7f7fb2492c2b08
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31774902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34a16b900cd9c658ddc60b921684ffb64fdc25dccbc6cb2d0ba445fa99c76cb1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:23:37 GMT
ADD file:75ca842ac2d6e9f6617bb3df280af1e4c9619c9805fd5e00c1c3d6b8b4e3d802 in / 
# Fri, 11 Dec 2020 02:23:39 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 04:53:56 GMT
ENV HAPROXY_VERSION=2.3.2
# Fri, 11 Dec 2020 04:53:57 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.2.tar.gz
# Fri, 11 Dec 2020 04:53:58 GMT
ENV HAPROXY_SHA256=99cb73bb791a2cd18898d0595e14fdc820a6cbd622c762f4ed83f2884d038fd5
# Fri, 11 Dec 2020 04:54:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 04:54:42 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 04:54:44 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 04:54:44 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 04:54:46 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c06905228d4fc5a5c840a70e2e6ced56596a8bc73abc69e6a1867bbb6f7ae7e7`  
		Last Modified: Fri, 11 Dec 2020 02:33:07 GMT  
		Size: 22.7 MB (22707662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b18920727745d1198efa252a298135ebb3e0cee3f2be2ec4aed8608d42e8c7c`  
		Last Modified: Fri, 11 Dec 2020 05:04:59 GMT  
		Size: 9.1 MB (9066859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:503a299b85cfeda421f53031cf13ae1d8f2328cf24410ca507aa257db3a584e8`  
		Last Modified: Fri, 11 Dec 2020 05:04:57 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:latest` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:4797dffb4de987894cd0d7e3fddf97dd39e17fd34f409630724501d5d54f3375
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35320778 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1073c1f4bbe1be3699a00df24887f2b7b22c658b160f8e69caeaed50a856a06d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:45:53 GMT
ADD file:a5a2f039c00bc638b88cefdff4c3cd1865b4d415bf80c4fe6b496d975af7cc1f in / 
# Fri, 11 Dec 2020 02:45:57 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 05:31:27 GMT
ENV HAPROXY_VERSION=2.3.2
# Fri, 11 Dec 2020 05:31:28 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.2.tar.gz
# Fri, 11 Dec 2020 05:31:29 GMT
ENV HAPROXY_SHA256=99cb73bb791a2cd18898d0595e14fdc820a6cbd622c762f4ed83f2884d038fd5
# Fri, 11 Dec 2020 05:32:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 05:32:23 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 05:32:24 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 05:32:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:32:26 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c9648d7fcbb6d597cf33916d8fcd207fde8ec05d764b4480d4f3e884e142a902`  
		Last Modified: Fri, 11 Dec 2020 02:53:14 GMT  
		Size: 25.9 MB (25856191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a03032109a3408c7f6452a59eba9ff651f3be467ace9c735b2c151cb7b9cb31`  
		Last Modified: Fri, 11 Dec 2020 05:43:52 GMT  
		Size: 9.5 MB (9464207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780c192d356a56d112c0bff8106c349e11329c5e23d76dd868a996bf09dd50f9`  
		Last Modified: Fri, 11 Dec 2020 05:43:50 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:latest` - linux; 386

```console
$ docker pull haproxy@sha256:3b84c007b2fb56ce5380065119d78475dba59a3bfeb417be3edb6c2bdda80d60
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37287145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1fd13752edbb99935735f761ee08efa7ec780f27a6f8d7026ea8b5086d9c332`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:07 GMT
ADD file:a0879774b23f70c4db7f7b04736cca142beb0b22e93f5952364ca990a1675552 in / 
# Fri, 11 Dec 2020 02:03:08 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 05:06:25 GMT
ENV HAPROXY_VERSION=2.3.2
# Fri, 11 Dec 2020 05:06:25 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.2.tar.gz
# Fri, 11 Dec 2020 05:06:26 GMT
ENV HAPROXY_SHA256=99cb73bb791a2cd18898d0595e14fdc820a6cbd622c762f4ed83f2884d038fd5
# Fri, 11 Dec 2020 05:08:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 05:08:06 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 05:08:07 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 05:08:07 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:08:08 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:cfec07a090788e68b692f30d34e11dc7af0f1c8112fbc846e8e40e24faf882d7`  
		Last Modified: Fri, 11 Dec 2020 02:09:41 GMT  
		Size: 27.8 MB (27757584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d24160835d3ce6cd6a891511665f008d92aa7b2785ad76b373c67d9e555158af`  
		Last Modified: Fri, 11 Dec 2020 05:25:25 GMT  
		Size: 9.5 MB (9529181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c720f841b372f39c960735d688b1a090f8287dd22c78278da10850ed3675fd9`  
		Last Modified: Fri, 11 Dec 2020 05:25:22 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:latest` - linux; mips64le

```console
$ docker pull haproxy@sha256:47fe68bf4ccd8b76178f984ee18686fc7618231049db8d91d3b31ab017a7d93c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.0 MB (34986193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b7bee85f1b7b1ba34fa6c15d4003eb40217a24da9445980254f2f8cf07239f2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:30 GMT
ADD file:edb758d587972f30ef28b162dcabf79f61b685afa3c6066cb611c61abea124f3 in / 
# Fri, 11 Dec 2020 02:03:30 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 03:18:39 GMT
ENV HAPROXY_VERSION=2.3.2
# Fri, 11 Dec 2020 03:18:39 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.2.tar.gz
# Fri, 11 Dec 2020 03:18:39 GMT
ENV HAPROXY_SHA256=99cb73bb791a2cd18898d0595e14fdc820a6cbd622c762f4ed83f2884d038fd5
# Fri, 11 Dec 2020 03:21:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 03:21:02 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 03:21:02 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 03:21:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:21:03 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:bed35f8e8e003f268bd91c8bc28d93f0b1463296add14ab3ec84c3d3d30e9025`  
		Last Modified: Fri, 11 Dec 2020 02:10:15 GMT  
		Size: 25.8 MB (25769881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56160242f2040d557d6d1772d02a223df3069a8367382e6a1e259b1196effe92`  
		Last Modified: Fri, 11 Dec 2020 03:33:03 GMT  
		Size: 9.2 MB (9215932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ccc4a11e34e39a69c2886e2edd20c1c5a156411ca4db70a665bfb097227c14`  
		Last Modified: Fri, 11 Dec 2020 03:32:56 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:latest` - linux; ppc64le

```console
$ docker pull haproxy@sha256:37819fd7b83a49c2986493f3be3d2183c638125f75688d202a861d4a97fec17d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40649597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e9b50a06cb8bcebb665437264710388e31be79f6c9b4b6da1f03f81369ecdaa`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 03:34:02 GMT
ADD file:eca1a7737bd5e84ff883c4c284c0cd22492145d9cd7ae3b8e7b490e3d8e5aefb in / 
# Fri, 11 Dec 2020 03:34:11 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 05:25:33 GMT
ENV HAPROXY_VERSION=2.3.2
# Fri, 11 Dec 2020 05:25:36 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.2.tar.gz
# Fri, 11 Dec 2020 05:25:40 GMT
ENV HAPROXY_SHA256=99cb73bb791a2cd18898d0595e14fdc820a6cbd622c762f4ed83f2884d038fd5
# Fri, 11 Dec 2020 05:28:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 05:28:25 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 05:28:27 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 05:28:32 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:28:34 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c0f0648876332890be87a9f32ec4ad2a939e805be3152ab991a923f7dec2b35d`  
		Last Modified: Fri, 11 Dec 2020 03:41:39 GMT  
		Size: 30.5 MB (30524717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19f0165c728ecb9e371716d3a364af6237f7d0bbaef67fba0be7aeee08ba4677`  
		Last Modified: Fri, 11 Dec 2020 05:53:36 GMT  
		Size: 10.1 MB (10124500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb3355b62bacf1809975a9c89f56412ce4e0bca80b083087057b7e3d425e420e`  
		Last Modified: Fri, 11 Dec 2020 05:53:34 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:latest` - linux; s390x

```console
$ docker pull haproxy@sha256:95130cc7eabcb463bf983aa7983a3aea1a424f8693893ecf23af0faf2e0b9dd5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35063292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42304927f097e7b29030c4c8a900826d39241b05fd329b83314d68ddfe39d491`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:12:11 GMT
ADD file:db86ce5a1665b6d8ac734c54ac249a811c58484f569b935b14772445962428aa in / 
# Fri, 11 Dec 2020 02:12:15 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 03:16:37 GMT
ENV HAPROXY_VERSION=2.3.2
# Fri, 11 Dec 2020 03:16:37 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.2.tar.gz
# Fri, 11 Dec 2020 03:16:38 GMT
ENV HAPROXY_SHA256=99cb73bb791a2cd18898d0595e14fdc820a6cbd622c762f4ed83f2884d038fd5
# Fri, 11 Dec 2020 03:17:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 03:17:50 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 03:17:50 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 03:17:50 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:17:51 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:f4cf10ca9f31aab0854647d7878dc4db838e93b892b843dde3db24f2e909a106`  
		Last Modified: Fri, 11 Dec 2020 02:17:07 GMT  
		Size: 25.7 MB (25713957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e1407baabb38f88b38bde51950dda870904b2cbb0781a1c2927cb795c59834f`  
		Last Modified: Fri, 11 Dec 2020 03:27:48 GMT  
		Size: 9.3 MB (9348954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:014aca4270aeead92d2682142602ba0bfb1a50c5869a2e05879a84d4af45c88c`  
		Last Modified: Fri, 11 Dec 2020 03:27:47 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:lts`

```console
$ docker pull haproxy@sha256:09bdec22b056a76eb6186125206eafb2cebca84d054bc7f34fbfb3a6ecc808bf
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
$ docker pull haproxy@sha256:8d256391453d747a976fc2981ac618686650d5b269c4adb0d4a3fa12b4135f05
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.4 MB (36361780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5cf79a9a418029a83d802f592e7af8c7b86e63fe965984432ed4a46f512706c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:06:10 GMT
ADD file:3a7bff4e139bcacc5831fd70a035c130a91b5da001dd91c08b2acd635c7064e8 in / 
# Fri, 11 Dec 2020 02:06:10 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 06:32:14 GMT
ENV HAPROXY_VERSION=2.2.6
# Fri, 11 Dec 2020 06:32:14 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.6.tar.gz
# Fri, 11 Dec 2020 06:32:15 GMT
ENV HAPROXY_SHA256=be1c6754cbaceafc4837e0c6036c7f81027a3992516435cbbbc5dc749bf5a087
# Fri, 11 Dec 2020 06:33:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 06:33:57 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 06:33:58 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 06:33:58 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 06:33:58 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:6ec7b7d162b24bd6df88abde89ceb6d7bbc2be927f025c9dd061af2b0c328cfe`  
		Last Modified: Fri, 11 Dec 2020 02:12:26 GMT  
		Size: 27.1 MB (27099295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec8cba38ca5dd282c67ba27b309ce8ac7ed06c07962c2c3c556979cd4aef595`  
		Last Modified: Fri, 11 Dec 2020 06:48:17 GMT  
		Size: 9.3 MB (9262105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f769eb67a743777a835e601828829fe93fab0c4a8aeba36631702dd503565f1f`  
		Last Modified: Fri, 11 Dec 2020 06:48:14 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:63132c4d6f537017f665eadc3498ac659596f62dad4497376bff9f68ef41967b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.7 MB (33712088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7379ce9c6013e5f08258df1958d56349c25821e28de8fad2b6ef4c49c716525`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:49 GMT
ADD file:58ebb3ffaf26d9b7621efba5f109ae9d22832f2f22865cda36604b138cbdb7b8 in / 
# Fri, 11 Dec 2020 02:04:56 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 03:27:36 GMT
ENV HAPROXY_VERSION=2.2.6
# Fri, 11 Dec 2020 03:27:37 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.6.tar.gz
# Fri, 11 Dec 2020 03:27:37 GMT
ENV HAPROXY_SHA256=be1c6754cbaceafc4837e0c6036c7f81027a3992516435cbbbc5dc749bf5a087
# Fri, 11 Dec 2020 03:28:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 03:28:25 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 03:28:26 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 03:28:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:28:28 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:8cbd1f790d64c77fcac6c9dbfe4d4c82f0365de9438f1a42b0560dc88f9e6a55`  
		Last Modified: Fri, 11 Dec 2020 02:14:44 GMT  
		Size: 24.8 MB (24843461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bbc3be8af28f619ffcbaf075fa11239304fd31314feac5bab52a950a53fec09`  
		Last Modified: Fri, 11 Dec 2020 03:35:25 GMT  
		Size: 8.9 MB (8868246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c87b4e1920b700942381841e8dda8cbd8348bbdb4c3954bbf205ef55c21eaaf5`  
		Last Modified: Fri, 11 Dec 2020 03:35:22 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:bfb727159cb18123ffe505ce5378158b3d39f733c16c50c4e0510322d2a68ef5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31385471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e846073708d57e8a4ccea6bc82f7c5f5a0478ede7cf5a1b2a00104ed74cdbb38`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:23:37 GMT
ADD file:75ca842ac2d6e9f6617bb3df280af1e4c9619c9805fd5e00c1c3d6b8b4e3d802 in / 
# Fri, 11 Dec 2020 02:23:39 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 04:55:36 GMT
ENV HAPROXY_VERSION=2.2.6
# Fri, 11 Dec 2020 04:55:37 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.6.tar.gz
# Fri, 11 Dec 2020 04:55:37 GMT
ENV HAPROXY_SHA256=be1c6754cbaceafc4837e0c6036c7f81027a3992516435cbbbc5dc749bf5a087
# Fri, 11 Dec 2020 04:56:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 04:56:22 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 04:56:23 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 04:56:23 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 04:56:24 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c06905228d4fc5a5c840a70e2e6ced56596a8bc73abc69e6a1867bbb6f7ae7e7`  
		Last Modified: Fri, 11 Dec 2020 02:33:07 GMT  
		Size: 22.7 MB (22707662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c7ae28f106557ec472cc950af6eeda82b3a0dd7783c1dac977b40d916f4fda`  
		Last Modified: Fri, 11 Dec 2020 05:05:27 GMT  
		Size: 8.7 MB (8677429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1905cfd88afb156e0ea86b3b5bccd788096b16684660928f90fff8fde968989`  
		Last Modified: Fri, 11 Dec 2020 05:05:25 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:35eeeed1ab0350d953a6fecebb8bb7d37929b15b1380f730f4a79251a23814cc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.9 MB (34938817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9431c867864058dea4ec59609fcd43b6302908aca8f0b3d18be96f688aec51ee`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:45:53 GMT
ADD file:a5a2f039c00bc638b88cefdff4c3cd1865b4d415bf80c4fe6b496d975af7cc1f in / 
# Fri, 11 Dec 2020 02:45:57 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 05:33:26 GMT
ENV HAPROXY_VERSION=2.2.6
# Fri, 11 Dec 2020 05:33:27 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.6.tar.gz
# Fri, 11 Dec 2020 05:33:28 GMT
ENV HAPROXY_SHA256=be1c6754cbaceafc4837e0c6036c7f81027a3992516435cbbbc5dc749bf5a087
# Fri, 11 Dec 2020 05:34:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 05:34:32 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 05:34:33 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 05:34:36 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:34:39 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c9648d7fcbb6d597cf33916d8fcd207fde8ec05d764b4480d4f3e884e142a902`  
		Last Modified: Fri, 11 Dec 2020 02:53:14 GMT  
		Size: 25.9 MB (25856191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1add3f9207b5ef098d2aafd4a2e15d79ca7abe80a71e060e771f2dfe4ec8f9b5`  
		Last Modified: Fri, 11 Dec 2020 05:44:16 GMT  
		Size: 9.1 MB (9082245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5a7da4f421bf47a867df37a1fa1e7a758d1464a7268d2289c0e1c300322eff4`  
		Last Modified: Fri, 11 Dec 2020 05:44:13 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; 386

```console
$ docker pull haproxy@sha256:d87b7f3d94a73cc2d813ace1731a23ee4160bb5e16a510a282d22a2c72768923
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.9 MB (36898031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7c1b93169b077d16b58324f9d72e7b4bc73a701ca1c17bcd95fd6b7fa5655e0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:07 GMT
ADD file:a0879774b23f70c4db7f7b04736cca142beb0b22e93f5952364ca990a1675552 in / 
# Fri, 11 Dec 2020 02:03:08 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 05:10:44 GMT
ENV HAPROXY_VERSION=2.2.6
# Fri, 11 Dec 2020 05:10:44 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.6.tar.gz
# Fri, 11 Dec 2020 05:10:44 GMT
ENV HAPROXY_SHA256=be1c6754cbaceafc4837e0c6036c7f81027a3992516435cbbbc5dc749bf5a087
# Fri, 11 Dec 2020 05:12:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 05:12:23 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 05:12:23 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 05:12:23 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:12:23 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:cfec07a090788e68b692f30d34e11dc7af0f1c8112fbc846e8e40e24faf882d7`  
		Last Modified: Fri, 11 Dec 2020 02:09:41 GMT  
		Size: 27.8 MB (27757584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:081e978aa8c309ca75402a34a8e617d85ad6e185cf19fb056864296178948ae0`  
		Last Modified: Fri, 11 Dec 2020 05:25:45 GMT  
		Size: 9.1 MB (9140066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5178ce4deb6b15b8657bb5b2e232df5606ea097853a30df0d4943b6ebb8ffc`  
		Last Modified: Fri, 11 Dec 2020 05:25:42 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; mips64le

```console
$ docker pull haproxy@sha256:1693fdc275c879fb7436b059c1a506ec7287c117479ed39dac7db7588abae3e5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.6 MB (34602107 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9c743e757ccc7273b9f380196c105abd0ea2b5530b2fb5a065b5997defd61c0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:30 GMT
ADD file:edb758d587972f30ef28b162dcabf79f61b685afa3c6066cb611c61abea124f3 in / 
# Fri, 11 Dec 2020 02:03:30 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 03:21:20 GMT
ENV HAPROXY_VERSION=2.2.6
# Fri, 11 Dec 2020 03:21:21 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.6.tar.gz
# Fri, 11 Dec 2020 03:21:21 GMT
ENV HAPROXY_SHA256=be1c6754cbaceafc4837e0c6036c7f81027a3992516435cbbbc5dc749bf5a087
# Fri, 11 Dec 2020 03:23:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 03:23:42 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 03:23:42 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 03:23:42 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:23:43 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:bed35f8e8e003f268bd91c8bc28d93f0b1463296add14ab3ec84c3d3d30e9025`  
		Last Modified: Fri, 11 Dec 2020 02:10:15 GMT  
		Size: 25.8 MB (25769881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c5f65a386c1ed85efa2abfe435e79442cf5db1892acfe55e0d9db56e3148905`  
		Last Modified: Fri, 11 Dec 2020 03:33:24 GMT  
		Size: 8.8 MB (8831846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9539bf3bf1abc25ce84fdec18ef846805479679554d31d61ca022f443eac5c15`  
		Last Modified: Fri, 11 Dec 2020 03:33:18 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; ppc64le

```console
$ docker pull haproxy@sha256:3312f227706a464629651ea9a5b0707c1bf6679d957df5c2560f66b6b2745cb6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40252016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d85fd237b4c4712e373ae95f36cfe3f5ae604d1cd847f83c57dc824008d24ffa`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 03:34:02 GMT
ADD file:eca1a7737bd5e84ff883c4c284c0cd22492145d9cd7ae3b8e7b490e3d8e5aefb in / 
# Fri, 11 Dec 2020 03:34:11 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 05:29:57 GMT
ENV HAPROXY_VERSION=2.2.6
# Fri, 11 Dec 2020 05:30:00 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.6.tar.gz
# Fri, 11 Dec 2020 05:30:03 GMT
ENV HAPROXY_SHA256=be1c6754cbaceafc4837e0c6036c7f81027a3992516435cbbbc5dc749bf5a087
# Fri, 11 Dec 2020 05:33:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 05:33:30 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 05:33:31 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 05:33:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 05:33:40 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c0f0648876332890be87a9f32ec4ad2a939e805be3152ab991a923f7dec2b35d`  
		Last Modified: Fri, 11 Dec 2020 03:41:39 GMT  
		Size: 30.5 MB (30524717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:477fcdb8fd9422a6d91a0b51b4a556ededd7ad2a1e2f89b36a11a751938c739c`  
		Last Modified: Fri, 11 Dec 2020 05:54:08 GMT  
		Size: 9.7 MB (9726919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1528107bda347188426c219b16ea67b373659dec38137713456ea09c7a010e`  
		Last Modified: Fri, 11 Dec 2020 05:54:06 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; s390x

```console
$ docker pull haproxy@sha256:a591d35c15413d1a3e1e9b23e2c722e673a6f31d6e3df6bbb08d2e5f78babef5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34675346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:582fe644d7a4d5b108df1cbf93e36b3e9734da0f3cc338828c268022ebb6c0e5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 11 Dec 2020 02:12:11 GMT
ADD file:db86ce5a1665b6d8ac734c54ac249a811c58484f569b935b14772445962428aa in / 
# Fri, 11 Dec 2020 02:12:15 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 03:18:54 GMT
ENV HAPROXY_VERSION=2.2.6
# Fri, 11 Dec 2020 03:18:54 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.6.tar.gz
# Fri, 11 Dec 2020 03:18:55 GMT
ENV HAPROXY_SHA256=be1c6754cbaceafc4837e0c6036c7f81027a3992516435cbbbc5dc749bf5a087
# Fri, 11 Dec 2020 03:19:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 03:19:50 GMT
STOPSIGNAL SIGUSR1
# Fri, 11 Dec 2020 03:19:50 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 11 Dec 2020 03:19:51 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:19:51 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:f4cf10ca9f31aab0854647d7878dc4db838e93b892b843dde3db24f2e909a106`  
		Last Modified: Fri, 11 Dec 2020 02:17:07 GMT  
		Size: 25.7 MB (25713957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fb580d8c3a873086ed2fa8f054f0b2f3b10607a065695564201de95b7086b30`  
		Last Modified: Fri, 11 Dec 2020 03:28:12 GMT  
		Size: 9.0 MB (8961008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f34dafa5401bd4ca0f465d6a4c19fb8caeac5cdc0c00820cc720ff4b7d93f8`  
		Last Modified: Fri, 11 Dec 2020 03:28:11 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:lts-alpine`

```console
$ docker pull haproxy@sha256:9bc2f658ba59c0bf73cf5ead746088fb3538c62b6ae04fa243b9a6e0e93fc276
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
$ docker pull haproxy@sha256:526dee11e5d239cff7277e614050859fc31b2c2defceb086c2b566b990f58153
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.8 MB (9840056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d6dea3f03bbca57a5827517780f65ab2ed5951a9e3e35ec438d27703daf3ebd`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:30:59 GMT
ENV HAPROXY_VERSION=2.2.6
# Thu, 17 Dec 2020 13:30:59 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.6.tar.gz
# Thu, 17 Dec 2020 13:31:00 GMT
ENV HAPROXY_SHA256=be1c6754cbaceafc4837e0c6036c7f81027a3992516435cbbbc5dc749bf5a087
# Thu, 17 Dec 2020 13:32:52 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 13:32:52 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 13:32:52 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 13:32:52 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 13:32:53 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759eb7f81a327bc1a3d612ac3a50b3b84b78a3516fcc3aabcc01e8dbfd5b9e40`  
		Last Modified: Thu, 17 Dec 2020 13:38:14 GMT  
		Size: 7.0 MB (7040609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85c4cdd2faa6bed3ca9ba8bed31b1e2574744ac8cfdc1c7108e30e5e4fd72565`  
		Last Modified: Thu, 17 Dec 2020 13:38:13 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts-alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:2719f3b4fcb4af0feb5a5edf06c49e8a56653644170a7486ea333a5b835bd42d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9506086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0e394b8272efd1126be17e7b53d6b303ca7a952d8cd36247fc1d447090b13fc`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:37:18 GMT
ENV HAPROXY_VERSION=2.2.6
# Thu, 17 Dec 2020 01:37:19 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.6.tar.gz
# Thu, 17 Dec 2020 01:37:21 GMT
ENV HAPROXY_SHA256=be1c6754cbaceafc4837e0c6036c7f81027a3992516435cbbbc5dc749bf5a087
# Thu, 17 Dec 2020 01:37:54 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:37:55 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:37:55 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 01:37:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:37:57 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85db562c8ad7ba86d9e7b120b60063560d79bfa30565b71dfe8a474e25d730f6`  
		Last Modified: Thu, 17 Dec 2020 01:41:30 GMT  
		Size: 6.9 MB (6901544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:232105dd31bf2e77869f401d6d599b724067ac9f2142a6bef35c760ccbfc8940`  
		Last Modified: Thu, 17 Dec 2020 01:41:27 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:daa8862e7c0f0b79f9c2ea2eb57a3788c86f9e0933de00610975716d73c4ebb0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9269715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3641a5ac74cfeb1efef1023f9b65091f0d0ddf47e5f2a930029b78565b59573c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:39:30 GMT
ENV HAPROXY_VERSION=2.2.6
# Thu, 17 Dec 2020 01:39:31 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.6.tar.gz
# Thu, 17 Dec 2020 01:39:32 GMT
ENV HAPROXY_SHA256=be1c6754cbaceafc4837e0c6036c7f81027a3992516435cbbbc5dc749bf5a087
# Thu, 17 Dec 2020 01:39:59 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:40:00 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:40:01 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 01:40:02 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:40:02 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b6e463615171e2a31179dd5ff1429d294d7ab17460f19303a0d5adcdce81757`  
		Last Modified: Thu, 17 Dec 2020 01:43:35 GMT  
		Size: 6.9 MB (6861780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7962c64ebb536fd12e3b688fcd64bd1df74149b49fd9b0520993e274c6e174`  
		Last Modified: Thu, 17 Dec 2020 01:43:32 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:30f8dd480c7bc2d7e8272f78dbb1e4d041de19e06298f26cd7503208692c8d80
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9709280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d600a937a50a5d5ace5d635075a67ffeed8714c9cd6cce90cccf68d4c6326b0c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:24:58 GMT
ENV HAPROXY_VERSION=2.2.6
# Thu, 17 Dec 2020 01:25:00 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.6.tar.gz
# Thu, 17 Dec 2020 01:25:01 GMT
ENV HAPROXY_SHA256=be1c6754cbaceafc4837e0c6036c7f81027a3992516435cbbbc5dc749bf5a087
# Thu, 17 Dec 2020 01:25:24 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:25:25 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:25:26 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 01:25:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:25:27 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5bed8e0c2754d35b1f66e5672f12caaccc4ccdd8586e63ab1890e73ba592f42`  
		Last Modified: Thu, 17 Dec 2020 01:30:31 GMT  
		Size: 7.0 MB (6999852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f29e8e256e27e16150bcdfc08f5158e053ff5b588556906ff5accd0943a7d1`  
		Last Modified: Thu, 17 Dec 2020 01:30:30 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts-alpine` - linux; 386

```console
$ docker pull haproxy@sha256:72f2efb3ad6b3004c443030e00d357f061958441d278a361537fb72656f3d907
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.8 MB (9773186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41212fb3cc8f9751506f26530dc2286344e63bb880d8a9ad4ef56025ab2d9814`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 17 Dec 2020 00:38:32 GMT
ADD file:de33fda50a142403e842620d20bc4404e66fc4ace16edc6946c4539e8a797458 in / 
# Thu, 17 Dec 2020 00:38:32 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:28:14 GMT
ENV HAPROXY_VERSION=2.2.6
# Thu, 17 Dec 2020 02:28:14 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.6.tar.gz
# Thu, 17 Dec 2020 02:28:14 GMT
ENV HAPROXY_SHA256=be1c6754cbaceafc4837e0c6036c7f81027a3992516435cbbbc5dc749bf5a087
# Thu, 17 Dec 2020 02:29:36 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 02:29:36 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 02:29:37 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 02:29:37 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 02:29:37 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:455793c72b878001f0905634ed52a2524ba51796e7377bf00683a85123f7dce9`  
		Last Modified: Thu, 17 Dec 2020 00:39:18 GMT  
		Size: 2.8 MB (2794130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d138995e356aece6ca41b32bb307e0afaa434035ffc74910401a28f9eeea344`  
		Last Modified: Thu, 17 Dec 2020 02:34:56 GMT  
		Size: 7.0 MB (6978676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0fb3a312dbd21c06c01bb58d7da51e9321383895092ed35a567a9fed213c114`  
		Last Modified: Thu, 17 Dec 2020 02:34:54 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts-alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:bec2a820948b8188b294d1bcd1ac7394cdd3c6031285be0c10940ca2a469e655
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.2 MB (10187069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6ad91eb8f93d270fd69f9895dc48452bc82037af79cfc72117b61b4b47184d7`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 17 Dec 2020 00:20:42 GMT
ADD file:0a38c9b4955f8faa79627c166fca80ef342e443a16ce2925a30eeae317bbd786 in / 
# Thu, 17 Dec 2020 00:20:48 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 02:42:08 GMT
ENV HAPROXY_VERSION=2.2.6
# Thu, 17 Dec 2020 02:42:16 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.6.tar.gz
# Thu, 17 Dec 2020 02:42:26 GMT
ENV HAPROXY_SHA256=be1c6754cbaceafc4837e0c6036c7f81027a3992516435cbbbc5dc749bf5a087
# Thu, 17 Dec 2020 02:43:07 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 02:43:16 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 02:43:22 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 02:43:28 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 02:43:33 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:a9d343b7bcc225fe7ac17d96a81329510ab7f31a50472311cafe7168d3107317`  
		Last Modified: Thu, 17 Dec 2020 00:21:33 GMT  
		Size: 2.8 MB (2805226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77cd771ed6b5e28c4a26cf193ce198e156b11fc7f6f673db8150a9d3120daefc`  
		Last Modified: Thu, 17 Dec 2020 02:50:13 GMT  
		Size: 7.4 MB (7381462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8848329b6093e7e582622ed4c4addc36d9fc50bb4643bf47f01440775e10773`  
		Last Modified: Thu, 17 Dec 2020 02:50:12 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts-alpine` - linux; s390x

```console
$ docker pull haproxy@sha256:62f9c9c476998bc0d23607d30d909c35fc5c89640982ed8b6cf21f74eaef2e9d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.7 MB (9653023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b66e3eb0a0d2ba561a17f668ee34c3254f2f3d409dca460dca0ec86b8f4f1a51`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 16 Dec 2020 23:41:37 GMT
ADD file:3ad3856d165e8760af85574a8ffa75ca44b7e1b97b64d1d6d4608445efa4b860 in / 
# Wed, 16 Dec 2020 23:41:37 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:26:18 GMT
ENV HAPROXY_VERSION=2.2.6
# Thu, 17 Dec 2020 01:26:18 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.6.tar.gz
# Thu, 17 Dec 2020 01:26:19 GMT
ENV HAPROXY_SHA256=be1c6754cbaceafc4837e0c6036c7f81027a3992516435cbbbc5dc749bf5a087
# Thu, 17 Dec 2020 01:27:05 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Thu, 17 Dec 2020 01:27:06 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Dec 2020 01:27:07 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 17 Dec 2020 01:27:07 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 01:27:08 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:ee52640a49e15b8b7c8edb66c2d048b26abdee8d828d6e5ef4e10a28cb15a84f`  
		Last Modified: Wed, 16 Dec 2020 23:42:15 GMT  
		Size: 2.6 MB (2567018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9ec00b782bf6a7bcf6d4c23d67da618049c965a58a5f25bac4ded1c3db27b4`  
		Last Modified: Thu, 17 Dec 2020 01:31:34 GMT  
		Size: 7.1 MB (7085625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a55622d8f9ba26c780c474e60ce94e0755d30d28639d58ab1fbd7f129d4e30d`  
		Last Modified: Thu, 17 Dec 2020 01:31:33 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
