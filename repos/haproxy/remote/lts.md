## `haproxy:lts`

```console
$ docker pull haproxy@sha256:3f5cfc2de716dc93dc3b8fb9c7f101487821ea0ffadaebcf9885cfad62603329
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
$ docker pull haproxy@sha256:38986480a8e8e9327d4219375ae8c35b63fd9e389d039687c0f15918a1886390
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39466163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7c7171197a4c20ff9256bb2b949800fa9e49470510e7c39af47525117468d07`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 02 May 2023 23:46:59 GMT
ADD file:a2378c1b12e95db69e24b9d347441678c6f23239292cce3c822b1524992b6ec4 in / 
# Tue, 02 May 2023 23:47:00 GMT
CMD ["bash"]
# Wed, 03 May 2023 21:12:57 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Wed, 03 May 2023 21:14:20 GMT
ENV HAPROXY_VERSION=2.6.13
# Wed, 03 May 2023 21:14:20 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.6/src/haproxy-2.6.13.tar.gz
# Wed, 03 May 2023 21:14:20 GMT
ENV HAPROXY_SHA256=d69ff5233dbca657132ef280d111222ec1e33f5be1c1937d4e9ff516f63f5243
# Wed, 03 May 2023 21:14:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 03 May 2023 21:14:53 GMT
STOPSIGNAL SIGUSR1
# Wed, 03 May 2023 21:14:53 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 03 May 2023 21:14:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 May 2023 21:14:53 GMT
USER haproxy
# Wed, 03 May 2023 21:14:53 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:9e3ea8720c6de96cc9ad544dddc695a3ab73f5581c5d954e0504cc4f80fb5e5c`  
		Last Modified: Tue, 02 May 2023 23:50:22 GMT  
		Size: 31.4 MB (31403516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ead48c794e510566abe6fca2ed17abede9c4c0f4787d57d5bed855556f121f`  
		Last Modified: Wed, 03 May 2023 21:18:15 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:648c3007f7199ff1bd5a35a8e81e9e36419d47d8cf5cfde1a37c7a7908c43346`  
		Last Modified: Wed, 03 May 2023 21:18:47 GMT  
		Size: 8.1 MB (8060762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3a0bb4d104cc512f66e7b9552d934767cb30c74b4f71720494665952cc1754`  
		Last Modified: Wed, 03 May 2023 21:18:46 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:da496774a60ca312b5f73cbbe39a387e0806f4a0cf142567396c46086c20f32e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.9 MB (36851662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77972008013d17cb90ad2ac32d3f0579d9ed793e831b14737d6bdd7a7827bca7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 02 May 2023 22:48:53 GMT
ADD file:ca82c0d9094c1022a00b5f2157a02e1a9032aafc357a41c76c6b60bd74d25395 in / 
# Tue, 02 May 2023 22:48:53 GMT
CMD ["bash"]
# Wed, 03 May 2023 08:59:54 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Wed, 03 May 2023 09:01:13 GMT
ENV HAPROXY_VERSION=2.6.13
# Wed, 03 May 2023 09:01:14 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.6/src/haproxy-2.6.13.tar.gz
# Wed, 03 May 2023 09:01:14 GMT
ENV HAPROXY_SHA256=d69ff5233dbca657132ef280d111222ec1e33f5be1c1937d4e9ff516f63f5243
# Wed, 03 May 2023 09:01:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 03 May 2023 09:01:44 GMT
STOPSIGNAL SIGUSR1
# Wed, 03 May 2023 09:01:44 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 03 May 2023 09:01:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 May 2023 09:01:45 GMT
USER haproxy
# Wed, 03 May 2023 09:01:45 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:eb6ee5d3f82142e70aca665cea92048b1a46ff1aa5c5be47a04c27a471470c07`  
		Last Modified: Tue, 02 May 2023 22:51:25 GMT  
		Size: 28.9 MB (28903418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da417f762af8426d1f4e7224ccffe481c6619d696bec1f4ee9d3527ff87b1d0e`  
		Last Modified: Wed, 03 May 2023 09:03:41 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcd8cccff45e8bc149bdb48f4462438bb70a2912c9175ed0a2b6d87edfda1393`  
		Last Modified: Wed, 03 May 2023 09:04:14 GMT  
		Size: 7.9 MB (7946360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea3d68c2e3999415fa1d778293559e3707b51fb392f59fa41e33160cc857bb0a`  
		Last Modified: Wed, 03 May 2023 09:04:12 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:d26f058d4876d7a676ec32bffe4d8ee7cb8b62e8718e42f5fc11f6144e129f10
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.4 MB (34376589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdcafd1b474acd6dfcaf36433aaf3943f355062e1fd7732f2333a3e1ff6e5edb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 02 May 2023 23:47:57 GMT
ADD file:69d82e947b50a0f0ec610822ffe7c23ec1f6eb41bc17068502380f827cbcce40 in / 
# Tue, 02 May 2023 23:47:57 GMT
CMD ["bash"]
# Wed, 03 May 2023 22:13:53 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Wed, 03 May 2023 22:15:01 GMT
ENV HAPROXY_VERSION=2.6.13
# Wed, 03 May 2023 22:15:01 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.6/src/haproxy-2.6.13.tar.gz
# Wed, 03 May 2023 22:15:01 GMT
ENV HAPROXY_SHA256=d69ff5233dbca657132ef280d111222ec1e33f5be1c1937d4e9ff516f63f5243
# Wed, 03 May 2023 22:15:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 03 May 2023 22:15:28 GMT
STOPSIGNAL SIGUSR1
# Wed, 03 May 2023 22:15:28 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 03 May 2023 22:15:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 May 2023 22:15:28 GMT
USER haproxy
# Wed, 03 May 2023 22:15:28 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:9c7c4e67baad3ce38491ce8c1ffaa9ca9ce37409270ce53ab3472054f35d097e`  
		Last Modified: Tue, 02 May 2023 23:51:30 GMT  
		Size: 26.6 MB (26564648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60385b656c25b844b71c8b0ae55269df1f0a70bc2ae302c27bd04ab12789d060`  
		Last Modified: Wed, 03 May 2023 22:18:17 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb038a529eaad6ecf8af0ea34eea2e6fe12aa3ceeeec40225038ca7d0bc2be6`  
		Last Modified: Wed, 03 May 2023 22:18:50 GMT  
		Size: 7.8 MB (7810055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7de3fd76b15a44f5bfb99f7f4c7c0320f2e6289fa6d5b16c10805c9183ae478d`  
		Last Modified: Wed, 03 May 2023 22:18:48 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:3a144b8da65806fbb90cd34d89983d903467eda1819b9729aa608c45104c4f02
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.1 MB (38127091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8b6a343b7e9ee10c8da8e0b0bcb3506ba7f7a462c642190ce1b16238f409bc7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 18:03:26 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Wed, 03 May 2023 18:04:35 GMT
ENV HAPROXY_VERSION=2.6.13
# Wed, 03 May 2023 18:04:35 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.6/src/haproxy-2.6.13.tar.gz
# Wed, 03 May 2023 18:04:35 GMT
ENV HAPROXY_SHA256=d69ff5233dbca657132ef280d111222ec1e33f5be1c1937d4e9ff516f63f5243
# Wed, 03 May 2023 18:04:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 03 May 2023 18:04:59 GMT
STOPSIGNAL SIGUSR1
# Wed, 03 May 2023 18:04:59 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 03 May 2023 18:04:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 May 2023 18:04:59 GMT
USER haproxy
# Wed, 03 May 2023 18:04:59 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b6580e723b3959fc6b5aa5b328c60a932fe59f60d8d8609468209dbd9d5d02`  
		Last Modified: Wed, 03 May 2023 18:07:25 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abf7d1fc8e6b2e3956adf8282f42fcdf79d0479d92aa7a0e6d3e1b52e7577a61`  
		Last Modified: Wed, 03 May 2023 18:07:56 GMT  
		Size: 8.1 MB (8072472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d9694009a62ab3294539ce7622a745ada727413855ec7668931c81bfe80cf5`  
		Last Modified: Wed, 03 May 2023 18:07:55 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; 386

```console
$ docker pull haproxy@sha256:53b28e846a7f6f9996d3e7d131d8958cae7e763d885827e2ef5085d449e03a4c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40229344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fcd5d809a7d62c47c96ba044ab11c874c2a96bb6656fd96ab68bfb256bf3313`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 03 May 2023 00:00:58 GMT
ADD file:caea439e2dbe0148904e3b9a0c5a843d2d0b7c196725d2b41790594e64dcdce8 in / 
# Wed, 03 May 2023 00:00:58 GMT
CMD ["bash"]
# Wed, 03 May 2023 22:40:03 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Wed, 03 May 2023 22:42:22 GMT
ENV HAPROXY_VERSION=2.6.13
# Wed, 03 May 2023 22:42:22 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.6/src/haproxy-2.6.13.tar.gz
# Wed, 03 May 2023 22:42:22 GMT
ENV HAPROXY_SHA256=d69ff5233dbca657132ef280d111222ec1e33f5be1c1937d4e9ff516f63f5243
# Wed, 03 May 2023 22:43:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 03 May 2023 22:43:20 GMT
STOPSIGNAL SIGUSR1
# Wed, 03 May 2023 22:43:20 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 03 May 2023 22:43:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 May 2023 22:43:20 GMT
USER haproxy
# Wed, 03 May 2023 22:43:20 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:10b34014bd1c165cc57a10e7492f17dce658513b7329319fe6c193c85bf752db`  
		Last Modified: Wed, 03 May 2023 00:05:12 GMT  
		Size: 32.4 MB (32388208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:510967bab0cc8080787589baa0b54c8f8d7da83cf9ba2e885877ff4574314f99`  
		Last Modified: Wed, 03 May 2023 22:48:13 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53eac648b8ba7333b712b0064b8d57782eb123f98df573f6ceb7f3e24e390c95`  
		Last Modified: Wed, 03 May 2023 22:48:47 GMT  
		Size: 7.8 MB (7839250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b645efb59b9702017604581ec8b50f67b616033474a1b053aa3d991cb2ff1a2`  
		Last Modified: Wed, 03 May 2023 22:48:46 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; mips64le

```console
$ docker pull haproxy@sha256:af28ca430dd98b126c3603371dec2815b4b35f31a1e6bbde582125acbbf4bb52
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.8 MB (37800853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2ee78432839e78ee88954088765b1142fd8a3f77a02d3d2c7473c6383354a5b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 02 May 2023 23:49:45 GMT
ADD file:c3427ec4e3a2c988fdd372b529660d45ee105e317d6a964ce96f8f9009a3c21e in / 
# Tue, 02 May 2023 23:49:49 GMT
CMD ["bash"]
# Thu, 04 May 2023 01:32:33 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Thu, 04 May 2023 01:40:41 GMT
ENV HAPROXY_VERSION=2.6.13
# Thu, 04 May 2023 01:40:43 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.6/src/haproxy-2.6.13.tar.gz
# Thu, 04 May 2023 01:40:46 GMT
ENV HAPROXY_SHA256=d69ff5233dbca657132ef280d111222ec1e33f5be1c1937d4e9ff516f63f5243
# Thu, 04 May 2023 01:44:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 04 May 2023 01:44:03 GMT
STOPSIGNAL SIGUSR1
# Thu, 04 May 2023 01:44:05 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 04 May 2023 01:44:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 May 2023 01:44:09 GMT
USER haproxy
# Thu, 04 May 2023 01:44:12 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:498edd615f8781385e0d5246e189d80b5caceb207fe26608a12605d0a823d4df`  
		Last Modified: Tue, 02 May 2023 23:58:10 GMT  
		Size: 29.6 MB (29623482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98e3e1f1fd0ee7840a8696951cd0af6cc67d5d150fb905dbc25c0e907dfe760`  
		Last Modified: Thu, 04 May 2023 01:56:08 GMT  
		Size: 1.3 KB (1300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7e1e5dc7e829cab80ef7aef168305dc09af5f77e1300acf75e801df926be13b`  
		Last Modified: Thu, 04 May 2023 01:56:54 GMT  
		Size: 8.2 MB (8175618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e34a1b05a5f11e9fad4a009dc3f42747a74c5b7d23bba3e42e26617e38448d`  
		Last Modified: Thu, 04 May 2023 01:56:48 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; ppc64le

```console
$ docker pull haproxy@sha256:04a09ee3f2c3ba45f24afe18c0e2b3ef6111a75a7150db495418329fbfeab5b8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.7 MB (43744731 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5fd9e169b6018df950a6095c1628bc9fc4489bb3df03694bfbd042fb45e7120`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 03 May 2023 00:31:50 GMT
ADD file:ee3b3c43add645e1a2078f2a6e8544d223abf2754eb8039cbbc2cbdb911b49bb in / 
# Wed, 03 May 2023 00:31:52 GMT
CMD ["bash"]
# Wed, 03 May 2023 23:48:04 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Wed, 03 May 2023 23:51:11 GMT
ENV HAPROXY_VERSION=2.6.13
# Wed, 03 May 2023 23:51:11 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.6/src/haproxy-2.6.13.tar.gz
# Wed, 03 May 2023 23:51:12 GMT
ENV HAPROXY_SHA256=d69ff5233dbca657132ef280d111222ec1e33f5be1c1937d4e9ff516f63f5243
# Wed, 03 May 2023 23:52:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 03 May 2023 23:52:21 GMT
STOPSIGNAL SIGUSR1
# Wed, 03 May 2023 23:52:22 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 03 May 2023 23:52:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 May 2023 23:52:23 GMT
USER haproxy
# Wed, 03 May 2023 23:52:23 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:e39c6de44f96d2720b144cbaa9e763eac60a69222a96279f3962e8a701fb17ac`  
		Last Modified: Wed, 03 May 2023 00:36:56 GMT  
		Size: 35.3 MB (35280910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5a167b55ef4d6f0f6b337280b467d0d2ebc1d5bca0e2613a5e6a635f79e934c`  
		Last Modified: Wed, 03 May 2023 23:57:12 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0038f411509d97bbd18fc880484c0077fe42b00cce2ef11362c3bb89a02deafe`  
		Last Modified: Wed, 03 May 2023 23:57:50 GMT  
		Size: 8.5 MB (8461932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06556be8382474f1998d62ece3e916c49062e856b6ab04f6ab00d6b8fee26aab`  
		Last Modified: Wed, 03 May 2023 23:57:48 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; s390x

```console
$ docker pull haproxy@sha256:ca6fcf68fee4c61ad816cd3acc971e8b3b892d24628f9d4350cf428942f62dc0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.7 MB (37711597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eae8587792fdae64ffb106f3a6843de7b1005e1c7084068f36a676cf9033d271`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 03 May 2023 03:41:57 GMT
ADD file:7dcdb7d695d9510a1a7e1623776d63d56f7025bdd1702a13a3acd52af825b9c3 in / 
# Wed, 03 May 2023 03:41:59 GMT
CMD ["bash"]
# Wed, 03 May 2023 22:12:16 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Wed, 03 May 2023 22:13:35 GMT
ENV HAPROXY_VERSION=2.6.13
# Wed, 03 May 2023 22:13:35 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.6/src/haproxy-2.6.13.tar.gz
# Wed, 03 May 2023 22:13:35 GMT
ENV HAPROXY_SHA256=d69ff5233dbca657132ef280d111222ec1e33f5be1c1937d4e9ff516f63f5243
# Wed, 03 May 2023 22:14:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 03 May 2023 22:14:03 GMT
STOPSIGNAL SIGUSR1
# Wed, 03 May 2023 22:14:03 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 03 May 2023 22:14:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 May 2023 22:14:04 GMT
USER haproxy
# Wed, 03 May 2023 22:14:04 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:8e4cb8eb5d7a86a02dfc1d3645e982def0fc1c20e1fd14d9c6736177d3887dfa`  
		Last Modified: Wed, 03 May 2023 03:44:59 GMT  
		Size: 29.6 MB (29642157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cc781c042e577de5023198d4d9cdda11648fcac0ba88909c455d004ae9f89f5`  
		Last Modified: Wed, 03 May 2023 22:16:48 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffd62d08d6585d2349b406dd3961635761d0063ba4753901054c36c64d0fa6b`  
		Last Modified: Wed, 03 May 2023 22:17:11 GMT  
		Size: 8.1 MB (8067553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3917849bf12b21e9ae503faae3c029307db08668e55cf9be71339cadd737b2d2`  
		Last Modified: Wed, 03 May 2023 22:17:09 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
