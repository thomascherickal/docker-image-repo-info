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
-	[`haproxy:2.4`](#haproxy24)
-	[`haproxy:2.4-alpine`](#haproxy24-alpine)
-	[`haproxy:2.4.0`](#haproxy240)
-	[`haproxy:2.4.0-alpine`](#haproxy240-alpine)
-	[`haproxy:2.5-dev`](#haproxy25-dev)
-	[`haproxy:2.5-dev-alpine`](#haproxy25-dev-alpine)
-	[`haproxy:2.5-dev0`](#haproxy25-dev0)
-	[`haproxy:2.5-dev0-alpine`](#haproxy25-dev0-alpine)
-	[`haproxy:alpine`](#haproxyalpine)
-	[`haproxy:latest`](#haproxylatest)
-	[`haproxy:lts`](#haproxylts)
-	[`haproxy:lts-alpine`](#haproxylts-alpine)

## `haproxy:1.7`

```console
$ docker pull haproxy@sha256:c907961865fed8eb404ad26e4198dc9d7524a94172ef072e409afbff11c16118
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
$ docker pull haproxy@sha256:6cd59f93944285ca6351fea04ce732a4e316901834c389dfc8da73f5e9009884
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.5 MB (32541336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c047267f5d68ca463779e25e8bb179446b801d97b0aaa7f18727485df2f4402`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 07:10:16 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 07:16:36 GMT
ENV HAPROXY_VERSION=1.7.14
# Wed, 12 May 2021 07:16:36 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Wed, 12 May 2021 07:16:36 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Wed, 12 May 2021 07:17:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 07:17:27 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 07:17:27 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Wed, 12 May 2021 07:17:28 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 07:17:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 07:17:29 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a113359dddc15238d26b375f86574b596b4aee1263a9631a7384589c2a02f46`  
		Last Modified: Wed, 12 May 2021 07:18:16 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df03e50c708d3a5e8c928569266f6cdbcbfb440727dbba391676eab11ca1976d`  
		Last Modified: Wed, 12 May 2021 07:19:29 GMT  
		Size: 5.4 MB (5393450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef0307513f6a49cacd2e35122a505b64c2e522d061f0bc6a5c126ca2a135f59`  
		Last Modified: Wed, 12 May 2021 07:19:28 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df985c3c834696130d4495f7a5d2960b9fe597c88e4b0b5e1e162c1264d3a6f7`  
		Last Modified: Wed, 12 May 2021 07:19:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:bc5e6ea88874c23ccb51fc59fc02a46fb0cee70b05f3e2bf434a1f56c49db8c8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.9 MB (29901807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:332a59ad4a77387b974fcba0f0e75ccf21974180e638146387c0780aaff84a76`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:55:35 GMT
ADD file:241925c5ca73c99d58f93bc78d7c5bfb6f8b280201a9b55ade45ba0cc054c31d in / 
# Wed, 12 May 2021 00:55:46 GMT
CMD ["bash"]
# Wed, 12 May 2021 02:01:24 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 02:08:05 GMT
ENV HAPROXY_VERSION=1.7.14
# Wed, 12 May 2021 02:08:06 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Wed, 12 May 2021 02:08:07 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Wed, 12 May 2021 02:09:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 02:09:01 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 02:09:04 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Wed, 12 May 2021 02:09:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 02:09:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 02:09:11 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:48885a8e20b16cb3bb9d2c3aafc7f040d8609844f69ca8482c42b4829d01b6da`  
		Last Modified: Wed, 12 May 2021 01:10:24 GMT  
		Size: 24.9 MB (24879601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e012f5248a53449f692d1fe91241d026aa60efe5a3dc3f04add4638989918d2a`  
		Last Modified: Wed, 12 May 2021 02:09:37 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b6c9d2f9f2fafd6f415d31dbf4f0117415b8219299be0102b9d224a4b78899e`  
		Last Modified: Wed, 12 May 2021 02:10:24 GMT  
		Size: 5.0 MB (5020236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c048f52ddf32acf5cf02f7aa08668a24a8e4acb0ed04c2113ee8934b2bdf568`  
		Last Modified: Wed, 12 May 2021 02:10:23 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b26c17c5eaa5658e57b3379930fbbc0e935a92ade04461724d63688316f40a`  
		Last Modified: Wed, 12 May 2021 02:10:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:f533bb1ff5188db693cf9dd950768ea42fe37df7ba967f07b6f3c8006482cba1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.6 MB (27640414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:815186c82a18dd6dfda95f8640e42f298c73864936fe2d5d96a7725329763af7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:03:14 GMT
ADD file:94bf2394dc26abd9f028c2933057a8673c8562e58ec4a0f51bb9bde0a5e4dee0 in / 
# Wed, 12 May 2021 01:03:32 GMT
CMD ["bash"]
# Wed, 16 Jun 2021 12:48:11 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 13:05:25 GMT
ENV HAPROXY_VERSION=1.7.14
# Wed, 16 Jun 2021 13:05:25 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Wed, 16 Jun 2021 13:05:26 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Wed, 16 Jun 2021 13:06:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 16 Jun 2021 13:06:13 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 13:06:13 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Wed, 16 Jun 2021 13:06:14 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 16 Jun 2021 13:06:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 13:06:15 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:3035777cd90a3389593bc49a7b39b6f67f9f2679f4e04cc59515f4d5f83ad818`  
		Last Modified: Wed, 12 May 2021 01:19:13 GMT  
		Size: 22.7 MB (22746266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a03e197445bdc67b19867d9e201ef8f2078017e5ad57773c364b31ba9786e0e`  
		Last Modified: Wed, 16 Jun 2021 13:08:37 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:079f3d51d723c90e44d1626ec749c5138ba42a5005f274b9dd13140af7e8d6f7`  
		Last Modified: Wed, 16 Jun 2021 13:11:59 GMT  
		Size: 4.9 MB (4892172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5139f02a36cebaba4f1e0c6b19f8b76b2242c7e4ed18ac12768986d9409f2da0`  
		Last Modified: Wed, 16 Jun 2021 13:11:57 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e5402357d8118975af143599d1ad12a61156417a6567c9bb24d38381dc632a`  
		Last Modified: Wed, 16 Jun 2021 13:11:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:c3980fdaed041ee3bc80711cb5732b87f4d2413be95b69ecdc9cd97d1aaaae33
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31194261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78c326cc529a842fb9a46c39b95f6b651969dcc9a15cfe14678d74f3fd207b62`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:52:19 GMT
ADD file:91ba1791cab3ad29a1469d1e78f21f4c0b5d3d30598683b7104980604c318854 in / 
# Wed, 12 May 2021 00:52:34 GMT
CMD ["bash"]
# Wed, 16 Jun 2021 00:32:29 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 00:42:38 GMT
ENV HAPROXY_VERSION=1.7.14
# Wed, 16 Jun 2021 00:42:38 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Wed, 16 Jun 2021 00:42:38 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Wed, 16 Jun 2021 00:43:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 16 Jun 2021 00:43:03 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 00:43:03 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Wed, 16 Jun 2021 00:43:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 16 Jun 2021 00:43:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 00:43:05 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:fcad0c936ea5c12e1c8c4edb81a97c0cde04ee71e7067ee3b246474cf1854d7a`  
		Last Modified: Wed, 12 May 2021 01:02:02 GMT  
		Size: 25.9 MB (25911250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48fc449d8b117694f567c81827185f03f8e4fa5c56b0b6626bb4374515d222c3`  
		Last Modified: Wed, 16 Jun 2021 00:44:41 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f933aa9d32a51232efec6c3d35a50378432f4a70353633173b29d7667b38c4ac`  
		Last Modified: Wed, 16 Jun 2021 00:47:32 GMT  
		Size: 5.3 MB (5281036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b459d9d5876c6aaa1ea430b1d27748331def85b6ddefa4235f7567a804392359`  
		Last Modified: Wed, 16 Jun 2021 00:47:31 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ce0f01f12afd6715a0b35c244475bfc9af060a0d113250677ad62d183478cb7`  
		Last Modified: Wed, 16 Jun 2021 00:47:31 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7` - linux; 386

```console
$ docker pull haproxy@sha256:20dbd0f1d0f1320bd12d5ec0ff8f7c210bba90cc78df364fd972ee4e9a70215d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.1 MB (33121125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61ea7e6f531898142a40baf18e585511debea156e2a24a09516c99b819dbab59`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:39:52 GMT
ADD file:62173a7456d614031a7b20be741983644d9723c734eee663b099ad6b47af7b35 in / 
# Wed, 12 May 2021 00:39:53 GMT
CMD ["bash"]
# Wed, 12 May 2021 05:59:03 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 06:08:32 GMT
ENV HAPROXY_VERSION=1.7.14
# Wed, 12 May 2021 06:08:32 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Wed, 12 May 2021 06:08:33 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Wed, 12 May 2021 06:09:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 06:09:20 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 06:09:21 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Wed, 12 May 2021 06:09:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 06:09:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 06:09:24 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:9b548256784c8e079e5953ec08bd26ce8cbaed0d606a5d350b4bcd12710d2192`  
		Last Modified: Wed, 12 May 2021 00:46:39 GMT  
		Size: 27.8 MB (27795074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05508dc89a5d9449eccbd1b8bf3910253f410f4654f50f119641aa3b5dc3e5c6`  
		Last Modified: Wed, 12 May 2021 06:11:24 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a4a4b79c960ec829a77fd2bc860c23a5f2fb266e5ee0d377149181bcb82355`  
		Last Modified: Wed, 12 May 2021 06:13:13 GMT  
		Size: 5.3 MB (5324079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53fe521c247b1c8e0f2aeb9c1800b2c5f21a01795a283b95a8514e1b1e255539`  
		Last Modified: Wed, 12 May 2021 06:13:11 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b15c901021ec8030c9aca4655ff75b8031e18ef34b3327be8bdf174922cc68c`  
		Last Modified: Wed, 12 May 2021 06:13:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7` - linux; mips64le

```console
$ docker pull haproxy@sha256:f795a60ea78df2364a2e4984ceeff877d3baeff09d977f52fdd54eba48cc79ec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.8 MB (30842663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53c6d49c25835b8fb47b2b625ac95fbc4754fec5069099719f7295f2879ad4e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:09:45 GMT
ADD file:867397d3fb44b3b936a4ff02bbc3a1b760fb6865b5a85efab82fff224f704241 in / 
# Wed, 12 May 2021 01:09:46 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:37:27 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 01:49:37 GMT
ENV HAPROXY_VERSION=1.7.14
# Wed, 12 May 2021 01:49:37 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Wed, 12 May 2021 01:49:37 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Wed, 12 May 2021 01:51:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 01:51:02 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 01:51:03 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Wed, 12 May 2021 01:51:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 01:51:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 01:51:05 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:09564b0ac149fb24b77cbc75ce6fa5d9ba61bd7c99d11b42bd8339c3bb28e557`  
		Last Modified: Wed, 12 May 2021 01:16:36 GMT  
		Size: 25.8 MB (25812884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18fb24fa0e81746ee8c86b23e726e84be12b3f40b71800e0be7e202dd3e3eae3`  
		Last Modified: Wed, 12 May 2021 01:51:31 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab8418236221578f142bec8675b38b3c4231d94bbdbf70e973838cfc5033f8c5`  
		Last Modified: Wed, 12 May 2021 01:53:06 GMT  
		Size: 5.0 MB (5027808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fdc42c55f03fc902d4f2b0259468563900ee24506ca277235f410e81db03a70`  
		Last Modified: Wed, 12 May 2021 01:53:02 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70813dd08cabf2555ad8034c88a5360ff0ebbd5cc46681f75bbe4daf094e687d`  
		Last Modified: Wed, 12 May 2021 01:53:02 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7` - linux; ppc64le

```console
$ docker pull haproxy@sha256:89653da01efb9339f660089a18e081bd057adb9bac871d24a41febd0295c4f75
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36265334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0554d96098b8e9739c1e4794c2b0333c7f141c0598e04802e44fc3d4508897e6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:34:56 GMT
ADD file:3b8146cdc3649d94ad49435c94a21d700ed612ab90f010dcf8b22951b1804d34 in / 
# Wed, 12 May 2021 01:35:02 GMT
CMD ["bash"]
# Wed, 12 May 2021 06:07:29 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 06:46:02 GMT
ENV HAPROXY_VERSION=1.7.14
# Wed, 12 May 2021 06:46:11 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Wed, 12 May 2021 06:46:17 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Wed, 12 May 2021 06:55:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 06:55:51 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 06:55:58 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Wed, 12 May 2021 06:56:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 06:56:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 06:56:36 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:f8b445753f60bad25326d018945455601e4a65f124e956dec95c569816f21493`  
		Last Modified: Wed, 12 May 2021 01:44:19 GMT  
		Size: 30.6 MB (30552394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cfafb398e88c2b64b9fb82254775d63718baad006543dee4e7c370a09a23be9`  
		Last Modified: Wed, 12 May 2021 06:57:45 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11971eac7e1e481251943b3c552f4911136a49e1b4a847378af195c8f702bbaf`  
		Last Modified: Wed, 12 May 2021 06:58:58 GMT  
		Size: 5.7 MB (5710966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:630b15aa63cce85871a16dc1fb1cdf6406a44f8e3682614c6ee3d30f61c419bb`  
		Last Modified: Wed, 12 May 2021 06:58:57 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d711c5d8db4f4828bb5beff00055d4829bcce61815e41065bd5120b6a57062b5`  
		Last Modified: Wed, 12 May 2021 06:58:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7` - linux; s390x

```console
$ docker pull haproxy@sha256:118653410d0bed5a360bfa46f6b2edfb1024c8efd08ce9b60a90914ca8c79d42
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.9 MB (30891438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af44673de70fffb500a7ccb298770cbb81b30b05e1529b478e315875dde2ccb9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:43:38 GMT
ADD file:77af21d863769b75a5f055b85b2c9d6e878f9d77a4122397ae8dde6b69e945c6 in / 
# Wed, 12 May 2021 00:43:42 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:53:39 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 02:02:29 GMT
ENV HAPROXY_VERSION=1.7.14
# Wed, 12 May 2021 02:02:30 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Wed, 12 May 2021 02:02:31 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Wed, 12 May 2021 02:03:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 02:03:44 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 02:03:44 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Wed, 12 May 2021 02:03:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 02:03:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 02:03:48 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:ba4b99e0e723623b64d4ecb8d74102998d32137ea9bcc88b15fd2e4e34b38df9`  
		Last Modified: Wed, 12 May 2021 00:48:03 GMT  
		Size: 25.8 MB (25760171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f6911826fde538e80c00f0d90920d0d7d0a78db315f0bde1ee65726f99f6747`  
		Last Modified: Wed, 12 May 2021 02:04:41 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3825062d94e7ed1004fdf4d867e9d9d8601a126a49dc53cc7015a19931234553`  
		Last Modified: Wed, 12 May 2021 02:05:31 GMT  
		Size: 5.1 MB (5129295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895ddd30e13c0c1ce2c1704e70ce63214f57b353f96ca767d70b923c7e753bb4`  
		Last Modified: Wed, 12 May 2021 02:05:31 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1e47f8cdefd6f93e0376158814d5dc53f3443f15fbc58d2523f8ce27403724`  
		Last Modified: Wed, 12 May 2021 02:05:30 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:1.7-alpine`

```console
$ docker pull haproxy@sha256:9249b4a75142db9df142367f4bd2d88b75f57d0f9ef0d98c0d79ec3bced2fa8e
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
$ docker pull haproxy@sha256:10b8baccd68a870b7304a4bd92f6312ceaac517f3e9d284c6f98487812db7349
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 MB (3326549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34e7ec4226f06fe8e1afd92292b7ef1da3774af81fd40cd5d018a844ea7c9ff1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:41 GMT
ADD file:82fa6a18d24e3f535c9061d2e111d63fe6d8a27710bb34a17b326e605ff478be in / 
# Tue, 15 Jun 2021 22:57:41 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 11:13:31 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 11:13:31 GMT
ENV HAPROXY_VERSION=1.7.14
# Wed, 16 Jun 2021 11:13:31 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Wed, 16 Jun 2021 11:13:31 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Wed, 16 Jun 2021 11:13:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		CFLAGS+="-Wno-address-of-packed-member" 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 16 Jun 2021 11:13:43 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 11:13:43 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Wed, 16 Jun 2021 11:13:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 16 Jun 2021 11:13:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 11:13:44 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:b452d2916bdfd021add56f1eda6bdea35400671ef07b38316ef82fce92a88fee`  
		Last Modified: Wed, 14 Apr 2021 18:50:38 GMT  
		Size: 2.6 MB (2605253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1e514505f8f70d7f388fcca4beaa56511e29ca28e3019073887559dafe4683c`  
		Last Modified: Wed, 16 Jun 2021 11:16:21 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7547a858ab152e8d5bd1dd03f4b096f91d8542bef08874f9dbd4d55ad15ac4e9`  
		Last Modified: Wed, 16 Jun 2021 11:16:22 GMT  
		Size: 719.5 KB (719516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b68e070569e1649fa58c3802f9db39e5b66c5a3b687c1de5083747547046cb`  
		Last Modified: Wed, 16 Jun 2021 11:16:21 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c0840b326206d641b405ac171ca563f3320279daf478087f85e86244acab29`  
		Last Modified: Wed, 16 Jun 2021 11:16:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:f41597b4961a1169e1042d45eda7f678050f9255bc1a99ec40340bd0d3df8e03
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3087801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62dff852f8d7bc9a7f4e1d9354632afce5d8fed21ee3a70bcecf188f8c6a9968`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:24 GMT
ADD file:d844cc7b5e00fb62be39d903a2fb4a08f700e75112c8eef1f31101e846ed010d in / 
# Tue, 15 Jun 2021 23:15:25 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 13:06:28 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 13:06:28 GMT
ENV HAPROXY_VERSION=1.7.14
# Wed, 16 Jun 2021 13:06:29 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Wed, 16 Jun 2021 13:06:29 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Wed, 16 Jun 2021 13:06:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		CFLAGS+="-Wno-address-of-packed-member" 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 16 Jun 2021 13:06:48 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 13:06:49 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Wed, 16 Jun 2021 13:06:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 16 Jun 2021 13:06:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 13:06:51 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:420c7481a3a76d5d12df768d2745ddbe40357df0af780c756a5a7d1f2a43d288`  
		Last Modified: Wed, 14 Apr 2021 18:58:46 GMT  
		Size: 2.4 MB (2409178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:622ba2a5a8938fdcaf23c862a1a63fee54f149e93c421d70aff36e2d0b8a38d1`  
		Last Modified: Wed, 16 Jun 2021 13:12:12 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a38291baf3eb2ceae00692b5d084ffec81fea518676eb5b106077102a8d02e`  
		Last Modified: Wed, 16 Jun 2021 13:12:12 GMT  
		Size: 676.8 KB (676839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb45f8bfea3c28ed90738a0958a0319ac10103f242908f18708391ce5a0e5d81`  
		Last Modified: Wed, 16 Jun 2021 13:12:12 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c104d4df72499c9c16d034b44ee9183213341283c4f92354107220e104e9eca9`  
		Last Modified: Wed, 16 Jun 2021 13:12:12 GMT  
		Size: 121.0 B  
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
$ docker pull haproxy@sha256:c907961865fed8eb404ad26e4198dc9d7524a94172ef072e409afbff11c16118
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
$ docker pull haproxy@sha256:6cd59f93944285ca6351fea04ce732a4e316901834c389dfc8da73f5e9009884
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.5 MB (32541336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c047267f5d68ca463779e25e8bb179446b801d97b0aaa7f18727485df2f4402`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 07:10:16 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 07:16:36 GMT
ENV HAPROXY_VERSION=1.7.14
# Wed, 12 May 2021 07:16:36 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Wed, 12 May 2021 07:16:36 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Wed, 12 May 2021 07:17:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 07:17:27 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 07:17:27 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Wed, 12 May 2021 07:17:28 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 07:17:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 07:17:29 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a113359dddc15238d26b375f86574b596b4aee1263a9631a7384589c2a02f46`  
		Last Modified: Wed, 12 May 2021 07:18:16 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df03e50c708d3a5e8c928569266f6cdbcbfb440727dbba391676eab11ca1976d`  
		Last Modified: Wed, 12 May 2021 07:19:29 GMT  
		Size: 5.4 MB (5393450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef0307513f6a49cacd2e35122a505b64c2e522d061f0bc6a5c126ca2a135f59`  
		Last Modified: Wed, 12 May 2021 07:19:28 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df985c3c834696130d4495f7a5d2960b9fe597c88e4b0b5e1e162c1264d3a6f7`  
		Last Modified: Wed, 12 May 2021 07:19:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7.14` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:bc5e6ea88874c23ccb51fc59fc02a46fb0cee70b05f3e2bf434a1f56c49db8c8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.9 MB (29901807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:332a59ad4a77387b974fcba0f0e75ccf21974180e638146387c0780aaff84a76`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:55:35 GMT
ADD file:241925c5ca73c99d58f93bc78d7c5bfb6f8b280201a9b55ade45ba0cc054c31d in / 
# Wed, 12 May 2021 00:55:46 GMT
CMD ["bash"]
# Wed, 12 May 2021 02:01:24 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 02:08:05 GMT
ENV HAPROXY_VERSION=1.7.14
# Wed, 12 May 2021 02:08:06 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Wed, 12 May 2021 02:08:07 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Wed, 12 May 2021 02:09:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 02:09:01 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 02:09:04 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Wed, 12 May 2021 02:09:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 02:09:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 02:09:11 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:48885a8e20b16cb3bb9d2c3aafc7f040d8609844f69ca8482c42b4829d01b6da`  
		Last Modified: Wed, 12 May 2021 01:10:24 GMT  
		Size: 24.9 MB (24879601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e012f5248a53449f692d1fe91241d026aa60efe5a3dc3f04add4638989918d2a`  
		Last Modified: Wed, 12 May 2021 02:09:37 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b6c9d2f9f2fafd6f415d31dbf4f0117415b8219299be0102b9d224a4b78899e`  
		Last Modified: Wed, 12 May 2021 02:10:24 GMT  
		Size: 5.0 MB (5020236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c048f52ddf32acf5cf02f7aa08668a24a8e4acb0ed04c2113ee8934b2bdf568`  
		Last Modified: Wed, 12 May 2021 02:10:23 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b26c17c5eaa5658e57b3379930fbbc0e935a92ade04461724d63688316f40a`  
		Last Modified: Wed, 12 May 2021 02:10:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7.14` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:f533bb1ff5188db693cf9dd950768ea42fe37df7ba967f07b6f3c8006482cba1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.6 MB (27640414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:815186c82a18dd6dfda95f8640e42f298c73864936fe2d5d96a7725329763af7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:03:14 GMT
ADD file:94bf2394dc26abd9f028c2933057a8673c8562e58ec4a0f51bb9bde0a5e4dee0 in / 
# Wed, 12 May 2021 01:03:32 GMT
CMD ["bash"]
# Wed, 16 Jun 2021 12:48:11 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 13:05:25 GMT
ENV HAPROXY_VERSION=1.7.14
# Wed, 16 Jun 2021 13:05:25 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Wed, 16 Jun 2021 13:05:26 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Wed, 16 Jun 2021 13:06:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 16 Jun 2021 13:06:13 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 13:06:13 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Wed, 16 Jun 2021 13:06:14 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 16 Jun 2021 13:06:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 13:06:15 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:3035777cd90a3389593bc49a7b39b6f67f9f2679f4e04cc59515f4d5f83ad818`  
		Last Modified: Wed, 12 May 2021 01:19:13 GMT  
		Size: 22.7 MB (22746266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a03e197445bdc67b19867d9e201ef8f2078017e5ad57773c364b31ba9786e0e`  
		Last Modified: Wed, 16 Jun 2021 13:08:37 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:079f3d51d723c90e44d1626ec749c5138ba42a5005f274b9dd13140af7e8d6f7`  
		Last Modified: Wed, 16 Jun 2021 13:11:59 GMT  
		Size: 4.9 MB (4892172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5139f02a36cebaba4f1e0c6b19f8b76b2242c7e4ed18ac12768986d9409f2da0`  
		Last Modified: Wed, 16 Jun 2021 13:11:57 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e5402357d8118975af143599d1ad12a61156417a6567c9bb24d38381dc632a`  
		Last Modified: Wed, 16 Jun 2021 13:11:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7.14` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:c3980fdaed041ee3bc80711cb5732b87f4d2413be95b69ecdc9cd97d1aaaae33
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31194261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78c326cc529a842fb9a46c39b95f6b651969dcc9a15cfe14678d74f3fd207b62`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:52:19 GMT
ADD file:91ba1791cab3ad29a1469d1e78f21f4c0b5d3d30598683b7104980604c318854 in / 
# Wed, 12 May 2021 00:52:34 GMT
CMD ["bash"]
# Wed, 16 Jun 2021 00:32:29 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 00:42:38 GMT
ENV HAPROXY_VERSION=1.7.14
# Wed, 16 Jun 2021 00:42:38 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Wed, 16 Jun 2021 00:42:38 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Wed, 16 Jun 2021 00:43:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 16 Jun 2021 00:43:03 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 00:43:03 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Wed, 16 Jun 2021 00:43:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 16 Jun 2021 00:43:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 00:43:05 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:fcad0c936ea5c12e1c8c4edb81a97c0cde04ee71e7067ee3b246474cf1854d7a`  
		Last Modified: Wed, 12 May 2021 01:02:02 GMT  
		Size: 25.9 MB (25911250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48fc449d8b117694f567c81827185f03f8e4fa5c56b0b6626bb4374515d222c3`  
		Last Modified: Wed, 16 Jun 2021 00:44:41 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f933aa9d32a51232efec6c3d35a50378432f4a70353633173b29d7667b38c4ac`  
		Last Modified: Wed, 16 Jun 2021 00:47:32 GMT  
		Size: 5.3 MB (5281036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b459d9d5876c6aaa1ea430b1d27748331def85b6ddefa4235f7567a804392359`  
		Last Modified: Wed, 16 Jun 2021 00:47:31 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ce0f01f12afd6715a0b35c244475bfc9af060a0d113250677ad62d183478cb7`  
		Last Modified: Wed, 16 Jun 2021 00:47:31 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7.14` - linux; 386

```console
$ docker pull haproxy@sha256:20dbd0f1d0f1320bd12d5ec0ff8f7c210bba90cc78df364fd972ee4e9a70215d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.1 MB (33121125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61ea7e6f531898142a40baf18e585511debea156e2a24a09516c99b819dbab59`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:39:52 GMT
ADD file:62173a7456d614031a7b20be741983644d9723c734eee663b099ad6b47af7b35 in / 
# Wed, 12 May 2021 00:39:53 GMT
CMD ["bash"]
# Wed, 12 May 2021 05:59:03 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 06:08:32 GMT
ENV HAPROXY_VERSION=1.7.14
# Wed, 12 May 2021 06:08:32 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Wed, 12 May 2021 06:08:33 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Wed, 12 May 2021 06:09:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 06:09:20 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 06:09:21 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Wed, 12 May 2021 06:09:23 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 06:09:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 06:09:24 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:9b548256784c8e079e5953ec08bd26ce8cbaed0d606a5d350b4bcd12710d2192`  
		Last Modified: Wed, 12 May 2021 00:46:39 GMT  
		Size: 27.8 MB (27795074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05508dc89a5d9449eccbd1b8bf3910253f410f4654f50f119641aa3b5dc3e5c6`  
		Last Modified: Wed, 12 May 2021 06:11:24 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a4a4b79c960ec829a77fd2bc860c23a5f2fb266e5ee0d377149181bcb82355`  
		Last Modified: Wed, 12 May 2021 06:13:13 GMT  
		Size: 5.3 MB (5324079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53fe521c247b1c8e0f2aeb9c1800b2c5f21a01795a283b95a8514e1b1e255539`  
		Last Modified: Wed, 12 May 2021 06:13:11 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b15c901021ec8030c9aca4655ff75b8031e18ef34b3327be8bdf174922cc68c`  
		Last Modified: Wed, 12 May 2021 06:13:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7.14` - linux; mips64le

```console
$ docker pull haproxy@sha256:f795a60ea78df2364a2e4984ceeff877d3baeff09d977f52fdd54eba48cc79ec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.8 MB (30842663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53c6d49c25835b8fb47b2b625ac95fbc4754fec5069099719f7295f2879ad4e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:09:45 GMT
ADD file:867397d3fb44b3b936a4ff02bbc3a1b760fb6865b5a85efab82fff224f704241 in / 
# Wed, 12 May 2021 01:09:46 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:37:27 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 01:49:37 GMT
ENV HAPROXY_VERSION=1.7.14
# Wed, 12 May 2021 01:49:37 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Wed, 12 May 2021 01:49:37 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Wed, 12 May 2021 01:51:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 01:51:02 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 01:51:03 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Wed, 12 May 2021 01:51:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 01:51:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 01:51:05 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:09564b0ac149fb24b77cbc75ce6fa5d9ba61bd7c99d11b42bd8339c3bb28e557`  
		Last Modified: Wed, 12 May 2021 01:16:36 GMT  
		Size: 25.8 MB (25812884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18fb24fa0e81746ee8c86b23e726e84be12b3f40b71800e0be7e202dd3e3eae3`  
		Last Modified: Wed, 12 May 2021 01:51:31 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab8418236221578f142bec8675b38b3c4231d94bbdbf70e973838cfc5033f8c5`  
		Last Modified: Wed, 12 May 2021 01:53:06 GMT  
		Size: 5.0 MB (5027808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fdc42c55f03fc902d4f2b0259468563900ee24506ca277235f410e81db03a70`  
		Last Modified: Wed, 12 May 2021 01:53:02 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70813dd08cabf2555ad8034c88a5360ff0ebbd5cc46681f75bbe4daf094e687d`  
		Last Modified: Wed, 12 May 2021 01:53:02 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7.14` - linux; ppc64le

```console
$ docker pull haproxy@sha256:89653da01efb9339f660089a18e081bd057adb9bac871d24a41febd0295c4f75
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36265334 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0554d96098b8e9739c1e4794c2b0333c7f141c0598e04802e44fc3d4508897e6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:34:56 GMT
ADD file:3b8146cdc3649d94ad49435c94a21d700ed612ab90f010dcf8b22951b1804d34 in / 
# Wed, 12 May 2021 01:35:02 GMT
CMD ["bash"]
# Wed, 12 May 2021 06:07:29 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 06:46:02 GMT
ENV HAPROXY_VERSION=1.7.14
# Wed, 12 May 2021 06:46:11 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Wed, 12 May 2021 06:46:17 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Wed, 12 May 2021 06:55:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 06:55:51 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 06:55:58 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Wed, 12 May 2021 06:56:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 06:56:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 06:56:36 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:f8b445753f60bad25326d018945455601e4a65f124e956dec95c569816f21493`  
		Last Modified: Wed, 12 May 2021 01:44:19 GMT  
		Size: 30.6 MB (30552394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cfafb398e88c2b64b9fb82254775d63718baad006543dee4e7c370a09a23be9`  
		Last Modified: Wed, 12 May 2021 06:57:45 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11971eac7e1e481251943b3c552f4911136a49e1b4a847378af195c8f702bbaf`  
		Last Modified: Wed, 12 May 2021 06:58:58 GMT  
		Size: 5.7 MB (5710966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:630b15aa63cce85871a16dc1fb1cdf6406a44f8e3682614c6ee3d30f61c419bb`  
		Last Modified: Wed, 12 May 2021 06:58:57 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d711c5d8db4f4828bb5beff00055d4829bcce61815e41065bd5120b6a57062b5`  
		Last Modified: Wed, 12 May 2021 06:58:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7.14` - linux; s390x

```console
$ docker pull haproxy@sha256:118653410d0bed5a360bfa46f6b2edfb1024c8efd08ce9b60a90914ca8c79d42
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.9 MB (30891438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af44673de70fffb500a7ccb298770cbb81b30b05e1529b478e315875dde2ccb9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:43:38 GMT
ADD file:77af21d863769b75a5f055b85b2c9d6e878f9d77a4122397ae8dde6b69e945c6 in / 
# Wed, 12 May 2021 00:43:42 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:53:39 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 02:02:29 GMT
ENV HAPROXY_VERSION=1.7.14
# Wed, 12 May 2021 02:02:30 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Wed, 12 May 2021 02:02:31 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Wed, 12 May 2021 02:03:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 02:03:44 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 02:03:44 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Wed, 12 May 2021 02:03:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 02:03:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 02:03:48 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:ba4b99e0e723623b64d4ecb8d74102998d32137ea9bcc88b15fd2e4e34b38df9`  
		Last Modified: Wed, 12 May 2021 00:48:03 GMT  
		Size: 25.8 MB (25760171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f6911826fde538e80c00f0d90920d0d7d0a78db315f0bde1ee65726f99f6747`  
		Last Modified: Wed, 12 May 2021 02:04:41 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3825062d94e7ed1004fdf4d867e9d9d8601a126a49dc53cc7015a19931234553`  
		Last Modified: Wed, 12 May 2021 02:05:31 GMT  
		Size: 5.1 MB (5129295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895ddd30e13c0c1ce2c1704e70ce63214f57b353f96ca767d70b923c7e753bb4`  
		Last Modified: Wed, 12 May 2021 02:05:31 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1e47f8cdefd6f93e0376158814d5dc53f3443f15fbc58d2523f8ce27403724`  
		Last Modified: Wed, 12 May 2021 02:05:30 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:1.7.14-alpine`

```console
$ docker pull haproxy@sha256:9249b4a75142db9df142367f4bd2d88b75f57d0f9ef0d98c0d79ec3bced2fa8e
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
$ docker pull haproxy@sha256:10b8baccd68a870b7304a4bd92f6312ceaac517f3e9d284c6f98487812db7349
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 MB (3326549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34e7ec4226f06fe8e1afd92292b7ef1da3774af81fd40cd5d018a844ea7c9ff1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:41 GMT
ADD file:82fa6a18d24e3f535c9061d2e111d63fe6d8a27710bb34a17b326e605ff478be in / 
# Tue, 15 Jun 2021 22:57:41 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 11:13:31 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 11:13:31 GMT
ENV HAPROXY_VERSION=1.7.14
# Wed, 16 Jun 2021 11:13:31 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Wed, 16 Jun 2021 11:13:31 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Wed, 16 Jun 2021 11:13:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		CFLAGS+="-Wno-address-of-packed-member" 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 16 Jun 2021 11:13:43 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 11:13:43 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Wed, 16 Jun 2021 11:13:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 16 Jun 2021 11:13:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 11:13:44 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:b452d2916bdfd021add56f1eda6bdea35400671ef07b38316ef82fce92a88fee`  
		Last Modified: Wed, 14 Apr 2021 18:50:38 GMT  
		Size: 2.6 MB (2605253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1e514505f8f70d7f388fcca4beaa56511e29ca28e3019073887559dafe4683c`  
		Last Modified: Wed, 16 Jun 2021 11:16:21 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7547a858ab152e8d5bd1dd03f4b096f91d8542bef08874f9dbd4d55ad15ac4e9`  
		Last Modified: Wed, 16 Jun 2021 11:16:22 GMT  
		Size: 719.5 KB (719516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b68e070569e1649fa58c3802f9db39e5b66c5a3b687c1de5083747547046cb`  
		Last Modified: Wed, 16 Jun 2021 11:16:21 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c0840b326206d641b405ac171ca563f3320279daf478087f85e86244acab29`  
		Last Modified: Wed, 16 Jun 2021 11:16:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.7.14-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:f41597b4961a1169e1042d45eda7f678050f9255bc1a99ec40340bd0d3df8e03
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3087801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62dff852f8d7bc9a7f4e1d9354632afce5d8fed21ee3a70bcecf188f8c6a9968`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:24 GMT
ADD file:d844cc7b5e00fb62be39d903a2fb4a08f700e75112c8eef1f31101e846ed010d in / 
# Tue, 15 Jun 2021 23:15:25 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 13:06:28 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 13:06:28 GMT
ENV HAPROXY_VERSION=1.7.14
# Wed, 16 Jun 2021 13:06:29 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.7/src/haproxy-1.7.14.tar.gz
# Wed, 16 Jun 2021 13:06:29 GMT
ENV HAPROXY_SHA256=1f9fb6c5a342803037a622c7dd04702b0d010a88b5c3922cd3da71a34f3377a4
# Wed, 16 Jun 2021 13:06:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		CFLAGS+="-Wno-address-of-packed-member" 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 16 Jun 2021 13:06:48 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 13:06:49 GMT
COPY file:9a05f2c8b43e780abf69d813f7c45613cced5481a65611bf8127c6f222dff4e3 in /usr/local/bin/ 
# Wed, 16 Jun 2021 13:06:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 16 Jun 2021 13:06:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 13:06:51 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:420c7481a3a76d5d12df768d2745ddbe40357df0af780c756a5a7d1f2a43d288`  
		Last Modified: Wed, 14 Apr 2021 18:58:46 GMT  
		Size: 2.4 MB (2409178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:622ba2a5a8938fdcaf23c862a1a63fee54f149e93c421d70aff36e2d0b8a38d1`  
		Last Modified: Wed, 16 Jun 2021 13:12:12 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a38291baf3eb2ceae00692b5d084ffec81fea518676eb5b106077102a8d02e`  
		Last Modified: Wed, 16 Jun 2021 13:12:12 GMT  
		Size: 676.8 KB (676839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb45f8bfea3c28ed90738a0958a0319ac10103f242908f18708391ce5a0e5d81`  
		Last Modified: Wed, 16 Jun 2021 13:12:12 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c104d4df72499c9c16d034b44ee9183213341283c4f92354107220e104e9eca9`  
		Last Modified: Wed, 16 Jun 2021 13:12:12 GMT  
		Size: 121.0 B  
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
$ docker pull haproxy@sha256:3687b0945509ed429031b71ce9baaf51ac0f395c98b1111e0fd5b224aa2281ea
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
$ docker pull haproxy@sha256:64d45752aae0bb3a1f453c5bf8784cc2584eec03a71a88c26908d9874a59ce18
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33800155 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ceb49d4303b385ae4ec7f99f331815d7dc5ff4b5e19b42505434d40973ac0bd8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 07:10:16 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 07:15:31 GMT
ENV HAPROXY_VERSION=1.8.30
# Wed, 12 May 2021 07:15:31 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Wed, 12 May 2021 07:15:31 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Wed, 12 May 2021 07:16:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 07:16:23 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 07:16:23 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 12 May 2021 07:16:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 07:16:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 07:16:26 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a113359dddc15238d26b375f86574b596b4aee1263a9631a7384589c2a02f46`  
		Last Modified: Wed, 12 May 2021 07:18:16 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19eaa5d34e4ee89879a0294969800a35f9914055323ddeb939573f963a1fa4a4`  
		Last Modified: Wed, 12 May 2021 07:19:16 GMT  
		Size: 6.7 MB (6652289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceb7dbac58865e63e8aae0d3e7563353941a8d9ae939fb1c120ffcdd651d271f`  
		Last Modified: Wed, 12 May 2021 07:19:14 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c67d5f37ab678c0b58a85431b4a68427a2aafe61bda9670fab9cfadce74e6c7`  
		Last Modified: Wed, 12 May 2021 07:19:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:033dc007b9fd1b71bb79c6426c292a4384b8d9a76a45e844f915d0a891494721
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.1 MB (31112790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50929a1753a1ebffbf3f1495998b098a1ffb15fe95860657f9ea8bcb6f38a5db`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:55:35 GMT
ADD file:241925c5ca73c99d58f93bc78d7c5bfb6f8b280201a9b55ade45ba0cc054c31d in / 
# Wed, 12 May 2021 00:55:46 GMT
CMD ["bash"]
# Wed, 12 May 2021 02:01:24 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 02:06:57 GMT
ENV HAPROXY_VERSION=1.8.30
# Wed, 12 May 2021 02:06:57 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Wed, 12 May 2021 02:06:58 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Wed, 12 May 2021 02:07:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 02:07:49 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 02:07:50 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 12 May 2021 02:07:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 02:07:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 02:07:58 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:48885a8e20b16cb3bb9d2c3aafc7f040d8609844f69ca8482c42b4829d01b6da`  
		Last Modified: Wed, 12 May 2021 01:10:24 GMT  
		Size: 24.9 MB (24879601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e012f5248a53449f692d1fe91241d026aa60efe5a3dc3f04add4638989918d2a`  
		Last Modified: Wed, 12 May 2021 02:09:37 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21338fd0bfb55990c2c424c288a91c3b4ff525c954f212bfa5df546c9a26ee22`  
		Last Modified: Wed, 12 May 2021 02:10:17 GMT  
		Size: 6.2 MB (6231244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1d13df6c276b46a99a45c541c542e2d3f82086a28b44db2a26b0a2bf796830`  
		Last Modified: Wed, 12 May 2021 02:10:15 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4ac3b2830e321ef4a46bef81b407d9ac6587d79e93cf2f7b4de18fb14aee569`  
		Last Modified: Wed, 12 May 2021 02:10:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:111bd77421801aaa477bd0c2907469b642f166addc73024189356acfb902c4a5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.8 MB (28819032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43a1a120e2bc22fea4c4093de642801bf5f4455253ff841fce789dc51248bce3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:03:14 GMT
ADD file:94bf2394dc26abd9f028c2933057a8673c8562e58ec4a0f51bb9bde0a5e4dee0 in / 
# Wed, 12 May 2021 01:03:32 GMT
CMD ["bash"]
# Wed, 16 Jun 2021 12:48:11 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 13:02:56 GMT
ENV HAPROXY_VERSION=1.8.30
# Wed, 16 Jun 2021 13:02:57 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Wed, 16 Jun 2021 13:02:57 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Wed, 16 Jun 2021 13:03:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 16 Jun 2021 13:03:57 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 13:03:57 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 13:03:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 16 Jun 2021 13:03:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 13:03:59 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:3035777cd90a3389593bc49a7b39b6f67f9f2679f4e04cc59515f4d5f83ad818`  
		Last Modified: Wed, 12 May 2021 01:19:13 GMT  
		Size: 22.7 MB (22746266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a03e197445bdc67b19867d9e201ef8f2078017e5ad57773c364b31ba9786e0e`  
		Last Modified: Wed, 16 Jun 2021 13:08:37 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0af6350d4dcc917fbfd28fbf27bac7eaf3daf5903fa5325b8c04420118133805`  
		Last Modified: Wed, 16 Jun 2021 13:11:30 GMT  
		Size: 6.1 MB (6070814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a510ce2b22b66d1e15a6cd27d6759f25b4fd95463be5e08d98aa901cc01c32`  
		Last Modified: Wed, 16 Jun 2021 13:11:29 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a1aefacf2ef6cfe44dc2bc9002d4c6d62ed47ca66a674dbe6796f6e0cfeffd`  
		Last Modified: Wed, 16 Jun 2021 13:11:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:86848440e16a2373e486103dcbacfc8a33eafb92275c6a0960525c6fb1183ddd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.4 MB (32366967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12e5ee86898df3afbfc21978e7b44c1309c53279821a620a721741cf96f669c0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:52:19 GMT
ADD file:91ba1791cab3ad29a1469d1e78f21f4c0b5d3d30598683b7104980604c318854 in / 
# Wed, 12 May 2021 00:52:34 GMT
CMD ["bash"]
# Wed, 16 Jun 2021 00:32:29 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 00:41:24 GMT
ENV HAPROXY_VERSION=1.8.30
# Wed, 16 Jun 2021 00:41:24 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Wed, 16 Jun 2021 00:41:24 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Wed, 16 Jun 2021 00:41:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 16 Jun 2021 00:41:52 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 00:41:52 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 00:41:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 16 Jun 2021 00:41:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 00:41:54 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:fcad0c936ea5c12e1c8c4edb81a97c0cde04ee71e7067ee3b246474cf1854d7a`  
		Last Modified: Wed, 12 May 2021 01:02:02 GMT  
		Size: 25.9 MB (25911250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48fc449d8b117694f567c81827185f03f8e4fa5c56b0b6626bb4374515d222c3`  
		Last Modified: Wed, 16 Jun 2021 00:44:41 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1221bd3f90acbe8ded46033504384bb9e014236749666ae3536d7d0321838525`  
		Last Modified: Wed, 16 Jun 2021 00:47:07 GMT  
		Size: 6.5 MB (6453763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b268e700a6349de4f2b72ed80843a9f328f13aed36e689c12a23a451a0903a2`  
		Last Modified: Wed, 16 Jun 2021 00:47:06 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33da51e157834077b9f60850081b5a9d886e4b0a329103642bf8f4bc67bd65aa`  
		Last Modified: Wed, 16 Jun 2021 00:47:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8` - linux; 386

```console
$ docker pull haproxy@sha256:21c2d9a0c6e5a9a8c315fdd9bc53f94af01da803e554faac920fba04455bf90c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.4 MB (34373871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7c21debda92dee3a043250b71a2740e3d5275f9e9ecbc72dffb4ab9e2e4465c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:39:52 GMT
ADD file:62173a7456d614031a7b20be741983644d9723c734eee663b099ad6b47af7b35 in / 
# Wed, 12 May 2021 00:39:53 GMT
CMD ["bash"]
# Wed, 12 May 2021 05:59:03 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 06:07:27 GMT
ENV HAPROXY_VERSION=1.8.30
# Wed, 12 May 2021 06:07:28 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Wed, 12 May 2021 06:07:28 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Wed, 12 May 2021 06:08:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 06:08:13 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 06:08:13 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 12 May 2021 06:08:14 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 06:08:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 06:08:15 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:9b548256784c8e079e5953ec08bd26ce8cbaed0d606a5d350b4bcd12710d2192`  
		Last Modified: Wed, 12 May 2021 00:46:39 GMT  
		Size: 27.8 MB (27795074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05508dc89a5d9449eccbd1b8bf3910253f410f4654f50f119641aa3b5dc3e5c6`  
		Last Modified: Wed, 12 May 2021 06:11:24 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c99ab06802c43f06db3c943e7de64d1c6c5b939b8d5e33fed7bfc2e93866ba5b`  
		Last Modified: Wed, 12 May 2021 06:12:54 GMT  
		Size: 6.6 MB (6576850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16c363da2b54ad765ac79f79505205c9e769f4784e17b9509bd3a98a376d2095`  
		Last Modified: Wed, 12 May 2021 06:12:52 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5422806f328eea326bd87bc5f2e8ff1bfc87b6195db8f928974eee49cb74a03e`  
		Last Modified: Wed, 12 May 2021 06:12:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8` - linux; mips64le

```console
$ docker pull haproxy@sha256:f9ead6faf7e2314cfe33976b61451bb6040d434a4e541e62105a2bae241efe40
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.0 MB (31958239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06759cfc9ba604fc0f2543cf80303d8e8a7a2539735dba19843eb3e001d084d6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:09:45 GMT
ADD file:867397d3fb44b3b936a4ff02bbc3a1b760fb6865b5a85efab82fff224f704241 in / 
# Wed, 12 May 2021 01:09:46 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:37:27 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 01:47:41 GMT
ENV HAPROXY_VERSION=1.8.30
# Wed, 12 May 2021 01:47:41 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Wed, 12 May 2021 01:47:42 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Wed, 12 May 2021 01:49:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 01:49:22 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 01:49:22 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 12 May 2021 01:49:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 01:49:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 01:49:25 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:09564b0ac149fb24b77cbc75ce6fa5d9ba61bd7c99d11b42bd8339c3bb28e557`  
		Last Modified: Wed, 12 May 2021 01:16:36 GMT  
		Size: 25.8 MB (25812884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18fb24fa0e81746ee8c86b23e726e84be12b3f40b71800e0be7e202dd3e3eae3`  
		Last Modified: Wed, 12 May 2021 01:51:31 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d536e38cc8f29f20e30580081c74c512c9ae3f0ff986bdc5c8462a4acfa49b`  
		Last Modified: Wed, 12 May 2021 01:52:52 GMT  
		Size: 6.1 MB (6143407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3afef2553ac4e96785734752570fda3ad56c9775988122c93a33ef40a23e1ed2`  
		Last Modified: Wed, 12 May 2021 01:52:48 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2860e7bb1ccb1aeb315170e2622e271fd846f0630b4abfacb1ef5f11f834b05`  
		Last Modified: Wed, 12 May 2021 01:52:48 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8` - linux; ppc64le

```console
$ docker pull haproxy@sha256:288a6c59bb73576b6d9a433b500aecfb9d691ead39accda1a74d1be309f635f5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.5 MB (37498007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39ea2203c980613d67bb34fa3ddbb13eb8b4bbef5b3501e55271bd7c5f6cdc54`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:34:56 GMT
ADD file:3b8146cdc3649d94ad49435c94a21d700ed612ab90f010dcf8b22951b1804d34 in / 
# Wed, 12 May 2021 01:35:02 GMT
CMD ["bash"]
# Wed, 12 May 2021 06:07:29 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 06:36:44 GMT
ENV HAPROXY_VERSION=1.8.30
# Wed, 12 May 2021 06:36:52 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Wed, 12 May 2021 06:36:58 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Wed, 12 May 2021 06:44:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 06:45:06 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 06:45:09 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 12 May 2021 06:45:28 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 06:45:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 06:45:44 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:f8b445753f60bad25326d018945455601e4a65f124e956dec95c569816f21493`  
		Last Modified: Wed, 12 May 2021 01:44:19 GMT  
		Size: 30.6 MB (30552394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cfafb398e88c2b64b9fb82254775d63718baad006543dee4e7c370a09a23be9`  
		Last Modified: Wed, 12 May 2021 06:57:45 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa852ca23d74409c6c77dff16e8c085705cbfe47825da98bf2977f795ed70a42`  
		Last Modified: Wed, 12 May 2021 06:58:45 GMT  
		Size: 6.9 MB (6943665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95d1b041f05f0ba370c6def872f7d984dedb1d11930f9673ea194b55121b98d`  
		Last Modified: Wed, 12 May 2021 06:58:44 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c1d9c73439e3875ba215b460f1b8ddd6dfa67981252d0c68e5f92df1352470f`  
		Last Modified: Wed, 12 May 2021 06:58:44 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8` - linux; s390x

```console
$ docker pull haproxy@sha256:63569a1dbf7c071978be8dec571d0f96c880f1ca6997727b30d03419dd777353
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.0 MB (31994933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1040faf17b451416027573ff397f5c8138f023f7d46ab48d83f0afdc13bc3941`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:43:38 GMT
ADD file:77af21d863769b75a5f055b85b2c9d6e878f9d77a4122397ae8dde6b69e945c6 in / 
# Wed, 12 May 2021 00:43:42 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:53:39 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 02:01:01 GMT
ENV HAPROXY_VERSION=1.8.30
# Wed, 12 May 2021 02:01:02 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Wed, 12 May 2021 02:01:02 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Wed, 12 May 2021 02:02:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 02:02:14 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 02:02:15 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 12 May 2021 02:02:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 02:02:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 02:02:18 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:ba4b99e0e723623b64d4ecb8d74102998d32137ea9bcc88b15fd2e4e34b38df9`  
		Last Modified: Wed, 12 May 2021 00:48:03 GMT  
		Size: 25.8 MB (25760171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f6911826fde538e80c00f0d90920d0d7d0a78db315f0bde1ee65726f99f6747`  
		Last Modified: Wed, 12 May 2021 02:04:41 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5fca0cbd7101e00507b467578b1a05cba41baa05417f03a0a3370fe5f3e26fe`  
		Last Modified: Wed, 12 May 2021 02:05:22 GMT  
		Size: 6.2 MB (6232813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55267a56ccd26b0b6ac08d314fd2e33384f7dfe60facbdd94c11baf5e4d8cb43`  
		Last Modified: Wed, 12 May 2021 02:05:21 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a18a178044b85ea32ddb4c83da610149f4926211cd7ec8ca3cbe6d897b67e363`  
		Last Modified: Wed, 12 May 2021 02:05:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:1.8-alpine`

```console
$ docker pull haproxy@sha256:5a804b94a04d9de18abf16069bcd4e731d653c6cb7db189bb63a5ab58911c1bc
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
$ docker pull haproxy@sha256:5356dd56eb64f4baf6fc5010747f90ec4a81e7e75b93d5987d581990748f0c60
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6862890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9590f2647adea71bd046a2c4be2d20f7447ddcd590917797589be7258556c22a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:34 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Tue, 15 Jun 2021 22:57:34 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 11:05:46 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 11:12:38 GMT
ENV HAPROXY_VERSION=1.8.30
# Wed, 16 Jun 2021 11:12:38 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Wed, 16 Jun 2021 11:12:38 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Wed, 16 Jun 2021 11:13:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 16 Jun 2021 11:13:16 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 11:13:16 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 11:13:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 16 Jun 2021 11:13:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 11:13:18 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1be2f4fa6ca9f7822eb93cc888d093da91b0748abe26e3ba14d94b6a757977`  
		Last Modified: Wed, 16 Jun 2021 11:14:47 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc33cd1edcbed00d6de0516ad54c58f777c5eb77854cdd4c9fa44d4bf1a9c34`  
		Last Modified: Wed, 16 Jun 2021 11:16:09 GMT  
		Size: 4.2 MB (4239002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4d63ef015b2750653b7debe28a13bb2e6a514ea97d5581289123a0bb7878af`  
		Last Modified: Wed, 16 Jun 2021 11:16:08 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d0e3196e3d535c06dd2eedfa2b2001944b67943558864b1aa1e990ab5e56868`  
		Last Modified: Wed, 16 Jun 2021 11:16:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:61519fb0a1eb5902fa3b5e033e91e50dc90610841c2f4eed5ca5f36eefba4af8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6576726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:608b246853a10a002dff753dbfafbdf16fcbc87fdbc189641e0d44c22d176fbb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:15 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Tue, 15 Jun 2021 23:15:16 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 12:49:38 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 13:04:11 GMT
ENV HAPROXY_VERSION=1.8.30
# Wed, 16 Jun 2021 13:04:11 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Wed, 16 Jun 2021 13:04:11 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Wed, 16 Jun 2021 13:05:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 16 Jun 2021 13:05:10 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 13:05:10 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 13:05:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 16 Jun 2021 13:05:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 13:05:12 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0137e317a40af64134eac5d8b4d74173e380ac844679531b4f1fbdeeec3eb1f5`  
		Last Modified: Wed, 16 Jun 2021 13:08:54 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02436fa8e8feb3311e77ffa0069e486a521aa14e9a8bb220d62dd69e887aff8d`  
		Last Modified: Wed, 16 Jun 2021 13:11:44 GMT  
		Size: 4.2 MB (4150822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be721f988c8108beb2896dd0eae35e581815dff464670328c2aae2b09c9e4c6c`  
		Last Modified: Wed, 16 Jun 2021 13:11:43 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7030e6fe96f60fd3689ea19fa70f2c62ac37a3faa4287388cb753260ba3f41d5`  
		Last Modified: Wed, 16 Jun 2021 13:11:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:49dc4c60db834e95cfccbe79c1d1df0cac9a8388605bbb0bf872309bad71d253
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (7045899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:112c4f55e708f8f82dff41fe3784076a4eb38f25df8dae8289b444a989530f2b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 00:33:20 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 00:42:01 GMT
ENV HAPROXY_VERSION=1.8.30
# Wed, 16 Jun 2021 00:42:01 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Wed, 16 Jun 2021 00:42:01 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Wed, 16 Jun 2021 00:42:31 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 16 Jun 2021 00:42:31 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 00:42:31 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 00:42:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 16 Jun 2021 00:42:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 00:42:33 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd643f981edaf0694f3dad8fb6389455756f11cc027101d1de96b178f289891`  
		Last Modified: Wed, 16 Jun 2021 00:44:55 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef416388def2ffbbfae1c53809aa546e4c81fe81b0cf7a801047dffc1297fa0`  
		Last Modified: Wed, 16 Jun 2021 00:47:19 GMT  
		Size: 4.3 MB (4332117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d020e3bd33d1f7b451ed72e9929a1f1aa47b7f4c5f400f1750d81aac9c2ff5`  
		Last Modified: Wed, 16 Jun 2021 00:47:18 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9158d063fd1d2717ade3813ca514aeb92fca4865ccd2e074cec4048a6c9f15fb`  
		Last Modified: Wed, 16 Jun 2021 00:47:18 GMT  
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
$ docker pull haproxy@sha256:3687b0945509ed429031b71ce9baaf51ac0f395c98b1111e0fd5b224aa2281ea
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
$ docker pull haproxy@sha256:64d45752aae0bb3a1f453c5bf8784cc2584eec03a71a88c26908d9874a59ce18
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33800155 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ceb49d4303b385ae4ec7f99f331815d7dc5ff4b5e19b42505434d40973ac0bd8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 07:10:16 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 07:15:31 GMT
ENV HAPROXY_VERSION=1.8.30
# Wed, 12 May 2021 07:15:31 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Wed, 12 May 2021 07:15:31 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Wed, 12 May 2021 07:16:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 07:16:23 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 07:16:23 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 12 May 2021 07:16:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 07:16:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 07:16:26 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a113359dddc15238d26b375f86574b596b4aee1263a9631a7384589c2a02f46`  
		Last Modified: Wed, 12 May 2021 07:18:16 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19eaa5d34e4ee89879a0294969800a35f9914055323ddeb939573f963a1fa4a4`  
		Last Modified: Wed, 12 May 2021 07:19:16 GMT  
		Size: 6.7 MB (6652289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceb7dbac58865e63e8aae0d3e7563353941a8d9ae939fb1c120ffcdd651d271f`  
		Last Modified: Wed, 12 May 2021 07:19:14 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c67d5f37ab678c0b58a85431b4a68427a2aafe61bda9670fab9cfadce74e6c7`  
		Last Modified: Wed, 12 May 2021 07:19:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8.30` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:033dc007b9fd1b71bb79c6426c292a4384b8d9a76a45e844f915d0a891494721
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.1 MB (31112790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50929a1753a1ebffbf3f1495998b098a1ffb15fe95860657f9ea8bcb6f38a5db`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:55:35 GMT
ADD file:241925c5ca73c99d58f93bc78d7c5bfb6f8b280201a9b55ade45ba0cc054c31d in / 
# Wed, 12 May 2021 00:55:46 GMT
CMD ["bash"]
# Wed, 12 May 2021 02:01:24 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 02:06:57 GMT
ENV HAPROXY_VERSION=1.8.30
# Wed, 12 May 2021 02:06:57 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Wed, 12 May 2021 02:06:58 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Wed, 12 May 2021 02:07:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 02:07:49 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 02:07:50 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 12 May 2021 02:07:55 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 02:07:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 02:07:58 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:48885a8e20b16cb3bb9d2c3aafc7f040d8609844f69ca8482c42b4829d01b6da`  
		Last Modified: Wed, 12 May 2021 01:10:24 GMT  
		Size: 24.9 MB (24879601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e012f5248a53449f692d1fe91241d026aa60efe5a3dc3f04add4638989918d2a`  
		Last Modified: Wed, 12 May 2021 02:09:37 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21338fd0bfb55990c2c424c288a91c3b4ff525c954f212bfa5df546c9a26ee22`  
		Last Modified: Wed, 12 May 2021 02:10:17 GMT  
		Size: 6.2 MB (6231244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1d13df6c276b46a99a45c541c542e2d3f82086a28b44db2a26b0a2bf796830`  
		Last Modified: Wed, 12 May 2021 02:10:15 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4ac3b2830e321ef4a46bef81b407d9ac6587d79e93cf2f7b4de18fb14aee569`  
		Last Modified: Wed, 12 May 2021 02:10:15 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8.30` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:111bd77421801aaa477bd0c2907469b642f166addc73024189356acfb902c4a5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.8 MB (28819032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43a1a120e2bc22fea4c4093de642801bf5f4455253ff841fce789dc51248bce3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:03:14 GMT
ADD file:94bf2394dc26abd9f028c2933057a8673c8562e58ec4a0f51bb9bde0a5e4dee0 in / 
# Wed, 12 May 2021 01:03:32 GMT
CMD ["bash"]
# Wed, 16 Jun 2021 12:48:11 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 13:02:56 GMT
ENV HAPROXY_VERSION=1.8.30
# Wed, 16 Jun 2021 13:02:57 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Wed, 16 Jun 2021 13:02:57 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Wed, 16 Jun 2021 13:03:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 16 Jun 2021 13:03:57 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 13:03:57 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 13:03:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 16 Jun 2021 13:03:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 13:03:59 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:3035777cd90a3389593bc49a7b39b6f67f9f2679f4e04cc59515f4d5f83ad818`  
		Last Modified: Wed, 12 May 2021 01:19:13 GMT  
		Size: 22.7 MB (22746266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a03e197445bdc67b19867d9e201ef8f2078017e5ad57773c364b31ba9786e0e`  
		Last Modified: Wed, 16 Jun 2021 13:08:37 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0af6350d4dcc917fbfd28fbf27bac7eaf3daf5903fa5325b8c04420118133805`  
		Last Modified: Wed, 16 Jun 2021 13:11:30 GMT  
		Size: 6.1 MB (6070814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a510ce2b22b66d1e15a6cd27d6759f25b4fd95463be5e08d98aa901cc01c32`  
		Last Modified: Wed, 16 Jun 2021 13:11:29 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a1aefacf2ef6cfe44dc2bc9002d4c6d62ed47ca66a674dbe6796f6e0cfeffd`  
		Last Modified: Wed, 16 Jun 2021 13:11:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8.30` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:86848440e16a2373e486103dcbacfc8a33eafb92275c6a0960525c6fb1183ddd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.4 MB (32366967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12e5ee86898df3afbfc21978e7b44c1309c53279821a620a721741cf96f669c0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:52:19 GMT
ADD file:91ba1791cab3ad29a1469d1e78f21f4c0b5d3d30598683b7104980604c318854 in / 
# Wed, 12 May 2021 00:52:34 GMT
CMD ["bash"]
# Wed, 16 Jun 2021 00:32:29 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 00:41:24 GMT
ENV HAPROXY_VERSION=1.8.30
# Wed, 16 Jun 2021 00:41:24 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Wed, 16 Jun 2021 00:41:24 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Wed, 16 Jun 2021 00:41:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 16 Jun 2021 00:41:52 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 00:41:52 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 00:41:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 16 Jun 2021 00:41:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 00:41:54 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:fcad0c936ea5c12e1c8c4edb81a97c0cde04ee71e7067ee3b246474cf1854d7a`  
		Last Modified: Wed, 12 May 2021 01:02:02 GMT  
		Size: 25.9 MB (25911250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48fc449d8b117694f567c81827185f03f8e4fa5c56b0b6626bb4374515d222c3`  
		Last Modified: Wed, 16 Jun 2021 00:44:41 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1221bd3f90acbe8ded46033504384bb9e014236749666ae3536d7d0321838525`  
		Last Modified: Wed, 16 Jun 2021 00:47:07 GMT  
		Size: 6.5 MB (6453763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b268e700a6349de4f2b72ed80843a9f328f13aed36e689c12a23a451a0903a2`  
		Last Modified: Wed, 16 Jun 2021 00:47:06 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33da51e157834077b9f60850081b5a9d886e4b0a329103642bf8f4bc67bd65aa`  
		Last Modified: Wed, 16 Jun 2021 00:47:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8.30` - linux; 386

```console
$ docker pull haproxy@sha256:21c2d9a0c6e5a9a8c315fdd9bc53f94af01da803e554faac920fba04455bf90c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.4 MB (34373871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7c21debda92dee3a043250b71a2740e3d5275f9e9ecbc72dffb4ab9e2e4465c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:39:52 GMT
ADD file:62173a7456d614031a7b20be741983644d9723c734eee663b099ad6b47af7b35 in / 
# Wed, 12 May 2021 00:39:53 GMT
CMD ["bash"]
# Wed, 12 May 2021 05:59:03 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 06:07:27 GMT
ENV HAPROXY_VERSION=1.8.30
# Wed, 12 May 2021 06:07:28 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Wed, 12 May 2021 06:07:28 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Wed, 12 May 2021 06:08:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 06:08:13 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 06:08:13 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 12 May 2021 06:08:14 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 06:08:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 06:08:15 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:9b548256784c8e079e5953ec08bd26ce8cbaed0d606a5d350b4bcd12710d2192`  
		Last Modified: Wed, 12 May 2021 00:46:39 GMT  
		Size: 27.8 MB (27795074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05508dc89a5d9449eccbd1b8bf3910253f410f4654f50f119641aa3b5dc3e5c6`  
		Last Modified: Wed, 12 May 2021 06:11:24 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c99ab06802c43f06db3c943e7de64d1c6c5b939b8d5e33fed7bfc2e93866ba5b`  
		Last Modified: Wed, 12 May 2021 06:12:54 GMT  
		Size: 6.6 MB (6576850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16c363da2b54ad765ac79f79505205c9e769f4784e17b9509bd3a98a376d2095`  
		Last Modified: Wed, 12 May 2021 06:12:52 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5422806f328eea326bd87bc5f2e8ff1bfc87b6195db8f928974eee49cb74a03e`  
		Last Modified: Wed, 12 May 2021 06:12:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8.30` - linux; mips64le

```console
$ docker pull haproxy@sha256:f9ead6faf7e2314cfe33976b61451bb6040d434a4e541e62105a2bae241efe40
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.0 MB (31958239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06759cfc9ba604fc0f2543cf80303d8e8a7a2539735dba19843eb3e001d084d6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:09:45 GMT
ADD file:867397d3fb44b3b936a4ff02bbc3a1b760fb6865b5a85efab82fff224f704241 in / 
# Wed, 12 May 2021 01:09:46 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:37:27 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 01:47:41 GMT
ENV HAPROXY_VERSION=1.8.30
# Wed, 12 May 2021 01:47:41 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Wed, 12 May 2021 01:47:42 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Wed, 12 May 2021 01:49:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 01:49:22 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 01:49:22 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 12 May 2021 01:49:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 01:49:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 01:49:25 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:09564b0ac149fb24b77cbc75ce6fa5d9ba61bd7c99d11b42bd8339c3bb28e557`  
		Last Modified: Wed, 12 May 2021 01:16:36 GMT  
		Size: 25.8 MB (25812884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18fb24fa0e81746ee8c86b23e726e84be12b3f40b71800e0be7e202dd3e3eae3`  
		Last Modified: Wed, 12 May 2021 01:51:31 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d536e38cc8f29f20e30580081c74c512c9ae3f0ff986bdc5c8462a4acfa49b`  
		Last Modified: Wed, 12 May 2021 01:52:52 GMT  
		Size: 6.1 MB (6143407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3afef2553ac4e96785734752570fda3ad56c9775988122c93a33ef40a23e1ed2`  
		Last Modified: Wed, 12 May 2021 01:52:48 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2860e7bb1ccb1aeb315170e2622e271fd846f0630b4abfacb1ef5f11f834b05`  
		Last Modified: Wed, 12 May 2021 01:52:48 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8.30` - linux; ppc64le

```console
$ docker pull haproxy@sha256:288a6c59bb73576b6d9a433b500aecfb9d691ead39accda1a74d1be309f635f5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.5 MB (37498007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39ea2203c980613d67bb34fa3ddbb13eb8b4bbef5b3501e55271bd7c5f6cdc54`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:34:56 GMT
ADD file:3b8146cdc3649d94ad49435c94a21d700ed612ab90f010dcf8b22951b1804d34 in / 
# Wed, 12 May 2021 01:35:02 GMT
CMD ["bash"]
# Wed, 12 May 2021 06:07:29 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 06:36:44 GMT
ENV HAPROXY_VERSION=1.8.30
# Wed, 12 May 2021 06:36:52 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Wed, 12 May 2021 06:36:58 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Wed, 12 May 2021 06:44:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 06:45:06 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 06:45:09 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 12 May 2021 06:45:28 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 06:45:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 06:45:44 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:f8b445753f60bad25326d018945455601e4a65f124e956dec95c569816f21493`  
		Last Modified: Wed, 12 May 2021 01:44:19 GMT  
		Size: 30.6 MB (30552394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cfafb398e88c2b64b9fb82254775d63718baad006543dee4e7c370a09a23be9`  
		Last Modified: Wed, 12 May 2021 06:57:45 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa852ca23d74409c6c77dff16e8c085705cbfe47825da98bf2977f795ed70a42`  
		Last Modified: Wed, 12 May 2021 06:58:45 GMT  
		Size: 6.9 MB (6943665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95d1b041f05f0ba370c6def872f7d984dedb1d11930f9673ea194b55121b98d`  
		Last Modified: Wed, 12 May 2021 06:58:44 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c1d9c73439e3875ba215b460f1b8ddd6dfa67981252d0c68e5f92df1352470f`  
		Last Modified: Wed, 12 May 2021 06:58:44 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8.30` - linux; s390x

```console
$ docker pull haproxy@sha256:63569a1dbf7c071978be8dec571d0f96c880f1ca6997727b30d03419dd777353
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.0 MB (31994933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1040faf17b451416027573ff397f5c8138f023f7d46ab48d83f0afdc13bc3941`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:43:38 GMT
ADD file:77af21d863769b75a5f055b85b2c9d6e878f9d77a4122397ae8dde6b69e945c6 in / 
# Wed, 12 May 2021 00:43:42 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:53:39 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 02:01:01 GMT
ENV HAPROXY_VERSION=1.8.30
# Wed, 12 May 2021 02:01:02 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Wed, 12 May 2021 02:01:02 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Wed, 12 May 2021 02:02:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 02:02:14 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 02:02:15 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 12 May 2021 02:02:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 02:02:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 02:02:18 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:ba4b99e0e723623b64d4ecb8d74102998d32137ea9bcc88b15fd2e4e34b38df9`  
		Last Modified: Wed, 12 May 2021 00:48:03 GMT  
		Size: 25.8 MB (25760171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f6911826fde538e80c00f0d90920d0d7d0a78db315f0bde1ee65726f99f6747`  
		Last Modified: Wed, 12 May 2021 02:04:41 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5fca0cbd7101e00507b467578b1a05cba41baa05417f03a0a3370fe5f3e26fe`  
		Last Modified: Wed, 12 May 2021 02:05:22 GMT  
		Size: 6.2 MB (6232813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55267a56ccd26b0b6ac08d314fd2e33384f7dfe60facbdd94c11baf5e4d8cb43`  
		Last Modified: Wed, 12 May 2021 02:05:21 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a18a178044b85ea32ddb4c83da610149f4926211cd7ec8ca3cbe6d897b67e363`  
		Last Modified: Wed, 12 May 2021 02:05:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:1.8.30-alpine`

```console
$ docker pull haproxy@sha256:5a804b94a04d9de18abf16069bcd4e731d653c6cb7db189bb63a5ab58911c1bc
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
$ docker pull haproxy@sha256:5356dd56eb64f4baf6fc5010747f90ec4a81e7e75b93d5987d581990748f0c60
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6862890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9590f2647adea71bd046a2c4be2d20f7447ddcd590917797589be7258556c22a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:34 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Tue, 15 Jun 2021 22:57:34 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 11:05:46 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 11:12:38 GMT
ENV HAPROXY_VERSION=1.8.30
# Wed, 16 Jun 2021 11:12:38 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Wed, 16 Jun 2021 11:12:38 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Wed, 16 Jun 2021 11:13:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 16 Jun 2021 11:13:16 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 11:13:16 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 11:13:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 16 Jun 2021 11:13:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 11:13:18 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1be2f4fa6ca9f7822eb93cc888d093da91b0748abe26e3ba14d94b6a757977`  
		Last Modified: Wed, 16 Jun 2021 11:14:47 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc33cd1edcbed00d6de0516ad54c58f777c5eb77854cdd4c9fa44d4bf1a9c34`  
		Last Modified: Wed, 16 Jun 2021 11:16:09 GMT  
		Size: 4.2 MB (4239002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4d63ef015b2750653b7debe28a13bb2e6a514ea97d5581289123a0bb7878af`  
		Last Modified: Wed, 16 Jun 2021 11:16:08 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d0e3196e3d535c06dd2eedfa2b2001944b67943558864b1aa1e990ab5e56868`  
		Last Modified: Wed, 16 Jun 2021 11:16:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8.30-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:61519fb0a1eb5902fa3b5e033e91e50dc90610841c2f4eed5ca5f36eefba4af8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6576726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:608b246853a10a002dff753dbfafbdf16fcbc87fdbc189641e0d44c22d176fbb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:15 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Tue, 15 Jun 2021 23:15:16 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 12:49:38 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 13:04:11 GMT
ENV HAPROXY_VERSION=1.8.30
# Wed, 16 Jun 2021 13:04:11 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Wed, 16 Jun 2021 13:04:11 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Wed, 16 Jun 2021 13:05:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 16 Jun 2021 13:05:10 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 13:05:10 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 13:05:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 16 Jun 2021 13:05:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 13:05:12 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0137e317a40af64134eac5d8b4d74173e380ac844679531b4f1fbdeeec3eb1f5`  
		Last Modified: Wed, 16 Jun 2021 13:08:54 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02436fa8e8feb3311e77ffa0069e486a521aa14e9a8bb220d62dd69e887aff8d`  
		Last Modified: Wed, 16 Jun 2021 13:11:44 GMT  
		Size: 4.2 MB (4150822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be721f988c8108beb2896dd0eae35e581815dff464670328c2aae2b09c9e4c6c`  
		Last Modified: Wed, 16 Jun 2021 13:11:43 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7030e6fe96f60fd3689ea19fa70f2c62ac37a3faa4287388cb753260ba3f41d5`  
		Last Modified: Wed, 16 Jun 2021 13:11:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:1.8.30-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:49dc4c60db834e95cfccbe79c1d1df0cac9a8388605bbb0bf872309bad71d253
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.0 MB (7045899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:112c4f55e708f8f82dff41fe3784076a4eb38f25df8dae8289b444a989530f2b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 00:33:20 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 00:42:01 GMT
ENV HAPROXY_VERSION=1.8.30
# Wed, 16 Jun 2021 00:42:01 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/1.8/src/haproxy-1.8.30.tar.gz
# Wed, 16 Jun 2021 00:42:01 GMT
ENV HAPROXY_SHA256=066bfd9a0e5a3550fa621886a132379e5331d0c377e11f38bb6e8dfbec92be42
# Wed, 16 Jun 2021 00:42:31 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux2628 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 16 Jun 2021 00:42:31 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 00:42:31 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 00:42:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 16 Jun 2021 00:42:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 00:42:33 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd643f981edaf0694f3dad8fb6389455756f11cc027101d1de96b178f289891`  
		Last Modified: Wed, 16 Jun 2021 00:44:55 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef416388def2ffbbfae1c53809aa546e4c81fe81b0cf7a801047dffc1297fa0`  
		Last Modified: Wed, 16 Jun 2021 00:47:19 GMT  
		Size: 4.3 MB (4332117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d020e3bd33d1f7b451ed72e9929a1f1aa47b7f4c5f400f1750d81aac9c2ff5`  
		Last Modified: Wed, 16 Jun 2021 00:47:18 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9158d063fd1d2717ade3813ca514aeb92fca4865ccd2e074cec4048a6c9f15fb`  
		Last Modified: Wed, 16 Jun 2021 00:47:18 GMT  
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
$ docker pull haproxy@sha256:027cb20f4622789bdca9a2d1dad1dbe1c815ab0fa6c48962d4e2905dc863ca4a
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
$ docker pull haproxy@sha256:f78649851dd7007c6be318fc478349eaeab930b34b1f3e04630c5d98863cdf36
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.8 MB (35841576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e6a5d52777a6c96820960c401ef24e23479cf7406d271812edd0e9cf3c503d0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 07:10:16 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 07:14:27 GMT
ENV HAPROXY_VERSION=2.0.22
# Wed, 12 May 2021 07:14:27 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.22.tar.gz
# Wed, 12 May 2021 07:14:28 GMT
ENV HAPROXY_SHA256=5e1dccf30a3ad782d1e3298cc4e4955b168e4aa06cad4e3ea1c0334cdc0f966d
# Wed, 12 May 2021 07:15:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 07:15:16 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 07:15:17 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 12 May 2021 07:15:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 07:15:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 07:15:18 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a113359dddc15238d26b375f86574b596b4aee1263a9631a7384589c2a02f46`  
		Last Modified: Wed, 12 May 2021 07:18:16 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ef17e007dcb5e1a21b079413a5cf9b9e4f500bf8dd357565f5257e5ac999e5`  
		Last Modified: Wed, 12 May 2021 07:19:03 GMT  
		Size: 8.7 MB (8693710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39835bc542e628116edb82d04551b5f79ed3754c8e902f94ee455f977af7557`  
		Last Modified: Wed, 12 May 2021 07:19:00 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c2fd0cdd2e8e216f052f1237643e804ead3ec24804bf2aeb9f55e5357680438`  
		Last Modified: Wed, 12 May 2021 07:19:00 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:27920620d655110a7ac639a706f2b18a54bb86b6f6cced675a47bff416a76495
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.1 MB (33057092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56a2a995a8b6d0225b9bf846d890e720295bc8c37cf8b2857a58af03e5514fc9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:55:35 GMT
ADD file:241925c5ca73c99d58f93bc78d7c5bfb6f8b280201a9b55ade45ba0cc054c31d in / 
# Wed, 12 May 2021 00:55:46 GMT
CMD ["bash"]
# Wed, 12 May 2021 02:01:24 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 02:05:38 GMT
ENV HAPROXY_VERSION=2.0.22
# Wed, 12 May 2021 02:05:40 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.22.tar.gz
# Wed, 12 May 2021 02:05:41 GMT
ENV HAPROXY_SHA256=5e1dccf30a3ad782d1e3298cc4e4955b168e4aa06cad4e3ea1c0334cdc0f966d
# Wed, 12 May 2021 02:06:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 02:06:40 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 02:06:42 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 12 May 2021 02:06:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 02:06:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 02:06:46 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:48885a8e20b16cb3bb9d2c3aafc7f040d8609844f69ca8482c42b4829d01b6da`  
		Last Modified: Wed, 12 May 2021 01:10:24 GMT  
		Size: 24.9 MB (24879601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e012f5248a53449f692d1fe91241d026aa60efe5a3dc3f04add4638989918d2a`  
		Last Modified: Wed, 12 May 2021 02:09:37 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff495c9a309e2fa9b789fbd564eff7c6acbc0ec0d540decb4f6ad38405a6690b`  
		Last Modified: Wed, 12 May 2021 02:10:09 GMT  
		Size: 8.2 MB (8175544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8200556d4f9a337451f7509dca1a7b848f2b069acb9f935944d40c41555d5906`  
		Last Modified: Wed, 12 May 2021 02:10:07 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5839146baf20224f53664a20c42977a5dd978b36d65f7391901e97bc161fb0`  
		Last Modified: Wed, 12 May 2021 02:10:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:8b31a8cb4c8edc4298e8500f40b32fd832c2531802ca74550bdcf5ea50ff7bf1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.9 MB (30871031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34299d5cc0311e0b90fb3677358400146e7db04f01e749319f14dbc1aaf8bf17`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:03:14 GMT
ADD file:94bf2394dc26abd9f028c2933057a8673c8562e58ec4a0f51bb9bde0a5e4dee0 in / 
# Wed, 12 May 2021 01:03:32 GMT
CMD ["bash"]
# Wed, 16 Jun 2021 12:48:11 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 12:59:59 GMT
ENV HAPROXY_VERSION=2.0.22
# Wed, 16 Jun 2021 12:59:59 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.22.tar.gz
# Wed, 16 Jun 2021 13:00:00 GMT
ENV HAPROXY_SHA256=5e1dccf30a3ad782d1e3298cc4e4955b168e4aa06cad4e3ea1c0334cdc0f966d
# Wed, 16 Jun 2021 13:00:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 16 Jun 2021 13:00:57 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 13:00:57 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 13:00:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 16 Jun 2021 13:00:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 13:00:59 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:3035777cd90a3389593bc49a7b39b6f67f9f2679f4e04cc59515f4d5f83ad818`  
		Last Modified: Wed, 12 May 2021 01:19:13 GMT  
		Size: 22.7 MB (22746266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a03e197445bdc67b19867d9e201ef8f2078017e5ad57773c364b31ba9786e0e`  
		Last Modified: Wed, 16 Jun 2021 13:08:37 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3805e2d4a423cf313ce6db3444aa6e35f41c40477b9d3ace1a409a048b55cf64`  
		Last Modified: Wed, 16 Jun 2021 13:11:01 GMT  
		Size: 8.1 MB (8122813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbe71feb17fa99402198bfd3804e74ca6f7e68932a48f56cba01c8ec129c0cc6`  
		Last Modified: Wed, 16 Jun 2021 13:10:59 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c20e406cf1bda8f491303e5cd5b6c43d8a5c1b80f8b63d71727f6a7a7cf91917`  
		Last Modified: Wed, 16 Jun 2021 13:10:59 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:464d5d5fba2fa70dcdc2923d2d1273bc09a873c4971d32110ab6fdad234c374c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.4 MB (34443915 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d7934e0fd872f8d43e86caae23d98e25dfc6b17d499413d39f293548433bb49`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:52:19 GMT
ADD file:91ba1791cab3ad29a1469d1e78f21f4c0b5d3d30598683b7104980604c318854 in / 
# Wed, 12 May 2021 00:52:34 GMT
CMD ["bash"]
# Wed, 16 Jun 2021 00:32:29 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 00:39:48 GMT
ENV HAPROXY_VERSION=2.0.22
# Wed, 16 Jun 2021 00:39:48 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.22.tar.gz
# Wed, 16 Jun 2021 00:39:48 GMT
ENV HAPROXY_SHA256=5e1dccf30a3ad782d1e3298cc4e4955b168e4aa06cad4e3ea1c0334cdc0f966d
# Wed, 16 Jun 2021 00:40:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 16 Jun 2021 00:40:23 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 00:40:24 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 00:40:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 16 Jun 2021 00:40:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 00:40:25 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:fcad0c936ea5c12e1c8c4edb81a97c0cde04ee71e7067ee3b246474cf1854d7a`  
		Last Modified: Wed, 12 May 2021 01:02:02 GMT  
		Size: 25.9 MB (25911250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48fc449d8b117694f567c81827185f03f8e4fa5c56b0b6626bb4374515d222c3`  
		Last Modified: Wed, 16 Jun 2021 00:44:41 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:668d83c0f08dd9b0124ac7386ef89c4db8cc844558bd53b45971a3a44c8ae4bd`  
		Last Modified: Wed, 16 Jun 2021 00:46:42 GMT  
		Size: 8.5 MB (8530711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed34fa0de0623ab8083efb532442b802307ac8fe99fd01555d90b7c86d1b091`  
		Last Modified: Wed, 16 Jun 2021 00:46:40 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf57345646f39af1bcac3b0059fd35533f0faece73797186e60fe40b9d7eecb`  
		Last Modified: Wed, 16 Jun 2021 00:46:40 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0` - linux; 386

```console
$ docker pull haproxy@sha256:7fad63c2da8f3cba02bd8654ab6904a35650755797dbe4d12f2e2c4b2cc51dab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36284849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:263b0cf27d366f901e9bffd86ab2600e4fff7c126c53f1757f7d69530f163616`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:39:52 GMT
ADD file:62173a7456d614031a7b20be741983644d9723c734eee663b099ad6b47af7b35 in / 
# Wed, 12 May 2021 00:39:53 GMT
CMD ["bash"]
# Wed, 12 May 2021 05:59:03 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 06:05:22 GMT
ENV HAPROXY_VERSION=2.0.22
# Wed, 12 May 2021 06:05:22 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.22.tar.gz
# Wed, 12 May 2021 06:05:23 GMT
ENV HAPROXY_SHA256=5e1dccf30a3ad782d1e3298cc4e4955b168e4aa06cad4e3ea1c0334cdc0f966d
# Wed, 12 May 2021 06:06:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 06:06:58 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 06:06:58 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 12 May 2021 06:07:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 06:07:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 06:07:00 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:9b548256784c8e079e5953ec08bd26ce8cbaed0d606a5d350b4bcd12710d2192`  
		Last Modified: Wed, 12 May 2021 00:46:39 GMT  
		Size: 27.8 MB (27795074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05508dc89a5d9449eccbd1b8bf3910253f410f4654f50f119641aa3b5dc3e5c6`  
		Last Modified: Wed, 12 May 2021 06:11:24 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e346586e0915e2daa6815e8bec87ec0f8f8f267e9c62dadf29a93e994612873`  
		Last Modified: Wed, 12 May 2021 06:12:36 GMT  
		Size: 8.5 MB (8487828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482fbb2a4474c28fa3913340d8be30afc9680b33b4ac7c06e956384c5487e95f`  
		Last Modified: Wed, 12 May 2021 06:12:33 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67815e290e0195f801a146b4d03d912913d186faf10c62505ac46df9d935a0a8`  
		Last Modified: Wed, 12 May 2021 06:12:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0` - linux; mips64le

```console
$ docker pull haproxy@sha256:703d482ea480eafa3634ce6b10535726427a4061634919ecd774603034866c5c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (33966651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17f681293affe5a82f10d46fa9431404fd01491198a4a1d32bf73c129e5faf85`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:09:45 GMT
ADD file:867397d3fb44b3b936a4ff02bbc3a1b760fb6865b5a85efab82fff224f704241 in / 
# Wed, 12 May 2021 01:09:46 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:37:27 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 01:45:15 GMT
ENV HAPROXY_VERSION=2.0.22
# Wed, 12 May 2021 01:45:15 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.22.tar.gz
# Wed, 12 May 2021 01:45:15 GMT
ENV HAPROXY_SHA256=5e1dccf30a3ad782d1e3298cc4e4955b168e4aa06cad4e3ea1c0334cdc0f966d
# Wed, 12 May 2021 01:47:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 01:47:24 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 01:47:25 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 12 May 2021 01:47:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 01:47:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 01:47:27 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:09564b0ac149fb24b77cbc75ce6fa5d9ba61bd7c99d11b42bd8339c3bb28e557`  
		Last Modified: Wed, 12 May 2021 01:16:36 GMT  
		Size: 25.8 MB (25812884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18fb24fa0e81746ee8c86b23e726e84be12b3f40b71800e0be7e202dd3e3eae3`  
		Last Modified: Wed, 12 May 2021 01:51:31 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:126e9074709b91f049f5c71c06b4ec6a6c66666a542eb324cb2c7c0993624be4`  
		Last Modified: Wed, 12 May 2021 01:52:34 GMT  
		Size: 8.2 MB (8151818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60187521dbf0bc00458fe91acda107b78f2297ad88ee73f1c0c5863435530b3e`  
		Last Modified: Wed, 12 May 2021 01:52:28 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba86cc28fd2d409645d5c2945f2b1cb1fe64c72ce734b6c00b4eff0b4d7ac8e`  
		Last Modified: Wed, 12 May 2021 01:52:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0` - linux; ppc64le

```console
$ docker pull haproxy@sha256:6001e093455291cc7eeadda19847d8ca77cbb4c75ea42e49a56e9916229c0b6c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39510479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39c3e91bb44a90268e204b6e22d380bc535092e61d63273d17112d799385166c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:34:56 GMT
ADD file:3b8146cdc3649d94ad49435c94a21d700ed612ab90f010dcf8b22951b1804d34 in / 
# Wed, 12 May 2021 01:35:02 GMT
CMD ["bash"]
# Wed, 12 May 2021 06:07:29 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 06:28:42 GMT
ENV HAPROXY_VERSION=2.0.22
# Wed, 12 May 2021 06:28:50 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.22.tar.gz
# Wed, 12 May 2021 06:28:56 GMT
ENV HAPROXY_SHA256=5e1dccf30a3ad782d1e3298cc4e4955b168e4aa06cad4e3ea1c0334cdc0f966d
# Wed, 12 May 2021 06:35:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 06:35:36 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 06:35:43 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 12 May 2021 06:35:59 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 06:36:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 06:36:17 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:f8b445753f60bad25326d018945455601e4a65f124e956dec95c569816f21493`  
		Last Modified: Wed, 12 May 2021 01:44:19 GMT  
		Size: 30.6 MB (30552394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cfafb398e88c2b64b9fb82254775d63718baad006543dee4e7c370a09a23be9`  
		Last Modified: Wed, 12 May 2021 06:57:45 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed2bd94de1d364382c24fdda66264fb5dfd7e4fbf08ab5c80dba3b341103e857`  
		Last Modified: Wed, 12 May 2021 06:58:32 GMT  
		Size: 9.0 MB (8956135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dfa0b494fc82e26bf96c59fbe1b782d43ec39c74fa16c0c8c0da98eb4fa5ed3`  
		Last Modified: Wed, 12 May 2021 06:58:30 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d23e76501516e547357854758d673951677c50b142db0fe6bb76defbc30e26`  
		Last Modified: Wed, 12 May 2021 06:58:30 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0` - linux; s390x

```console
$ docker pull haproxy@sha256:e424c33f16837d6985336edcba2cad5f80487d80236e6e552cead95fe70fd026
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (34010417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee563465bd52126b1d3b8a4b790b62ab5dc6e285bf9119fe6c76e71ec3e6238a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:43:38 GMT
ADD file:77af21d863769b75a5f055b85b2c9d6e878f9d77a4122397ae8dde6b69e945c6 in / 
# Wed, 12 May 2021 00:43:42 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:53:39 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 01:59:05 GMT
ENV HAPROXY_VERSION=2.0.22
# Wed, 12 May 2021 01:59:06 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.22.tar.gz
# Wed, 12 May 2021 01:59:07 GMT
ENV HAPROXY_SHA256=5e1dccf30a3ad782d1e3298cc4e4955b168e4aa06cad4e3ea1c0334cdc0f966d
# Wed, 12 May 2021 02:00:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 02:00:33 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 02:00:34 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 12 May 2021 02:00:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 02:00:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 02:00:37 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:ba4b99e0e723623b64d4ecb8d74102998d32137ea9bcc88b15fd2e4e34b38df9`  
		Last Modified: Wed, 12 May 2021 00:48:03 GMT  
		Size: 25.8 MB (25760171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f6911826fde538e80c00f0d90920d0d7d0a78db315f0bde1ee65726f99f6747`  
		Last Modified: Wed, 12 May 2021 02:04:41 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d8cf025e1994949424ab4b86f4aa01f7ec7538416e81e1f82be99c48c6b2683`  
		Last Modified: Wed, 12 May 2021 02:05:13 GMT  
		Size: 8.2 MB (8248296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c961b3e8c09c87f6f8b3c52abb897f0ef1a78bfa250405b3fc1ca885d894cb`  
		Last Modified: Wed, 12 May 2021 02:05:12 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47b2ca5009a6b12b635ab621cc7b7f81a244c8db1703208caad52787e1ce805`  
		Last Modified: Wed, 12 May 2021 02:05:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.0-alpine`

```console
$ docker pull haproxy@sha256:ef18b50e028a53f7093ae4200dea1edffedf93c3ef0af10f3863e461955ad004
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
$ docker pull haproxy@sha256:9ff441bd26af002880c970fbdb3bc672f5844c283e24d265b22c5221d777d81b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8704916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:570c06f9545972876546b42042bdeb1293ad586fc23de2a354c226e06c2e3003`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:34 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Tue, 15 Jun 2021 22:57:34 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 11:05:46 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 11:11:23 GMT
ENV HAPROXY_VERSION=2.0.22
# Wed, 16 Jun 2021 11:11:23 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.22.tar.gz
# Wed, 16 Jun 2021 11:11:24 GMT
ENV HAPROXY_SHA256=5e1dccf30a3ad782d1e3298cc4e4955b168e4aa06cad4e3ea1c0334cdc0f966d
# Wed, 16 Jun 2021 11:12:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 16 Jun 2021 11:12:28 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 11:12:28 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 11:12:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 16 Jun 2021 11:12:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 11:12:30 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1be2f4fa6ca9f7822eb93cc888d093da91b0748abe26e3ba14d94b6a757977`  
		Last Modified: Wed, 16 Jun 2021 11:14:47 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d11c4044324019913e146cd4d6bee39e6ec8733792817d25c9457ef5c2688e9`  
		Last Modified: Wed, 16 Jun 2021 11:15:55 GMT  
		Size: 6.1 MB (6081031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d18350cf82687b07ed564a908fbadb038201c5c4ab7ab3bb9e98e9860aaa948`  
		Last Modified: Wed, 16 Jun 2021 11:15:53 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3960bbe90dd98db97d888525c48350dea0ad904a8ac99c2d375ff2244885151f`  
		Last Modified: Wed, 16 Jun 2021 11:15:54 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:8889bcb54133fa7698b74424ff777ddaed54da9b6fbd4d3e053e31b21e89c748
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.5 MB (8454307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f8fac1aaff278ecdfb406c44b13c86b7579e53af66eda46896ea9bd6e73610d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:15 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Tue, 15 Jun 2021 23:15:16 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 12:49:38 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 13:01:13 GMT
ENV HAPROXY_VERSION=2.0.22
# Wed, 16 Jun 2021 13:01:14 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.22.tar.gz
# Wed, 16 Jun 2021 13:01:14 GMT
ENV HAPROXY_SHA256=5e1dccf30a3ad782d1e3298cc4e4955b168e4aa06cad4e3ea1c0334cdc0f966d
# Wed, 16 Jun 2021 13:02:41 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 16 Jun 2021 13:02:41 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 13:02:42 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 13:02:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 16 Jun 2021 13:02:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 13:02:43 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0137e317a40af64134eac5d8b4d74173e380ac844679531b4f1fbdeeec3eb1f5`  
		Last Modified: Wed, 16 Jun 2021 13:08:54 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:174689a3a0729e18019e4c19ccfa7ed064331aef4db9735794ff244008a25a2f`  
		Last Modified: Wed, 16 Jun 2021 13:11:16 GMT  
		Size: 6.0 MB (6028402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87dd56b17d2502748d212849e9da37db8b487a66a9a23675f4820571db0756d1`  
		Last Modified: Wed, 16 Jun 2021 13:11:14 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd8362c07e2db3dca413152e8fe307756c39b5bb0b64a901c0c442d1bddb0eda`  
		Last Modified: Wed, 16 Jun 2021 13:11:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:ce19c77cc39fcd19139167b959b52742db2eb63ae30b53d24149c4394eb42c93
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8958247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:710f161051a520894ca2596c05aa98b3efad3a7f37d31455a6904a71ac38415e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 00:33:20 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 00:40:32 GMT
ENV HAPROXY_VERSION=2.0.22
# Wed, 16 Jun 2021 00:40:32 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.22.tar.gz
# Wed, 16 Jun 2021 00:40:32 GMT
ENV HAPROXY_SHA256=5e1dccf30a3ad782d1e3298cc4e4955b168e4aa06cad4e3ea1c0334cdc0f966d
# Wed, 16 Jun 2021 00:41:14 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 16 Jun 2021 00:41:14 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 00:41:14 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 00:41:15 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 16 Jun 2021 00:41:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 00:41:15 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd643f981edaf0694f3dad8fb6389455756f11cc027101d1de96b178f289891`  
		Last Modified: Wed, 16 Jun 2021 00:44:55 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf9e4de488b2aa29d67878b8044e1d1f4ec2ac690a2430b94a93ceaa20485d3c`  
		Last Modified: Wed, 16 Jun 2021 00:46:54 GMT  
		Size: 6.2 MB (6244464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dba35f10535d6a7901b11e29b33405a186846eeebf9f29272cdceb2855532af`  
		Last Modified: Wed, 16 Jun 2021 00:46:53 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce9630bec170adbb487c613754095c7f018601e2f6b6a666574514f99df8d6e`  
		Last Modified: Wed, 16 Jun 2021 00:46:53 GMT  
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
$ docker pull haproxy@sha256:027cb20f4622789bdca9a2d1dad1dbe1c815ab0fa6c48962d4e2905dc863ca4a
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
$ docker pull haproxy@sha256:f78649851dd7007c6be318fc478349eaeab930b34b1f3e04630c5d98863cdf36
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.8 MB (35841576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e6a5d52777a6c96820960c401ef24e23479cf7406d271812edd0e9cf3c503d0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 07:10:16 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 07:14:27 GMT
ENV HAPROXY_VERSION=2.0.22
# Wed, 12 May 2021 07:14:27 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.22.tar.gz
# Wed, 12 May 2021 07:14:28 GMT
ENV HAPROXY_SHA256=5e1dccf30a3ad782d1e3298cc4e4955b168e4aa06cad4e3ea1c0334cdc0f966d
# Wed, 12 May 2021 07:15:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 07:15:16 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 07:15:17 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 12 May 2021 07:15:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 07:15:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 07:15:18 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a113359dddc15238d26b375f86574b596b4aee1263a9631a7384589c2a02f46`  
		Last Modified: Wed, 12 May 2021 07:18:16 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ef17e007dcb5e1a21b079413a5cf9b9e4f500bf8dd357565f5257e5ac999e5`  
		Last Modified: Wed, 12 May 2021 07:19:03 GMT  
		Size: 8.7 MB (8693710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39835bc542e628116edb82d04551b5f79ed3754c8e902f94ee455f977af7557`  
		Last Modified: Wed, 12 May 2021 07:19:00 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c2fd0cdd2e8e216f052f1237643e804ead3ec24804bf2aeb9f55e5357680438`  
		Last Modified: Wed, 12 May 2021 07:19:00 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0.22` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:27920620d655110a7ac639a706f2b18a54bb86b6f6cced675a47bff416a76495
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.1 MB (33057092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56a2a995a8b6d0225b9bf846d890e720295bc8c37cf8b2857a58af03e5514fc9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:55:35 GMT
ADD file:241925c5ca73c99d58f93bc78d7c5bfb6f8b280201a9b55ade45ba0cc054c31d in / 
# Wed, 12 May 2021 00:55:46 GMT
CMD ["bash"]
# Wed, 12 May 2021 02:01:24 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 02:05:38 GMT
ENV HAPROXY_VERSION=2.0.22
# Wed, 12 May 2021 02:05:40 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.22.tar.gz
# Wed, 12 May 2021 02:05:41 GMT
ENV HAPROXY_SHA256=5e1dccf30a3ad782d1e3298cc4e4955b168e4aa06cad4e3ea1c0334cdc0f966d
# Wed, 12 May 2021 02:06:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 02:06:40 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 02:06:42 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 12 May 2021 02:06:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 02:06:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 02:06:46 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:48885a8e20b16cb3bb9d2c3aafc7f040d8609844f69ca8482c42b4829d01b6da`  
		Last Modified: Wed, 12 May 2021 01:10:24 GMT  
		Size: 24.9 MB (24879601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e012f5248a53449f692d1fe91241d026aa60efe5a3dc3f04add4638989918d2a`  
		Last Modified: Wed, 12 May 2021 02:09:37 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff495c9a309e2fa9b789fbd564eff7c6acbc0ec0d540decb4f6ad38405a6690b`  
		Last Modified: Wed, 12 May 2021 02:10:09 GMT  
		Size: 8.2 MB (8175544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8200556d4f9a337451f7509dca1a7b848f2b069acb9f935944d40c41555d5906`  
		Last Modified: Wed, 12 May 2021 02:10:07 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5839146baf20224f53664a20c42977a5dd978b36d65f7391901e97bc161fb0`  
		Last Modified: Wed, 12 May 2021 02:10:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0.22` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:8b31a8cb4c8edc4298e8500f40b32fd832c2531802ca74550bdcf5ea50ff7bf1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.9 MB (30871031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34299d5cc0311e0b90fb3677358400146e7db04f01e749319f14dbc1aaf8bf17`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:03:14 GMT
ADD file:94bf2394dc26abd9f028c2933057a8673c8562e58ec4a0f51bb9bde0a5e4dee0 in / 
# Wed, 12 May 2021 01:03:32 GMT
CMD ["bash"]
# Wed, 16 Jun 2021 12:48:11 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 12:59:59 GMT
ENV HAPROXY_VERSION=2.0.22
# Wed, 16 Jun 2021 12:59:59 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.22.tar.gz
# Wed, 16 Jun 2021 13:00:00 GMT
ENV HAPROXY_SHA256=5e1dccf30a3ad782d1e3298cc4e4955b168e4aa06cad4e3ea1c0334cdc0f966d
# Wed, 16 Jun 2021 13:00:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 16 Jun 2021 13:00:57 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 13:00:57 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 13:00:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 16 Jun 2021 13:00:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 13:00:59 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:3035777cd90a3389593bc49a7b39b6f67f9f2679f4e04cc59515f4d5f83ad818`  
		Last Modified: Wed, 12 May 2021 01:19:13 GMT  
		Size: 22.7 MB (22746266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a03e197445bdc67b19867d9e201ef8f2078017e5ad57773c364b31ba9786e0e`  
		Last Modified: Wed, 16 Jun 2021 13:08:37 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3805e2d4a423cf313ce6db3444aa6e35f41c40477b9d3ace1a409a048b55cf64`  
		Last Modified: Wed, 16 Jun 2021 13:11:01 GMT  
		Size: 8.1 MB (8122813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbe71feb17fa99402198bfd3804e74ca6f7e68932a48f56cba01c8ec129c0cc6`  
		Last Modified: Wed, 16 Jun 2021 13:10:59 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c20e406cf1bda8f491303e5cd5b6c43d8a5c1b80f8b63d71727f6a7a7cf91917`  
		Last Modified: Wed, 16 Jun 2021 13:10:59 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0.22` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:464d5d5fba2fa70dcdc2923d2d1273bc09a873c4971d32110ab6fdad234c374c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.4 MB (34443915 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d7934e0fd872f8d43e86caae23d98e25dfc6b17d499413d39f293548433bb49`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:52:19 GMT
ADD file:91ba1791cab3ad29a1469d1e78f21f4c0b5d3d30598683b7104980604c318854 in / 
# Wed, 12 May 2021 00:52:34 GMT
CMD ["bash"]
# Wed, 16 Jun 2021 00:32:29 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 00:39:48 GMT
ENV HAPROXY_VERSION=2.0.22
# Wed, 16 Jun 2021 00:39:48 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.22.tar.gz
# Wed, 16 Jun 2021 00:39:48 GMT
ENV HAPROXY_SHA256=5e1dccf30a3ad782d1e3298cc4e4955b168e4aa06cad4e3ea1c0334cdc0f966d
# Wed, 16 Jun 2021 00:40:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 16 Jun 2021 00:40:23 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 00:40:24 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 00:40:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 16 Jun 2021 00:40:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 00:40:25 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:fcad0c936ea5c12e1c8c4edb81a97c0cde04ee71e7067ee3b246474cf1854d7a`  
		Last Modified: Wed, 12 May 2021 01:02:02 GMT  
		Size: 25.9 MB (25911250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48fc449d8b117694f567c81827185f03f8e4fa5c56b0b6626bb4374515d222c3`  
		Last Modified: Wed, 16 Jun 2021 00:44:41 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:668d83c0f08dd9b0124ac7386ef89c4db8cc844558bd53b45971a3a44c8ae4bd`  
		Last Modified: Wed, 16 Jun 2021 00:46:42 GMT  
		Size: 8.5 MB (8530711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed34fa0de0623ab8083efb532442b802307ac8fe99fd01555d90b7c86d1b091`  
		Last Modified: Wed, 16 Jun 2021 00:46:40 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf57345646f39af1bcac3b0059fd35533f0faece73797186e60fe40b9d7eecb`  
		Last Modified: Wed, 16 Jun 2021 00:46:40 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0.22` - linux; 386

```console
$ docker pull haproxy@sha256:7fad63c2da8f3cba02bd8654ab6904a35650755797dbe4d12f2e2c4b2cc51dab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36284849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:263b0cf27d366f901e9bffd86ab2600e4fff7c126c53f1757f7d69530f163616`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:39:52 GMT
ADD file:62173a7456d614031a7b20be741983644d9723c734eee663b099ad6b47af7b35 in / 
# Wed, 12 May 2021 00:39:53 GMT
CMD ["bash"]
# Wed, 12 May 2021 05:59:03 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 06:05:22 GMT
ENV HAPROXY_VERSION=2.0.22
# Wed, 12 May 2021 06:05:22 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.22.tar.gz
# Wed, 12 May 2021 06:05:23 GMT
ENV HAPROXY_SHA256=5e1dccf30a3ad782d1e3298cc4e4955b168e4aa06cad4e3ea1c0334cdc0f966d
# Wed, 12 May 2021 06:06:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 06:06:58 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 06:06:58 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 12 May 2021 06:07:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 06:07:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 06:07:00 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:9b548256784c8e079e5953ec08bd26ce8cbaed0d606a5d350b4bcd12710d2192`  
		Last Modified: Wed, 12 May 2021 00:46:39 GMT  
		Size: 27.8 MB (27795074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05508dc89a5d9449eccbd1b8bf3910253f410f4654f50f119641aa3b5dc3e5c6`  
		Last Modified: Wed, 12 May 2021 06:11:24 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e346586e0915e2daa6815e8bec87ec0f8f8f267e9c62dadf29a93e994612873`  
		Last Modified: Wed, 12 May 2021 06:12:36 GMT  
		Size: 8.5 MB (8487828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482fbb2a4474c28fa3913340d8be30afc9680b33b4ac7c06e956384c5487e95f`  
		Last Modified: Wed, 12 May 2021 06:12:33 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67815e290e0195f801a146b4d03d912913d186faf10c62505ac46df9d935a0a8`  
		Last Modified: Wed, 12 May 2021 06:12:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0.22` - linux; mips64le

```console
$ docker pull haproxy@sha256:703d482ea480eafa3634ce6b10535726427a4061634919ecd774603034866c5c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (33966651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17f681293affe5a82f10d46fa9431404fd01491198a4a1d32bf73c129e5faf85`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:09:45 GMT
ADD file:867397d3fb44b3b936a4ff02bbc3a1b760fb6865b5a85efab82fff224f704241 in / 
# Wed, 12 May 2021 01:09:46 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:37:27 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 01:45:15 GMT
ENV HAPROXY_VERSION=2.0.22
# Wed, 12 May 2021 01:45:15 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.22.tar.gz
# Wed, 12 May 2021 01:45:15 GMT
ENV HAPROXY_SHA256=5e1dccf30a3ad782d1e3298cc4e4955b168e4aa06cad4e3ea1c0334cdc0f966d
# Wed, 12 May 2021 01:47:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 01:47:24 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 01:47:25 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 12 May 2021 01:47:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 01:47:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 01:47:27 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:09564b0ac149fb24b77cbc75ce6fa5d9ba61bd7c99d11b42bd8339c3bb28e557`  
		Last Modified: Wed, 12 May 2021 01:16:36 GMT  
		Size: 25.8 MB (25812884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18fb24fa0e81746ee8c86b23e726e84be12b3f40b71800e0be7e202dd3e3eae3`  
		Last Modified: Wed, 12 May 2021 01:51:31 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:126e9074709b91f049f5c71c06b4ec6a6c66666a542eb324cb2c7c0993624be4`  
		Last Modified: Wed, 12 May 2021 01:52:34 GMT  
		Size: 8.2 MB (8151818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60187521dbf0bc00458fe91acda107b78f2297ad88ee73f1c0c5863435530b3e`  
		Last Modified: Wed, 12 May 2021 01:52:28 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba86cc28fd2d409645d5c2945f2b1cb1fe64c72ce734b6c00b4eff0b4d7ac8e`  
		Last Modified: Wed, 12 May 2021 01:52:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0.22` - linux; ppc64le

```console
$ docker pull haproxy@sha256:6001e093455291cc7eeadda19847d8ca77cbb4c75ea42e49a56e9916229c0b6c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39510479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39c3e91bb44a90268e204b6e22d380bc535092e61d63273d17112d799385166c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:34:56 GMT
ADD file:3b8146cdc3649d94ad49435c94a21d700ed612ab90f010dcf8b22951b1804d34 in / 
# Wed, 12 May 2021 01:35:02 GMT
CMD ["bash"]
# Wed, 12 May 2021 06:07:29 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 06:28:42 GMT
ENV HAPROXY_VERSION=2.0.22
# Wed, 12 May 2021 06:28:50 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.22.tar.gz
# Wed, 12 May 2021 06:28:56 GMT
ENV HAPROXY_SHA256=5e1dccf30a3ad782d1e3298cc4e4955b168e4aa06cad4e3ea1c0334cdc0f966d
# Wed, 12 May 2021 06:35:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 06:35:36 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 06:35:43 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 12 May 2021 06:35:59 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 06:36:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 06:36:17 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:f8b445753f60bad25326d018945455601e4a65f124e956dec95c569816f21493`  
		Last Modified: Wed, 12 May 2021 01:44:19 GMT  
		Size: 30.6 MB (30552394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cfafb398e88c2b64b9fb82254775d63718baad006543dee4e7c370a09a23be9`  
		Last Modified: Wed, 12 May 2021 06:57:45 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed2bd94de1d364382c24fdda66264fb5dfd7e4fbf08ab5c80dba3b341103e857`  
		Last Modified: Wed, 12 May 2021 06:58:32 GMT  
		Size: 9.0 MB (8956135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dfa0b494fc82e26bf96c59fbe1b782d43ec39c74fa16c0c8c0da98eb4fa5ed3`  
		Last Modified: Wed, 12 May 2021 06:58:30 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d23e76501516e547357854758d673951677c50b142db0fe6bb76defbc30e26`  
		Last Modified: Wed, 12 May 2021 06:58:30 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0.22` - linux; s390x

```console
$ docker pull haproxy@sha256:e424c33f16837d6985336edcba2cad5f80487d80236e6e552cead95fe70fd026
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (34010417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee563465bd52126b1d3b8a4b790b62ab5dc6e285bf9119fe6c76e71ec3e6238a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:43:38 GMT
ADD file:77af21d863769b75a5f055b85b2c9d6e878f9d77a4122397ae8dde6b69e945c6 in / 
# Wed, 12 May 2021 00:43:42 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:53:39 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 01:59:05 GMT
ENV HAPROXY_VERSION=2.0.22
# Wed, 12 May 2021 01:59:06 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.22.tar.gz
# Wed, 12 May 2021 01:59:07 GMT
ENV HAPROXY_SHA256=5e1dccf30a3ad782d1e3298cc4e4955b168e4aa06cad4e3ea1c0334cdc0f966d
# Wed, 12 May 2021 02:00:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 02:00:33 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 02:00:34 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 12 May 2021 02:00:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 02:00:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 02:00:37 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:ba4b99e0e723623b64d4ecb8d74102998d32137ea9bcc88b15fd2e4e34b38df9`  
		Last Modified: Wed, 12 May 2021 00:48:03 GMT  
		Size: 25.8 MB (25760171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f6911826fde538e80c00f0d90920d0d7d0a78db315f0bde1ee65726f99f6747`  
		Last Modified: Wed, 12 May 2021 02:04:41 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d8cf025e1994949424ab4b86f4aa01f7ec7538416e81e1f82be99c48c6b2683`  
		Last Modified: Wed, 12 May 2021 02:05:13 GMT  
		Size: 8.2 MB (8248296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c961b3e8c09c87f6f8b3c52abb897f0ef1a78bfa250405b3fc1ca885d894cb`  
		Last Modified: Wed, 12 May 2021 02:05:12 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47b2ca5009a6b12b635ab621cc7b7f81a244c8db1703208caad52787e1ce805`  
		Last Modified: Wed, 12 May 2021 02:05:12 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.0.22-alpine`

```console
$ docker pull haproxy@sha256:ef18b50e028a53f7093ae4200dea1edffedf93c3ef0af10f3863e461955ad004
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
$ docker pull haproxy@sha256:9ff441bd26af002880c970fbdb3bc672f5844c283e24d265b22c5221d777d81b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8704916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:570c06f9545972876546b42042bdeb1293ad586fc23de2a354c226e06c2e3003`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:34 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Tue, 15 Jun 2021 22:57:34 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 11:05:46 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 11:11:23 GMT
ENV HAPROXY_VERSION=2.0.22
# Wed, 16 Jun 2021 11:11:23 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.22.tar.gz
# Wed, 16 Jun 2021 11:11:24 GMT
ENV HAPROXY_SHA256=5e1dccf30a3ad782d1e3298cc4e4955b168e4aa06cad4e3ea1c0334cdc0f966d
# Wed, 16 Jun 2021 11:12:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 16 Jun 2021 11:12:28 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 11:12:28 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 11:12:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 16 Jun 2021 11:12:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 11:12:30 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1be2f4fa6ca9f7822eb93cc888d093da91b0748abe26e3ba14d94b6a757977`  
		Last Modified: Wed, 16 Jun 2021 11:14:47 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d11c4044324019913e146cd4d6bee39e6ec8733792817d25c9457ef5c2688e9`  
		Last Modified: Wed, 16 Jun 2021 11:15:55 GMT  
		Size: 6.1 MB (6081031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d18350cf82687b07ed564a908fbadb038201c5c4ab7ab3bb9e98e9860aaa948`  
		Last Modified: Wed, 16 Jun 2021 11:15:53 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3960bbe90dd98db97d888525c48350dea0ad904a8ac99c2d375ff2244885151f`  
		Last Modified: Wed, 16 Jun 2021 11:15:54 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0.22-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:8889bcb54133fa7698b74424ff777ddaed54da9b6fbd4d3e053e31b21e89c748
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.5 MB (8454307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f8fac1aaff278ecdfb406c44b13c86b7579e53af66eda46896ea9bd6e73610d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:15 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Tue, 15 Jun 2021 23:15:16 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 12:49:38 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 13:01:13 GMT
ENV HAPROXY_VERSION=2.0.22
# Wed, 16 Jun 2021 13:01:14 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.22.tar.gz
# Wed, 16 Jun 2021 13:01:14 GMT
ENV HAPROXY_SHA256=5e1dccf30a3ad782d1e3298cc4e4955b168e4aa06cad4e3ea1c0334cdc0f966d
# Wed, 16 Jun 2021 13:02:41 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 16 Jun 2021 13:02:41 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 13:02:42 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 13:02:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 16 Jun 2021 13:02:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 13:02:43 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0137e317a40af64134eac5d8b4d74173e380ac844679531b4f1fbdeeec3eb1f5`  
		Last Modified: Wed, 16 Jun 2021 13:08:54 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:174689a3a0729e18019e4c19ccfa7ed064331aef4db9735794ff244008a25a2f`  
		Last Modified: Wed, 16 Jun 2021 13:11:16 GMT  
		Size: 6.0 MB (6028402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87dd56b17d2502748d212849e9da37db8b487a66a9a23675f4820571db0756d1`  
		Last Modified: Wed, 16 Jun 2021 13:11:14 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd8362c07e2db3dca413152e8fe307756c39b5bb0b64a901c0c442d1bddb0eda`  
		Last Modified: Wed, 16 Jun 2021 13:11:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.0.22-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:ce19c77cc39fcd19139167b959b52742db2eb63ae30b53d24149c4394eb42c93
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8958247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:710f161051a520894ca2596c05aa98b3efad3a7f37d31455a6904a71ac38415e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 00:33:20 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 00:40:32 GMT
ENV HAPROXY_VERSION=2.0.22
# Wed, 16 Jun 2021 00:40:32 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.22.tar.gz
# Wed, 16 Jun 2021 00:40:32 GMT
ENV HAPROXY_SHA256=5e1dccf30a3ad782d1e3298cc4e4955b168e4aa06cad4e3ea1c0334cdc0f966d
# Wed, 16 Jun 2021 00:41:14 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 16 Jun 2021 00:41:14 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 00:41:14 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 00:41:15 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 16 Jun 2021 00:41:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 00:41:15 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd643f981edaf0694f3dad8fb6389455756f11cc027101d1de96b178f289891`  
		Last Modified: Wed, 16 Jun 2021 00:44:55 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf9e4de488b2aa29d67878b8044e1d1f4ec2ac690a2430b94a93ceaa20485d3c`  
		Last Modified: Wed, 16 Jun 2021 00:46:54 GMT  
		Size: 6.2 MB (6244464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dba35f10535d6a7901b11e29b33405a186846eeebf9f29272cdceb2855532af`  
		Last Modified: Wed, 16 Jun 2021 00:46:53 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce9630bec170adbb487c613754095c7f018601e2f6b6a666574514f99df8d6e`  
		Last Modified: Wed, 16 Jun 2021 00:46:53 GMT  
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
$ docker pull haproxy@sha256:e21c2a2f7f68fad8dbd622ed2c11ac24638a4d7c84dfeff8df1bcfa3ca0f5b02
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
$ docker pull haproxy@sha256:36aa98fff27dcb2d12c93e68515a6686378c783ea9b1ab1d01ce993a5cbc73e1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.5 MB (36456882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dab1cc236da4978d9fbd4228673dff63592602eba08f6dc940913a862483619`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 07:10:16 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 07:12:59 GMT
ENV HAPROXY_VERSION=2.2.14
# Wed, 12 May 2021 07:12:59 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Wed, 12 May 2021 07:13:00 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Wed, 12 May 2021 07:14:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 07:14:18 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 07:14:19 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 12 May 2021 07:14:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 07:14:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 07:14:20 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a113359dddc15238d26b375f86574b596b4aee1263a9631a7384589c2a02f46`  
		Last Modified: Wed, 12 May 2021 07:18:16 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce57e8a2356e45f88d6ced00b3b9eec7b48f92168ef61338c0e36bee522cdf2b`  
		Last Modified: Wed, 12 May 2021 07:18:47 GMT  
		Size: 9.3 MB (9309017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a21ae969825c26039288a303bddf95391487564b9d309d3500412c82c587f29`  
		Last Modified: Wed, 12 May 2021 07:18:45 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e154e81f6d1cf5ca9e6726aef4a64f9fdd04a24bab984cd21dac17080004feaf`  
		Last Modified: Wed, 12 May 2021 07:18:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:9794c13ea712f7ed6881ea208e2fd383348c09f3c2742d41ba83d5aa49287433
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33794739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f42f2243feb31e79f986feaa6a5cfd29738ed366dfdd531ddd447c526e466e11`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:55:35 GMT
ADD file:241925c5ca73c99d58f93bc78d7c5bfb6f8b280201a9b55ade45ba0cc054c31d in / 
# Wed, 12 May 2021 00:55:46 GMT
CMD ["bash"]
# Wed, 12 May 2021 02:01:24 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 02:04:19 GMT
ENV HAPROXY_VERSION=2.2.14
# Wed, 12 May 2021 02:04:20 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Wed, 12 May 2021 02:04:22 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Wed, 12 May 2021 02:05:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 02:05:14 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 02:05:15 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 12 May 2021 02:05:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 02:05:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 02:05:23 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:48885a8e20b16cb3bb9d2c3aafc7f040d8609844f69ca8482c42b4829d01b6da`  
		Last Modified: Wed, 12 May 2021 01:10:24 GMT  
		Size: 24.9 MB (24879601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e012f5248a53449f692d1fe91241d026aa60efe5a3dc3f04add4638989918d2a`  
		Last Modified: Wed, 12 May 2021 02:09:37 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9801d19b7ae90b0a5bd4f1fab7b81a0f392825a5831065fe93490ace1e8ba6`  
		Last Modified: Wed, 12 May 2021 02:09:59 GMT  
		Size: 8.9 MB (8913193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6582836c09b2edadce61be9caabd42dc794db9cd00edfceb71ab1e221cb486f`  
		Last Modified: Wed, 12 May 2021 02:09:56 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f8cd4122dc63b8e9afb002f3e28ed09f9c1d716f3a93a725ef97ed8debb5122`  
		Last Modified: Wed, 12 May 2021 02:09:56 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:1a18cddd7e15cebbc8aeb3db3d49a3ddfbf93d88bc1633cc06ed7710b7276dd8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.5 MB (31471028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bf2c2a94446dabe83faf588182e40770c2024f9c1d3eb442f500177b790bf44`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:03:14 GMT
ADD file:94bf2394dc26abd9f028c2933057a8673c8562e58ec4a0f51bb9bde0a5e4dee0 in / 
# Wed, 12 May 2021 01:03:32 GMT
CMD ["bash"]
# Wed, 16 Jun 2021 12:48:11 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 12:57:16 GMT
ENV HAPROXY_VERSION=2.2.14
# Wed, 16 Jun 2021 12:57:16 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Wed, 16 Jun 2021 12:57:17 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Wed, 16 Jun 2021 12:58:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 16 Jun 2021 12:58:37 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 12:58:37 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 12:58:38 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 16 Jun 2021 12:58:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 12:58:38 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:3035777cd90a3389593bc49a7b39b6f67f9f2679f4e04cc59515f4d5f83ad818`  
		Last Modified: Wed, 12 May 2021 01:19:13 GMT  
		Size: 22.7 MB (22746266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a03e197445bdc67b19867d9e201ef8f2078017e5ad57773c364b31ba9786e0e`  
		Last Modified: Wed, 16 Jun 2021 13:08:37 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a7f6f8c915bd1a6b48f730fa9021df49ddc135d25c3d2647e19653646c81d76`  
		Last Modified: Wed, 16 Jun 2021 13:10:29 GMT  
		Size: 8.7 MB (8722809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b08690033c42ac48ac22c19f5a170c443042811b6478c29ca62b1f8c22d60405`  
		Last Modified: Wed, 16 Jun 2021 13:10:27 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbbb25bc9a88d8d2885e7655078001397c12394c1eb7dfffed08d4afcbf12088`  
		Last Modified: Wed, 16 Jun 2021 13:10:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:a6fb349acaa1f3153d517b09790399603f3bdc1fb6482b7fc48ba3da4c332ba6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.0 MB (35036109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa08b9b9a2dbb4aa712762bce833331d0f919660933949fc0e6d3e19d535581a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:52:19 GMT
ADD file:91ba1791cab3ad29a1469d1e78f21f4c0b5d3d30598683b7104980604c318854 in / 
# Wed, 12 May 2021 00:52:34 GMT
CMD ["bash"]
# Wed, 16 Jun 2021 00:32:29 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 00:38:12 GMT
ENV HAPROXY_VERSION=2.2.14
# Wed, 16 Jun 2021 00:38:12 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Wed, 16 Jun 2021 00:38:13 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Wed, 16 Jun 2021 00:38:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 16 Jun 2021 00:38:49 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 00:38:50 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 00:38:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 16 Jun 2021 00:38:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 00:38:51 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:fcad0c936ea5c12e1c8c4edb81a97c0cde04ee71e7067ee3b246474cf1854d7a`  
		Last Modified: Wed, 12 May 2021 01:02:02 GMT  
		Size: 25.9 MB (25911250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48fc449d8b117694f567c81827185f03f8e4fa5c56b0b6626bb4374515d222c3`  
		Last Modified: Wed, 16 Jun 2021 00:44:41 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d3d0956859fc9b54a7daaf82cec02c80fa7ded81273456f95542cf6d64128d`  
		Last Modified: Wed, 16 Jun 2021 00:46:16 GMT  
		Size: 9.1 MB (9122905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a28d7c7cadd917ff1125c907068bf642dedcbda91d794b5a1f4346fe0cc6417f`  
		Last Modified: Wed, 16 Jun 2021 00:46:14 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:422c3354a6398bfaac49561575a7839a5ede61117177deedfe8833e8b42c3fa1`  
		Last Modified: Wed, 16 Jun 2021 00:46:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2` - linux; 386

```console
$ docker pull haproxy@sha256:aa53847eb9379394d7b8a20a77cc9e9b7138d4902a964d851575c6d9ffed46d0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36986807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b23c745e4959a63996d75404f0278ae5c8f22759fdb0e9b02270d8923f1f22db`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:39:52 GMT
ADD file:62173a7456d614031a7b20be741983644d9723c734eee663b099ad6b47af7b35 in / 
# Wed, 12 May 2021 00:39:53 GMT
CMD ["bash"]
# Wed, 12 May 2021 05:59:03 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 06:03:15 GMT
ENV HAPROXY_VERSION=2.2.14
# Wed, 12 May 2021 06:03:16 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Wed, 12 May 2021 06:03:16 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Wed, 12 May 2021 06:04:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 06:04:59 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 06:05:00 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 12 May 2021 06:05:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 06:05:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 06:05:02 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:9b548256784c8e079e5953ec08bd26ce8cbaed0d606a5d350b4bcd12710d2192`  
		Last Modified: Wed, 12 May 2021 00:46:39 GMT  
		Size: 27.8 MB (27795074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05508dc89a5d9449eccbd1b8bf3910253f410f4654f50f119641aa3b5dc3e5c6`  
		Last Modified: Wed, 12 May 2021 06:11:24 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7280424fa09c0966592c9cb625c0758831c87c3c81942752dc11cf73a464a65`  
		Last Modified: Wed, 12 May 2021 06:12:11 GMT  
		Size: 9.2 MB (9189784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f788c80822fb5def6f69c985b54c7aa69f7e91ea3824727dfddba7f6772e7d49`  
		Last Modified: Wed, 12 May 2021 06:12:08 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e219cc6901948963354dce74cbefff75cb59aa944edfbd1b9c6bd7fe6efcb853`  
		Last Modified: Wed, 12 May 2021 06:12:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2` - linux; mips64le

```console
$ docker pull haproxy@sha256:e1c2dad45dff2975488f39cc6dc1abca01182d8e3c4413018bfcda7eba01d3ec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34685329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e11d95019b4bd97a948fe6e9dea89aa8187ca59d9d6a0dd47d148e14159abcb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:09:45 GMT
ADD file:867397d3fb44b3b936a4ff02bbc3a1b760fb6865b5a85efab82fff224f704241 in / 
# Wed, 12 May 2021 01:09:46 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:37:27 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 01:42:33 GMT
ENV HAPROXY_VERSION=2.2.14
# Wed, 12 May 2021 01:42:34 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Wed, 12 May 2021 01:42:34 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Wed, 12 May 2021 01:44:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 01:44:55 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 01:44:56 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 12 May 2021 01:44:57 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 01:44:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 01:44:58 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:09564b0ac149fb24b77cbc75ce6fa5d9ba61bd7c99d11b42bd8339c3bb28e557`  
		Last Modified: Wed, 12 May 2021 01:16:36 GMT  
		Size: 25.8 MB (25812884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18fb24fa0e81746ee8c86b23e726e84be12b3f40b71800e0be7e202dd3e3eae3`  
		Last Modified: Wed, 12 May 2021 01:51:31 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75e4ffbdb19bf59d4597dcfb801a70f24e09fad44e98f3c8dc6778e67706c1cf`  
		Last Modified: Wed, 12 May 2021 01:52:16 GMT  
		Size: 8.9 MB (8870498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d75e58f932335918c79b406d5f66258335ea44229d3618fc37516e0d72a054d2`  
		Last Modified: Wed, 12 May 2021 01:52:07 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3258ef7e9fb3e5cd76b106ec88a0ede2cd56578f8110ca421988021dbf7d5bc5`  
		Last Modified: Wed, 12 May 2021 01:52:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2` - linux; ppc64le

```console
$ docker pull haproxy@sha256:319f7bae4d558e479dec60b688b69e85a5e50471e599b0c37ca8fe3d0a0d6b2a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40329546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45b00610b81e8a7e221af06253830cb1809d9131f91da6125f39724d6976f5cf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:34:56 GMT
ADD file:3b8146cdc3649d94ad49435c94a21d700ed612ab90f010dcf8b22951b1804d34 in / 
# Wed, 12 May 2021 01:35:02 GMT
CMD ["bash"]
# Wed, 12 May 2021 06:07:29 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 06:22:13 GMT
ENV HAPROXY_VERSION=2.2.14
# Wed, 12 May 2021 06:22:18 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Wed, 12 May 2021 06:22:24 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Wed, 12 May 2021 06:27:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 06:27:44 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 06:27:48 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 12 May 2021 06:28:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 06:28:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 06:28:17 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:f8b445753f60bad25326d018945455601e4a65f124e956dec95c569816f21493`  
		Last Modified: Wed, 12 May 2021 01:44:19 GMT  
		Size: 30.6 MB (30552394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cfafb398e88c2b64b9fb82254775d63718baad006543dee4e7c370a09a23be9`  
		Last Modified: Wed, 12 May 2021 06:57:45 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8acd792e93450fd09e1ff3d6e290d3b6e970010aeee7e4c237d139b092405c6e`  
		Last Modified: Wed, 12 May 2021 06:58:16 GMT  
		Size: 9.8 MB (9775201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d363af0309019290c9372f642779a744c643b8d02797455c2182c9f38b1f70b0`  
		Last Modified: Wed, 12 May 2021 06:58:14 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ffb4d4b17b47ae317fa7c3c086a45eecc3143c7631e6ee7d80677bdbcd263f`  
		Last Modified: Wed, 12 May 2021 06:58:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2` - linux; s390x

```console
$ docker pull haproxy@sha256:88d4465a398b20357befa2125b348a2d4d4fd38846a5b0bc40ff403ce3411bb1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34770545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a9ed7ac70d50e098fef07714cb33343740076728f19c59485f610a0ce2b0d52`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:43:38 GMT
ADD file:77af21d863769b75a5f055b85b2c9d6e878f9d77a4122397ae8dde6b69e945c6 in / 
# Wed, 12 May 2021 00:43:42 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:53:39 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 01:57:10 GMT
ENV HAPROXY_VERSION=2.2.14
# Wed, 12 May 2021 01:57:11 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Wed, 12 May 2021 01:57:11 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Wed, 12 May 2021 01:58:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 01:58:43 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 01:58:43 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 12 May 2021 01:58:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 01:58:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 01:58:46 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:ba4b99e0e723623b64d4ecb8d74102998d32137ea9bcc88b15fd2e4e34b38df9`  
		Last Modified: Wed, 12 May 2021 00:48:03 GMT  
		Size: 25.8 MB (25760171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f6911826fde538e80c00f0d90920d0d7d0a78db315f0bde1ee65726f99f6747`  
		Last Modified: Wed, 12 May 2021 02:04:41 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d13bfedee585dcd4452959bf438e9169b2dfbe277be615e7f46be40ea2a32c9`  
		Last Modified: Wed, 12 May 2021 02:05:02 GMT  
		Size: 9.0 MB (9008423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ad5f54a60f3ec7b35b6b26e386c96f02273dc7605250e397f759936d99af12f`  
		Last Modified: Wed, 12 May 2021 02:05:00 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f74de135cd0b02764be0d540e5d8b8aefa807bf2d0ad81ba1d5dd3d34f08b5f7`  
		Last Modified: Wed, 12 May 2021 02:05:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.2-alpine`

```console
$ docker pull haproxy@sha256:ed1a283a87e2326659dd8a78b098da8d7104aaf9487c29af58142cc8bce39f6e
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
$ docker pull haproxy@sha256:843beeb4ab666f0116244dd8500c2242e96a9b966b28e226844b7142d4ad10bd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9270291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:971f6f8cf8b517efcdae3e9823c681d724b6c75df980deff3aa1e8548aa8547f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:34 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Tue, 15 Jun 2021 22:57:34 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 11:05:46 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 11:09:56 GMT
ENV HAPROXY_VERSION=2.2.14
# Wed, 16 Jun 2021 11:09:56 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Wed, 16 Jun 2021 11:09:56 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Wed, 16 Jun 2021 11:11:04 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 16 Jun 2021 11:11:04 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 11:11:04 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 11:11:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 16 Jun 2021 11:11:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 11:11:06 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1be2f4fa6ca9f7822eb93cc888d093da91b0748abe26e3ba14d94b6a757977`  
		Last Modified: Wed, 16 Jun 2021 11:14:47 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1a1a2850005aaff668796013f3aeb1cd2c3ce9a5411e8fed8122a085a624467`  
		Last Modified: Wed, 16 Jun 2021 11:15:40 GMT  
		Size: 6.6 MB (6646404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32dbeff2aec20ce0c4ba58aac6d200cfd0a8e2bd7e86d720ce462cefb7ec7442`  
		Last Modified: Wed, 16 Jun 2021 11:15:39 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97e2471f12eacf30f0dbfe3024096f548f75f5825cd44f9240c7ff193be4bf3b`  
		Last Modified: Wed, 16 Jun 2021 11:15:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:71e9a22b3384bdfd721b422c69e9689f7ee3e1b42433ebc15a63c6de45c588e2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8961889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:197d66e79595a1f39ec57840337cbf3c6b7b804f73406e12bbe983e4cd4ce1c3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:15 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Tue, 15 Jun 2021 23:15:16 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 12:49:38 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 12:58:45 GMT
ENV HAPROXY_VERSION=2.2.14
# Wed, 16 Jun 2021 12:58:46 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Wed, 16 Jun 2021 12:58:46 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Wed, 16 Jun 2021 12:59:41 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 16 Jun 2021 12:59:41 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 12:59:42 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 12:59:42 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 16 Jun 2021 12:59:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 12:59:43 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0137e317a40af64134eac5d8b4d74173e380ac844679531b4f1fbdeeec3eb1f5`  
		Last Modified: Wed, 16 Jun 2021 13:08:54 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80330a3beceeeee15efbab331000f2e900c85c498bd6dabb7c6fcd3b2ac511c0`  
		Last Modified: Wed, 16 Jun 2021 13:10:45 GMT  
		Size: 6.5 MB (6535985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:750fa69962e93c5a7b5988610bf31d54c5f24c8bb78eb4af47aab9f966928d7a`  
		Last Modified: Wed, 16 Jun 2021 13:10:43 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92efec0eb24989a4cef1cc58290c66449deab35e795e1b53b5066511b347508b`  
		Last Modified: Wed, 16 Jun 2021 13:10:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:96a54898cda2d86ab749cae4be00faaa3777756652a65311345c8bfc33b52cfd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9495042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75de00676085ad0b98b06da4e3f90844176a41797f49e804b5e454582d8086fd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 00:33:20 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 00:38:56 GMT
ENV HAPROXY_VERSION=2.2.14
# Wed, 16 Jun 2021 00:38:56 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Wed, 16 Jun 2021 00:38:57 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Wed, 16 Jun 2021 00:39:40 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 16 Jun 2021 00:39:40 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 00:39:41 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 00:39:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 16 Jun 2021 00:39:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 00:39:42 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd643f981edaf0694f3dad8fb6389455756f11cc027101d1de96b178f289891`  
		Last Modified: Wed, 16 Jun 2021 00:44:55 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ccf648e7b295e02b4acb888c0facdcc8958509fd6903355133ab86ac3e096b0`  
		Last Modified: Wed, 16 Jun 2021 00:46:29 GMT  
		Size: 6.8 MB (6781264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4551c1ee9934cf8bd0c3d9d53e5a60b4127dc8a67714ac54bf67da3a393610`  
		Last Modified: Wed, 16 Jun 2021 00:46:28 GMT  
		Size: 446.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f23d51122d88e10da20d1f5cac248e1819b4226b35f8d651f5e60250d2fe3cf`  
		Last Modified: Wed, 16 Jun 2021 00:46:28 GMT  
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
$ docker pull haproxy@sha256:e21c2a2f7f68fad8dbd622ed2c11ac24638a4d7c84dfeff8df1bcfa3ca0f5b02
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
$ docker pull haproxy@sha256:36aa98fff27dcb2d12c93e68515a6686378c783ea9b1ab1d01ce993a5cbc73e1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.5 MB (36456882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dab1cc236da4978d9fbd4228673dff63592602eba08f6dc940913a862483619`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 07:10:16 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 07:12:59 GMT
ENV HAPROXY_VERSION=2.2.14
# Wed, 12 May 2021 07:12:59 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Wed, 12 May 2021 07:13:00 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Wed, 12 May 2021 07:14:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 07:14:18 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 07:14:19 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 12 May 2021 07:14:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 07:14:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 07:14:20 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a113359dddc15238d26b375f86574b596b4aee1263a9631a7384589c2a02f46`  
		Last Modified: Wed, 12 May 2021 07:18:16 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce57e8a2356e45f88d6ced00b3b9eec7b48f92168ef61338c0e36bee522cdf2b`  
		Last Modified: Wed, 12 May 2021 07:18:47 GMT  
		Size: 9.3 MB (9309017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a21ae969825c26039288a303bddf95391487564b9d309d3500412c82c587f29`  
		Last Modified: Wed, 12 May 2021 07:18:45 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e154e81f6d1cf5ca9e6726aef4a64f9fdd04a24bab984cd21dac17080004feaf`  
		Last Modified: Wed, 12 May 2021 07:18:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.14` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:9794c13ea712f7ed6881ea208e2fd383348c09f3c2742d41ba83d5aa49287433
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33794739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f42f2243feb31e79f986feaa6a5cfd29738ed366dfdd531ddd447c526e466e11`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:55:35 GMT
ADD file:241925c5ca73c99d58f93bc78d7c5bfb6f8b280201a9b55ade45ba0cc054c31d in / 
# Wed, 12 May 2021 00:55:46 GMT
CMD ["bash"]
# Wed, 12 May 2021 02:01:24 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 02:04:19 GMT
ENV HAPROXY_VERSION=2.2.14
# Wed, 12 May 2021 02:04:20 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Wed, 12 May 2021 02:04:22 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Wed, 12 May 2021 02:05:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 02:05:14 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 02:05:15 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 12 May 2021 02:05:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 02:05:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 02:05:23 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:48885a8e20b16cb3bb9d2c3aafc7f040d8609844f69ca8482c42b4829d01b6da`  
		Last Modified: Wed, 12 May 2021 01:10:24 GMT  
		Size: 24.9 MB (24879601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e012f5248a53449f692d1fe91241d026aa60efe5a3dc3f04add4638989918d2a`  
		Last Modified: Wed, 12 May 2021 02:09:37 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9801d19b7ae90b0a5bd4f1fab7b81a0f392825a5831065fe93490ace1e8ba6`  
		Last Modified: Wed, 12 May 2021 02:09:59 GMT  
		Size: 8.9 MB (8913193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6582836c09b2edadce61be9caabd42dc794db9cd00edfceb71ab1e221cb486f`  
		Last Modified: Wed, 12 May 2021 02:09:56 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f8cd4122dc63b8e9afb002f3e28ed09f9c1d716f3a93a725ef97ed8debb5122`  
		Last Modified: Wed, 12 May 2021 02:09:56 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.14` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:1a18cddd7e15cebbc8aeb3db3d49a3ddfbf93d88bc1633cc06ed7710b7276dd8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.5 MB (31471028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bf2c2a94446dabe83faf588182e40770c2024f9c1d3eb442f500177b790bf44`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:03:14 GMT
ADD file:94bf2394dc26abd9f028c2933057a8673c8562e58ec4a0f51bb9bde0a5e4dee0 in / 
# Wed, 12 May 2021 01:03:32 GMT
CMD ["bash"]
# Wed, 16 Jun 2021 12:48:11 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 12:57:16 GMT
ENV HAPROXY_VERSION=2.2.14
# Wed, 16 Jun 2021 12:57:16 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Wed, 16 Jun 2021 12:57:17 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Wed, 16 Jun 2021 12:58:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 16 Jun 2021 12:58:37 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 12:58:37 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 12:58:38 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 16 Jun 2021 12:58:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 12:58:38 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:3035777cd90a3389593bc49a7b39b6f67f9f2679f4e04cc59515f4d5f83ad818`  
		Last Modified: Wed, 12 May 2021 01:19:13 GMT  
		Size: 22.7 MB (22746266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a03e197445bdc67b19867d9e201ef8f2078017e5ad57773c364b31ba9786e0e`  
		Last Modified: Wed, 16 Jun 2021 13:08:37 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a7f6f8c915bd1a6b48f730fa9021df49ddc135d25c3d2647e19653646c81d76`  
		Last Modified: Wed, 16 Jun 2021 13:10:29 GMT  
		Size: 8.7 MB (8722809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b08690033c42ac48ac22c19f5a170c443042811b6478c29ca62b1f8c22d60405`  
		Last Modified: Wed, 16 Jun 2021 13:10:27 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbbb25bc9a88d8d2885e7655078001397c12394c1eb7dfffed08d4afcbf12088`  
		Last Modified: Wed, 16 Jun 2021 13:10:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.14` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:a6fb349acaa1f3153d517b09790399603f3bdc1fb6482b7fc48ba3da4c332ba6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.0 MB (35036109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa08b9b9a2dbb4aa712762bce833331d0f919660933949fc0e6d3e19d535581a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:52:19 GMT
ADD file:91ba1791cab3ad29a1469d1e78f21f4c0b5d3d30598683b7104980604c318854 in / 
# Wed, 12 May 2021 00:52:34 GMT
CMD ["bash"]
# Wed, 16 Jun 2021 00:32:29 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 00:38:12 GMT
ENV HAPROXY_VERSION=2.2.14
# Wed, 16 Jun 2021 00:38:12 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Wed, 16 Jun 2021 00:38:13 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Wed, 16 Jun 2021 00:38:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 16 Jun 2021 00:38:49 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 00:38:50 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 00:38:50 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 16 Jun 2021 00:38:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 00:38:51 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:fcad0c936ea5c12e1c8c4edb81a97c0cde04ee71e7067ee3b246474cf1854d7a`  
		Last Modified: Wed, 12 May 2021 01:02:02 GMT  
		Size: 25.9 MB (25911250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48fc449d8b117694f567c81827185f03f8e4fa5c56b0b6626bb4374515d222c3`  
		Last Modified: Wed, 16 Jun 2021 00:44:41 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d3d0956859fc9b54a7daaf82cec02c80fa7ded81273456f95542cf6d64128d`  
		Last Modified: Wed, 16 Jun 2021 00:46:16 GMT  
		Size: 9.1 MB (9122905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a28d7c7cadd917ff1125c907068bf642dedcbda91d794b5a1f4346fe0cc6417f`  
		Last Modified: Wed, 16 Jun 2021 00:46:14 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:422c3354a6398bfaac49561575a7839a5ede61117177deedfe8833e8b42c3fa1`  
		Last Modified: Wed, 16 Jun 2021 00:46:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.14` - linux; 386

```console
$ docker pull haproxy@sha256:aa53847eb9379394d7b8a20a77cc9e9b7138d4902a964d851575c6d9ffed46d0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36986807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b23c745e4959a63996d75404f0278ae5c8f22759fdb0e9b02270d8923f1f22db`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:39:52 GMT
ADD file:62173a7456d614031a7b20be741983644d9723c734eee663b099ad6b47af7b35 in / 
# Wed, 12 May 2021 00:39:53 GMT
CMD ["bash"]
# Wed, 12 May 2021 05:59:03 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 06:03:15 GMT
ENV HAPROXY_VERSION=2.2.14
# Wed, 12 May 2021 06:03:16 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Wed, 12 May 2021 06:03:16 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Wed, 12 May 2021 06:04:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 06:04:59 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 06:05:00 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 12 May 2021 06:05:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 06:05:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 06:05:02 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:9b548256784c8e079e5953ec08bd26ce8cbaed0d606a5d350b4bcd12710d2192`  
		Last Modified: Wed, 12 May 2021 00:46:39 GMT  
		Size: 27.8 MB (27795074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05508dc89a5d9449eccbd1b8bf3910253f410f4654f50f119641aa3b5dc3e5c6`  
		Last Modified: Wed, 12 May 2021 06:11:24 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7280424fa09c0966592c9cb625c0758831c87c3c81942752dc11cf73a464a65`  
		Last Modified: Wed, 12 May 2021 06:12:11 GMT  
		Size: 9.2 MB (9189784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f788c80822fb5def6f69c985b54c7aa69f7e91ea3824727dfddba7f6772e7d49`  
		Last Modified: Wed, 12 May 2021 06:12:08 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e219cc6901948963354dce74cbefff75cb59aa944edfbd1b9c6bd7fe6efcb853`  
		Last Modified: Wed, 12 May 2021 06:12:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.14` - linux; mips64le

```console
$ docker pull haproxy@sha256:e1c2dad45dff2975488f39cc6dc1abca01182d8e3c4413018bfcda7eba01d3ec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34685329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e11d95019b4bd97a948fe6e9dea89aa8187ca59d9d6a0dd47d148e14159abcb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:09:45 GMT
ADD file:867397d3fb44b3b936a4ff02bbc3a1b760fb6865b5a85efab82fff224f704241 in / 
# Wed, 12 May 2021 01:09:46 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:37:27 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 01:42:33 GMT
ENV HAPROXY_VERSION=2.2.14
# Wed, 12 May 2021 01:42:34 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Wed, 12 May 2021 01:42:34 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Wed, 12 May 2021 01:44:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 01:44:55 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 01:44:56 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 12 May 2021 01:44:57 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 01:44:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 01:44:58 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:09564b0ac149fb24b77cbc75ce6fa5d9ba61bd7c99d11b42bd8339c3bb28e557`  
		Last Modified: Wed, 12 May 2021 01:16:36 GMT  
		Size: 25.8 MB (25812884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18fb24fa0e81746ee8c86b23e726e84be12b3f40b71800e0be7e202dd3e3eae3`  
		Last Modified: Wed, 12 May 2021 01:51:31 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75e4ffbdb19bf59d4597dcfb801a70f24e09fad44e98f3c8dc6778e67706c1cf`  
		Last Modified: Wed, 12 May 2021 01:52:16 GMT  
		Size: 8.9 MB (8870498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d75e58f932335918c79b406d5f66258335ea44229d3618fc37516e0d72a054d2`  
		Last Modified: Wed, 12 May 2021 01:52:07 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3258ef7e9fb3e5cd76b106ec88a0ede2cd56578f8110ca421988021dbf7d5bc5`  
		Last Modified: Wed, 12 May 2021 01:52:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.14` - linux; ppc64le

```console
$ docker pull haproxy@sha256:319f7bae4d558e479dec60b688b69e85a5e50471e599b0c37ca8fe3d0a0d6b2a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40329546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45b00610b81e8a7e221af06253830cb1809d9131f91da6125f39724d6976f5cf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:34:56 GMT
ADD file:3b8146cdc3649d94ad49435c94a21d700ed612ab90f010dcf8b22951b1804d34 in / 
# Wed, 12 May 2021 01:35:02 GMT
CMD ["bash"]
# Wed, 12 May 2021 06:07:29 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 06:22:13 GMT
ENV HAPROXY_VERSION=2.2.14
# Wed, 12 May 2021 06:22:18 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Wed, 12 May 2021 06:22:24 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Wed, 12 May 2021 06:27:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 06:27:44 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 06:27:48 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 12 May 2021 06:28:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 06:28:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 06:28:17 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:f8b445753f60bad25326d018945455601e4a65f124e956dec95c569816f21493`  
		Last Modified: Wed, 12 May 2021 01:44:19 GMT  
		Size: 30.6 MB (30552394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cfafb398e88c2b64b9fb82254775d63718baad006543dee4e7c370a09a23be9`  
		Last Modified: Wed, 12 May 2021 06:57:45 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8acd792e93450fd09e1ff3d6e290d3b6e970010aeee7e4c237d139b092405c6e`  
		Last Modified: Wed, 12 May 2021 06:58:16 GMT  
		Size: 9.8 MB (9775201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d363af0309019290c9372f642779a744c643b8d02797455c2182c9f38b1f70b0`  
		Last Modified: Wed, 12 May 2021 06:58:14 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ffb4d4b17b47ae317fa7c3c086a45eecc3143c7631e6ee7d80677bdbcd263f`  
		Last Modified: Wed, 12 May 2021 06:58:14 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.14` - linux; s390x

```console
$ docker pull haproxy@sha256:88d4465a398b20357befa2125b348a2d4d4fd38846a5b0bc40ff403ce3411bb1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34770545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a9ed7ac70d50e098fef07714cb33343740076728f19c59485f610a0ce2b0d52`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:43:38 GMT
ADD file:77af21d863769b75a5f055b85b2c9d6e878f9d77a4122397ae8dde6b69e945c6 in / 
# Wed, 12 May 2021 00:43:42 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:53:39 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 01:57:10 GMT
ENV HAPROXY_VERSION=2.2.14
# Wed, 12 May 2021 01:57:11 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Wed, 12 May 2021 01:57:11 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Wed, 12 May 2021 01:58:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 01:58:43 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 01:58:43 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 12 May 2021 01:58:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 01:58:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 01:58:46 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:ba4b99e0e723623b64d4ecb8d74102998d32137ea9bcc88b15fd2e4e34b38df9`  
		Last Modified: Wed, 12 May 2021 00:48:03 GMT  
		Size: 25.8 MB (25760171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f6911826fde538e80c00f0d90920d0d7d0a78db315f0bde1ee65726f99f6747`  
		Last Modified: Wed, 12 May 2021 02:04:41 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d13bfedee585dcd4452959bf438e9169b2dfbe277be615e7f46be40ea2a32c9`  
		Last Modified: Wed, 12 May 2021 02:05:02 GMT  
		Size: 9.0 MB (9008423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ad5f54a60f3ec7b35b6b26e386c96f02273dc7605250e397f759936d99af12f`  
		Last Modified: Wed, 12 May 2021 02:05:00 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f74de135cd0b02764be0d540e5d8b8aefa807bf2d0ad81ba1d5dd3d34f08b5f7`  
		Last Modified: Wed, 12 May 2021 02:05:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.2.14-alpine`

```console
$ docker pull haproxy@sha256:ed1a283a87e2326659dd8a78b098da8d7104aaf9487c29af58142cc8bce39f6e
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
$ docker pull haproxy@sha256:843beeb4ab666f0116244dd8500c2242e96a9b966b28e226844b7142d4ad10bd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9270291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:971f6f8cf8b517efcdae3e9823c681d724b6c75df980deff3aa1e8548aa8547f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:34 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Tue, 15 Jun 2021 22:57:34 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 11:05:46 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 11:09:56 GMT
ENV HAPROXY_VERSION=2.2.14
# Wed, 16 Jun 2021 11:09:56 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Wed, 16 Jun 2021 11:09:56 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Wed, 16 Jun 2021 11:11:04 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 16 Jun 2021 11:11:04 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 11:11:04 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 11:11:05 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 16 Jun 2021 11:11:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 11:11:06 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1be2f4fa6ca9f7822eb93cc888d093da91b0748abe26e3ba14d94b6a757977`  
		Last Modified: Wed, 16 Jun 2021 11:14:47 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1a1a2850005aaff668796013f3aeb1cd2c3ce9a5411e8fed8122a085a624467`  
		Last Modified: Wed, 16 Jun 2021 11:15:40 GMT  
		Size: 6.6 MB (6646404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32dbeff2aec20ce0c4ba58aac6d200cfd0a8e2bd7e86d720ce462cefb7ec7442`  
		Last Modified: Wed, 16 Jun 2021 11:15:39 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97e2471f12eacf30f0dbfe3024096f548f75f5825cd44f9240c7ff193be4bf3b`  
		Last Modified: Wed, 16 Jun 2021 11:15:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.14-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:71e9a22b3384bdfd721b422c69e9689f7ee3e1b42433ebc15a63c6de45c588e2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8961889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:197d66e79595a1f39ec57840337cbf3c6b7b804f73406e12bbe983e4cd4ce1c3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:15 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Tue, 15 Jun 2021 23:15:16 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 12:49:38 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 12:58:45 GMT
ENV HAPROXY_VERSION=2.2.14
# Wed, 16 Jun 2021 12:58:46 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Wed, 16 Jun 2021 12:58:46 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Wed, 16 Jun 2021 12:59:41 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 16 Jun 2021 12:59:41 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 12:59:42 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 12:59:42 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 16 Jun 2021 12:59:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 12:59:43 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0137e317a40af64134eac5d8b4d74173e380ac844679531b4f1fbdeeec3eb1f5`  
		Last Modified: Wed, 16 Jun 2021 13:08:54 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80330a3beceeeee15efbab331000f2e900c85c498bd6dabb7c6fcd3b2ac511c0`  
		Last Modified: Wed, 16 Jun 2021 13:10:45 GMT  
		Size: 6.5 MB (6535985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:750fa69962e93c5a7b5988610bf31d54c5f24c8bb78eb4af47aab9f966928d7a`  
		Last Modified: Wed, 16 Jun 2021 13:10:43 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92efec0eb24989a4cef1cc58290c66449deab35e795e1b53b5066511b347508b`  
		Last Modified: Wed, 16 Jun 2021 13:10:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.2.14-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:96a54898cda2d86ab749cae4be00faaa3777756652a65311345c8bfc33b52cfd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9495042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75de00676085ad0b98b06da4e3f90844176a41797f49e804b5e454582d8086fd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 00:33:20 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 00:38:56 GMT
ENV HAPROXY_VERSION=2.2.14
# Wed, 16 Jun 2021 00:38:56 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.14.tar.gz
# Wed, 16 Jun 2021 00:38:57 GMT
ENV HAPROXY_SHA256=6a9b702f04b07786f3e5878de8172a727acfdfdbc1cefe1c7a438df372f2fb61
# Wed, 16 Jun 2021 00:39:40 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 16 Jun 2021 00:39:40 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 00:39:41 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 00:39:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 16 Jun 2021 00:39:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 00:39:42 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd643f981edaf0694f3dad8fb6389455756f11cc027101d1de96b178f289891`  
		Last Modified: Wed, 16 Jun 2021 00:44:55 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ccf648e7b295e02b4acb888c0facdcc8958509fd6903355133ab86ac3e096b0`  
		Last Modified: Wed, 16 Jun 2021 00:46:29 GMT  
		Size: 6.8 MB (6781264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4551c1ee9934cf8bd0c3d9d53e5a60b4127dc8a67714ac54bf67da3a393610`  
		Last Modified: Wed, 16 Jun 2021 00:46:28 GMT  
		Size: 446.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f23d51122d88e10da20d1f5cac248e1819b4226b35f8d651f5e60250d2fe3cf`  
		Last Modified: Wed, 16 Jun 2021 00:46:28 GMT  
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
$ docker pull haproxy@sha256:f7eb9dd6ee951545392bacd7567d6c2d215ae8daa9a43685bd0d6789fa37e161
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
$ docker pull haproxy@sha256:878153ca139f443e3ea3d66f3fc33d5a5b7050f8b361c9f3bf0015b39e137887
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.7 MB (36703569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:397cf3d55facb34bf019a7287d6eee93d61f2e4ca0d2f3f4f02ca5bc8c7fae7b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 07:10:16 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 07:11:29 GMT
ENV HAPROXY_VERSION=2.3.10
# Wed, 12 May 2021 07:11:29 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Wed, 12 May 2021 07:11:29 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Wed, 12 May 2021 07:12:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 07:12:47 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 07:12:48 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 12 May 2021 07:12:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 07:12:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 07:12:50 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a113359dddc15238d26b375f86574b596b4aee1263a9631a7384589c2a02f46`  
		Last Modified: Wed, 12 May 2021 07:18:16 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3f7a3e95320bd3b858bcc5659e5cc4a4da75578d496c29c4d1133d2041e9ba`  
		Last Modified: Wed, 12 May 2021 07:18:31 GMT  
		Size: 9.6 MB (9555706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55f06dddfab5bacfad04ff5c99fb0770226dbd84b6c4dffc74e9a8e0ff999dbc`  
		Last Modified: Wed, 12 May 2021 07:18:29 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78a4c0ac4427c3c1aa020906333824c6efceabc63e14027845c6272f452b622a`  
		Last Modified: Wed, 12 May 2021 07:18:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:d43f1d3562cb2fa60d0be9d3b620282fa984f662e017a9ba144b8bfb84673ad1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (34047800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baa8e4c660c86f16d6f61b99b4994ece5bbc85bc80d0cba37efcf2118117df84`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:55:35 GMT
ADD file:241925c5ca73c99d58f93bc78d7c5bfb6f8b280201a9b55ade45ba0cc054c31d in / 
# Wed, 12 May 2021 00:55:46 GMT
CMD ["bash"]
# Wed, 12 May 2021 02:01:24 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 02:03:00 GMT
ENV HAPROXY_VERSION=2.3.10
# Wed, 12 May 2021 02:03:01 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Wed, 12 May 2021 02:03:03 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Wed, 12 May 2021 02:03:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 02:03:57 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 02:03:58 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 12 May 2021 02:04:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 02:04:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 02:04:03 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:48885a8e20b16cb3bb9d2c3aafc7f040d8609844f69ca8482c42b4829d01b6da`  
		Last Modified: Wed, 12 May 2021 01:10:24 GMT  
		Size: 24.9 MB (24879601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e012f5248a53449f692d1fe91241d026aa60efe5a3dc3f04add4638989918d2a`  
		Last Modified: Wed, 12 May 2021 02:09:37 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a617943ece0d6fd97cbf6ef47775b098381f83e9b6831b128429cbec515c4ae4`  
		Last Modified: Wed, 12 May 2021 02:09:48 GMT  
		Size: 9.2 MB (9166251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b3bb2158860ebb6c2d5b24daf3e90ad819871fb4d01f0afbd90834f34ed3122`  
		Last Modified: Wed, 12 May 2021 02:09:46 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61cef01e5c20289f1994d99ffadab22b8bda428ecdcc045fb38fac18e5b8d181`  
		Last Modified: Wed, 12 May 2021 02:09:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:2496ea1e954a6c885e124ffa1d5865ec1981211dd864d42f5c32fbeb328ccce5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31777742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92f52685b49b9cf5f030b825bc40fdf193698548078eba663d040edd7aaab9e9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:03:14 GMT
ADD file:94bf2394dc26abd9f028c2933057a8673c8562e58ec4a0f51bb9bde0a5e4dee0 in / 
# Wed, 12 May 2021 01:03:32 GMT
CMD ["bash"]
# Wed, 16 Jun 2021 12:48:11 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 12:54:04 GMT
ENV HAPROXY_VERSION=2.3.10
# Wed, 16 Jun 2021 12:54:04 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Wed, 16 Jun 2021 12:54:04 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Wed, 16 Jun 2021 12:55:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 16 Jun 2021 12:55:23 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 12:55:23 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 12:55:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 16 Jun 2021 12:55:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 12:55:25 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:3035777cd90a3389593bc49a7b39b6f67f9f2679f4e04cc59515f4d5f83ad818`  
		Last Modified: Wed, 12 May 2021 01:19:13 GMT  
		Size: 22.7 MB (22746266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a03e197445bdc67b19867d9e201ef8f2078017e5ad57773c364b31ba9786e0e`  
		Last Modified: Wed, 16 Jun 2021 13:08:37 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ad6dc421c7a055a77c01258a3e2c4b0ab1c412de045cbbc4e33383d5980eb0b`  
		Last Modified: Wed, 16 Jun 2021 13:09:58 GMT  
		Size: 9.0 MB (9029523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9844bbf11af539a524ec7e2a3b4364c0f673b838b27c544962dfe19068d75f84`  
		Last Modified: Wed, 16 Jun 2021 13:09:56 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75bcc1c33aa4033f63ea4466f30028db465ed8a62c5d0e9073b9b3fcdc30e8d5`  
		Last Modified: Wed, 16 Jun 2021 13:09:56 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:e53fbc846f66a066e84e62122c5db2b3d27add5622a0e2ab3ffdef21c689552c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.4 MB (35357687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0519ada563649f5cc801ce954144851eeca3d666044da2fa5851eb2f08919b82`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:52:19 GMT
ADD file:91ba1791cab3ad29a1469d1e78f21f4c0b5d3d30598683b7104980604c318854 in / 
# Wed, 12 May 2021 00:52:34 GMT
CMD ["bash"]
# Wed, 16 Jun 2021 00:32:29 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 00:36:37 GMT
ENV HAPROXY_VERSION=2.3.10
# Wed, 16 Jun 2021 00:36:37 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Wed, 16 Jun 2021 00:36:37 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Wed, 16 Jun 2021 00:37:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 16 Jun 2021 00:37:14 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 00:37:14 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 00:37:15 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 16 Jun 2021 00:37:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 00:37:15 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:fcad0c936ea5c12e1c8c4edb81a97c0cde04ee71e7067ee3b246474cf1854d7a`  
		Last Modified: Wed, 12 May 2021 01:02:02 GMT  
		Size: 25.9 MB (25911250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48fc449d8b117694f567c81827185f03f8e4fa5c56b0b6626bb4374515d222c3`  
		Last Modified: Wed, 16 Jun 2021 00:44:41 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1eaaaff0322942d81968b3acd0481937d56b2a1d1f4f1d03a899d5858bdcaf6`  
		Last Modified: Wed, 16 Jun 2021 00:45:50 GMT  
		Size: 9.4 MB (9444483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98860cf8a02be9ef3a49a43f2c27c150ca661925e2e369957ec1d1cf70f0e2e2`  
		Last Modified: Wed, 16 Jun 2021 00:45:48 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da3612db213383517335096472473355290614e78411fed325fa67344fe58a2`  
		Last Modified: Wed, 16 Jun 2021 00:45:48 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3` - linux; 386

```console
$ docker pull haproxy@sha256:70fa271d05b63930402356ff924da43d41c0d1d7c64877038bdde273ab3bc4fd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.2 MB (37215726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e85e17339f305734fade2b3cbfe419a59fe98516c81bb10cc4cd29d7ec8f11b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:39:52 GMT
ADD file:62173a7456d614031a7b20be741983644d9723c734eee663b099ad6b47af7b35 in / 
# Wed, 12 May 2021 00:39:53 GMT
CMD ["bash"]
# Wed, 12 May 2021 05:59:03 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 06:01:09 GMT
ENV HAPROXY_VERSION=2.3.10
# Wed, 12 May 2021 06:01:09 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Wed, 12 May 2021 06:01:09 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Wed, 12 May 2021 06:02:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 06:02:49 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 06:02:50 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 12 May 2021 06:02:52 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 06:02:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 06:02:52 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:9b548256784c8e079e5953ec08bd26ce8cbaed0d606a5d350b4bcd12710d2192`  
		Last Modified: Wed, 12 May 2021 00:46:39 GMT  
		Size: 27.8 MB (27795074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05508dc89a5d9449eccbd1b8bf3910253f410f4654f50f119641aa3b5dc3e5c6`  
		Last Modified: Wed, 12 May 2021 06:11:24 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:849cc39997a093cde0059996ade753c50e1efbec01e4d6681bc4d2c727895b19`  
		Last Modified: Wed, 12 May 2021 06:11:46 GMT  
		Size: 9.4 MB (9418704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c0fe4d04b8b40b9ed9c1efb7bc915b4602216c0936811764c5e5c45627e17f`  
		Last Modified: Wed, 12 May 2021 06:11:43 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47ed114536b8e85a4ce1b667bd7898cc49a45b23fe824577fd430e39c55c2e9a`  
		Last Modified: Wed, 12 May 2021 06:11:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3` - linux; mips64le

```console
$ docker pull haproxy@sha256:f392a9d743f3e049d630298108c18267d054f314fd8ace3d032c9db8a6ca9f6f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.9 MB (34949632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1c339fb5f05e469ba22c11b5a05e185246843328a1ebc2a8be9acd3a67cbdd7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:09:45 GMT
ADD file:867397d3fb44b3b936a4ff02bbc3a1b760fb6865b5a85efab82fff224f704241 in / 
# Wed, 12 May 2021 01:09:46 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:37:27 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 01:40:07 GMT
ENV HAPROXY_VERSION=2.3.10
# Wed, 12 May 2021 01:40:07 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Wed, 12 May 2021 01:40:08 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Wed, 12 May 2021 01:42:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 01:42:26 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 01:42:27 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 12 May 2021 01:42:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 01:42:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 01:42:29 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:09564b0ac149fb24b77cbc75ce6fa5d9ba61bd7c99d11b42bd8339c3bb28e557`  
		Last Modified: Wed, 12 May 2021 01:16:36 GMT  
		Size: 25.8 MB (25812884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18fb24fa0e81746ee8c86b23e726e84be12b3f40b71800e0be7e202dd3e3eae3`  
		Last Modified: Wed, 12 May 2021 01:51:31 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d58c1dddcd12c187ebfebbb18da2ce837151a06e986089a803ac84b27e804e5`  
		Last Modified: Wed, 12 May 2021 01:51:54 GMT  
		Size: 9.1 MB (9134800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83e09c177e0a7da979dc28ee1c4c7eae4184c925df2618883850ae4e8d7cb33e`  
		Last Modified: Wed, 12 May 2021 01:51:47 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a04e9851f9ca945969dc6d2bf1a2214e3c854fe6bae19bffcc499284e0e5dac`  
		Last Modified: Wed, 12 May 2021 01:51:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3` - linux; ppc64le

```console
$ docker pull haproxy@sha256:71729202394a382dd519fd96232e56c7c4260f1e067ba90a87b5d1056d86587d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40596494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5ef273ec4c24979f2b2b97559fa3347d48eb581213239dbf8752cf7ebbcbcaf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:34:56 GMT
ADD file:3b8146cdc3649d94ad49435c94a21d700ed612ab90f010dcf8b22951b1804d34 in / 
# Wed, 12 May 2021 01:35:02 GMT
CMD ["bash"]
# Wed, 12 May 2021 06:07:29 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 06:13:27 GMT
ENV HAPROXY_VERSION=2.3.10
# Wed, 12 May 2021 06:13:36 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Wed, 12 May 2021 06:13:43 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Wed, 12 May 2021 06:21:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 06:21:17 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 06:21:19 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 12 May 2021 06:21:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 06:21:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 06:21:41 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:f8b445753f60bad25326d018945455601e4a65f124e956dec95c569816f21493`  
		Last Modified: Wed, 12 May 2021 01:44:19 GMT  
		Size: 30.6 MB (30552394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cfafb398e88c2b64b9fb82254775d63718baad006543dee4e7c370a09a23be9`  
		Last Modified: Wed, 12 May 2021 06:57:45 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca38ade2c4b0dbe25972ab7df2f59983c12e78922ba921fc2b36425e64976161`  
		Last Modified: Wed, 12 May 2021 06:58:00 GMT  
		Size: 10.0 MB (10042150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e0269d6abfa761cb3bde1fe0e9732cab73d90156b2bbc126ba1ea0f34029d7d`  
		Last Modified: Wed, 12 May 2021 06:57:58 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cda1d8de82dbc81bc095c4a849cc0de64f7e7f861c74bfc9057fa2bd94d5e420`  
		Last Modified: Wed, 12 May 2021 06:57:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3` - linux; s390x

```console
$ docker pull haproxy@sha256:e5327e973a3af0626d84df85292d6fdb80d6824f74a79fff1310025a7f5b99b1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35053171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:641efd705ce48f0b0aedd7f8169bd9ce78adc1092b1923105701aff2fb74ce2f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:43:38 GMT
ADD file:77af21d863769b75a5f055b85b2c9d6e878f9d77a4122397ae8dde6b69e945c6 in / 
# Wed, 12 May 2021 00:43:42 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:53:39 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 01:55:16 GMT
ENV HAPROXY_VERSION=2.3.10
# Wed, 12 May 2021 01:55:16 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Wed, 12 May 2021 01:55:17 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Wed, 12 May 2021 01:56:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 01:56:47 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 01:56:47 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 12 May 2021 01:56:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 01:56:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 01:56:50 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:ba4b99e0e723623b64d4ecb8d74102998d32137ea9bcc88b15fd2e4e34b38df9`  
		Last Modified: Wed, 12 May 2021 00:48:03 GMT  
		Size: 25.8 MB (25760171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f6911826fde538e80c00f0d90920d0d7d0a78db315f0bde1ee65726f99f6747`  
		Last Modified: Wed, 12 May 2021 02:04:41 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfa01d4e827245f4b78cbf9e16f268159ae2f238c1dde6a31a8ac314a0edead3`  
		Last Modified: Wed, 12 May 2021 02:04:51 GMT  
		Size: 9.3 MB (9291050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee074595907f3cf4dfbbd7aaa8ed781fe222645e28bc2ef60d5d6e2d78b906a`  
		Last Modified: Wed, 12 May 2021 02:04:49 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12cc438138dc10efdca9b812bd4031fc1d8e7a1765d667578c0d352b1d8fa8b7`  
		Last Modified: Wed, 12 May 2021 02:04:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.3-alpine`

```console
$ docker pull haproxy@sha256:6adfd05299ec5853767a07a9be5927ed7af4a1d3090a11023fc5dee9bcbc61cc
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
$ docker pull haproxy@sha256:7e565aed42b751cb26411e6c1d88e39cf7e8fc171540a33f4422a10fb7301f94
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9602774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21c13da72decae55e6ac8c66fd932d9523d8444ebcbaa2541a4f3c0628ac4dcf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:34 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Tue, 15 Jun 2021 22:57:34 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 11:05:46 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 11:08:42 GMT
ENV HAPROXY_VERSION=2.3.10
# Wed, 16 Jun 2021 11:08:42 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Wed, 16 Jun 2021 11:08:42 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Wed, 16 Jun 2021 11:09:45 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 16 Jun 2021 11:09:45 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 11:09:45 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 11:09:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 16 Jun 2021 11:09:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 11:09:46 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1be2f4fa6ca9f7822eb93cc888d093da91b0748abe26e3ba14d94b6a757977`  
		Last Modified: Wed, 16 Jun 2021 11:14:47 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:421eee1632f6494727f107f264b2c31e6d8fd065cc60ad004324e369eef85bac`  
		Last Modified: Wed, 16 Jun 2021 11:15:26 GMT  
		Size: 7.0 MB (6978889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d8cd13718b7346d706799522f00a9e96153bcf071b9f069bd1b8ee091d1498`  
		Last Modified: Wed, 16 Jun 2021 11:15:25 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbc47ad843ba2363324daa094b77a862c6b81fd1426205ecc119f95eb88f03d9`  
		Last Modified: Wed, 16 Jun 2021 11:15:25 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:bf1e38a4b623c746033e9fd425edc198d892fdf7ad5a88c4ca0b0ee7ac33d1b3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9294238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edb6abc42f9533d693ff60edb2ba783b2cabe41c5934e646506e63dd59687c0f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:15 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Tue, 15 Jun 2021 23:15:16 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 12:49:38 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 12:55:33 GMT
ENV HAPROXY_VERSION=2.3.10
# Wed, 16 Jun 2021 12:55:33 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Wed, 16 Jun 2021 12:55:34 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Wed, 16 Jun 2021 12:57:01 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 16 Jun 2021 12:57:01 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 12:57:02 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 12:57:03 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 16 Jun 2021 12:57:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 12:57:03 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0137e317a40af64134eac5d8b4d74173e380ac844679531b4f1fbdeeec3eb1f5`  
		Last Modified: Wed, 16 Jun 2021 13:08:54 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e84e72dbee22d1ac49a6985cdd6b056e2402d4873fb83d3dad1811e6ae3148f`  
		Last Modified: Wed, 16 Jun 2021 13:10:14 GMT  
		Size: 6.9 MB (6868335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a64fd2254bdb4bc39153370563299643f326db4c721acde7f8736ad84ae11dd`  
		Last Modified: Wed, 16 Jun 2021 13:10:11 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c3ef255e673ff2987950c1e13fe53874bc56e45d2212514b994f81a8c979fef`  
		Last Modified: Wed, 16 Jun 2021 13:10:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:2c74f3aaebcc0407c15661196a96034eedb9ceade7e908b424d938fe3eb84803
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.8 MB (9810477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cea2a9db36132a78772ef355958be453e53d451378930e86277bcee0d6dfe6ed`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 00:33:20 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 00:37:21 GMT
ENV HAPROXY_VERSION=2.3.10
# Wed, 16 Jun 2021 00:37:21 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Wed, 16 Jun 2021 00:37:21 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Wed, 16 Jun 2021 00:38:05 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 16 Jun 2021 00:38:05 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 00:38:05 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 00:38:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 16 Jun 2021 00:38:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 00:38:06 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd643f981edaf0694f3dad8fb6389455756f11cc027101d1de96b178f289891`  
		Last Modified: Wed, 16 Jun 2021 00:44:55 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:230e3af7a1cbeba09e771f7ee68dda242fb159cff58a5785a70067fb9fcd7b77`  
		Last Modified: Wed, 16 Jun 2021 00:46:02 GMT  
		Size: 7.1 MB (7096696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:685a3b78a41c28e673dc6215b7187d1409c4f9e55b70b0c9913c20e34063ee6a`  
		Last Modified: Wed, 16 Jun 2021 00:46:01 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a2a6a3b01d623a2e05550669f369c628087fe8b5898391412c3a22b4041254`  
		Last Modified: Wed, 16 Jun 2021 00:46:01 GMT  
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
$ docker pull haproxy@sha256:f7eb9dd6ee951545392bacd7567d6c2d215ae8daa9a43685bd0d6789fa37e161
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
$ docker pull haproxy@sha256:878153ca139f443e3ea3d66f3fc33d5a5b7050f8b361c9f3bf0015b39e137887
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.7 MB (36703569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:397cf3d55facb34bf019a7287d6eee93d61f2e4ca0d2f3f4f02ca5bc8c7fae7b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 07:10:16 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 07:11:29 GMT
ENV HAPROXY_VERSION=2.3.10
# Wed, 12 May 2021 07:11:29 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Wed, 12 May 2021 07:11:29 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Wed, 12 May 2021 07:12:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 07:12:47 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 07:12:48 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 12 May 2021 07:12:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 07:12:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 07:12:50 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a113359dddc15238d26b375f86574b596b4aee1263a9631a7384589c2a02f46`  
		Last Modified: Wed, 12 May 2021 07:18:16 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3f7a3e95320bd3b858bcc5659e5cc4a4da75578d496c29c4d1133d2041e9ba`  
		Last Modified: Wed, 12 May 2021 07:18:31 GMT  
		Size: 9.6 MB (9555706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55f06dddfab5bacfad04ff5c99fb0770226dbd84b6c4dffc74e9a8e0ff999dbc`  
		Last Modified: Wed, 12 May 2021 07:18:29 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78a4c0ac4427c3c1aa020906333824c6efceabc63e14027845c6272f452b622a`  
		Last Modified: Wed, 12 May 2021 07:18:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.10` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:d43f1d3562cb2fa60d0be9d3b620282fa984f662e017a9ba144b8bfb84673ad1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (34047800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baa8e4c660c86f16d6f61b99b4994ece5bbc85bc80d0cba37efcf2118117df84`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:55:35 GMT
ADD file:241925c5ca73c99d58f93bc78d7c5bfb6f8b280201a9b55ade45ba0cc054c31d in / 
# Wed, 12 May 2021 00:55:46 GMT
CMD ["bash"]
# Wed, 12 May 2021 02:01:24 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 02:03:00 GMT
ENV HAPROXY_VERSION=2.3.10
# Wed, 12 May 2021 02:03:01 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Wed, 12 May 2021 02:03:03 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Wed, 12 May 2021 02:03:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 02:03:57 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 02:03:58 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 12 May 2021 02:04:01 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 02:04:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 02:04:03 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:48885a8e20b16cb3bb9d2c3aafc7f040d8609844f69ca8482c42b4829d01b6da`  
		Last Modified: Wed, 12 May 2021 01:10:24 GMT  
		Size: 24.9 MB (24879601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e012f5248a53449f692d1fe91241d026aa60efe5a3dc3f04add4638989918d2a`  
		Last Modified: Wed, 12 May 2021 02:09:37 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a617943ece0d6fd97cbf6ef47775b098381f83e9b6831b128429cbec515c4ae4`  
		Last Modified: Wed, 12 May 2021 02:09:48 GMT  
		Size: 9.2 MB (9166251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b3bb2158860ebb6c2d5b24daf3e90ad819871fb4d01f0afbd90834f34ed3122`  
		Last Modified: Wed, 12 May 2021 02:09:46 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61cef01e5c20289f1994d99ffadab22b8bda428ecdcc045fb38fac18e5b8d181`  
		Last Modified: Wed, 12 May 2021 02:09:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.10` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:2496ea1e954a6c885e124ffa1d5865ec1981211dd864d42f5c32fbeb328ccce5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31777742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92f52685b49b9cf5f030b825bc40fdf193698548078eba663d040edd7aaab9e9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:03:14 GMT
ADD file:94bf2394dc26abd9f028c2933057a8673c8562e58ec4a0f51bb9bde0a5e4dee0 in / 
# Wed, 12 May 2021 01:03:32 GMT
CMD ["bash"]
# Wed, 16 Jun 2021 12:48:11 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 12:54:04 GMT
ENV HAPROXY_VERSION=2.3.10
# Wed, 16 Jun 2021 12:54:04 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Wed, 16 Jun 2021 12:54:04 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Wed, 16 Jun 2021 12:55:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 16 Jun 2021 12:55:23 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 12:55:23 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 12:55:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 16 Jun 2021 12:55:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 12:55:25 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:3035777cd90a3389593bc49a7b39b6f67f9f2679f4e04cc59515f4d5f83ad818`  
		Last Modified: Wed, 12 May 2021 01:19:13 GMT  
		Size: 22.7 MB (22746266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a03e197445bdc67b19867d9e201ef8f2078017e5ad57773c364b31ba9786e0e`  
		Last Modified: Wed, 16 Jun 2021 13:08:37 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ad6dc421c7a055a77c01258a3e2c4b0ab1c412de045cbbc4e33383d5980eb0b`  
		Last Modified: Wed, 16 Jun 2021 13:09:58 GMT  
		Size: 9.0 MB (9029523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9844bbf11af539a524ec7e2a3b4364c0f673b838b27c544962dfe19068d75f84`  
		Last Modified: Wed, 16 Jun 2021 13:09:56 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75bcc1c33aa4033f63ea4466f30028db465ed8a62c5d0e9073b9b3fcdc30e8d5`  
		Last Modified: Wed, 16 Jun 2021 13:09:56 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.10` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:e53fbc846f66a066e84e62122c5db2b3d27add5622a0e2ab3ffdef21c689552c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.4 MB (35357687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0519ada563649f5cc801ce954144851eeca3d666044da2fa5851eb2f08919b82`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:52:19 GMT
ADD file:91ba1791cab3ad29a1469d1e78f21f4c0b5d3d30598683b7104980604c318854 in / 
# Wed, 12 May 2021 00:52:34 GMT
CMD ["bash"]
# Wed, 16 Jun 2021 00:32:29 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 00:36:37 GMT
ENV HAPROXY_VERSION=2.3.10
# Wed, 16 Jun 2021 00:36:37 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Wed, 16 Jun 2021 00:36:37 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Wed, 16 Jun 2021 00:37:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 16 Jun 2021 00:37:14 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 00:37:14 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 00:37:15 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 16 Jun 2021 00:37:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 00:37:15 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:fcad0c936ea5c12e1c8c4edb81a97c0cde04ee71e7067ee3b246474cf1854d7a`  
		Last Modified: Wed, 12 May 2021 01:02:02 GMT  
		Size: 25.9 MB (25911250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48fc449d8b117694f567c81827185f03f8e4fa5c56b0b6626bb4374515d222c3`  
		Last Modified: Wed, 16 Jun 2021 00:44:41 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1eaaaff0322942d81968b3acd0481937d56b2a1d1f4f1d03a899d5858bdcaf6`  
		Last Modified: Wed, 16 Jun 2021 00:45:50 GMT  
		Size: 9.4 MB (9444483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98860cf8a02be9ef3a49a43f2c27c150ca661925e2e369957ec1d1cf70f0e2e2`  
		Last Modified: Wed, 16 Jun 2021 00:45:48 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da3612db213383517335096472473355290614e78411fed325fa67344fe58a2`  
		Last Modified: Wed, 16 Jun 2021 00:45:48 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.10` - linux; 386

```console
$ docker pull haproxy@sha256:70fa271d05b63930402356ff924da43d41c0d1d7c64877038bdde273ab3bc4fd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.2 MB (37215726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e85e17339f305734fade2b3cbfe419a59fe98516c81bb10cc4cd29d7ec8f11b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:39:52 GMT
ADD file:62173a7456d614031a7b20be741983644d9723c734eee663b099ad6b47af7b35 in / 
# Wed, 12 May 2021 00:39:53 GMT
CMD ["bash"]
# Wed, 12 May 2021 05:59:03 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 06:01:09 GMT
ENV HAPROXY_VERSION=2.3.10
# Wed, 12 May 2021 06:01:09 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Wed, 12 May 2021 06:01:09 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Wed, 12 May 2021 06:02:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 06:02:49 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 06:02:50 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 12 May 2021 06:02:52 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 06:02:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 06:02:52 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:9b548256784c8e079e5953ec08bd26ce8cbaed0d606a5d350b4bcd12710d2192`  
		Last Modified: Wed, 12 May 2021 00:46:39 GMT  
		Size: 27.8 MB (27795074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05508dc89a5d9449eccbd1b8bf3910253f410f4654f50f119641aa3b5dc3e5c6`  
		Last Modified: Wed, 12 May 2021 06:11:24 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:849cc39997a093cde0059996ade753c50e1efbec01e4d6681bc4d2c727895b19`  
		Last Modified: Wed, 12 May 2021 06:11:46 GMT  
		Size: 9.4 MB (9418704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c0fe4d04b8b40b9ed9c1efb7bc915b4602216c0936811764c5e5c45627e17f`  
		Last Modified: Wed, 12 May 2021 06:11:43 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47ed114536b8e85a4ce1b667bd7898cc49a45b23fe824577fd430e39c55c2e9a`  
		Last Modified: Wed, 12 May 2021 06:11:43 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.10` - linux; mips64le

```console
$ docker pull haproxy@sha256:f392a9d743f3e049d630298108c18267d054f314fd8ace3d032c9db8a6ca9f6f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.9 MB (34949632 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1c339fb5f05e469ba22c11b5a05e185246843328a1ebc2a8be9acd3a67cbdd7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:09:45 GMT
ADD file:867397d3fb44b3b936a4ff02bbc3a1b760fb6865b5a85efab82fff224f704241 in / 
# Wed, 12 May 2021 01:09:46 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:37:27 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 01:40:07 GMT
ENV HAPROXY_VERSION=2.3.10
# Wed, 12 May 2021 01:40:07 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Wed, 12 May 2021 01:40:08 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Wed, 12 May 2021 01:42:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 01:42:26 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 01:42:27 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 12 May 2021 01:42:29 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 01:42:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 01:42:29 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:09564b0ac149fb24b77cbc75ce6fa5d9ba61bd7c99d11b42bd8339c3bb28e557`  
		Last Modified: Wed, 12 May 2021 01:16:36 GMT  
		Size: 25.8 MB (25812884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18fb24fa0e81746ee8c86b23e726e84be12b3f40b71800e0be7e202dd3e3eae3`  
		Last Modified: Wed, 12 May 2021 01:51:31 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d58c1dddcd12c187ebfebbb18da2ce837151a06e986089a803ac84b27e804e5`  
		Last Modified: Wed, 12 May 2021 01:51:54 GMT  
		Size: 9.1 MB (9134800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83e09c177e0a7da979dc28ee1c4c7eae4184c925df2618883850ae4e8d7cb33e`  
		Last Modified: Wed, 12 May 2021 01:51:47 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a04e9851f9ca945969dc6d2bf1a2214e3c854fe6bae19bffcc499284e0e5dac`  
		Last Modified: Wed, 12 May 2021 01:51:47 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.10` - linux; ppc64le

```console
$ docker pull haproxy@sha256:71729202394a382dd519fd96232e56c7c4260f1e067ba90a87b5d1056d86587d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40596494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5ef273ec4c24979f2b2b97559fa3347d48eb581213239dbf8752cf7ebbcbcaf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:34:56 GMT
ADD file:3b8146cdc3649d94ad49435c94a21d700ed612ab90f010dcf8b22951b1804d34 in / 
# Wed, 12 May 2021 01:35:02 GMT
CMD ["bash"]
# Wed, 12 May 2021 06:07:29 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 06:13:27 GMT
ENV HAPROXY_VERSION=2.3.10
# Wed, 12 May 2021 06:13:36 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Wed, 12 May 2021 06:13:43 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Wed, 12 May 2021 06:21:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 06:21:17 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 06:21:19 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 12 May 2021 06:21:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 06:21:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 06:21:41 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:f8b445753f60bad25326d018945455601e4a65f124e956dec95c569816f21493`  
		Last Modified: Wed, 12 May 2021 01:44:19 GMT  
		Size: 30.6 MB (30552394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cfafb398e88c2b64b9fb82254775d63718baad006543dee4e7c370a09a23be9`  
		Last Modified: Wed, 12 May 2021 06:57:45 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca38ade2c4b0dbe25972ab7df2f59983c12e78922ba921fc2b36425e64976161`  
		Last Modified: Wed, 12 May 2021 06:58:00 GMT  
		Size: 10.0 MB (10042150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e0269d6abfa761cb3bde1fe0e9732cab73d90156b2bbc126ba1ea0f34029d7d`  
		Last Modified: Wed, 12 May 2021 06:57:58 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cda1d8de82dbc81bc095c4a849cc0de64f7e7f861c74bfc9057fa2bd94d5e420`  
		Last Modified: Wed, 12 May 2021 06:57:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.10` - linux; s390x

```console
$ docker pull haproxy@sha256:e5327e973a3af0626d84df85292d6fdb80d6824f74a79fff1310025a7f5b99b1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35053171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:641efd705ce48f0b0aedd7f8169bd9ce78adc1092b1923105701aff2fb74ce2f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:43:38 GMT
ADD file:77af21d863769b75a5f055b85b2c9d6e878f9d77a4122397ae8dde6b69e945c6 in / 
# Wed, 12 May 2021 00:43:42 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:53:39 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 12 May 2021 01:55:16 GMT
ENV HAPROXY_VERSION=2.3.10
# Wed, 12 May 2021 01:55:16 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Wed, 12 May 2021 01:55:17 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Wed, 12 May 2021 01:56:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 12 May 2021 01:56:47 GMT
STOPSIGNAL SIGUSR1
# Wed, 12 May 2021 01:56:47 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 12 May 2021 01:56:49 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 12 May 2021 01:56:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 12 May 2021 01:56:50 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:ba4b99e0e723623b64d4ecb8d74102998d32137ea9bcc88b15fd2e4e34b38df9`  
		Last Modified: Wed, 12 May 2021 00:48:03 GMT  
		Size: 25.8 MB (25760171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f6911826fde538e80c00f0d90920d0d7d0a78db315f0bde1ee65726f99f6747`  
		Last Modified: Wed, 12 May 2021 02:04:41 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfa01d4e827245f4b78cbf9e16f268159ae2f238c1dde6a31a8ac314a0edead3`  
		Last Modified: Wed, 12 May 2021 02:04:51 GMT  
		Size: 9.3 MB (9291050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee074595907f3cf4dfbbd7aaa8ed781fe222645e28bc2ef60d5d6e2d78b906a`  
		Last Modified: Wed, 12 May 2021 02:04:49 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12cc438138dc10efdca9b812bd4031fc1d8e7a1765d667578c0d352b1d8fa8b7`  
		Last Modified: Wed, 12 May 2021 02:04:49 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.3.10-alpine`

```console
$ docker pull haproxy@sha256:6adfd05299ec5853767a07a9be5927ed7af4a1d3090a11023fc5dee9bcbc61cc
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
$ docker pull haproxy@sha256:7e565aed42b751cb26411e6c1d88e39cf7e8fc171540a33f4422a10fb7301f94
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9602774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21c13da72decae55e6ac8c66fd932d9523d8444ebcbaa2541a4f3c0628ac4dcf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:34 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Tue, 15 Jun 2021 22:57:34 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 11:05:46 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 11:08:42 GMT
ENV HAPROXY_VERSION=2.3.10
# Wed, 16 Jun 2021 11:08:42 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Wed, 16 Jun 2021 11:08:42 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Wed, 16 Jun 2021 11:09:45 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 16 Jun 2021 11:09:45 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 11:09:45 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 11:09:46 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 16 Jun 2021 11:09:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 11:09:46 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1be2f4fa6ca9f7822eb93cc888d093da91b0748abe26e3ba14d94b6a757977`  
		Last Modified: Wed, 16 Jun 2021 11:14:47 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:421eee1632f6494727f107f264b2c31e6d8fd065cc60ad004324e369eef85bac`  
		Last Modified: Wed, 16 Jun 2021 11:15:26 GMT  
		Size: 7.0 MB (6978889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d8cd13718b7346d706799522f00a9e96153bcf071b9f069bd1b8ee091d1498`  
		Last Modified: Wed, 16 Jun 2021 11:15:25 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbc47ad843ba2363324daa094b77a862c6b81fd1426205ecc119f95eb88f03d9`  
		Last Modified: Wed, 16 Jun 2021 11:15:25 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.10-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:bf1e38a4b623c746033e9fd425edc198d892fdf7ad5a88c4ca0b0ee7ac33d1b3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9294238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edb6abc42f9533d693ff60edb2ba783b2cabe41c5934e646506e63dd59687c0f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:15 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Tue, 15 Jun 2021 23:15:16 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 12:49:38 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 12:55:33 GMT
ENV HAPROXY_VERSION=2.3.10
# Wed, 16 Jun 2021 12:55:33 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Wed, 16 Jun 2021 12:55:34 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Wed, 16 Jun 2021 12:57:01 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 16 Jun 2021 12:57:01 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 12:57:02 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 12:57:03 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 16 Jun 2021 12:57:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 12:57:03 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0137e317a40af64134eac5d8b4d74173e380ac844679531b4f1fbdeeec3eb1f5`  
		Last Modified: Wed, 16 Jun 2021 13:08:54 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e84e72dbee22d1ac49a6985cdd6b056e2402d4873fb83d3dad1811e6ae3148f`  
		Last Modified: Wed, 16 Jun 2021 13:10:14 GMT  
		Size: 6.9 MB (6868335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a64fd2254bdb4bc39153370563299643f326db4c721acde7f8736ad84ae11dd`  
		Last Modified: Wed, 16 Jun 2021 13:10:11 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c3ef255e673ff2987950c1e13fe53874bc56e45d2212514b994f81a8c979fef`  
		Last Modified: Wed, 16 Jun 2021 13:10:11 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.3.10-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:2c74f3aaebcc0407c15661196a96034eedb9ceade7e908b424d938fe3eb84803
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.8 MB (9810477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cea2a9db36132a78772ef355958be453e53d451378930e86277bcee0d6dfe6ed`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 00:33:20 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 00:37:21 GMT
ENV HAPROXY_VERSION=2.3.10
# Wed, 16 Jun 2021 00:37:21 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.3/src/haproxy-2.3.10.tar.gz
# Wed, 16 Jun 2021 00:37:21 GMT
ENV HAPROXY_SHA256=9946e0cfc83f29072b3431e37246221cf9d4a9d28a158c075714d345266f4f35
# Wed, 16 Jun 2021 00:38:05 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 16 Jun 2021 00:38:05 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 00:38:05 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 00:38:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh / # backwards compat
# Wed, 16 Jun 2021 00:38:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 00:38:06 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd643f981edaf0694f3dad8fb6389455756f11cc027101d1de96b178f289891`  
		Last Modified: Wed, 16 Jun 2021 00:44:55 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:230e3af7a1cbeba09e771f7ee68dda242fb159cff58a5785a70067fb9fcd7b77`  
		Last Modified: Wed, 16 Jun 2021 00:46:02 GMT  
		Size: 7.1 MB (7096696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:685a3b78a41c28e673dc6215b7187d1409c4f9e55b70b0c9913c20e34063ee6a`  
		Last Modified: Wed, 16 Jun 2021 00:46:01 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a2a6a3b01d623a2e05550669f369c628087fe8b5898391412c3a22b4041254`  
		Last Modified: Wed, 16 Jun 2021 00:46:01 GMT  
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

## `haproxy:2.4`

```console
$ docker pull haproxy@sha256:e07d23cbfa10322d03ab965fab14a83793a3cf210cf6598b9bac04441b931b88
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

### `haproxy:2.4` - linux; amd64

```console
$ docker pull haproxy@sha256:bf2db25a5ee139ffcb728ea9acea1b0671fdcd761670753f6a9eb493fe7a439f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.2 MB (37226610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b68c771805b9ba3241a23c54e6f43e04a27da28659bca2760faca537bef973cd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 07:10:16 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:21:49 GMT
ENV HAPROXY_VERSION=2.4.0
# Fri, 14 May 2021 19:21:49 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Fri, 14 May 2021 19:21:49 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Fri, 14 May 2021 19:22:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 14 May 2021 19:22:36 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:22:36 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:22:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:22:37 GMT
USER haproxy
# Fri, 14 May 2021 19:22:37 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a113359dddc15238d26b375f86574b596b4aee1263a9631a7384589c2a02f46`  
		Last Modified: Wed, 12 May 2021 07:18:16 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e62dbde04094c3619ac833a9545588b66612ff4a0b35b59c7624708810658bb3`  
		Last Modified: Fri, 14 May 2021 19:25:20 GMT  
		Size: 10.1 MB (10078868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba498b86933facd6fdd59d94d7db13019b879e7cc25d041a68633d89e0494e2`  
		Last Modified: Fri, 14 May 2021 19:25:19 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:9bbe3920a362fbdd01643eb1d30ed94397a87cddd058275eccf322d60149697c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.6 MB (34593921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08b4c280b3718ed88ca7f0c20d62f39aa02eeacfcf409626e51607b0ac6f0949`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:55:35 GMT
ADD file:241925c5ca73c99d58f93bc78d7c5bfb6f8b280201a9b55ade45ba0cc054c31d in / 
# Wed, 12 May 2021 00:55:46 GMT
CMD ["bash"]
# Wed, 12 May 2021 02:01:24 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:49:51 GMT
ENV HAPROXY_VERSION=2.4.0
# Fri, 14 May 2021 19:49:53 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Fri, 14 May 2021 19:49:53 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Fri, 14 May 2021 19:50:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 14 May 2021 19:50:56 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:51:04 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:51:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:51:06 GMT
USER haproxy
# Fri, 14 May 2021 19:51:09 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:48885a8e20b16cb3bb9d2c3aafc7f040d8609844f69ca8482c42b4829d01b6da`  
		Last Modified: Wed, 12 May 2021 01:10:24 GMT  
		Size: 24.9 MB (24879601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e012f5248a53449f692d1fe91241d026aa60efe5a3dc3f04add4638989918d2a`  
		Last Modified: Wed, 12 May 2021 02:09:37 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:723c7fb393e70925e6268f228609b020286d9861091b490e8d2a0f254c59a09c`  
		Last Modified: Fri, 14 May 2021 19:52:16 GMT  
		Size: 9.7 MB (9712493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:001bde1f3aa007c516863db1818955f87f02ec4c19a730bf84f2399ddac9c7e2`  
		Last Modified: Fri, 14 May 2021 19:52:13 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:b5345ed4dd11a7cb423f4f59dbe9c7ba7cd2abe7afb893b77ddbfb32e5a77302
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.3 MB (32300104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c11a7eb8b982fbc0502c09a9021ba71ea4f9fed9830124aad9547d935b4dcd71`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:03:14 GMT
ADD file:94bf2394dc26abd9f028c2933057a8673c8562e58ec4a0f51bb9bde0a5e4dee0 in / 
# Wed, 12 May 2021 01:03:32 GMT
CMD ["bash"]
# Wed, 16 Jun 2021 12:48:11 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 12:50:51 GMT
ENV HAPROXY_VERSION=2.4.0
# Wed, 16 Jun 2021 12:50:51 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Wed, 16 Jun 2021 12:50:52 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Wed, 16 Jun 2021 12:51:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 16 Jun 2021 12:51:50 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 12:51:51 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 12:51:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 12:51:51 GMT
USER haproxy
# Wed, 16 Jun 2021 12:51:52 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:3035777cd90a3389593bc49a7b39b6f67f9f2679f4e04cc59515f4d5f83ad818`  
		Last Modified: Wed, 12 May 2021 01:19:13 GMT  
		Size: 22.7 MB (22746266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a03e197445bdc67b19867d9e201ef8f2078017e5ad57773c364b31ba9786e0e`  
		Last Modified: Wed, 16 Jun 2021 13:08:37 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dea3a7558a13f5154fb9ce6385d9667552cb71886d1e477e2519abbd5734d85`  
		Last Modified: Wed, 16 Jun 2021 13:09:11 GMT  
		Size: 9.6 MB (9552006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92403e8a9c35756b9b7e782fa08d4faae23520c5824807583c41db0674112c28`  
		Last Modified: Wed, 16 Jun 2021 13:09:08 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:7c4943ca2e6c7241331ed74abbd91deb9045a58ff899ea1c47d32878cce737fc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35869597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aad490d428518fedc8dee040fcd2c90f725415ef49be148b71b8c0e7929f2bdb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:52:19 GMT
ADD file:91ba1791cab3ad29a1469d1e78f21f4c0b5d3d30598683b7104980604c318854 in / 
# Wed, 12 May 2021 00:52:34 GMT
CMD ["bash"]
# Wed, 16 Jun 2021 00:32:29 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 00:34:32 GMT
ENV HAPROXY_VERSION=2.4.0
# Wed, 16 Jun 2021 00:34:33 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Wed, 16 Jun 2021 00:34:33 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Wed, 16 Jun 2021 00:35:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 16 Jun 2021 00:35:13 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 00:35:14 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 00:35:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 00:35:14 GMT
USER haproxy
# Wed, 16 Jun 2021 00:35:14 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:fcad0c936ea5c12e1c8c4edb81a97c0cde04ee71e7067ee3b246474cf1854d7a`  
		Last Modified: Wed, 12 May 2021 01:02:02 GMT  
		Size: 25.9 MB (25911250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48fc449d8b117694f567c81827185f03f8e4fa5c56b0b6626bb4374515d222c3`  
		Last Modified: Wed, 16 Jun 2021 00:44:41 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:928814acb1c13f0fd28a553528d1e135f7ffeb4a27bee2232022efda91ed70f2`  
		Last Modified: Wed, 16 Jun 2021 00:45:10 GMT  
		Size: 10.0 MB (9956513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c75f63ea187e14fb0d9052b1e9be0ce47a1c6d1dd4f03382ac3db42f865452`  
		Last Modified: Wed, 16 Jun 2021 00:45:08 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4` - linux; 386

```console
$ docker pull haproxy@sha256:65807594f3fdb74f4aeb45cfb58775a8e9e60d00cf4ff637bdcf4343938cfc9c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.7 MB (37714061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b65e677154b7269853270de51028128fb357bdb375ab0bb6229de8bcc8796694`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:39:52 GMT
ADD file:62173a7456d614031a7b20be741983644d9723c734eee663b099ad6b47af7b35 in / 
# Wed, 12 May 2021 00:39:53 GMT
CMD ["bash"]
# Wed, 12 May 2021 05:59:03 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:43:27 GMT
ENV HAPROXY_VERSION=2.4.0
# Fri, 14 May 2021 19:43:27 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Fri, 14 May 2021 19:43:28 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Fri, 14 May 2021 19:44:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 14 May 2021 19:44:27 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:44:27 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:44:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:44:27 GMT
USER haproxy
# Fri, 14 May 2021 19:44:28 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:9b548256784c8e079e5953ec08bd26ce8cbaed0d606a5d350b4bcd12710d2192`  
		Last Modified: Wed, 12 May 2021 00:46:39 GMT  
		Size: 27.8 MB (27795074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05508dc89a5d9449eccbd1b8bf3910253f410f4654f50f119641aa3b5dc3e5c6`  
		Last Modified: Wed, 12 May 2021 06:11:24 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c528b6c319705bef71d9a02c957c8f71879b2f0d4911c0e693640c3485da157`  
		Last Modified: Fri, 14 May 2021 19:49:52 GMT  
		Size: 9.9 MB (9917160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20b09ad55a92c274b5ad2a914359180d1b3a163768611adacc46db20bed561f2`  
		Last Modified: Fri, 14 May 2021 19:49:49 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4` - linux; mips64le

```console
$ docker pull haproxy@sha256:9eb21e12824743325f9a8ef93e2a38ec1eee12f374450edafc57ada973db7e36
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.5 MB (35507073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f68f334085d45c2aedb154ace750cc256f9188c28fec0134800ffcdf4d83c465`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:09:45 GMT
ADD file:867397d3fb44b3b936a4ff02bbc3a1b760fb6865b5a85efab82fff224f704241 in / 
# Wed, 12 May 2021 01:09:46 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:37:27 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:10:19 GMT
ENV HAPROXY_VERSION=2.4.0
# Fri, 14 May 2021 19:10:19 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Fri, 14 May 2021 19:10:19 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Fri, 14 May 2021 19:12:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 14 May 2021 19:12:46 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:12:47 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:12:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:12:47 GMT
USER haproxy
# Fri, 14 May 2021 19:12:48 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:09564b0ac149fb24b77cbc75ce6fa5d9ba61bd7c99d11b42bd8339c3bb28e557`  
		Last Modified: Wed, 12 May 2021 01:16:36 GMT  
		Size: 25.8 MB (25812884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18fb24fa0e81746ee8c86b23e726e84be12b3f40b71800e0be7e202dd3e3eae3`  
		Last Modified: Wed, 12 May 2021 01:51:31 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50629214220b6d4a25551564eda69255924a81c1d5abdf51759814d8ae33f010`  
		Last Modified: Fri, 14 May 2021 19:13:53 GMT  
		Size: 9.7 MB (9692361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d077c778db1d6d702a26fab8b56bdb796d3f66d02c2d7bc48f3136d5d38fad0`  
		Last Modified: Fri, 14 May 2021 19:13:41 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4` - linux; ppc64le

```console
$ docker pull haproxy@sha256:ac3ce547cea71c004c0f5a85e52ff3b02f4b9ccb85ec55b9c62a29c1b0de2cdc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.1 MB (41134988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:917d9f0f429d84e805182b59da973eb98c74a1ec123db86414d9e0b287ebe1a6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:34:56 GMT
ADD file:3b8146cdc3649d94ad49435c94a21d700ed612ab90f010dcf8b22951b1804d34 in / 
# Wed, 12 May 2021 01:35:02 GMT
CMD ["bash"]
# Wed, 12 May 2021 06:07:29 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:29:30 GMT
ENV HAPROXY_VERSION=2.4.0
# Fri, 14 May 2021 19:29:37 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Fri, 14 May 2021 19:29:46 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Fri, 14 May 2021 19:40:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 14 May 2021 19:40:15 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:40:21 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:40:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:40:38 GMT
USER haproxy
# Fri, 14 May 2021 19:40:51 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:f8b445753f60bad25326d018945455601e4a65f124e956dec95c569816f21493`  
		Last Modified: Wed, 12 May 2021 01:44:19 GMT  
		Size: 30.6 MB (30552394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cfafb398e88c2b64b9fb82254775d63718baad006543dee4e7c370a09a23be9`  
		Last Modified: Wed, 12 May 2021 06:57:45 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b5a44e105c7ef3c0bbf570908dcb769a92fe1dc738dd5a563b76186b5557de`  
		Last Modified: Fri, 14 May 2021 19:46:14 GMT  
		Size: 10.6 MB (10580763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc69ed04682daa398fdabe5de724c14c1e3de1e7616f7bdcc79754f464d2dc13`  
		Last Modified: Fri, 14 May 2021 19:46:12 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4` - linux; s390x

```console
$ docker pull haproxy@sha256:039479598c8aa940517ee6f080fcf62a4ebf12c189b385b1e924c5a53ad06d1b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.5 MB (35515830 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5edca0e2116433b35c4e5ad43d19aa27b5303a10ab98b9094ea0eb2afdf57a1b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:43:38 GMT
ADD file:77af21d863769b75a5f055b85b2c9d6e878f9d77a4122397ae8dde6b69e945c6 in / 
# Wed, 12 May 2021 00:43:42 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:53:39 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:44:04 GMT
ENV HAPROXY_VERSION=2.4.0
# Fri, 14 May 2021 19:44:05 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Fri, 14 May 2021 19:44:05 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Fri, 14 May 2021 19:45:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 14 May 2021 19:45:07 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:45:08 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:45:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:45:09 GMT
USER haproxy
# Fri, 14 May 2021 19:45:09 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:ba4b99e0e723623b64d4ecb8d74102998d32137ea9bcc88b15fd2e4e34b38df9`  
		Last Modified: Wed, 12 May 2021 00:48:03 GMT  
		Size: 25.8 MB (25760171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f6911826fde538e80c00f0d90920d0d7d0a78db315f0bde1ee65726f99f6747`  
		Last Modified: Wed, 12 May 2021 02:04:41 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f093e4ce124ac637de93e3142fecae0c3318de7bd46e44842d671a7f6dbbc99`  
		Last Modified: Fri, 14 May 2021 19:47:51 GMT  
		Size: 9.8 MB (9753831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e979e3b25df89cd6dc9a3c62ae51d2fb6120a89a1a317126572e322c98ef03d3`  
		Last Modified: Fri, 14 May 2021 19:47:50 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.4-alpine`

```console
$ docker pull haproxy@sha256:f95a3663351046fcbf511c58ab51c27de20535d4d57ad23f1ff223236f9a55b5
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

### `haproxy:2.4-alpine` - linux; amd64

```console
$ docker pull haproxy@sha256:5cdbb12744cb989283fc2b3382cdef754a91a927ebe0f9590e603e5b71ba12aa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.2 MB (10189742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd47a280c45025ffbb379774e72f23fd33817110a32a6bc2bc9bfcd85d63862d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:37:38 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:22:49 GMT
ENV HAPROXY_VERSION=2.4.0
# Fri, 14 May 2021 19:22:49 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Fri, 14 May 2021 19:22:49 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Fri, 14 May 2021 19:23:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 14 May 2021 19:23:46 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:23:47 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:23:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:23:47 GMT
USER haproxy
# Fri, 14 May 2021 19:23:47 GMT
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
	-	`sha256:c44c996abc09e09ebd634f300b1f28f57d01f9130f916d9fdc38c37af7ee07c3`  
		Last Modified: Fri, 14 May 2021 19:25:37 GMT  
		Size: 7.4 MB (7376144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d9724e441af85a227fe782cd0b74e214d015f6c418bc9f5721ffc2b212fb1f`  
		Last Modified: Fri, 14 May 2021 19:25:36 GMT  
		Size: 445.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:69efaabcd2ab486de14ef6e2d6b516cb6b759129d42f7307075eacd194ba30b8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.2 MB (10236015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:547431eed6be392afc4baa1caf17cee9637ac4f56f3b37fa341952b199469d70`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:34 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Tue, 15 Jun 2021 22:57:34 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 11:05:46 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 11:07:14 GMT
ENV HAPROXY_VERSION=2.4.0
# Wed, 16 Jun 2021 11:07:14 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Wed, 16 Jun 2021 11:07:14 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Wed, 16 Jun 2021 11:08:32 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 16 Jun 2021 11:08:32 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 11:08:32 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 11:08:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 11:08:33 GMT
USER haproxy
# Wed, 16 Jun 2021 11:08:33 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1be2f4fa6ca9f7822eb93cc888d093da91b0748abe26e3ba14d94b6a757977`  
		Last Modified: Wed, 16 Jun 2021 11:14:47 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:921895821382ed60acd8406262950cfc04c55cbb7c92da354645f645fb554f21`  
		Last Modified: Wed, 16 Jun 2021 11:15:04 GMT  
		Size: 7.6 MB (7612250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aad1b8d3a0f3d5b3f80e86e995d24362cfa6b5eed57f6b2bd55c98482b02627`  
		Last Modified: Wed, 16 Jun 2021 11:15:02 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:edc40093cc1582d4de4f547bb1177784b83f7bdbfeb7bf2d6535ea524497e38e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9868170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2fb528c799b2206e2681f9c635b06b33b9fff9ad0950bd8fa77dafe72b68755`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:15 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Tue, 15 Jun 2021 23:15:16 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 12:49:38 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 12:52:05 GMT
ENV HAPROXY_VERSION=2.4.0
# Wed, 16 Jun 2021 12:52:06 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Wed, 16 Jun 2021 12:52:06 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Wed, 16 Jun 2021 12:53:49 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 16 Jun 2021 12:53:50 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 12:53:50 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 12:53:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 12:53:51 GMT
USER haproxy
# Wed, 16 Jun 2021 12:53:51 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0137e317a40af64134eac5d8b4d74173e380ac844679531b4f1fbdeeec3eb1f5`  
		Last Modified: Wed, 16 Jun 2021 13:08:54 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3338967b5822f35583ac2b289978e0842b8f53fbe0360d31e51bce77406f426`  
		Last Modified: Wed, 16 Jun 2021 13:09:34 GMT  
		Size: 7.4 MB (7442384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057d230ccbd07a75040acffce5ba60dc0d991e074f80db7252266f5015aa5227`  
		Last Modified: Wed, 16 Jun 2021 13:09:32 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:0c1515801d8462766011d15c30f9c895daf84d0bdc94c8075f18ea1a0feb0bcb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.5 MB (10501833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5552ae74aa48a3157768b495d7f900cbe8308844a4eabbb3d31efffaf91beccf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 00:33:20 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 00:35:24 GMT
ENV HAPROXY_VERSION=2.4.0
# Wed, 16 Jun 2021 00:35:24 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Wed, 16 Jun 2021 00:35:24 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Wed, 16 Jun 2021 00:36:22 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 16 Jun 2021 00:36:22 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 00:36:22 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 00:36:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 00:36:22 GMT
USER haproxy
# Wed, 16 Jun 2021 00:36:23 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd643f981edaf0694f3dad8fb6389455756f11cc027101d1de96b178f289891`  
		Last Modified: Wed, 16 Jun 2021 00:44:55 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6612ce2d4bb46fc19cf4e91024ff675545a937cbf9920f5bf6d952ae91fe7e`  
		Last Modified: Wed, 16 Jun 2021 00:45:30 GMT  
		Size: 7.8 MB (7788170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451357d82c6c73d346029d9a73684cbf29c7f1443a4ed10b429007517a0a55b4`  
		Last Modified: Wed, 16 Jun 2021 00:45:27 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-alpine` - linux; 386

```console
$ docker pull haproxy@sha256:b6abb61fc5ca1faf9b49535b6d98a3ef2111b0cd553924ef5a681ffee22cb985
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (9953623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73c76984e00747ccebeec0318f85ee97b2f87f01eaf1b469043ab8ba4c6b4c5d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 01:50:06 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:44:40 GMT
ENV HAPROXY_VERSION=2.4.0
# Fri, 14 May 2021 19:44:40 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Fri, 14 May 2021 19:44:41 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Fri, 14 May 2021 19:46:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 14 May 2021 19:46:10 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:46:11 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:46:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:46:11 GMT
USER haproxy
# Fri, 14 May 2021 19:46:12 GMT
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
	-	`sha256:8331d4e675ebb11e0c29cae6830bda8fd3aa0499ef4bfe6ed7795c45349755a6`  
		Last Modified: Fri, 14 May 2021 19:50:14 GMT  
		Size: 7.1 MB (7133090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff87370dafdb2f94def6b9ba29cf0aca9f8849bf8c40cabf7b2762bcd53c3ce5`  
		Last Modified: Fri, 14 May 2021 19:50:11 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4-alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:b10a0c2c25132ccb0f3287d4b5a8a7876b5a9bb1bd5ae187218218f106a5e2fd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.5 MB (10509060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33dc9abd75900761fcf0d1d1308ee36b9899b33670e0f85e101b0708df8be39c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:25:09 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:41:17 GMT
ENV HAPROXY_VERSION=2.4.0
# Fri, 14 May 2021 19:41:25 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Fri, 14 May 2021 19:41:37 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Fri, 14 May 2021 19:42:41 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 14 May 2021 19:43:13 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:43:25 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:43:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:43:56 GMT
USER haproxy
# Fri, 14 May 2021 19:44:09 GMT
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
	-	`sha256:084faba90127a3d6a1b87cb6cd6f44df9c75eb60f15c6d18b1121ca3562c4a97`  
		Last Modified: Fri, 14 May 2021 19:46:31 GMT  
		Size: 7.7 MB (7694282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecef18bca166de5b45c4de6bfb9e7ee9df71b6603ff3c1a4c2eb5fbf3dd6e4a1`  
		Last Modified: Fri, 14 May 2021 19:46:30 GMT  
		Size: 452.0 B  
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

## `haproxy:2.4.0`

```console
$ docker pull haproxy@sha256:e07d23cbfa10322d03ab965fab14a83793a3cf210cf6598b9bac04441b931b88
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

### `haproxy:2.4.0` - linux; amd64

```console
$ docker pull haproxy@sha256:bf2db25a5ee139ffcb728ea9acea1b0671fdcd761670753f6a9eb493fe7a439f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.2 MB (37226610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b68c771805b9ba3241a23c54e6f43e04a27da28659bca2760faca537bef973cd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 07:10:16 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:21:49 GMT
ENV HAPROXY_VERSION=2.4.0
# Fri, 14 May 2021 19:21:49 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Fri, 14 May 2021 19:21:49 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Fri, 14 May 2021 19:22:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 14 May 2021 19:22:36 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:22:36 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:22:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:22:37 GMT
USER haproxy
# Fri, 14 May 2021 19:22:37 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a113359dddc15238d26b375f86574b596b4aee1263a9631a7384589c2a02f46`  
		Last Modified: Wed, 12 May 2021 07:18:16 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e62dbde04094c3619ac833a9545588b66612ff4a0b35b59c7624708810658bb3`  
		Last Modified: Fri, 14 May 2021 19:25:20 GMT  
		Size: 10.1 MB (10078868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba498b86933facd6fdd59d94d7db13019b879e7cc25d041a68633d89e0494e2`  
		Last Modified: Fri, 14 May 2021 19:25:19 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4.0` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:9bbe3920a362fbdd01643eb1d30ed94397a87cddd058275eccf322d60149697c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.6 MB (34593921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08b4c280b3718ed88ca7f0c20d62f39aa02eeacfcf409626e51607b0ac6f0949`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:55:35 GMT
ADD file:241925c5ca73c99d58f93bc78d7c5bfb6f8b280201a9b55ade45ba0cc054c31d in / 
# Wed, 12 May 2021 00:55:46 GMT
CMD ["bash"]
# Wed, 12 May 2021 02:01:24 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:49:51 GMT
ENV HAPROXY_VERSION=2.4.0
# Fri, 14 May 2021 19:49:53 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Fri, 14 May 2021 19:49:53 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Fri, 14 May 2021 19:50:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 14 May 2021 19:50:56 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:51:04 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:51:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:51:06 GMT
USER haproxy
# Fri, 14 May 2021 19:51:09 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:48885a8e20b16cb3bb9d2c3aafc7f040d8609844f69ca8482c42b4829d01b6da`  
		Last Modified: Wed, 12 May 2021 01:10:24 GMT  
		Size: 24.9 MB (24879601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e012f5248a53449f692d1fe91241d026aa60efe5a3dc3f04add4638989918d2a`  
		Last Modified: Wed, 12 May 2021 02:09:37 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:723c7fb393e70925e6268f228609b020286d9861091b490e8d2a0f254c59a09c`  
		Last Modified: Fri, 14 May 2021 19:52:16 GMT  
		Size: 9.7 MB (9712493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:001bde1f3aa007c516863db1818955f87f02ec4c19a730bf84f2399ddac9c7e2`  
		Last Modified: Fri, 14 May 2021 19:52:13 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4.0` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:b5345ed4dd11a7cb423f4f59dbe9c7ba7cd2abe7afb893b77ddbfb32e5a77302
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.3 MB (32300104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c11a7eb8b982fbc0502c09a9021ba71ea4f9fed9830124aad9547d935b4dcd71`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:03:14 GMT
ADD file:94bf2394dc26abd9f028c2933057a8673c8562e58ec4a0f51bb9bde0a5e4dee0 in / 
# Wed, 12 May 2021 01:03:32 GMT
CMD ["bash"]
# Wed, 16 Jun 2021 12:48:11 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 12:50:51 GMT
ENV HAPROXY_VERSION=2.4.0
# Wed, 16 Jun 2021 12:50:51 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Wed, 16 Jun 2021 12:50:52 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Wed, 16 Jun 2021 12:51:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 16 Jun 2021 12:51:50 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 12:51:51 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 12:51:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 12:51:51 GMT
USER haproxy
# Wed, 16 Jun 2021 12:51:52 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:3035777cd90a3389593bc49a7b39b6f67f9f2679f4e04cc59515f4d5f83ad818`  
		Last Modified: Wed, 12 May 2021 01:19:13 GMT  
		Size: 22.7 MB (22746266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a03e197445bdc67b19867d9e201ef8f2078017e5ad57773c364b31ba9786e0e`  
		Last Modified: Wed, 16 Jun 2021 13:08:37 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dea3a7558a13f5154fb9ce6385d9667552cb71886d1e477e2519abbd5734d85`  
		Last Modified: Wed, 16 Jun 2021 13:09:11 GMT  
		Size: 9.6 MB (9552006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92403e8a9c35756b9b7e782fa08d4faae23520c5824807583c41db0674112c28`  
		Last Modified: Wed, 16 Jun 2021 13:09:08 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4.0` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:7c4943ca2e6c7241331ed74abbd91deb9045a58ff899ea1c47d32878cce737fc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35869597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aad490d428518fedc8dee040fcd2c90f725415ef49be148b71b8c0e7929f2bdb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:52:19 GMT
ADD file:91ba1791cab3ad29a1469d1e78f21f4c0b5d3d30598683b7104980604c318854 in / 
# Wed, 12 May 2021 00:52:34 GMT
CMD ["bash"]
# Wed, 16 Jun 2021 00:32:29 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 00:34:32 GMT
ENV HAPROXY_VERSION=2.4.0
# Wed, 16 Jun 2021 00:34:33 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Wed, 16 Jun 2021 00:34:33 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Wed, 16 Jun 2021 00:35:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 16 Jun 2021 00:35:13 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 00:35:14 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 00:35:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 00:35:14 GMT
USER haproxy
# Wed, 16 Jun 2021 00:35:14 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:fcad0c936ea5c12e1c8c4edb81a97c0cde04ee71e7067ee3b246474cf1854d7a`  
		Last Modified: Wed, 12 May 2021 01:02:02 GMT  
		Size: 25.9 MB (25911250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48fc449d8b117694f567c81827185f03f8e4fa5c56b0b6626bb4374515d222c3`  
		Last Modified: Wed, 16 Jun 2021 00:44:41 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:928814acb1c13f0fd28a553528d1e135f7ffeb4a27bee2232022efda91ed70f2`  
		Last Modified: Wed, 16 Jun 2021 00:45:10 GMT  
		Size: 10.0 MB (9956513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c75f63ea187e14fb0d9052b1e9be0ce47a1c6d1dd4f03382ac3db42f865452`  
		Last Modified: Wed, 16 Jun 2021 00:45:08 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4.0` - linux; 386

```console
$ docker pull haproxy@sha256:65807594f3fdb74f4aeb45cfb58775a8e9e60d00cf4ff637bdcf4343938cfc9c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.7 MB (37714061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b65e677154b7269853270de51028128fb357bdb375ab0bb6229de8bcc8796694`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:39:52 GMT
ADD file:62173a7456d614031a7b20be741983644d9723c734eee663b099ad6b47af7b35 in / 
# Wed, 12 May 2021 00:39:53 GMT
CMD ["bash"]
# Wed, 12 May 2021 05:59:03 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:43:27 GMT
ENV HAPROXY_VERSION=2.4.0
# Fri, 14 May 2021 19:43:27 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Fri, 14 May 2021 19:43:28 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Fri, 14 May 2021 19:44:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 14 May 2021 19:44:27 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:44:27 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:44:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:44:27 GMT
USER haproxy
# Fri, 14 May 2021 19:44:28 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:9b548256784c8e079e5953ec08bd26ce8cbaed0d606a5d350b4bcd12710d2192`  
		Last Modified: Wed, 12 May 2021 00:46:39 GMT  
		Size: 27.8 MB (27795074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05508dc89a5d9449eccbd1b8bf3910253f410f4654f50f119641aa3b5dc3e5c6`  
		Last Modified: Wed, 12 May 2021 06:11:24 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c528b6c319705bef71d9a02c957c8f71879b2f0d4911c0e693640c3485da157`  
		Last Modified: Fri, 14 May 2021 19:49:52 GMT  
		Size: 9.9 MB (9917160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20b09ad55a92c274b5ad2a914359180d1b3a163768611adacc46db20bed561f2`  
		Last Modified: Fri, 14 May 2021 19:49:49 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4.0` - linux; mips64le

```console
$ docker pull haproxy@sha256:9eb21e12824743325f9a8ef93e2a38ec1eee12f374450edafc57ada973db7e36
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.5 MB (35507073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f68f334085d45c2aedb154ace750cc256f9188c28fec0134800ffcdf4d83c465`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:09:45 GMT
ADD file:867397d3fb44b3b936a4ff02bbc3a1b760fb6865b5a85efab82fff224f704241 in / 
# Wed, 12 May 2021 01:09:46 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:37:27 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:10:19 GMT
ENV HAPROXY_VERSION=2.4.0
# Fri, 14 May 2021 19:10:19 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Fri, 14 May 2021 19:10:19 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Fri, 14 May 2021 19:12:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 14 May 2021 19:12:46 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:12:47 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:12:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:12:47 GMT
USER haproxy
# Fri, 14 May 2021 19:12:48 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:09564b0ac149fb24b77cbc75ce6fa5d9ba61bd7c99d11b42bd8339c3bb28e557`  
		Last Modified: Wed, 12 May 2021 01:16:36 GMT  
		Size: 25.8 MB (25812884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18fb24fa0e81746ee8c86b23e726e84be12b3f40b71800e0be7e202dd3e3eae3`  
		Last Modified: Wed, 12 May 2021 01:51:31 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50629214220b6d4a25551564eda69255924a81c1d5abdf51759814d8ae33f010`  
		Last Modified: Fri, 14 May 2021 19:13:53 GMT  
		Size: 9.7 MB (9692361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d077c778db1d6d702a26fab8b56bdb796d3f66d02c2d7bc48f3136d5d38fad0`  
		Last Modified: Fri, 14 May 2021 19:13:41 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4.0` - linux; ppc64le

```console
$ docker pull haproxy@sha256:ac3ce547cea71c004c0f5a85e52ff3b02f4b9ccb85ec55b9c62a29c1b0de2cdc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.1 MB (41134988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:917d9f0f429d84e805182b59da973eb98c74a1ec123db86414d9e0b287ebe1a6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:34:56 GMT
ADD file:3b8146cdc3649d94ad49435c94a21d700ed612ab90f010dcf8b22951b1804d34 in / 
# Wed, 12 May 2021 01:35:02 GMT
CMD ["bash"]
# Wed, 12 May 2021 06:07:29 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:29:30 GMT
ENV HAPROXY_VERSION=2.4.0
# Fri, 14 May 2021 19:29:37 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Fri, 14 May 2021 19:29:46 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Fri, 14 May 2021 19:40:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 14 May 2021 19:40:15 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:40:21 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:40:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:40:38 GMT
USER haproxy
# Fri, 14 May 2021 19:40:51 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:f8b445753f60bad25326d018945455601e4a65f124e956dec95c569816f21493`  
		Last Modified: Wed, 12 May 2021 01:44:19 GMT  
		Size: 30.6 MB (30552394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cfafb398e88c2b64b9fb82254775d63718baad006543dee4e7c370a09a23be9`  
		Last Modified: Wed, 12 May 2021 06:57:45 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b5a44e105c7ef3c0bbf570908dcb769a92fe1dc738dd5a563b76186b5557de`  
		Last Modified: Fri, 14 May 2021 19:46:14 GMT  
		Size: 10.6 MB (10580763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc69ed04682daa398fdabe5de724c14c1e3de1e7616f7bdcc79754f464d2dc13`  
		Last Modified: Fri, 14 May 2021 19:46:12 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4.0` - linux; s390x

```console
$ docker pull haproxy@sha256:039479598c8aa940517ee6f080fcf62a4ebf12c189b385b1e924c5a53ad06d1b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.5 MB (35515830 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5edca0e2116433b35c4e5ad43d19aa27b5303a10ab98b9094ea0eb2afdf57a1b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:43:38 GMT
ADD file:77af21d863769b75a5f055b85b2c9d6e878f9d77a4122397ae8dde6b69e945c6 in / 
# Wed, 12 May 2021 00:43:42 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:53:39 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:44:04 GMT
ENV HAPROXY_VERSION=2.4.0
# Fri, 14 May 2021 19:44:05 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Fri, 14 May 2021 19:44:05 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Fri, 14 May 2021 19:45:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 14 May 2021 19:45:07 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:45:08 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:45:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:45:09 GMT
USER haproxy
# Fri, 14 May 2021 19:45:09 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:ba4b99e0e723623b64d4ecb8d74102998d32137ea9bcc88b15fd2e4e34b38df9`  
		Last Modified: Wed, 12 May 2021 00:48:03 GMT  
		Size: 25.8 MB (25760171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f6911826fde538e80c00f0d90920d0d7d0a78db315f0bde1ee65726f99f6747`  
		Last Modified: Wed, 12 May 2021 02:04:41 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f093e4ce124ac637de93e3142fecae0c3318de7bd46e44842d671a7f6dbbc99`  
		Last Modified: Fri, 14 May 2021 19:47:51 GMT  
		Size: 9.8 MB (9753831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e979e3b25df89cd6dc9a3c62ae51d2fb6120a89a1a317126572e322c98ef03d3`  
		Last Modified: Fri, 14 May 2021 19:47:50 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.4.0-alpine`

```console
$ docker pull haproxy@sha256:f95a3663351046fcbf511c58ab51c27de20535d4d57ad23f1ff223236f9a55b5
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

### `haproxy:2.4.0-alpine` - linux; amd64

```console
$ docker pull haproxy@sha256:5cdbb12744cb989283fc2b3382cdef754a91a927ebe0f9590e603e5b71ba12aa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.2 MB (10189742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd47a280c45025ffbb379774e72f23fd33817110a32a6bc2bc9bfcd85d63862d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:37:38 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:22:49 GMT
ENV HAPROXY_VERSION=2.4.0
# Fri, 14 May 2021 19:22:49 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Fri, 14 May 2021 19:22:49 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Fri, 14 May 2021 19:23:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 14 May 2021 19:23:46 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:23:47 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:23:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:23:47 GMT
USER haproxy
# Fri, 14 May 2021 19:23:47 GMT
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
	-	`sha256:c44c996abc09e09ebd634f300b1f28f57d01f9130f916d9fdc38c37af7ee07c3`  
		Last Modified: Fri, 14 May 2021 19:25:37 GMT  
		Size: 7.4 MB (7376144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d9724e441af85a227fe782cd0b74e214d015f6c418bc9f5721ffc2b212fb1f`  
		Last Modified: Fri, 14 May 2021 19:25:36 GMT  
		Size: 445.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4.0-alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:69efaabcd2ab486de14ef6e2d6b516cb6b759129d42f7307075eacd194ba30b8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.2 MB (10236015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:547431eed6be392afc4baa1caf17cee9637ac4f56f3b37fa341952b199469d70`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:34 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Tue, 15 Jun 2021 22:57:34 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 11:05:46 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 11:07:14 GMT
ENV HAPROXY_VERSION=2.4.0
# Wed, 16 Jun 2021 11:07:14 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Wed, 16 Jun 2021 11:07:14 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Wed, 16 Jun 2021 11:08:32 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 16 Jun 2021 11:08:32 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 11:08:32 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 11:08:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 11:08:33 GMT
USER haproxy
# Wed, 16 Jun 2021 11:08:33 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1be2f4fa6ca9f7822eb93cc888d093da91b0748abe26e3ba14d94b6a757977`  
		Last Modified: Wed, 16 Jun 2021 11:14:47 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:921895821382ed60acd8406262950cfc04c55cbb7c92da354645f645fb554f21`  
		Last Modified: Wed, 16 Jun 2021 11:15:04 GMT  
		Size: 7.6 MB (7612250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aad1b8d3a0f3d5b3f80e86e995d24362cfa6b5eed57f6b2bd55c98482b02627`  
		Last Modified: Wed, 16 Jun 2021 11:15:02 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4.0-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:edc40093cc1582d4de4f547bb1177784b83f7bdbfeb7bf2d6535ea524497e38e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9868170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2fb528c799b2206e2681f9c635b06b33b9fff9ad0950bd8fa77dafe72b68755`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:15 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Tue, 15 Jun 2021 23:15:16 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 12:49:38 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 12:52:05 GMT
ENV HAPROXY_VERSION=2.4.0
# Wed, 16 Jun 2021 12:52:06 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Wed, 16 Jun 2021 12:52:06 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Wed, 16 Jun 2021 12:53:49 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 16 Jun 2021 12:53:50 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 12:53:50 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 12:53:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 12:53:51 GMT
USER haproxy
# Wed, 16 Jun 2021 12:53:51 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0137e317a40af64134eac5d8b4d74173e380ac844679531b4f1fbdeeec3eb1f5`  
		Last Modified: Wed, 16 Jun 2021 13:08:54 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3338967b5822f35583ac2b289978e0842b8f53fbe0360d31e51bce77406f426`  
		Last Modified: Wed, 16 Jun 2021 13:09:34 GMT  
		Size: 7.4 MB (7442384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057d230ccbd07a75040acffce5ba60dc0d991e074f80db7252266f5015aa5227`  
		Last Modified: Wed, 16 Jun 2021 13:09:32 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4.0-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:0c1515801d8462766011d15c30f9c895daf84d0bdc94c8075f18ea1a0feb0bcb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.5 MB (10501833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5552ae74aa48a3157768b495d7f900cbe8308844a4eabbb3d31efffaf91beccf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 00:33:20 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 00:35:24 GMT
ENV HAPROXY_VERSION=2.4.0
# Wed, 16 Jun 2021 00:35:24 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Wed, 16 Jun 2021 00:35:24 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Wed, 16 Jun 2021 00:36:22 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 16 Jun 2021 00:36:22 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 00:36:22 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 00:36:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 00:36:22 GMT
USER haproxy
# Wed, 16 Jun 2021 00:36:23 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd643f981edaf0694f3dad8fb6389455756f11cc027101d1de96b178f289891`  
		Last Modified: Wed, 16 Jun 2021 00:44:55 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6612ce2d4bb46fc19cf4e91024ff675545a937cbf9920f5bf6d952ae91fe7e`  
		Last Modified: Wed, 16 Jun 2021 00:45:30 GMT  
		Size: 7.8 MB (7788170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451357d82c6c73d346029d9a73684cbf29c7f1443a4ed10b429007517a0a55b4`  
		Last Modified: Wed, 16 Jun 2021 00:45:27 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4.0-alpine` - linux; 386

```console
$ docker pull haproxy@sha256:b6abb61fc5ca1faf9b49535b6d98a3ef2111b0cd553924ef5a681ffee22cb985
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (9953623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73c76984e00747ccebeec0318f85ee97b2f87f01eaf1b469043ab8ba4c6b4c5d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 01:50:06 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:44:40 GMT
ENV HAPROXY_VERSION=2.4.0
# Fri, 14 May 2021 19:44:40 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Fri, 14 May 2021 19:44:41 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Fri, 14 May 2021 19:46:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 14 May 2021 19:46:10 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:46:11 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:46:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:46:11 GMT
USER haproxy
# Fri, 14 May 2021 19:46:12 GMT
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
	-	`sha256:8331d4e675ebb11e0c29cae6830bda8fd3aa0499ef4bfe6ed7795c45349755a6`  
		Last Modified: Fri, 14 May 2021 19:50:14 GMT  
		Size: 7.1 MB (7133090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff87370dafdb2f94def6b9ba29cf0aca9f8849bf8c40cabf7b2762bcd53c3ce5`  
		Last Modified: Fri, 14 May 2021 19:50:11 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4.0-alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:b10a0c2c25132ccb0f3287d4b5a8a7876b5a9bb1bd5ae187218218f106a5e2fd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.5 MB (10509060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33dc9abd75900761fcf0d1d1308ee36b9899b33670e0f85e101b0708df8be39c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:25:09 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:41:17 GMT
ENV HAPROXY_VERSION=2.4.0
# Fri, 14 May 2021 19:41:25 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Fri, 14 May 2021 19:41:37 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Fri, 14 May 2021 19:42:41 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 14 May 2021 19:43:13 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:43:25 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:43:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:43:56 GMT
USER haproxy
# Fri, 14 May 2021 19:44:09 GMT
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
	-	`sha256:084faba90127a3d6a1b87cb6cd6f44df9c75eb60f15c6d18b1121ca3562c4a97`  
		Last Modified: Fri, 14 May 2021 19:46:31 GMT  
		Size: 7.7 MB (7694282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecef18bca166de5b45c4de6bfb9e7ee9df71b6603ff3c1a4c2eb5fbf3dd6e4a1`  
		Last Modified: Fri, 14 May 2021 19:46:30 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.4.0-alpine` - linux; s390x

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

## `haproxy:2.5-dev`

```console
$ docker pull haproxy@sha256:237f3a20dc6bbfd2ee3c75326165057e518ca5cdcd98f2de082c1992efa51b09
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

### `haproxy:2.5-dev` - linux; amd64

```console
$ docker pull haproxy@sha256:94860d8a03e79710309b1e2354f844953cda2540d2b39430ef63413355aacaeb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.2 MB (37226596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:580c396cdd8f2ea8ed5471631a98eca0ad069ec7c23d96af2fa964670e88e83d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 07:10:16 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:19:37 GMT
ENV HAPROXY_VERSION=2.5-dev0
# Fri, 14 May 2021 19:19:37 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev0.tar.gz
# Fri, 14 May 2021 19:19:37 GMT
ENV HAPROXY_SHA256=6ee45b5047649b2df3fd48f6659860e8845d970bd4e0c1764490a54c3047bd23
# Fri, 14 May 2021 19:20:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 14 May 2021 19:20:25 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:20:25 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:20:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:20:26 GMT
USER haproxy
# Fri, 14 May 2021 19:20:26 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a113359dddc15238d26b375f86574b596b4aee1263a9631a7384589c2a02f46`  
		Last Modified: Wed, 12 May 2021 07:18:16 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07916fe168cacca8071add213910cff4cdf31148ab436b9c3cb422ed81e05548`  
		Last Modified: Fri, 14 May 2021 19:24:57 GMT  
		Size: 10.1 MB (10078854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed2ebcf98870d342d90ca4389bfc5870ff4b1d8f90ced270671fbc950e020d9`  
		Last Modified: Fri, 14 May 2021 19:24:55 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.5-dev` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:a27135465278aacad59ade7b483d4b4ba90b26766bc8ed9fe64c57bb51988a01
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.6 MB (34593987 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:801c27be356ff5f41151433f9c86a8dd2c90c098115eef25dff0f13d73c816ec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:55:35 GMT
ADD file:241925c5ca73c99d58f93bc78d7c5bfb6f8b280201a9b55ade45ba0cc054c31d in / 
# Wed, 12 May 2021 00:55:46 GMT
CMD ["bash"]
# Wed, 12 May 2021 02:01:24 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:48:32 GMT
ENV HAPROXY_VERSION=2.5-dev0
# Fri, 14 May 2021 19:48:35 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev0.tar.gz
# Fri, 14 May 2021 19:48:39 GMT
ENV HAPROXY_SHA256=6ee45b5047649b2df3fd48f6659860e8845d970bd4e0c1764490a54c3047bd23
# Fri, 14 May 2021 19:49:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 14 May 2021 19:49:34 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:49:36 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:49:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:49:39 GMT
USER haproxy
# Fri, 14 May 2021 19:49:41 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:48885a8e20b16cb3bb9d2c3aafc7f040d8609844f69ca8482c42b4829d01b6da`  
		Last Modified: Wed, 12 May 2021 01:10:24 GMT  
		Size: 24.9 MB (24879601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e012f5248a53449f692d1fe91241d026aa60efe5a3dc3f04add4638989918d2a`  
		Last Modified: Wed, 12 May 2021 02:09:37 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e7da76ad965c7a1ebc5170350ae86257ad416bc69f338c35c5c1010b0b3ccb`  
		Last Modified: Fri, 14 May 2021 19:52:07 GMT  
		Size: 9.7 MB (9712561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14ee5b187309e12ebe183ebfc18779534ee2711ebb2c0ac1c45a1f7918eb8a8d`  
		Last Modified: Fri, 14 May 2021 19:52:04 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.5-dev` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:943cca4802d65e394db9c06454b0e6bc001b509ff70e1a7137e799269f180101
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.3 MB (32300069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04a86fb5247cf09f7dfb7259e63b63b8209f2d8f4824b83cd21991e6eaca4431`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:03:14 GMT
ADD file:94bf2394dc26abd9f028c2933057a8673c8562e58ec4a0f51bb9bde0a5e4dee0 in / 
# Wed, 12 May 2021 01:03:32 GMT
CMD ["bash"]
# Wed, 16 Jun 2021 12:48:11 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 12:48:12 GMT
ENV HAPROXY_VERSION=2.5-dev0
# Wed, 16 Jun 2021 12:48:12 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev0.tar.gz
# Wed, 16 Jun 2021 12:48:12 GMT
ENV HAPROXY_SHA256=6ee45b5047649b2df3fd48f6659860e8845d970bd4e0c1764490a54c3047bd23
# Wed, 16 Jun 2021 12:49:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 16 Jun 2021 12:49:29 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 12:49:29 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 12:49:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 12:49:30 GMT
USER haproxy
# Wed, 16 Jun 2021 12:49:30 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:3035777cd90a3389593bc49a7b39b6f67f9f2679f4e04cc59515f4d5f83ad818`  
		Last Modified: Wed, 12 May 2021 01:19:13 GMT  
		Size: 22.7 MB (22746266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a03e197445bdc67b19867d9e201ef8f2078017e5ad57773c364b31ba9786e0e`  
		Last Modified: Wed, 16 Jun 2021 13:08:37 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7c6b3e4a9b1a6dc00562feaeef1e4f64db1a78717eeba29e1cb961cf69e100`  
		Last Modified: Wed, 16 Jun 2021 13:08:40 GMT  
		Size: 9.6 MB (9551972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e82a9b15d5ab4eaab5639356f784cc71e949d02a99e48b750031a6eebf7779e`  
		Last Modified: Wed, 16 Jun 2021 13:08:37 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.5-dev` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:595617552f25762811016a01d06182c34e93de809adcf5c7ac362ffa77a131ab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35869756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:078d649414b2b33bf555ce9f592675c3461e9b63b74cb33dba9314b1818fb0f1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:52:19 GMT
ADD file:91ba1791cab3ad29a1469d1e78f21f4c0b5d3d30598683b7104980604c318854 in / 
# Wed, 12 May 2021 00:52:34 GMT
CMD ["bash"]
# Wed, 16 Jun 2021 00:32:29 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 00:32:29 GMT
ENV HAPROXY_VERSION=2.5-dev0
# Wed, 16 Jun 2021 00:32:29 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev0.tar.gz
# Wed, 16 Jun 2021 00:32:29 GMT
ENV HAPROXY_SHA256=6ee45b5047649b2df3fd48f6659860e8845d970bd4e0c1764490a54c3047bd23
# Wed, 16 Jun 2021 00:33:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 16 Jun 2021 00:33:11 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 00:33:12 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 00:33:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 00:33:12 GMT
USER haproxy
# Wed, 16 Jun 2021 00:33:12 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:fcad0c936ea5c12e1c8c4edb81a97c0cde04ee71e7067ee3b246474cf1854d7a`  
		Last Modified: Wed, 12 May 2021 01:02:02 GMT  
		Size: 25.9 MB (25911250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48fc449d8b117694f567c81827185f03f8e4fa5c56b0b6626bb4374515d222c3`  
		Last Modified: Wed, 16 Jun 2021 00:44:41 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8135eb5907974b22ed24c77d24bc06d4a43f8bc1068b0331a7c54e7f98a1373e`  
		Last Modified: Wed, 16 Jun 2021 00:44:44 GMT  
		Size: 10.0 MB (9956672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96286578d6965f9c6d5331fa62850859e567868a736a46eea6b9fcaa4b4c721`  
		Last Modified: Wed, 16 Jun 2021 00:44:42 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.5-dev` - linux; 386

```console
$ docker pull haproxy@sha256:4818184df76a6db0daf560227647d920a0d8d84102343c6a450100d760843c7d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.7 MB (37714119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86602f62eea8f959e07e787b425ee37f65163ba3ba1f917746fa95d99ed6344d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:39:52 GMT
ADD file:62173a7456d614031a7b20be741983644d9723c734eee663b099ad6b47af7b35 in / 
# Wed, 12 May 2021 00:39:53 GMT
CMD ["bash"]
# Wed, 12 May 2021 05:59:03 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:39:33 GMT
ENV HAPROXY_VERSION=2.5-dev0
# Fri, 14 May 2021 19:39:33 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev0.tar.gz
# Fri, 14 May 2021 19:39:34 GMT
ENV HAPROXY_SHA256=6ee45b5047649b2df3fd48f6659860e8845d970bd4e0c1764490a54c3047bd23
# Fri, 14 May 2021 19:41:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 14 May 2021 19:41:19 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:41:19 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:41:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:41:20 GMT
USER haproxy
# Fri, 14 May 2021 19:41:20 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:9b548256784c8e079e5953ec08bd26ce8cbaed0d606a5d350b4bcd12710d2192`  
		Last Modified: Wed, 12 May 2021 00:46:39 GMT  
		Size: 27.8 MB (27795074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05508dc89a5d9449eccbd1b8bf3910253f410f4654f50f119641aa3b5dc3e5c6`  
		Last Modified: Wed, 12 May 2021 06:11:24 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b6beeadf27a1509a0fa11ddf384e5cc9a4d39f17471c3e75094e11248b85733`  
		Last Modified: Fri, 14 May 2021 19:49:17 GMT  
		Size: 9.9 MB (9917219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:885d032fc0cf1d2f780c4126c7b34f78db1fab6318e6ea8d828fa1883111334b`  
		Last Modified: Fri, 14 May 2021 19:49:14 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.5-dev` - linux; mips64le

```console
$ docker pull haproxy@sha256:f80c0f5ee4bdbecd018ed1121c31642c56065cc68b0cceef97eafdae1c371659
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.5 MB (35507187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f6d67d6b66401c98e97760b715e6f490204701c245f75567a9013be6f1d61c3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:09:45 GMT
ADD file:867397d3fb44b3b936a4ff02bbc3a1b760fb6865b5a85efab82fff224f704241 in / 
# Wed, 12 May 2021 01:09:46 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:37:27 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:07:38 GMT
ENV HAPROXY_VERSION=2.5-dev0
# Fri, 14 May 2021 19:07:38 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev0.tar.gz
# Fri, 14 May 2021 19:07:38 GMT
ENV HAPROXY_SHA256=6ee45b5047649b2df3fd48f6659860e8845d970bd4e0c1764490a54c3047bd23
# Fri, 14 May 2021 19:10:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 14 May 2021 19:10:07 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:10:07 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:10:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:10:08 GMT
USER haproxy
# Fri, 14 May 2021 19:10:08 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:09564b0ac149fb24b77cbc75ce6fa5d9ba61bd7c99d11b42bd8339c3bb28e557`  
		Last Modified: Wed, 12 May 2021 01:16:36 GMT  
		Size: 25.8 MB (25812884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18fb24fa0e81746ee8c86b23e726e84be12b3f40b71800e0be7e202dd3e3eae3`  
		Last Modified: Wed, 12 May 2021 01:51:31 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a14f83716acbd65ee4781ecb0bc3e3966cc3d3689fc77bdf10d2390f980b4bb0`  
		Last Modified: Fri, 14 May 2021 19:13:31 GMT  
		Size: 9.7 MB (9692475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca85f4488a5df908de028c81a5ca721c9212e1dcb4396a364c34d0462cd21cda`  
		Last Modified: Fri, 14 May 2021 19:13:25 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.5-dev` - linux; ppc64le

```console
$ docker pull haproxy@sha256:d09cf44884a2d0f385438e4d51071d9a2d2e8112f11a3919cc46f6f7b59e49b1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.1 MB (41134810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb4dca6a8087805c959dca0f4523be691899acaf50114f0b5fe9b3ea1d11b9d8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:34:56 GMT
ADD file:3b8146cdc3649d94ad49435c94a21d700ed612ab90f010dcf8b22951b1804d34 in / 
# Wed, 12 May 2021 01:35:02 GMT
CMD ["bash"]
# Wed, 12 May 2021 06:07:29 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:19:10 GMT
ENV HAPROXY_VERSION=2.5-dev0
# Fri, 14 May 2021 19:19:21 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev0.tar.gz
# Fri, 14 May 2021 19:19:38 GMT
ENV HAPROXY_SHA256=6ee45b5047649b2df3fd48f6659860e8845d970bd4e0c1764490a54c3047bd23
# Fri, 14 May 2021 19:25:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 14 May 2021 19:25:48 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:25:51 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:25:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:26:16 GMT
USER haproxy
# Fri, 14 May 2021 19:26:35 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:f8b445753f60bad25326d018945455601e4a65f124e956dec95c569816f21493`  
		Last Modified: Wed, 12 May 2021 01:44:19 GMT  
		Size: 30.6 MB (30552394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cfafb398e88c2b64b9fb82254775d63718baad006543dee4e7c370a09a23be9`  
		Last Modified: Wed, 12 May 2021 06:57:45 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5239aa4cfd5894578b60de77c5ab080ebd4c249c38e04f91be085f9f62a7d9ec`  
		Last Modified: Fri, 14 May 2021 19:45:50 GMT  
		Size: 10.6 MB (10580585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3572a713611862b697496d0630f49ab1f5fc1ce67a35ac3436d00310d7788317`  
		Last Modified: Fri, 14 May 2021 19:45:48 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.5-dev` - linux; s390x

```console
$ docker pull haproxy@sha256:1b7612cfc7002b9c02fd81ec474323144c32f2dcc6b8f469c58b3bbe02e14e93
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.5 MB (35515916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d780835422e668835c6bc1ddc576ca61799043c0c08844b2ba5cc1f515031f4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:43:38 GMT
ADD file:77af21d863769b75a5f055b85b2c9d6e878f9d77a4122397ae8dde6b69e945c6 in / 
# Wed, 12 May 2021 00:43:42 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:53:39 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:41:37 GMT
ENV HAPROXY_VERSION=2.5-dev0
# Fri, 14 May 2021 19:41:38 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev0.tar.gz
# Fri, 14 May 2021 19:41:38 GMT
ENV HAPROXY_SHA256=6ee45b5047649b2df3fd48f6659860e8845d970bd4e0c1764490a54c3047bd23
# Fri, 14 May 2021 19:42:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 14 May 2021 19:42:38 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:42:38 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:42:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:42:40 GMT
USER haproxy
# Fri, 14 May 2021 19:42:40 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:ba4b99e0e723623b64d4ecb8d74102998d32137ea9bcc88b15fd2e4e34b38df9`  
		Last Modified: Wed, 12 May 2021 00:48:03 GMT  
		Size: 25.8 MB (25760171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f6911826fde538e80c00f0d90920d0d7d0a78db315f0bde1ee65726f99f6747`  
		Last Modified: Wed, 12 May 2021 02:04:41 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79794b7dd8a46be9daf1123a2599b782689c686d42be375cd71325a8c9d47d9b`  
		Last Modified: Fri, 14 May 2021 19:47:38 GMT  
		Size: 9.8 MB (9753917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ad84fafed2a196ba3cf9cc5f17bc43d6ea5ffd1d523db8e00200498f5e8a2b8`  
		Last Modified: Fri, 14 May 2021 19:47:37 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.5-dev-alpine`

```console
$ docker pull haproxy@sha256:634268262e6129476ef24000db2ef79619bd09e961eb90b5ecc16b33d7f69b5a
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

### `haproxy:2.5-dev-alpine` - linux; amd64

```console
$ docker pull haproxy@sha256:8d54fb4810bb12c77fc6ab920aedaaa592f52247dd055286be9ba2f32b2f85ab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.2 MB (10189725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcf65e388dfa603ed229ab8ee4ade4c5c217490339a38f0ecab4ce9e718b7b95`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:37:38 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:20:37 GMT
ENV HAPROXY_VERSION=2.5-dev0
# Fri, 14 May 2021 19:20:37 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev0.tar.gz
# Fri, 14 May 2021 19:20:37 GMT
ENV HAPROXY_SHA256=6ee45b5047649b2df3fd48f6659860e8845d970bd4e0c1764490a54c3047bd23
# Fri, 14 May 2021 19:21:35 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 14 May 2021 19:21:35 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:21:35 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:21:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:21:36 GMT
USER haproxy
# Fri, 14 May 2021 19:21:36 GMT
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
	-	`sha256:a5654ec0a61cffc907f11fd533e782c7d420f46e4a0ab41002971a039d412e28`  
		Last Modified: Fri, 14 May 2021 19:25:08 GMT  
		Size: 7.4 MB (7376126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98eb06d6867de036c21b979ab75f2d63bc35d88e5aed55c194b77895a3349bc6`  
		Last Modified: Fri, 14 May 2021 19:25:07 GMT  
		Size: 446.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.5-dev-alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:8c72313ccd22010e890cef6849aca5f7855bd84069113d1d7b5add1311c561ea
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.2 MB (10236029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4dfdd7ce3b5582fe58f646594e9bb147351576f384b1f602f302a9848ea3f2bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:34 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Tue, 15 Jun 2021 22:57:34 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 11:05:46 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 11:05:47 GMT
ENV HAPROXY_VERSION=2.5-dev0
# Wed, 16 Jun 2021 11:05:47 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev0.tar.gz
# Wed, 16 Jun 2021 11:05:47 GMT
ENV HAPROXY_SHA256=6ee45b5047649b2df3fd48f6659860e8845d970bd4e0c1764490a54c3047bd23
# Wed, 16 Jun 2021 11:07:02 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 16 Jun 2021 11:07:02 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 11:07:02 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 11:07:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 11:07:02 GMT
USER haproxy
# Wed, 16 Jun 2021 11:07:02 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1be2f4fa6ca9f7822eb93cc888d093da91b0748abe26e3ba14d94b6a757977`  
		Last Modified: Wed, 16 Jun 2021 11:14:47 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b33322df0e46221ce1f83b4a8d2d67cebbd65e1454b2b5fcf2cb87b7f04b78e9`  
		Last Modified: Wed, 16 Jun 2021 11:14:49 GMT  
		Size: 7.6 MB (7612264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29be445c55d5e82ded4491eaaf44e3f68c0ec6ccf4e114d258149784b30e036e`  
		Last Modified: Wed, 16 Jun 2021 11:14:47 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.5-dev-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:fd15f01684b62b3bde99e5b84c08352521fec3c9a95cab220fc856a7219ab177
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9868120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7d9c5359381d0d51032546e6da7a418bdaadd0e0913ecb8745f422ecd9e236b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:15 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Tue, 15 Jun 2021 23:15:16 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 12:49:38 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 12:49:38 GMT
ENV HAPROXY_VERSION=2.5-dev0
# Wed, 16 Jun 2021 12:49:38 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev0.tar.gz
# Wed, 16 Jun 2021 12:49:39 GMT
ENV HAPROXY_SHA256=6ee45b5047649b2df3fd48f6659860e8845d970bd4e0c1764490a54c3047bd23
# Wed, 16 Jun 2021 12:50:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 16 Jun 2021 12:50:43 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 12:50:43 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 12:50:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 12:50:44 GMT
USER haproxy
# Wed, 16 Jun 2021 12:50:44 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0137e317a40af64134eac5d8b4d74173e380ac844679531b4f1fbdeeec3eb1f5`  
		Last Modified: Wed, 16 Jun 2021 13:08:54 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e686098c2fe6f129450e66eb6d9c7ce86c697ac732596069222f18a8d3490328`  
		Last Modified: Wed, 16 Jun 2021 13:08:55 GMT  
		Size: 7.4 MB (7442337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86eb2125fbffaf9bbc271cb3bae5c6557c2bfbb39f0414659bb59524826d36e`  
		Last Modified: Wed, 16 Jun 2021 13:08:54 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.5-dev-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:8103b6ed44eac18a77d2e7a3fb1a94df32bd002a4f7fe8c80d6cc5e41cb97080
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.5 MB (10501874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c58d1e342476af6143bc530271568f69d20d2ad4b1c125825ba6f57addf45f64`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 00:33:20 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 00:33:21 GMT
ENV HAPROXY_VERSION=2.5-dev0
# Wed, 16 Jun 2021 00:33:21 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev0.tar.gz
# Wed, 16 Jun 2021 00:33:21 GMT
ENV HAPROXY_SHA256=6ee45b5047649b2df3fd48f6659860e8845d970bd4e0c1764490a54c3047bd23
# Wed, 16 Jun 2021 00:34:19 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 16 Jun 2021 00:34:19 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 00:34:19 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 00:34:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 00:34:19 GMT
USER haproxy
# Wed, 16 Jun 2021 00:34:20 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd643f981edaf0694f3dad8fb6389455756f11cc027101d1de96b178f289891`  
		Last Modified: Wed, 16 Jun 2021 00:44:55 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6facf5f29b5c7486ee54ae65cfcfd9359bc32841d6929d90857e2ceb6ad42db7`  
		Last Modified: Wed, 16 Jun 2021 00:44:57 GMT  
		Size: 7.8 MB (7788213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:805b8d6e7c52510535270f8103763fcbbb53f664e8b4c73dfffbd1b790a45c91`  
		Last Modified: Wed, 16 Jun 2021 00:44:55 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.5-dev-alpine` - linux; 386

```console
$ docker pull haproxy@sha256:90c591446451518bfe3db286df0768224fd594cc2626f9591eb5dbcb1d59ef52
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (9953621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:308ae049fbcfe98fe3ff9956634e3e170933fc9ee206f383f845fb4e85d308d1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 01:50:06 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:41:30 GMT
ENV HAPROXY_VERSION=2.5-dev0
# Fri, 14 May 2021 19:41:30 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev0.tar.gz
# Fri, 14 May 2021 19:41:30 GMT
ENV HAPROXY_SHA256=6ee45b5047649b2df3fd48f6659860e8845d970bd4e0c1764490a54c3047bd23
# Fri, 14 May 2021 19:43:20 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 14 May 2021 19:43:20 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:43:21 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:43:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:43:21 GMT
USER haproxy
# Fri, 14 May 2021 19:43:22 GMT
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
	-	`sha256:6d41ef451cdb4fa46ef6fc5edf2d0daff77b3a0443d092f29c4e02c55fa73d9f`  
		Last Modified: Fri, 14 May 2021 19:49:36 GMT  
		Size: 7.1 MB (7133087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb81ced7167e99b4d71df8069bddba1c694bae71c3351a42a14de4656b601173`  
		Last Modified: Fri, 14 May 2021 19:49:29 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.5-dev-alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:d2c891ccae2c71cd751c9ecca785dc7743e5c36587bcabb203f67767ac6ebcff
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.5 MB (10508917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1379c70c33d2a4c7ad7993c144c722de9b445b525842b9e0d9cd912b0983371`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:25:09 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:26:53 GMT
ENV HAPROXY_VERSION=2.5-dev0
# Fri, 14 May 2021 19:27:03 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev0.tar.gz
# Fri, 14 May 2021 19:27:10 GMT
ENV HAPROXY_SHA256=6ee45b5047649b2df3fd48f6659860e8845d970bd4e0c1764490a54c3047bd23
# Fri, 14 May 2021 19:28:14 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 14 May 2021 19:28:36 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:28:53 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:29:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:29:14 GMT
USER haproxy
# Fri, 14 May 2021 19:29:19 GMT
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
	-	`sha256:313093ffa1d341b2ffa6a4059417113837b356ffe24825ba70f6d1de53791caa`  
		Last Modified: Fri, 14 May 2021 19:46:01 GMT  
		Size: 7.7 MB (7694138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e1d5964e58cd579c96f9146c3b7f34cf9a9c9c8a0fc8eb874159f42cb8b5e6`  
		Last Modified: Fri, 14 May 2021 19:46:00 GMT  
		Size: 453.0 B  
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

## `haproxy:2.5-dev0`

```console
$ docker pull haproxy@sha256:237f3a20dc6bbfd2ee3c75326165057e518ca5cdcd98f2de082c1992efa51b09
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

### `haproxy:2.5-dev0` - linux; amd64

```console
$ docker pull haproxy@sha256:94860d8a03e79710309b1e2354f844953cda2540d2b39430ef63413355aacaeb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.2 MB (37226596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:580c396cdd8f2ea8ed5471631a98eca0ad069ec7c23d96af2fa964670e88e83d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 07:10:16 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:19:37 GMT
ENV HAPROXY_VERSION=2.5-dev0
# Fri, 14 May 2021 19:19:37 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev0.tar.gz
# Fri, 14 May 2021 19:19:37 GMT
ENV HAPROXY_SHA256=6ee45b5047649b2df3fd48f6659860e8845d970bd4e0c1764490a54c3047bd23
# Fri, 14 May 2021 19:20:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 14 May 2021 19:20:25 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:20:25 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:20:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:20:26 GMT
USER haproxy
# Fri, 14 May 2021 19:20:26 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a113359dddc15238d26b375f86574b596b4aee1263a9631a7384589c2a02f46`  
		Last Modified: Wed, 12 May 2021 07:18:16 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07916fe168cacca8071add213910cff4cdf31148ab436b9c3cb422ed81e05548`  
		Last Modified: Fri, 14 May 2021 19:24:57 GMT  
		Size: 10.1 MB (10078854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed2ebcf98870d342d90ca4389bfc5870ff4b1d8f90ced270671fbc950e020d9`  
		Last Modified: Fri, 14 May 2021 19:24:55 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.5-dev0` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:a27135465278aacad59ade7b483d4b4ba90b26766bc8ed9fe64c57bb51988a01
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.6 MB (34593987 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:801c27be356ff5f41151433f9c86a8dd2c90c098115eef25dff0f13d73c816ec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:55:35 GMT
ADD file:241925c5ca73c99d58f93bc78d7c5bfb6f8b280201a9b55ade45ba0cc054c31d in / 
# Wed, 12 May 2021 00:55:46 GMT
CMD ["bash"]
# Wed, 12 May 2021 02:01:24 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:48:32 GMT
ENV HAPROXY_VERSION=2.5-dev0
# Fri, 14 May 2021 19:48:35 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev0.tar.gz
# Fri, 14 May 2021 19:48:39 GMT
ENV HAPROXY_SHA256=6ee45b5047649b2df3fd48f6659860e8845d970bd4e0c1764490a54c3047bd23
# Fri, 14 May 2021 19:49:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 14 May 2021 19:49:34 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:49:36 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:49:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:49:39 GMT
USER haproxy
# Fri, 14 May 2021 19:49:41 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:48885a8e20b16cb3bb9d2c3aafc7f040d8609844f69ca8482c42b4829d01b6da`  
		Last Modified: Wed, 12 May 2021 01:10:24 GMT  
		Size: 24.9 MB (24879601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e012f5248a53449f692d1fe91241d026aa60efe5a3dc3f04add4638989918d2a`  
		Last Modified: Wed, 12 May 2021 02:09:37 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e7da76ad965c7a1ebc5170350ae86257ad416bc69f338c35c5c1010b0b3ccb`  
		Last Modified: Fri, 14 May 2021 19:52:07 GMT  
		Size: 9.7 MB (9712561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14ee5b187309e12ebe183ebfc18779534ee2711ebb2c0ac1c45a1f7918eb8a8d`  
		Last Modified: Fri, 14 May 2021 19:52:04 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.5-dev0` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:943cca4802d65e394db9c06454b0e6bc001b509ff70e1a7137e799269f180101
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.3 MB (32300069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04a86fb5247cf09f7dfb7259e63b63b8209f2d8f4824b83cd21991e6eaca4431`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:03:14 GMT
ADD file:94bf2394dc26abd9f028c2933057a8673c8562e58ec4a0f51bb9bde0a5e4dee0 in / 
# Wed, 12 May 2021 01:03:32 GMT
CMD ["bash"]
# Wed, 16 Jun 2021 12:48:11 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 12:48:12 GMT
ENV HAPROXY_VERSION=2.5-dev0
# Wed, 16 Jun 2021 12:48:12 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev0.tar.gz
# Wed, 16 Jun 2021 12:48:12 GMT
ENV HAPROXY_SHA256=6ee45b5047649b2df3fd48f6659860e8845d970bd4e0c1764490a54c3047bd23
# Wed, 16 Jun 2021 12:49:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 16 Jun 2021 12:49:29 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 12:49:29 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 12:49:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 12:49:30 GMT
USER haproxy
# Wed, 16 Jun 2021 12:49:30 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:3035777cd90a3389593bc49a7b39b6f67f9f2679f4e04cc59515f4d5f83ad818`  
		Last Modified: Wed, 12 May 2021 01:19:13 GMT  
		Size: 22.7 MB (22746266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a03e197445bdc67b19867d9e201ef8f2078017e5ad57773c364b31ba9786e0e`  
		Last Modified: Wed, 16 Jun 2021 13:08:37 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7c6b3e4a9b1a6dc00562feaeef1e4f64db1a78717eeba29e1cb961cf69e100`  
		Last Modified: Wed, 16 Jun 2021 13:08:40 GMT  
		Size: 9.6 MB (9551972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e82a9b15d5ab4eaab5639356f784cc71e949d02a99e48b750031a6eebf7779e`  
		Last Modified: Wed, 16 Jun 2021 13:08:37 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.5-dev0` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:595617552f25762811016a01d06182c34e93de809adcf5c7ac362ffa77a131ab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35869756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:078d649414b2b33bf555ce9f592675c3461e9b63b74cb33dba9314b1818fb0f1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:52:19 GMT
ADD file:91ba1791cab3ad29a1469d1e78f21f4c0b5d3d30598683b7104980604c318854 in / 
# Wed, 12 May 2021 00:52:34 GMT
CMD ["bash"]
# Wed, 16 Jun 2021 00:32:29 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 00:32:29 GMT
ENV HAPROXY_VERSION=2.5-dev0
# Wed, 16 Jun 2021 00:32:29 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev0.tar.gz
# Wed, 16 Jun 2021 00:32:29 GMT
ENV HAPROXY_SHA256=6ee45b5047649b2df3fd48f6659860e8845d970bd4e0c1764490a54c3047bd23
# Wed, 16 Jun 2021 00:33:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 16 Jun 2021 00:33:11 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 00:33:12 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 00:33:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 00:33:12 GMT
USER haproxy
# Wed, 16 Jun 2021 00:33:12 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:fcad0c936ea5c12e1c8c4edb81a97c0cde04ee71e7067ee3b246474cf1854d7a`  
		Last Modified: Wed, 12 May 2021 01:02:02 GMT  
		Size: 25.9 MB (25911250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48fc449d8b117694f567c81827185f03f8e4fa5c56b0b6626bb4374515d222c3`  
		Last Modified: Wed, 16 Jun 2021 00:44:41 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8135eb5907974b22ed24c77d24bc06d4a43f8bc1068b0331a7c54e7f98a1373e`  
		Last Modified: Wed, 16 Jun 2021 00:44:44 GMT  
		Size: 10.0 MB (9956672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96286578d6965f9c6d5331fa62850859e567868a736a46eea6b9fcaa4b4c721`  
		Last Modified: Wed, 16 Jun 2021 00:44:42 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.5-dev0` - linux; 386

```console
$ docker pull haproxy@sha256:4818184df76a6db0daf560227647d920a0d8d84102343c6a450100d760843c7d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.7 MB (37714119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86602f62eea8f959e07e787b425ee37f65163ba3ba1f917746fa95d99ed6344d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:39:52 GMT
ADD file:62173a7456d614031a7b20be741983644d9723c734eee663b099ad6b47af7b35 in / 
# Wed, 12 May 2021 00:39:53 GMT
CMD ["bash"]
# Wed, 12 May 2021 05:59:03 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:39:33 GMT
ENV HAPROXY_VERSION=2.5-dev0
# Fri, 14 May 2021 19:39:33 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev0.tar.gz
# Fri, 14 May 2021 19:39:34 GMT
ENV HAPROXY_SHA256=6ee45b5047649b2df3fd48f6659860e8845d970bd4e0c1764490a54c3047bd23
# Fri, 14 May 2021 19:41:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 14 May 2021 19:41:19 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:41:19 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:41:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:41:20 GMT
USER haproxy
# Fri, 14 May 2021 19:41:20 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:9b548256784c8e079e5953ec08bd26ce8cbaed0d606a5d350b4bcd12710d2192`  
		Last Modified: Wed, 12 May 2021 00:46:39 GMT  
		Size: 27.8 MB (27795074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05508dc89a5d9449eccbd1b8bf3910253f410f4654f50f119641aa3b5dc3e5c6`  
		Last Modified: Wed, 12 May 2021 06:11:24 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b6beeadf27a1509a0fa11ddf384e5cc9a4d39f17471c3e75094e11248b85733`  
		Last Modified: Fri, 14 May 2021 19:49:17 GMT  
		Size: 9.9 MB (9917219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:885d032fc0cf1d2f780c4126c7b34f78db1fab6318e6ea8d828fa1883111334b`  
		Last Modified: Fri, 14 May 2021 19:49:14 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.5-dev0` - linux; mips64le

```console
$ docker pull haproxy@sha256:f80c0f5ee4bdbecd018ed1121c31642c56065cc68b0cceef97eafdae1c371659
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.5 MB (35507187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f6d67d6b66401c98e97760b715e6f490204701c245f75567a9013be6f1d61c3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:09:45 GMT
ADD file:867397d3fb44b3b936a4ff02bbc3a1b760fb6865b5a85efab82fff224f704241 in / 
# Wed, 12 May 2021 01:09:46 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:37:27 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:07:38 GMT
ENV HAPROXY_VERSION=2.5-dev0
# Fri, 14 May 2021 19:07:38 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev0.tar.gz
# Fri, 14 May 2021 19:07:38 GMT
ENV HAPROXY_SHA256=6ee45b5047649b2df3fd48f6659860e8845d970bd4e0c1764490a54c3047bd23
# Fri, 14 May 2021 19:10:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 14 May 2021 19:10:07 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:10:07 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:10:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:10:08 GMT
USER haproxy
# Fri, 14 May 2021 19:10:08 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:09564b0ac149fb24b77cbc75ce6fa5d9ba61bd7c99d11b42bd8339c3bb28e557`  
		Last Modified: Wed, 12 May 2021 01:16:36 GMT  
		Size: 25.8 MB (25812884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18fb24fa0e81746ee8c86b23e726e84be12b3f40b71800e0be7e202dd3e3eae3`  
		Last Modified: Wed, 12 May 2021 01:51:31 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a14f83716acbd65ee4781ecb0bc3e3966cc3d3689fc77bdf10d2390f980b4bb0`  
		Last Modified: Fri, 14 May 2021 19:13:31 GMT  
		Size: 9.7 MB (9692475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca85f4488a5df908de028c81a5ca721c9212e1dcb4396a364c34d0462cd21cda`  
		Last Modified: Fri, 14 May 2021 19:13:25 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.5-dev0` - linux; ppc64le

```console
$ docker pull haproxy@sha256:d09cf44884a2d0f385438e4d51071d9a2d2e8112f11a3919cc46f6f7b59e49b1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.1 MB (41134810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb4dca6a8087805c959dca0f4523be691899acaf50114f0b5fe9b3ea1d11b9d8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:34:56 GMT
ADD file:3b8146cdc3649d94ad49435c94a21d700ed612ab90f010dcf8b22951b1804d34 in / 
# Wed, 12 May 2021 01:35:02 GMT
CMD ["bash"]
# Wed, 12 May 2021 06:07:29 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:19:10 GMT
ENV HAPROXY_VERSION=2.5-dev0
# Fri, 14 May 2021 19:19:21 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev0.tar.gz
# Fri, 14 May 2021 19:19:38 GMT
ENV HAPROXY_SHA256=6ee45b5047649b2df3fd48f6659860e8845d970bd4e0c1764490a54c3047bd23
# Fri, 14 May 2021 19:25:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 14 May 2021 19:25:48 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:25:51 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:25:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:26:16 GMT
USER haproxy
# Fri, 14 May 2021 19:26:35 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:f8b445753f60bad25326d018945455601e4a65f124e956dec95c569816f21493`  
		Last Modified: Wed, 12 May 2021 01:44:19 GMT  
		Size: 30.6 MB (30552394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cfafb398e88c2b64b9fb82254775d63718baad006543dee4e7c370a09a23be9`  
		Last Modified: Wed, 12 May 2021 06:57:45 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5239aa4cfd5894578b60de77c5ab080ebd4c249c38e04f91be085f9f62a7d9ec`  
		Last Modified: Fri, 14 May 2021 19:45:50 GMT  
		Size: 10.6 MB (10580585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3572a713611862b697496d0630f49ab1f5fc1ce67a35ac3436d00310d7788317`  
		Last Modified: Fri, 14 May 2021 19:45:48 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.5-dev0` - linux; s390x

```console
$ docker pull haproxy@sha256:1b7612cfc7002b9c02fd81ec474323144c32f2dcc6b8f469c58b3bbe02e14e93
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.5 MB (35515916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d780835422e668835c6bc1ddc576ca61799043c0c08844b2ba5cc1f515031f4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:43:38 GMT
ADD file:77af21d863769b75a5f055b85b2c9d6e878f9d77a4122397ae8dde6b69e945c6 in / 
# Wed, 12 May 2021 00:43:42 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:53:39 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:41:37 GMT
ENV HAPROXY_VERSION=2.5-dev0
# Fri, 14 May 2021 19:41:38 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev0.tar.gz
# Fri, 14 May 2021 19:41:38 GMT
ENV HAPROXY_SHA256=6ee45b5047649b2df3fd48f6659860e8845d970bd4e0c1764490a54c3047bd23
# Fri, 14 May 2021 19:42:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 14 May 2021 19:42:38 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:42:38 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:42:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:42:40 GMT
USER haproxy
# Fri, 14 May 2021 19:42:40 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:ba4b99e0e723623b64d4ecb8d74102998d32137ea9bcc88b15fd2e4e34b38df9`  
		Last Modified: Wed, 12 May 2021 00:48:03 GMT  
		Size: 25.8 MB (25760171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f6911826fde538e80c00f0d90920d0d7d0a78db315f0bde1ee65726f99f6747`  
		Last Modified: Wed, 12 May 2021 02:04:41 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79794b7dd8a46be9daf1123a2599b782689c686d42be375cd71325a8c9d47d9b`  
		Last Modified: Fri, 14 May 2021 19:47:38 GMT  
		Size: 9.8 MB (9753917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ad84fafed2a196ba3cf9cc5f17bc43d6ea5ffd1d523db8e00200498f5e8a2b8`  
		Last Modified: Fri, 14 May 2021 19:47:37 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:2.5-dev0-alpine`

```console
$ docker pull haproxy@sha256:634268262e6129476ef24000db2ef79619bd09e961eb90b5ecc16b33d7f69b5a
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

### `haproxy:2.5-dev0-alpine` - linux; amd64

```console
$ docker pull haproxy@sha256:8d54fb4810bb12c77fc6ab920aedaaa592f52247dd055286be9ba2f32b2f85ab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.2 MB (10189725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcf65e388dfa603ed229ab8ee4ade4c5c217490339a38f0ecab4ce9e718b7b95`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:37:38 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:20:37 GMT
ENV HAPROXY_VERSION=2.5-dev0
# Fri, 14 May 2021 19:20:37 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev0.tar.gz
# Fri, 14 May 2021 19:20:37 GMT
ENV HAPROXY_SHA256=6ee45b5047649b2df3fd48f6659860e8845d970bd4e0c1764490a54c3047bd23
# Fri, 14 May 2021 19:21:35 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 14 May 2021 19:21:35 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:21:35 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:21:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:21:36 GMT
USER haproxy
# Fri, 14 May 2021 19:21:36 GMT
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
	-	`sha256:a5654ec0a61cffc907f11fd533e782c7d420f46e4a0ab41002971a039d412e28`  
		Last Modified: Fri, 14 May 2021 19:25:08 GMT  
		Size: 7.4 MB (7376126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98eb06d6867de036c21b979ab75f2d63bc35d88e5aed55c194b77895a3349bc6`  
		Last Modified: Fri, 14 May 2021 19:25:07 GMT  
		Size: 446.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.5-dev0-alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:8c72313ccd22010e890cef6849aca5f7855bd84069113d1d7b5add1311c561ea
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.2 MB (10236029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4dfdd7ce3b5582fe58f646594e9bb147351576f384b1f602f302a9848ea3f2bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:34 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Tue, 15 Jun 2021 22:57:34 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 11:05:46 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 11:05:47 GMT
ENV HAPROXY_VERSION=2.5-dev0
# Wed, 16 Jun 2021 11:05:47 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev0.tar.gz
# Wed, 16 Jun 2021 11:05:47 GMT
ENV HAPROXY_SHA256=6ee45b5047649b2df3fd48f6659860e8845d970bd4e0c1764490a54c3047bd23
# Wed, 16 Jun 2021 11:07:02 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 16 Jun 2021 11:07:02 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 11:07:02 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 11:07:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 11:07:02 GMT
USER haproxy
# Wed, 16 Jun 2021 11:07:02 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1be2f4fa6ca9f7822eb93cc888d093da91b0748abe26e3ba14d94b6a757977`  
		Last Modified: Wed, 16 Jun 2021 11:14:47 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b33322df0e46221ce1f83b4a8d2d67cebbd65e1454b2b5fcf2cb87b7f04b78e9`  
		Last Modified: Wed, 16 Jun 2021 11:14:49 GMT  
		Size: 7.6 MB (7612264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29be445c55d5e82ded4491eaaf44e3f68c0ec6ccf4e114d258149784b30e036e`  
		Last Modified: Wed, 16 Jun 2021 11:14:47 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.5-dev0-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:fd15f01684b62b3bde99e5b84c08352521fec3c9a95cab220fc856a7219ab177
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9868120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7d9c5359381d0d51032546e6da7a418bdaadd0e0913ecb8745f422ecd9e236b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:15 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Tue, 15 Jun 2021 23:15:16 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 12:49:38 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 12:49:38 GMT
ENV HAPROXY_VERSION=2.5-dev0
# Wed, 16 Jun 2021 12:49:38 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev0.tar.gz
# Wed, 16 Jun 2021 12:49:39 GMT
ENV HAPROXY_SHA256=6ee45b5047649b2df3fd48f6659860e8845d970bd4e0c1764490a54c3047bd23
# Wed, 16 Jun 2021 12:50:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 16 Jun 2021 12:50:43 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 12:50:43 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 12:50:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 12:50:44 GMT
USER haproxy
# Wed, 16 Jun 2021 12:50:44 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0137e317a40af64134eac5d8b4d74173e380ac844679531b4f1fbdeeec3eb1f5`  
		Last Modified: Wed, 16 Jun 2021 13:08:54 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e686098c2fe6f129450e66eb6d9c7ce86c697ac732596069222f18a8d3490328`  
		Last Modified: Wed, 16 Jun 2021 13:08:55 GMT  
		Size: 7.4 MB (7442337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86eb2125fbffaf9bbc271cb3bae5c6557c2bfbb39f0414659bb59524826d36e`  
		Last Modified: Wed, 16 Jun 2021 13:08:54 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.5-dev0-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:8103b6ed44eac18a77d2e7a3fb1a94df32bd002a4f7fe8c80d6cc5e41cb97080
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.5 MB (10501874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c58d1e342476af6143bc530271568f69d20d2ad4b1c125825ba6f57addf45f64`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 00:33:20 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 00:33:21 GMT
ENV HAPROXY_VERSION=2.5-dev0
# Wed, 16 Jun 2021 00:33:21 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev0.tar.gz
# Wed, 16 Jun 2021 00:33:21 GMT
ENV HAPROXY_SHA256=6ee45b5047649b2df3fd48f6659860e8845d970bd4e0c1764490a54c3047bd23
# Wed, 16 Jun 2021 00:34:19 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 16 Jun 2021 00:34:19 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 00:34:19 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 00:34:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 00:34:19 GMT
USER haproxy
# Wed, 16 Jun 2021 00:34:20 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd643f981edaf0694f3dad8fb6389455756f11cc027101d1de96b178f289891`  
		Last Modified: Wed, 16 Jun 2021 00:44:55 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6facf5f29b5c7486ee54ae65cfcfd9359bc32841d6929d90857e2ceb6ad42db7`  
		Last Modified: Wed, 16 Jun 2021 00:44:57 GMT  
		Size: 7.8 MB (7788213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:805b8d6e7c52510535270f8103763fcbbb53f664e8b4c73dfffbd1b790a45c91`  
		Last Modified: Wed, 16 Jun 2021 00:44:55 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.5-dev0-alpine` - linux; 386

```console
$ docker pull haproxy@sha256:90c591446451518bfe3db286df0768224fd594cc2626f9591eb5dbcb1d59ef52
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (9953621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:308ae049fbcfe98fe3ff9956634e3e170933fc9ee206f383f845fb4e85d308d1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 01:50:06 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:41:30 GMT
ENV HAPROXY_VERSION=2.5-dev0
# Fri, 14 May 2021 19:41:30 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev0.tar.gz
# Fri, 14 May 2021 19:41:30 GMT
ENV HAPROXY_SHA256=6ee45b5047649b2df3fd48f6659860e8845d970bd4e0c1764490a54c3047bd23
# Fri, 14 May 2021 19:43:20 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 14 May 2021 19:43:20 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:43:21 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:43:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:43:21 GMT
USER haproxy
# Fri, 14 May 2021 19:43:22 GMT
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
	-	`sha256:6d41ef451cdb4fa46ef6fc5edf2d0daff77b3a0443d092f29c4e02c55fa73d9f`  
		Last Modified: Fri, 14 May 2021 19:49:36 GMT  
		Size: 7.1 MB (7133087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb81ced7167e99b4d71df8069bddba1c694bae71c3351a42a14de4656b601173`  
		Last Modified: Fri, 14 May 2021 19:49:29 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.5-dev0-alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:d2c891ccae2c71cd751c9ecca785dc7743e5c36587bcabb203f67767ac6ebcff
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.5 MB (10508917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1379c70c33d2a4c7ad7993c144c722de9b445b525842b9e0d9cd912b0983371`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:25:09 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:26:53 GMT
ENV HAPROXY_VERSION=2.5-dev0
# Fri, 14 May 2021 19:27:03 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/devel/haproxy-2.5-dev0.tar.gz
# Fri, 14 May 2021 19:27:10 GMT
ENV HAPROXY_SHA256=6ee45b5047649b2df3fd48f6659860e8845d970bd4e0c1764490a54c3047bd23
# Fri, 14 May 2021 19:28:14 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 14 May 2021 19:28:36 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:28:53 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:29:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:29:14 GMT
USER haproxy
# Fri, 14 May 2021 19:29:19 GMT
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
	-	`sha256:313093ffa1d341b2ffa6a4059417113837b356ffe24825ba70f6d1de53791caa`  
		Last Modified: Fri, 14 May 2021 19:46:01 GMT  
		Size: 7.7 MB (7694138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e1d5964e58cd579c96f9146c3b7f34cf9a9c9c8a0fc8eb874159f42cb8b5e6`  
		Last Modified: Fri, 14 May 2021 19:46:00 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:2.5-dev0-alpine` - linux; s390x

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

## `haproxy:alpine`

```console
$ docker pull haproxy@sha256:f95a3663351046fcbf511c58ab51c27de20535d4d57ad23f1ff223236f9a55b5
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
$ docker pull haproxy@sha256:5cdbb12744cb989283fc2b3382cdef754a91a927ebe0f9590e603e5b71ba12aa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.2 MB (10189742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd47a280c45025ffbb379774e72f23fd33817110a32a6bc2bc9bfcd85d63862d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:37:38 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:22:49 GMT
ENV HAPROXY_VERSION=2.4.0
# Fri, 14 May 2021 19:22:49 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Fri, 14 May 2021 19:22:49 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Fri, 14 May 2021 19:23:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 14 May 2021 19:23:46 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:23:47 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:23:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:23:47 GMT
USER haproxy
# Fri, 14 May 2021 19:23:47 GMT
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
	-	`sha256:c44c996abc09e09ebd634f300b1f28f57d01f9130f916d9fdc38c37af7ee07c3`  
		Last Modified: Fri, 14 May 2021 19:25:37 GMT  
		Size: 7.4 MB (7376144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d9724e441af85a227fe782cd0b74e214d015f6c418bc9f5721ffc2b212fb1f`  
		Last Modified: Fri, 14 May 2021 19:25:36 GMT  
		Size: 445.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:69efaabcd2ab486de14ef6e2d6b516cb6b759129d42f7307075eacd194ba30b8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.2 MB (10236015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:547431eed6be392afc4baa1caf17cee9637ac4f56f3b37fa341952b199469d70`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:34 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Tue, 15 Jun 2021 22:57:34 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 11:05:46 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 11:07:14 GMT
ENV HAPROXY_VERSION=2.4.0
# Wed, 16 Jun 2021 11:07:14 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Wed, 16 Jun 2021 11:07:14 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Wed, 16 Jun 2021 11:08:32 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 16 Jun 2021 11:08:32 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 11:08:32 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 11:08:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 11:08:33 GMT
USER haproxy
# Wed, 16 Jun 2021 11:08:33 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1be2f4fa6ca9f7822eb93cc888d093da91b0748abe26e3ba14d94b6a757977`  
		Last Modified: Wed, 16 Jun 2021 11:14:47 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:921895821382ed60acd8406262950cfc04c55cbb7c92da354645f645fb554f21`  
		Last Modified: Wed, 16 Jun 2021 11:15:04 GMT  
		Size: 7.6 MB (7612250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aad1b8d3a0f3d5b3f80e86e995d24362cfa6b5eed57f6b2bd55c98482b02627`  
		Last Modified: Wed, 16 Jun 2021 11:15:02 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:edc40093cc1582d4de4f547bb1177784b83f7bdbfeb7bf2d6535ea524497e38e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9868170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2fb528c799b2206e2681f9c635b06b33b9fff9ad0950bd8fa77dafe72b68755`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:15 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Tue, 15 Jun 2021 23:15:16 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 12:49:38 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 12:52:05 GMT
ENV HAPROXY_VERSION=2.4.0
# Wed, 16 Jun 2021 12:52:06 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Wed, 16 Jun 2021 12:52:06 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Wed, 16 Jun 2021 12:53:49 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 16 Jun 2021 12:53:50 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 12:53:50 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 12:53:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 12:53:51 GMT
USER haproxy
# Wed, 16 Jun 2021 12:53:51 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0137e317a40af64134eac5d8b4d74173e380ac844679531b4f1fbdeeec3eb1f5`  
		Last Modified: Wed, 16 Jun 2021 13:08:54 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3338967b5822f35583ac2b289978e0842b8f53fbe0360d31e51bce77406f426`  
		Last Modified: Wed, 16 Jun 2021 13:09:34 GMT  
		Size: 7.4 MB (7442384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057d230ccbd07a75040acffce5ba60dc0d991e074f80db7252266f5015aa5227`  
		Last Modified: Wed, 16 Jun 2021 13:09:32 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:0c1515801d8462766011d15c30f9c895daf84d0bdc94c8075f18ea1a0feb0bcb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.5 MB (10501833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5552ae74aa48a3157768b495d7f900cbe8308844a4eabbb3d31efffaf91beccf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 00:33:20 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 00:35:24 GMT
ENV HAPROXY_VERSION=2.4.0
# Wed, 16 Jun 2021 00:35:24 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Wed, 16 Jun 2021 00:35:24 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Wed, 16 Jun 2021 00:36:22 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 16 Jun 2021 00:36:22 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 00:36:22 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 00:36:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 00:36:22 GMT
USER haproxy
# Wed, 16 Jun 2021 00:36:23 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd643f981edaf0694f3dad8fb6389455756f11cc027101d1de96b178f289891`  
		Last Modified: Wed, 16 Jun 2021 00:44:55 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6612ce2d4bb46fc19cf4e91024ff675545a937cbf9920f5bf6d952ae91fe7e`  
		Last Modified: Wed, 16 Jun 2021 00:45:30 GMT  
		Size: 7.8 MB (7788170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451357d82c6c73d346029d9a73684cbf29c7f1443a4ed10b429007517a0a55b4`  
		Last Modified: Wed, 16 Jun 2021 00:45:27 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:alpine` - linux; 386

```console
$ docker pull haproxy@sha256:b6abb61fc5ca1faf9b49535b6d98a3ef2111b0cd553924ef5a681ffee22cb985
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (9953623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73c76984e00747ccebeec0318f85ee97b2f87f01eaf1b469043ab8ba4c6b4c5d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 01:50:06 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:44:40 GMT
ENV HAPROXY_VERSION=2.4.0
# Fri, 14 May 2021 19:44:40 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Fri, 14 May 2021 19:44:41 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Fri, 14 May 2021 19:46:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 14 May 2021 19:46:10 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:46:11 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:46:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:46:11 GMT
USER haproxy
# Fri, 14 May 2021 19:46:12 GMT
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
	-	`sha256:8331d4e675ebb11e0c29cae6830bda8fd3aa0499ef4bfe6ed7795c45349755a6`  
		Last Modified: Fri, 14 May 2021 19:50:14 GMT  
		Size: 7.1 MB (7133090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff87370dafdb2f94def6b9ba29cf0aca9f8849bf8c40cabf7b2762bcd53c3ce5`  
		Last Modified: Fri, 14 May 2021 19:50:11 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:b10a0c2c25132ccb0f3287d4b5a8a7876b5a9bb1bd5ae187218218f106a5e2fd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.5 MB (10509060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33dc9abd75900761fcf0d1d1308ee36b9899b33670e0f85e101b0708df8be39c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:25:09 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:41:17 GMT
ENV HAPROXY_VERSION=2.4.0
# Fri, 14 May 2021 19:41:25 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Fri, 14 May 2021 19:41:37 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Fri, 14 May 2021 19:42:41 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 14 May 2021 19:43:13 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:43:25 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:43:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:43:56 GMT
USER haproxy
# Fri, 14 May 2021 19:44:09 GMT
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
	-	`sha256:084faba90127a3d6a1b87cb6cd6f44df9c75eb60f15c6d18b1121ca3562c4a97`  
		Last Modified: Fri, 14 May 2021 19:46:31 GMT  
		Size: 7.7 MB (7694282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecef18bca166de5b45c4de6bfb9e7ee9df71b6603ff3c1a4c2eb5fbf3dd6e4a1`  
		Last Modified: Fri, 14 May 2021 19:46:30 GMT  
		Size: 452.0 B  
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
$ docker pull haproxy@sha256:e07d23cbfa10322d03ab965fab14a83793a3cf210cf6598b9bac04441b931b88
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
$ docker pull haproxy@sha256:bf2db25a5ee139ffcb728ea9acea1b0671fdcd761670753f6a9eb493fe7a439f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.2 MB (37226610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b68c771805b9ba3241a23c54e6f43e04a27da28659bca2760faca537bef973cd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 07:10:16 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:21:49 GMT
ENV HAPROXY_VERSION=2.4.0
# Fri, 14 May 2021 19:21:49 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Fri, 14 May 2021 19:21:49 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Fri, 14 May 2021 19:22:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 14 May 2021 19:22:36 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:22:36 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:22:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:22:37 GMT
USER haproxy
# Fri, 14 May 2021 19:22:37 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a113359dddc15238d26b375f86574b596b4aee1263a9631a7384589c2a02f46`  
		Last Modified: Wed, 12 May 2021 07:18:16 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e62dbde04094c3619ac833a9545588b66612ff4a0b35b59c7624708810658bb3`  
		Last Modified: Fri, 14 May 2021 19:25:20 GMT  
		Size: 10.1 MB (10078868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba498b86933facd6fdd59d94d7db13019b879e7cc25d041a68633d89e0494e2`  
		Last Modified: Fri, 14 May 2021 19:25:19 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:latest` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:9bbe3920a362fbdd01643eb1d30ed94397a87cddd058275eccf322d60149697c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.6 MB (34593921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08b4c280b3718ed88ca7f0c20d62f39aa02eeacfcf409626e51607b0ac6f0949`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:55:35 GMT
ADD file:241925c5ca73c99d58f93bc78d7c5bfb6f8b280201a9b55ade45ba0cc054c31d in / 
# Wed, 12 May 2021 00:55:46 GMT
CMD ["bash"]
# Wed, 12 May 2021 02:01:24 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:49:51 GMT
ENV HAPROXY_VERSION=2.4.0
# Fri, 14 May 2021 19:49:53 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Fri, 14 May 2021 19:49:53 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Fri, 14 May 2021 19:50:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 14 May 2021 19:50:56 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:51:04 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:51:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:51:06 GMT
USER haproxy
# Fri, 14 May 2021 19:51:09 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:48885a8e20b16cb3bb9d2c3aafc7f040d8609844f69ca8482c42b4829d01b6da`  
		Last Modified: Wed, 12 May 2021 01:10:24 GMT  
		Size: 24.9 MB (24879601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e012f5248a53449f692d1fe91241d026aa60efe5a3dc3f04add4638989918d2a`  
		Last Modified: Wed, 12 May 2021 02:09:37 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:723c7fb393e70925e6268f228609b020286d9861091b490e8d2a0f254c59a09c`  
		Last Modified: Fri, 14 May 2021 19:52:16 GMT  
		Size: 9.7 MB (9712493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:001bde1f3aa007c516863db1818955f87f02ec4c19a730bf84f2399ddac9c7e2`  
		Last Modified: Fri, 14 May 2021 19:52:13 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:latest` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:b5345ed4dd11a7cb423f4f59dbe9c7ba7cd2abe7afb893b77ddbfb32e5a77302
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.3 MB (32300104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c11a7eb8b982fbc0502c09a9021ba71ea4f9fed9830124aad9547d935b4dcd71`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:03:14 GMT
ADD file:94bf2394dc26abd9f028c2933057a8673c8562e58ec4a0f51bb9bde0a5e4dee0 in / 
# Wed, 12 May 2021 01:03:32 GMT
CMD ["bash"]
# Wed, 16 Jun 2021 12:48:11 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 12:50:51 GMT
ENV HAPROXY_VERSION=2.4.0
# Wed, 16 Jun 2021 12:50:51 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Wed, 16 Jun 2021 12:50:52 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Wed, 16 Jun 2021 12:51:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 16 Jun 2021 12:51:50 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 12:51:51 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 12:51:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 12:51:51 GMT
USER haproxy
# Wed, 16 Jun 2021 12:51:52 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:3035777cd90a3389593bc49a7b39b6f67f9f2679f4e04cc59515f4d5f83ad818`  
		Last Modified: Wed, 12 May 2021 01:19:13 GMT  
		Size: 22.7 MB (22746266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a03e197445bdc67b19867d9e201ef8f2078017e5ad57773c364b31ba9786e0e`  
		Last Modified: Wed, 16 Jun 2021 13:08:37 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dea3a7558a13f5154fb9ce6385d9667552cb71886d1e477e2519abbd5734d85`  
		Last Modified: Wed, 16 Jun 2021 13:09:11 GMT  
		Size: 9.6 MB (9552006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92403e8a9c35756b9b7e782fa08d4faae23520c5824807583c41db0674112c28`  
		Last Modified: Wed, 16 Jun 2021 13:09:08 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:latest` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:7c4943ca2e6c7241331ed74abbd91deb9045a58ff899ea1c47d32878cce737fc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35869597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aad490d428518fedc8dee040fcd2c90f725415ef49be148b71b8c0e7929f2bdb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:52:19 GMT
ADD file:91ba1791cab3ad29a1469d1e78f21f4c0b5d3d30598683b7104980604c318854 in / 
# Wed, 12 May 2021 00:52:34 GMT
CMD ["bash"]
# Wed, 16 Jun 2021 00:32:29 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 00:34:32 GMT
ENV HAPROXY_VERSION=2.4.0
# Wed, 16 Jun 2021 00:34:33 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Wed, 16 Jun 2021 00:34:33 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Wed, 16 Jun 2021 00:35:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 16 Jun 2021 00:35:13 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 00:35:14 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 00:35:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 00:35:14 GMT
USER haproxy
# Wed, 16 Jun 2021 00:35:14 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:fcad0c936ea5c12e1c8c4edb81a97c0cde04ee71e7067ee3b246474cf1854d7a`  
		Last Modified: Wed, 12 May 2021 01:02:02 GMT  
		Size: 25.9 MB (25911250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48fc449d8b117694f567c81827185f03f8e4fa5c56b0b6626bb4374515d222c3`  
		Last Modified: Wed, 16 Jun 2021 00:44:41 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:928814acb1c13f0fd28a553528d1e135f7ffeb4a27bee2232022efda91ed70f2`  
		Last Modified: Wed, 16 Jun 2021 00:45:10 GMT  
		Size: 10.0 MB (9956513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c75f63ea187e14fb0d9052b1e9be0ce47a1c6d1dd4f03382ac3db42f865452`  
		Last Modified: Wed, 16 Jun 2021 00:45:08 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:latest` - linux; 386

```console
$ docker pull haproxy@sha256:65807594f3fdb74f4aeb45cfb58775a8e9e60d00cf4ff637bdcf4343938cfc9c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.7 MB (37714061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b65e677154b7269853270de51028128fb357bdb375ab0bb6229de8bcc8796694`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:39:52 GMT
ADD file:62173a7456d614031a7b20be741983644d9723c734eee663b099ad6b47af7b35 in / 
# Wed, 12 May 2021 00:39:53 GMT
CMD ["bash"]
# Wed, 12 May 2021 05:59:03 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:43:27 GMT
ENV HAPROXY_VERSION=2.4.0
# Fri, 14 May 2021 19:43:27 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Fri, 14 May 2021 19:43:28 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Fri, 14 May 2021 19:44:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 14 May 2021 19:44:27 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:44:27 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:44:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:44:27 GMT
USER haproxy
# Fri, 14 May 2021 19:44:28 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:9b548256784c8e079e5953ec08bd26ce8cbaed0d606a5d350b4bcd12710d2192`  
		Last Modified: Wed, 12 May 2021 00:46:39 GMT  
		Size: 27.8 MB (27795074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05508dc89a5d9449eccbd1b8bf3910253f410f4654f50f119641aa3b5dc3e5c6`  
		Last Modified: Wed, 12 May 2021 06:11:24 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c528b6c319705bef71d9a02c957c8f71879b2f0d4911c0e693640c3485da157`  
		Last Modified: Fri, 14 May 2021 19:49:52 GMT  
		Size: 9.9 MB (9917160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20b09ad55a92c274b5ad2a914359180d1b3a163768611adacc46db20bed561f2`  
		Last Modified: Fri, 14 May 2021 19:49:49 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:latest` - linux; mips64le

```console
$ docker pull haproxy@sha256:9eb21e12824743325f9a8ef93e2a38ec1eee12f374450edafc57ada973db7e36
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.5 MB (35507073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f68f334085d45c2aedb154ace750cc256f9188c28fec0134800ffcdf4d83c465`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:09:45 GMT
ADD file:867397d3fb44b3b936a4ff02bbc3a1b760fb6865b5a85efab82fff224f704241 in / 
# Wed, 12 May 2021 01:09:46 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:37:27 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:10:19 GMT
ENV HAPROXY_VERSION=2.4.0
# Fri, 14 May 2021 19:10:19 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Fri, 14 May 2021 19:10:19 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Fri, 14 May 2021 19:12:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 14 May 2021 19:12:46 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:12:47 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:12:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:12:47 GMT
USER haproxy
# Fri, 14 May 2021 19:12:48 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:09564b0ac149fb24b77cbc75ce6fa5d9ba61bd7c99d11b42bd8339c3bb28e557`  
		Last Modified: Wed, 12 May 2021 01:16:36 GMT  
		Size: 25.8 MB (25812884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18fb24fa0e81746ee8c86b23e726e84be12b3f40b71800e0be7e202dd3e3eae3`  
		Last Modified: Wed, 12 May 2021 01:51:31 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50629214220b6d4a25551564eda69255924a81c1d5abdf51759814d8ae33f010`  
		Last Modified: Fri, 14 May 2021 19:13:53 GMT  
		Size: 9.7 MB (9692361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d077c778db1d6d702a26fab8b56bdb796d3f66d02c2d7bc48f3136d5d38fad0`  
		Last Modified: Fri, 14 May 2021 19:13:41 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:latest` - linux; ppc64le

```console
$ docker pull haproxy@sha256:ac3ce547cea71c004c0f5a85e52ff3b02f4b9ccb85ec55b9c62a29c1b0de2cdc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.1 MB (41134988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:917d9f0f429d84e805182b59da973eb98c74a1ec123db86414d9e0b287ebe1a6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:34:56 GMT
ADD file:3b8146cdc3649d94ad49435c94a21d700ed612ab90f010dcf8b22951b1804d34 in / 
# Wed, 12 May 2021 01:35:02 GMT
CMD ["bash"]
# Wed, 12 May 2021 06:07:29 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:29:30 GMT
ENV HAPROXY_VERSION=2.4.0
# Fri, 14 May 2021 19:29:37 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Fri, 14 May 2021 19:29:46 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Fri, 14 May 2021 19:40:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 14 May 2021 19:40:15 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:40:21 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:40:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:40:38 GMT
USER haproxy
# Fri, 14 May 2021 19:40:51 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:f8b445753f60bad25326d018945455601e4a65f124e956dec95c569816f21493`  
		Last Modified: Wed, 12 May 2021 01:44:19 GMT  
		Size: 30.6 MB (30552394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cfafb398e88c2b64b9fb82254775d63718baad006543dee4e7c370a09a23be9`  
		Last Modified: Wed, 12 May 2021 06:57:45 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b5a44e105c7ef3c0bbf570908dcb769a92fe1dc738dd5a563b76186b5557de`  
		Last Modified: Fri, 14 May 2021 19:46:14 GMT  
		Size: 10.6 MB (10580763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc69ed04682daa398fdabe5de724c14c1e3de1e7616f7bdcc79754f464d2dc13`  
		Last Modified: Fri, 14 May 2021 19:46:12 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:latest` - linux; s390x

```console
$ docker pull haproxy@sha256:039479598c8aa940517ee6f080fcf62a4ebf12c189b385b1e924c5a53ad06d1b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.5 MB (35515830 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5edca0e2116433b35c4e5ad43d19aa27b5303a10ab98b9094ea0eb2afdf57a1b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:43:38 GMT
ADD file:77af21d863769b75a5f055b85b2c9d6e878f9d77a4122397ae8dde6b69e945c6 in / 
# Wed, 12 May 2021 00:43:42 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:53:39 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:44:04 GMT
ENV HAPROXY_VERSION=2.4.0
# Fri, 14 May 2021 19:44:05 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Fri, 14 May 2021 19:44:05 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Fri, 14 May 2021 19:45:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 14 May 2021 19:45:07 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:45:08 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:45:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:45:09 GMT
USER haproxy
# Fri, 14 May 2021 19:45:09 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:ba4b99e0e723623b64d4ecb8d74102998d32137ea9bcc88b15fd2e4e34b38df9`  
		Last Modified: Wed, 12 May 2021 00:48:03 GMT  
		Size: 25.8 MB (25760171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f6911826fde538e80c00f0d90920d0d7d0a78db315f0bde1ee65726f99f6747`  
		Last Modified: Wed, 12 May 2021 02:04:41 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f093e4ce124ac637de93e3142fecae0c3318de7bd46e44842d671a7f6dbbc99`  
		Last Modified: Fri, 14 May 2021 19:47:51 GMT  
		Size: 9.8 MB (9753831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e979e3b25df89cd6dc9a3c62ae51d2fb6120a89a1a317126572e322c98ef03d3`  
		Last Modified: Fri, 14 May 2021 19:47:50 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:lts`

```console
$ docker pull haproxy@sha256:e07d23cbfa10322d03ab965fab14a83793a3cf210cf6598b9bac04441b931b88
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
$ docker pull haproxy@sha256:bf2db25a5ee139ffcb728ea9acea1b0671fdcd761670753f6a9eb493fe7a439f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.2 MB (37226610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b68c771805b9ba3241a23c54e6f43e04a27da28659bca2760faca537bef973cd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 07:10:16 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:21:49 GMT
ENV HAPROXY_VERSION=2.4.0
# Fri, 14 May 2021 19:21:49 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Fri, 14 May 2021 19:21:49 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Fri, 14 May 2021 19:22:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 14 May 2021 19:22:36 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:22:36 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:22:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:22:37 GMT
USER haproxy
# Fri, 14 May 2021 19:22:37 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a113359dddc15238d26b375f86574b596b4aee1263a9631a7384589c2a02f46`  
		Last Modified: Wed, 12 May 2021 07:18:16 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e62dbde04094c3619ac833a9545588b66612ff4a0b35b59c7624708810658bb3`  
		Last Modified: Fri, 14 May 2021 19:25:20 GMT  
		Size: 10.1 MB (10078868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba498b86933facd6fdd59d94d7db13019b879e7cc25d041a68633d89e0494e2`  
		Last Modified: Fri, 14 May 2021 19:25:19 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:9bbe3920a362fbdd01643eb1d30ed94397a87cddd058275eccf322d60149697c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.6 MB (34593921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08b4c280b3718ed88ca7f0c20d62f39aa02eeacfcf409626e51607b0ac6f0949`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:55:35 GMT
ADD file:241925c5ca73c99d58f93bc78d7c5bfb6f8b280201a9b55ade45ba0cc054c31d in / 
# Wed, 12 May 2021 00:55:46 GMT
CMD ["bash"]
# Wed, 12 May 2021 02:01:24 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:49:51 GMT
ENV HAPROXY_VERSION=2.4.0
# Fri, 14 May 2021 19:49:53 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Fri, 14 May 2021 19:49:53 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Fri, 14 May 2021 19:50:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 14 May 2021 19:50:56 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:51:04 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:51:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:51:06 GMT
USER haproxy
# Fri, 14 May 2021 19:51:09 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:48885a8e20b16cb3bb9d2c3aafc7f040d8609844f69ca8482c42b4829d01b6da`  
		Last Modified: Wed, 12 May 2021 01:10:24 GMT  
		Size: 24.9 MB (24879601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e012f5248a53449f692d1fe91241d026aa60efe5a3dc3f04add4638989918d2a`  
		Last Modified: Wed, 12 May 2021 02:09:37 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:723c7fb393e70925e6268f228609b020286d9861091b490e8d2a0f254c59a09c`  
		Last Modified: Fri, 14 May 2021 19:52:16 GMT  
		Size: 9.7 MB (9712493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:001bde1f3aa007c516863db1818955f87f02ec4c19a730bf84f2399ddac9c7e2`  
		Last Modified: Fri, 14 May 2021 19:52:13 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:b5345ed4dd11a7cb423f4f59dbe9c7ba7cd2abe7afb893b77ddbfb32e5a77302
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.3 MB (32300104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c11a7eb8b982fbc0502c09a9021ba71ea4f9fed9830124aad9547d935b4dcd71`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:03:14 GMT
ADD file:94bf2394dc26abd9f028c2933057a8673c8562e58ec4a0f51bb9bde0a5e4dee0 in / 
# Wed, 12 May 2021 01:03:32 GMT
CMD ["bash"]
# Wed, 16 Jun 2021 12:48:11 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 12:50:51 GMT
ENV HAPROXY_VERSION=2.4.0
# Wed, 16 Jun 2021 12:50:51 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Wed, 16 Jun 2021 12:50:52 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Wed, 16 Jun 2021 12:51:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 16 Jun 2021 12:51:50 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 12:51:51 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 12:51:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 12:51:51 GMT
USER haproxy
# Wed, 16 Jun 2021 12:51:52 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:3035777cd90a3389593bc49a7b39b6f67f9f2679f4e04cc59515f4d5f83ad818`  
		Last Modified: Wed, 12 May 2021 01:19:13 GMT  
		Size: 22.7 MB (22746266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a03e197445bdc67b19867d9e201ef8f2078017e5ad57773c364b31ba9786e0e`  
		Last Modified: Wed, 16 Jun 2021 13:08:37 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dea3a7558a13f5154fb9ce6385d9667552cb71886d1e477e2519abbd5734d85`  
		Last Modified: Wed, 16 Jun 2021 13:09:11 GMT  
		Size: 9.6 MB (9552006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92403e8a9c35756b9b7e782fa08d4faae23520c5824807583c41db0674112c28`  
		Last Modified: Wed, 16 Jun 2021 13:09:08 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:7c4943ca2e6c7241331ed74abbd91deb9045a58ff899ea1c47d32878cce737fc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35869597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aad490d428518fedc8dee040fcd2c90f725415ef49be148b71b8c0e7929f2bdb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:52:19 GMT
ADD file:91ba1791cab3ad29a1469d1e78f21f4c0b5d3d30598683b7104980604c318854 in / 
# Wed, 12 May 2021 00:52:34 GMT
CMD ["bash"]
# Wed, 16 Jun 2021 00:32:29 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 00:34:32 GMT
ENV HAPROXY_VERSION=2.4.0
# Wed, 16 Jun 2021 00:34:33 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Wed, 16 Jun 2021 00:34:33 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Wed, 16 Jun 2021 00:35:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 16 Jun 2021 00:35:13 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 00:35:14 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 00:35:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 00:35:14 GMT
USER haproxy
# Wed, 16 Jun 2021 00:35:14 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:fcad0c936ea5c12e1c8c4edb81a97c0cde04ee71e7067ee3b246474cf1854d7a`  
		Last Modified: Wed, 12 May 2021 01:02:02 GMT  
		Size: 25.9 MB (25911250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48fc449d8b117694f567c81827185f03f8e4fa5c56b0b6626bb4374515d222c3`  
		Last Modified: Wed, 16 Jun 2021 00:44:41 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:928814acb1c13f0fd28a553528d1e135f7ffeb4a27bee2232022efda91ed70f2`  
		Last Modified: Wed, 16 Jun 2021 00:45:10 GMT  
		Size: 10.0 MB (9956513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c75f63ea187e14fb0d9052b1e9be0ce47a1c6d1dd4f03382ac3db42f865452`  
		Last Modified: Wed, 16 Jun 2021 00:45:08 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; 386

```console
$ docker pull haproxy@sha256:65807594f3fdb74f4aeb45cfb58775a8e9e60d00cf4ff637bdcf4343938cfc9c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.7 MB (37714061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b65e677154b7269853270de51028128fb357bdb375ab0bb6229de8bcc8796694`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:39:52 GMT
ADD file:62173a7456d614031a7b20be741983644d9723c734eee663b099ad6b47af7b35 in / 
# Wed, 12 May 2021 00:39:53 GMT
CMD ["bash"]
# Wed, 12 May 2021 05:59:03 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:43:27 GMT
ENV HAPROXY_VERSION=2.4.0
# Fri, 14 May 2021 19:43:27 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Fri, 14 May 2021 19:43:28 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Fri, 14 May 2021 19:44:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 14 May 2021 19:44:27 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:44:27 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:44:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:44:27 GMT
USER haproxy
# Fri, 14 May 2021 19:44:28 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:9b548256784c8e079e5953ec08bd26ce8cbaed0d606a5d350b4bcd12710d2192`  
		Last Modified: Wed, 12 May 2021 00:46:39 GMT  
		Size: 27.8 MB (27795074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05508dc89a5d9449eccbd1b8bf3910253f410f4654f50f119641aa3b5dc3e5c6`  
		Last Modified: Wed, 12 May 2021 06:11:24 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c528b6c319705bef71d9a02c957c8f71879b2f0d4911c0e693640c3485da157`  
		Last Modified: Fri, 14 May 2021 19:49:52 GMT  
		Size: 9.9 MB (9917160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20b09ad55a92c274b5ad2a914359180d1b3a163768611adacc46db20bed561f2`  
		Last Modified: Fri, 14 May 2021 19:49:49 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; mips64le

```console
$ docker pull haproxy@sha256:9eb21e12824743325f9a8ef93e2a38ec1eee12f374450edafc57ada973db7e36
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.5 MB (35507073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f68f334085d45c2aedb154ace750cc256f9188c28fec0134800ffcdf4d83c465`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:09:45 GMT
ADD file:867397d3fb44b3b936a4ff02bbc3a1b760fb6865b5a85efab82fff224f704241 in / 
# Wed, 12 May 2021 01:09:46 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:37:27 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:10:19 GMT
ENV HAPROXY_VERSION=2.4.0
# Fri, 14 May 2021 19:10:19 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Fri, 14 May 2021 19:10:19 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Fri, 14 May 2021 19:12:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 14 May 2021 19:12:46 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:12:47 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:12:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:12:47 GMT
USER haproxy
# Fri, 14 May 2021 19:12:48 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:09564b0ac149fb24b77cbc75ce6fa5d9ba61bd7c99d11b42bd8339c3bb28e557`  
		Last Modified: Wed, 12 May 2021 01:16:36 GMT  
		Size: 25.8 MB (25812884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18fb24fa0e81746ee8c86b23e726e84be12b3f40b71800e0be7e202dd3e3eae3`  
		Last Modified: Wed, 12 May 2021 01:51:31 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50629214220b6d4a25551564eda69255924a81c1d5abdf51759814d8ae33f010`  
		Last Modified: Fri, 14 May 2021 19:13:53 GMT  
		Size: 9.7 MB (9692361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d077c778db1d6d702a26fab8b56bdb796d3f66d02c2d7bc48f3136d5d38fad0`  
		Last Modified: Fri, 14 May 2021 19:13:41 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; ppc64le

```console
$ docker pull haproxy@sha256:ac3ce547cea71c004c0f5a85e52ff3b02f4b9ccb85ec55b9c62a29c1b0de2cdc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.1 MB (41134988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:917d9f0f429d84e805182b59da973eb98c74a1ec123db86414d9e0b287ebe1a6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 01:34:56 GMT
ADD file:3b8146cdc3649d94ad49435c94a21d700ed612ab90f010dcf8b22951b1804d34 in / 
# Wed, 12 May 2021 01:35:02 GMT
CMD ["bash"]
# Wed, 12 May 2021 06:07:29 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:29:30 GMT
ENV HAPROXY_VERSION=2.4.0
# Fri, 14 May 2021 19:29:37 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Fri, 14 May 2021 19:29:46 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Fri, 14 May 2021 19:40:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 14 May 2021 19:40:15 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:40:21 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:40:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:40:38 GMT
USER haproxy
# Fri, 14 May 2021 19:40:51 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:f8b445753f60bad25326d018945455601e4a65f124e956dec95c569816f21493`  
		Last Modified: Wed, 12 May 2021 01:44:19 GMT  
		Size: 30.6 MB (30552394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cfafb398e88c2b64b9fb82254775d63718baad006543dee4e7c370a09a23be9`  
		Last Modified: Wed, 12 May 2021 06:57:45 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b5a44e105c7ef3c0bbf570908dcb769a92fe1dc738dd5a563b76186b5557de`  
		Last Modified: Fri, 14 May 2021 19:46:14 GMT  
		Size: 10.6 MB (10580763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc69ed04682daa398fdabe5de724c14c1e3de1e7616f7bdcc79754f464d2dc13`  
		Last Modified: Fri, 14 May 2021 19:46:12 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; s390x

```console
$ docker pull haproxy@sha256:039479598c8aa940517ee6f080fcf62a4ebf12c189b385b1e924c5a53ad06d1b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.5 MB (35515830 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5edca0e2116433b35c4e5ad43d19aa27b5303a10ab98b9094ea0eb2afdf57a1b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 May 2021 00:43:38 GMT
ADD file:77af21d863769b75a5f055b85b2c9d6e878f9d77a4122397ae8dde6b69e945c6 in / 
# Wed, 12 May 2021 00:43:42 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:53:39 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:44:04 GMT
ENV HAPROXY_VERSION=2.4.0
# Fri, 14 May 2021 19:44:05 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Fri, 14 May 2021 19:44:05 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Fri, 14 May 2021 19:45:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Fri, 14 May 2021 19:45:07 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:45:08 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:45:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:45:09 GMT
USER haproxy
# Fri, 14 May 2021 19:45:09 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:ba4b99e0e723623b64d4ecb8d74102998d32137ea9bcc88b15fd2e4e34b38df9`  
		Last Modified: Wed, 12 May 2021 00:48:03 GMT  
		Size: 25.8 MB (25760171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f6911826fde538e80c00f0d90920d0d7d0a78db315f0bde1ee65726f99f6747`  
		Last Modified: Wed, 12 May 2021 02:04:41 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f093e4ce124ac637de93e3142fecae0c3318de7bd46e44842d671a7f6dbbc99`  
		Last Modified: Fri, 14 May 2021 19:47:51 GMT  
		Size: 9.8 MB (9753831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e979e3b25df89cd6dc9a3c62ae51d2fb6120a89a1a317126572e322c98ef03d3`  
		Last Modified: Fri, 14 May 2021 19:47:50 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `haproxy:lts-alpine`

```console
$ docker pull haproxy@sha256:f95a3663351046fcbf511c58ab51c27de20535d4d57ad23f1ff223236f9a55b5
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
$ docker pull haproxy@sha256:5cdbb12744cb989283fc2b3382cdef754a91a927ebe0f9590e603e5b71ba12aa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.2 MB (10189742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd47a280c45025ffbb379774e72f23fd33817110a32a6bc2bc9bfcd85d63862d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:37:38 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:22:49 GMT
ENV HAPROXY_VERSION=2.4.0
# Fri, 14 May 2021 19:22:49 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Fri, 14 May 2021 19:22:49 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Fri, 14 May 2021 19:23:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 14 May 2021 19:23:46 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:23:47 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:23:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:23:47 GMT
USER haproxy
# Fri, 14 May 2021 19:23:47 GMT
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
	-	`sha256:c44c996abc09e09ebd634f300b1f28f57d01f9130f916d9fdc38c37af7ee07c3`  
		Last Modified: Fri, 14 May 2021 19:25:37 GMT  
		Size: 7.4 MB (7376144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d9724e441af85a227fe782cd0b74e214d015f6c418bc9f5721ffc2b212fb1f`  
		Last Modified: Fri, 14 May 2021 19:25:36 GMT  
		Size: 445.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts-alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:69efaabcd2ab486de14ef6e2d6b516cb6b759129d42f7307075eacd194ba30b8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.2 MB (10236015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:547431eed6be392afc4baa1caf17cee9637ac4f56f3b37fa341952b199469d70`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:34 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Tue, 15 Jun 2021 22:57:34 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 11:05:46 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 11:07:14 GMT
ENV HAPROXY_VERSION=2.4.0
# Wed, 16 Jun 2021 11:07:14 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Wed, 16 Jun 2021 11:07:14 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Wed, 16 Jun 2021 11:08:32 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 16 Jun 2021 11:08:32 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 11:08:32 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 11:08:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 11:08:33 GMT
USER haproxy
# Wed, 16 Jun 2021 11:08:33 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1be2f4fa6ca9f7822eb93cc888d093da91b0748abe26e3ba14d94b6a757977`  
		Last Modified: Wed, 16 Jun 2021 11:14:47 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:921895821382ed60acd8406262950cfc04c55cbb7c92da354645f645fb554f21`  
		Last Modified: Wed, 16 Jun 2021 11:15:04 GMT  
		Size: 7.6 MB (7612250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aad1b8d3a0f3d5b3f80e86e995d24362cfa6b5eed57f6b2bd55c98482b02627`  
		Last Modified: Wed, 16 Jun 2021 11:15:02 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts-alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:edc40093cc1582d4de4f547bb1177784b83f7bdbfeb7bf2d6535ea524497e38e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9868170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2fb528c799b2206e2681f9c635b06b33b9fff9ad0950bd8fa77dafe72b68755`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:15 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Tue, 15 Jun 2021 23:15:16 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 12:49:38 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 12:52:05 GMT
ENV HAPROXY_VERSION=2.4.0
# Wed, 16 Jun 2021 12:52:06 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Wed, 16 Jun 2021 12:52:06 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Wed, 16 Jun 2021 12:53:49 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 16 Jun 2021 12:53:50 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 12:53:50 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 12:53:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 12:53:51 GMT
USER haproxy
# Wed, 16 Jun 2021 12:53:51 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0137e317a40af64134eac5d8b4d74173e380ac844679531b4f1fbdeeec3eb1f5`  
		Last Modified: Wed, 16 Jun 2021 13:08:54 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3338967b5822f35583ac2b289978e0842b8f53fbe0360d31e51bce77406f426`  
		Last Modified: Wed, 16 Jun 2021 13:09:34 GMT  
		Size: 7.4 MB (7442384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057d230ccbd07a75040acffce5ba60dc0d991e074f80db7252266f5015aa5227`  
		Last Modified: Wed, 16 Jun 2021 13:09:32 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts-alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:0c1515801d8462766011d15c30f9c895daf84d0bdc94c8075f18ea1a0feb0bcb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.5 MB (10501833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5552ae74aa48a3157768b495d7f900cbe8308844a4eabbb3d31efffaf91beccf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 00:33:20 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Wed, 16 Jun 2021 00:35:24 GMT
ENV HAPROXY_VERSION=2.4.0
# Wed, 16 Jun 2021 00:35:24 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Wed, 16 Jun 2021 00:35:24 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Wed, 16 Jun 2021 00:36:22 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 16 Jun 2021 00:36:22 GMT
STOPSIGNAL SIGUSR1
# Wed, 16 Jun 2021 00:36:22 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 16 Jun 2021 00:36:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 00:36:22 GMT
USER haproxy
# Wed, 16 Jun 2021 00:36:23 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd643f981edaf0694f3dad8fb6389455756f11cc027101d1de96b178f289891`  
		Last Modified: Wed, 16 Jun 2021 00:44:55 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6612ce2d4bb46fc19cf4e91024ff675545a937cbf9920f5bf6d952ae91fe7e`  
		Last Modified: Wed, 16 Jun 2021 00:45:30 GMT  
		Size: 7.8 MB (7788170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451357d82c6c73d346029d9a73684cbf29c7f1443a4ed10b429007517a0a55b4`  
		Last Modified: Wed, 16 Jun 2021 00:45:27 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts-alpine` - linux; 386

```console
$ docker pull haproxy@sha256:b6abb61fc5ca1faf9b49535b6d98a3ef2111b0cd553924ef5a681ffee22cb985
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (9953623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73c76984e00747ccebeec0318f85ee97b2f87f01eaf1b469043ab8ba4c6b4c5d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 01:50:06 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:44:40 GMT
ENV HAPROXY_VERSION=2.4.0
# Fri, 14 May 2021 19:44:40 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Fri, 14 May 2021 19:44:41 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Fri, 14 May 2021 19:46:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 14 May 2021 19:46:10 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:46:11 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:46:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:46:11 GMT
USER haproxy
# Fri, 14 May 2021 19:46:12 GMT
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
	-	`sha256:8331d4e675ebb11e0c29cae6830bda8fd3aa0499ef4bfe6ed7795c45349755a6`  
		Last Modified: Fri, 14 May 2021 19:50:14 GMT  
		Size: 7.1 MB (7133090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff87370dafdb2f94def6b9ba29cf0aca9f8849bf8c40cabf7b2762bcd53c3ce5`  
		Last Modified: Fri, 14 May 2021 19:50:11 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts-alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:b10a0c2c25132ccb0f3287d4b5a8a7876b5a9bb1bd5ae187218218f106a5e2fd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.5 MB (10509060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33dc9abd75900761fcf0d1d1308ee36b9899b33670e0f85e101b0708df8be39c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:25:09 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 14 May 2021 19:41:17 GMT
ENV HAPROXY_VERSION=2.4.0
# Fri, 14 May 2021 19:41:25 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.0.tar.gz
# Fri, 14 May 2021 19:41:37 GMT
ENV HAPROXY_SHA256=0a6962adaf5a1291db87e3eb4ddf906a72fed535dbd2255b164b7d8394a53640
# Fri, 14 May 2021 19:42:41 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Fri, 14 May 2021 19:43:13 GMT
STOPSIGNAL SIGUSR1
# Fri, 14 May 2021 19:43:25 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Fri, 14 May 2021 19:43:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 14 May 2021 19:43:56 GMT
USER haproxy
# Fri, 14 May 2021 19:44:09 GMT
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
	-	`sha256:084faba90127a3d6a1b87cb6cd6f44df9c75eb60f15c6d18b1121ca3562c4a97`  
		Last Modified: Fri, 14 May 2021 19:46:31 GMT  
		Size: 7.7 MB (7694282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecef18bca166de5b45c4de6bfb9e7ee9df71b6603ff3c1a4c2eb5fbf3dd6e4a1`  
		Last Modified: Fri, 14 May 2021 19:46:30 GMT  
		Size: 452.0 B  
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
