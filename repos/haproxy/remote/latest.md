## `haproxy:latest`

```console
$ docker pull haproxy@sha256:a6639b3773f04356c916689bf1747f5325e843c44c688da50bff3574a56c6cb9
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
$ docker pull haproxy@sha256:d1fce0a85f97ac242541d240cd0fc72c0a7fc3241bb13684e5dab12eb7134b49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.6 MB (39627247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52c3cf883c55a4318d879b1794ff5d20eec7f6349a06b73527a539098e7295aa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 06 Dec 2022 01:20:54 GMT
ADD file:1f1efd56601ebc26a041a7b994a380ef68112b91a078e225753bee7b3196d22c in / 
# Tue, 06 Dec 2022 01:20:54 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 04:27:26 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Tue, 06 Dec 2022 04:28:16 GMT
ENV HAPROXY_VERSION=2.7.0
# Tue, 06 Dec 2022 04:28:16 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.7/src/haproxy-2.7.0.tar.gz
# Tue, 06 Dec 2022 04:28:16 GMT
ENV HAPROXY_SHA256=0f7bdebd9b0d7abfd89087bf36af6bd1520d3234266349786654e32e186b4768
# Tue, 06 Dec 2022 04:28:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Tue, 06 Dec 2022 04:28:54 GMT
STOPSIGNAL SIGUSR1
# Tue, 06 Dec 2022 04:28:54 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Tue, 06 Dec 2022 04:28:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 04:28:54 GMT
USER haproxy
# Tue, 06 Dec 2022 04:28:55 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:025c56f98b679f70b7a54241917e56da7b59ab9d2defecc6ebdb0bf2750484bb`  
		Last Modified: Tue, 06 Dec 2022 01:25:12 GMT  
		Size: 31.4 MB (31412852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c297050c4bb7915a5baac9a999924486e83e9e395480cfaa93a439e2da2a080`  
		Last Modified: Tue, 06 Dec 2022 04:34:18 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce2b578884d85de05c74f94e67f82ef282f08d4ac73b1a1871ec62d09a3dc26f`  
		Last Modified: Tue, 06 Dec 2022 04:34:34 GMT  
		Size: 8.2 MB (8212509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a00f43ccaed9443d25db9eb49e7539fe0cdf870a68fad75613f9a3d1a1d9368`  
		Last Modified: Tue, 06 Dec 2022 04:34:33 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:latest` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:a65a3507b224af75c8e763072e5b6e3db8c6056a6c3b56deeda31e324ac685cb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36988181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cfa25dba53c7a226d09ed8085550a257484aadda061e5006d416c1dd40fdd7d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 06 Dec 2022 01:49:26 GMT
ADD file:3333e32449573e158be62ea6948788daec95a151f49035d65db8d7cb72b42c53 in / 
# Tue, 06 Dec 2022 01:49:27 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 03:02:08 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Tue, 06 Dec 2022 03:02:52 GMT
ENV HAPROXY_VERSION=2.7.0
# Tue, 06 Dec 2022 03:02:52 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.7/src/haproxy-2.7.0.tar.gz
# Tue, 06 Dec 2022 03:02:52 GMT
ENV HAPROXY_SHA256=0f7bdebd9b0d7abfd89087bf36af6bd1520d3234266349786654e32e186b4768
# Tue, 06 Dec 2022 03:03:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Tue, 06 Dec 2022 03:03:28 GMT
STOPSIGNAL SIGUSR1
# Tue, 06 Dec 2022 03:03:28 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Tue, 06 Dec 2022 03:03:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 03:03:28 GMT
USER haproxy
# Tue, 06 Dec 2022 03:03:28 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:98c2ef299f89748b9c6075c728521ba8fe6e236fa46f50c465894cdb0ce69b35`  
		Last Modified: Tue, 06 Dec 2022 01:54:34 GMT  
		Size: 28.9 MB (28914353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5ac1ccbcd1bf8c8167c30ec597cbe62c2ea662051227b1e6877e41615ae062`  
		Last Modified: Tue, 06 Dec 2022 03:08:07 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1414a64e06ab68312a04761d7f240cf608ef3eb7f11d363c4fd6216edcd9d7c1`  
		Last Modified: Tue, 06 Dec 2022 03:08:26 GMT  
		Size: 8.1 MB (8071976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99938edee7c4d8b477758ab0705b1ba0c96c641bfe135da9438933fae5da388`  
		Last Modified: Tue, 06 Dec 2022 03:08:25 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:latest` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:9489550112ee62e690fd5da198d6e6ebcee9a2d2f0ef13698082fd0f4722f0de
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 MB (34500556 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43819b7cee1c1733e9346e16518b90c1398ea6e33e3de593ed51468d15d91bc3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 06 Dec 2022 00:58:51 GMT
ADD file:cb354f875d5631d5d4542ab57d0b9b323a261f5c631d5917127504d6eb54d85a in / 
# Tue, 06 Dec 2022 00:58:52 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:26:04 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Tue, 06 Dec 2022 01:26:50 GMT
ENV HAPROXY_VERSION=2.7.0
# Tue, 06 Dec 2022 01:26:50 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.7/src/haproxy-2.7.0.tar.gz
# Tue, 06 Dec 2022 01:26:50 GMT
ENV HAPROXY_SHA256=0f7bdebd9b0d7abfd89087bf36af6bd1520d3234266349786654e32e186b4768
# Tue, 06 Dec 2022 01:27:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Tue, 06 Dec 2022 01:27:19 GMT
STOPSIGNAL SIGUSR1
# Tue, 06 Dec 2022 01:27:19 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Tue, 06 Dec 2022 01:27:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 01:27:19 GMT
USER haproxy
# Tue, 06 Dec 2022 01:27:20 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:4f32a98d14d26603bb8e8cf9bda992e24606d2fe00101767049a01d5176929e1`  
		Last Modified: Tue, 06 Dec 2022 01:06:05 GMT  
		Size: 26.6 MB (26576348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8cbd1a21b2bc29fc9900d679231ccaa60f67c6184e66cd108219008bb0117d3`  
		Last Modified: Tue, 06 Dec 2022 01:34:58 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec67deaf1556dc3ba8a54016e1b59480741418f4998a0b6aedaeeeae43dfb0a`  
		Last Modified: Tue, 06 Dec 2022 01:35:23 GMT  
		Size: 7.9 MB (7922354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90a8f4964017251921f5f2b72370b3bc4a04052cba8b75cd03ed53b6d899495d`  
		Last Modified: Tue, 06 Dec 2022 01:35:21 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:latest` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:b8968a5fd7913e4075a7ec67e40f988d343a53685dea6269b60e30f53ab16fad
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.2 MB (38230903 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e906a1272f9a16834a9adf3ccc7e185ca8ff2791fcd9ca80c70b871cba0fa8a3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 03:38:54 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Tue, 06 Dec 2022 03:39:29 GMT
ENV HAPROXY_VERSION=2.7.0
# Tue, 06 Dec 2022 03:39:29 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.7/src/haproxy-2.7.0.tar.gz
# Tue, 06 Dec 2022 03:39:29 GMT
ENV HAPROXY_SHA256=0f7bdebd9b0d7abfd89087bf36af6bd1520d3234266349786654e32e186b4768
# Tue, 06 Dec 2022 03:39:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Tue, 06 Dec 2022 03:39:53 GMT
STOPSIGNAL SIGUSR1
# Tue, 06 Dec 2022 03:39:53 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Tue, 06 Dec 2022 03:39:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 03:39:53 GMT
USER haproxy
# Tue, 06 Dec 2022 03:39:54 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ae2d8a44ac017137594f8621ec941d2487bb2ec2198fc683dbe83e90d4d06d`  
		Last Modified: Tue, 06 Dec 2022 03:44:01 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4337ed04dd3c9b149db9032b64a057b3d532484149138b1f1f70d2deb5b42167`  
		Last Modified: Tue, 06 Dec 2022 03:44:17 GMT  
		Size: 8.2 MB (8168694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:468ea8721699e48dd6b36934e3de3842edae79f94e67f435b7950d7fc3bdde0a`  
		Last Modified: Tue, 06 Dec 2022 03:44:16 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:latest` - linux; 386

```console
$ docker pull haproxy@sha256:aadc9322645f814baa30032de8a0425a88e89ae0336c35394da75112ccc8fd13
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.4 MB (40378972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1ace3bdcca62499da2f8a4d2711fed2bfc4dbd2357acefd745bca4accdd8f06`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 06 Dec 2022 01:39:52 GMT
ADD file:3912079114d3e8e334fdf795a4793a492f37989804e1148b98fafbd4eaa00b7e in / 
# Tue, 06 Dec 2022 01:39:52 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:19:09 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Tue, 06 Dec 2022 02:20:05 GMT
ENV HAPROXY_VERSION=2.7.0
# Tue, 06 Dec 2022 02:20:06 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.7/src/haproxy-2.7.0.tar.gz
# Tue, 06 Dec 2022 02:20:07 GMT
ENV HAPROXY_SHA256=0f7bdebd9b0d7abfd89087bf36af6bd1520d3234266349786654e32e186b4768
# Tue, 06 Dec 2022 02:20:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Tue, 06 Dec 2022 02:20:43 GMT
STOPSIGNAL SIGUSR1
# Tue, 06 Dec 2022 02:20:45 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Tue, 06 Dec 2022 02:20:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 02:20:46 GMT
USER haproxy
# Tue, 06 Dec 2022 02:20:47 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:01cb95e209fce595702ddb2b5ed266e2a01b6687efe67d201d74a5aee9595995`  
		Last Modified: Tue, 06 Dec 2022 01:45:41 GMT  
		Size: 32.4 MB (32393046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d5682a6b48fe14c158e6132eac8a7385eaea455b701fcb80397fbd823c14f5`  
		Last Modified: Tue, 06 Dec 2022 02:28:40 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b8b42de23725968b3e8052f0bba2d85ce150eb259a750d93de33c3c78ee0f2`  
		Last Modified: Tue, 06 Dec 2022 02:29:00 GMT  
		Size: 8.0 MB (7984189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3572200c51b1d6c09dafa8cf0f2fb65b42d898b736c60da519a32361656f1a1`  
		Last Modified: Tue, 06 Dec 2022 02:28:59 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:latest` - linux; mips64le

```console
$ docker pull haproxy@sha256:a978ada01778df2e4fc2fb4f527b26a706c64aa24c212f17b1dea9c4562f2a5f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.9 MB (37916050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00e647b008f1849f2e05f1d1ddd401e9e88d31894f90e0e9e87e0a7464ecb521`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Nov 2022 04:13:42 GMT
ADD file:da7bed758c1e8c14583d53792170b6f4133a408ce2966e22ce52905f5c0d55a4 in / 
# Tue, 15 Nov 2022 04:13:46 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 23:43:27 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Thu, 01 Dec 2022 21:43:23 GMT
ENV HAPROXY_VERSION=2.7.0
# Thu, 01 Dec 2022 21:43:25 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.7/src/haproxy-2.7.0.tar.gz
# Thu, 01 Dec 2022 21:43:28 GMT
ENV HAPROXY_SHA256=0f7bdebd9b0d7abfd89087bf36af6bd1520d3234266349786654e32e186b4768
# Thu, 01 Dec 2022 21:46:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 01 Dec 2022 21:46:53 GMT
STOPSIGNAL SIGUSR1
# Thu, 01 Dec 2022 21:46:55 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 01 Dec 2022 21:46:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 21:47:00 GMT
USER haproxy
# Thu, 01 Dec 2022 21:47:02 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:27e2cdb4ebe2b6ee11014db328a4a8a055e3dcee2e275bf3aca6f03b39a09ad5`  
		Last Modified: Tue, 15 Nov 2022 04:21:14 GMT  
		Size: 29.6 MB (29635497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c19145edc1930601b168ceacf3561a59f54375c3954e812d75f040596a0e377d`  
		Last Modified: Wed, 16 Nov 2022 00:02:26 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c004852e4d9d6b2b470f0f4b604388d2c712800b2896318dfe85c3d3c8616ee4`  
		Last Modified: Thu, 01 Dec 2022 21:48:16 GMT  
		Size: 8.3 MB (8278797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c03d13deda7f779fd9e614d374fce23b4f38eec8bb77a94a860867a7377aff7`  
		Last Modified: Thu, 01 Dec 2022 21:48:07 GMT  
		Size: 457.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:latest` - linux; ppc64le

```console
$ docker pull haproxy@sha256:5622c382a242f1fa5083b1e4868b7211c3822e88902b140af7c9bfcf0aafa285
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.9 MB (43883625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdd15d3b6a535df422f710b68deaa2c5c7aee1ef9e62c193e047bd93adff09f1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 06 Dec 2022 01:18:04 GMT
ADD file:2231a44ea52d93df58e23883ba6b6911d4c554f4c1d172d80fb21c751ddcbbfc in / 
# Tue, 06 Dec 2022 01:18:06 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 01:45:22 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Tue, 06 Dec 2022 01:46:37 GMT
ENV HAPROXY_VERSION=2.7.0
# Tue, 06 Dec 2022 01:46:37 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.7/src/haproxy-2.7.0.tar.gz
# Tue, 06 Dec 2022 01:46:38 GMT
ENV HAPROXY_SHA256=0f7bdebd9b0d7abfd89087bf36af6bd1520d3234266349786654e32e186b4768
# Tue, 06 Dec 2022 01:47:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Tue, 06 Dec 2022 01:47:28 GMT
STOPSIGNAL SIGUSR1
# Tue, 06 Dec 2022 01:47:29 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Tue, 06 Dec 2022 01:47:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 06 Dec 2022 01:47:29 GMT
USER haproxy
# Tue, 06 Dec 2022 01:47:30 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:1f72e1168976861c676bf86a6c149129baba7e13200e8b70e6f24dc2ac2797df`  
		Last Modified: Tue, 06 Dec 2022 01:24:18 GMT  
		Size: 35.3 MB (35285293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b697b0e4b6ba50be9aa3b056b0ad1f0cf907bf72b2a666b2e6fcb0b3efc86e97`  
		Last Modified: Tue, 06 Dec 2022 01:54:27 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20c240a256487468db953174b7dbd089000abf914d2f30fd15b0abe099652707`  
		Last Modified: Tue, 06 Dec 2022 01:54:52 GMT  
		Size: 8.6 MB (8596451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d73b271728dfaa0d9da928b4c40effc7055cc6d2459a66307cdc472acf4b116b`  
		Last Modified: Tue, 06 Dec 2022 01:54:49 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:latest` - linux; s390x

```console
$ docker pull haproxy@sha256:35aeef3dea2fffeb21284652cc186f8ea0e64e907a511d573eb9d8851d669499
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.8 MB (37840938 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5ed940c1db617eede5f12e14968cc73f79ec156b1fc91a02269f05d9cda8afb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Nov 2022 01:42:51 GMT
ADD file:af482bbfc85f1f292de8bd5f2751ee2b67ec9e057eab3684f96984f0e4ecf943 in / 
# Tue, 15 Nov 2022 01:42:56 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 13:17:23 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Thu, 01 Dec 2022 21:10:55 GMT
ENV HAPROXY_VERSION=2.7.0
# Thu, 01 Dec 2022 21:10:55 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.7/src/haproxy-2.7.0.tar.gz
# Thu, 01 Dec 2022 21:10:55 GMT
ENV HAPROXY_SHA256=0f7bdebd9b0d7abfd89087bf36af6bd1520d3234266349786654e32e186b4768
# Thu, 01 Dec 2022 21:11:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 01 Dec 2022 21:11:34 GMT
STOPSIGNAL SIGUSR1
# Thu, 01 Dec 2022 21:11:34 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 01 Dec 2022 21:11:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 21:11:35 GMT
USER haproxy
# Thu, 01 Dec 2022 21:11:35 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:a6ad801d746b7bdde3a0ef72107d05694a38101de03b6eed340af802bdf13957`  
		Last Modified: Tue, 15 Nov 2022 01:47:33 GMT  
		Size: 29.6 MB (29643781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3beabbac8d8220cb7b1a7e7a740a6093ace46da9614c60eea0c8550523f8ae7`  
		Last Modified: Tue, 15 Nov 2022 13:30:29 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b59b1f5199119c913155ddffbd0ba887e62f803e8b1215511ceb29313eb7165`  
		Last Modified: Thu, 01 Dec 2022 21:18:38 GMT  
		Size: 8.2 MB (8195268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd29bc971bef4b0ffc50c013f58c312822df3ca1af18f7b9ea4f5ff064fc14f8`  
		Last Modified: Thu, 01 Dec 2022 21:18:37 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
