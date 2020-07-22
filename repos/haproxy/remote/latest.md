## `haproxy:latest`

```console
$ docker pull haproxy@sha256:5e8c072f36b5b85994813c4d3855b1f8822c769d28a6681791fb5bb2a1e264ab
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
$ docker pull haproxy@sha256:b4e4b260984801a7ab1c00a3f2e31fa8e19baf45fafc39cd0f3e6e7d847af7f2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36312613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e5227f896c4b067d569732d2db91f29b0d2d759b20ac00341338a5f327cb1f6`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 09 Jun 2020 01:20:56 GMT
ADD file:4d35f6c8bbbe6801cc5f44989730fb6d349a644ecb36eca481e7df25842d6321 in / 
# Tue, 09 Jun 2020 01:20:56 GMT
CMD ["bash"]
# Wed, 08 Jul 2020 17:26:31 GMT
ENV HAPROXY_VERSION=2.2.0
# Wed, 08 Jul 2020 17:26:32 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.0.tar.gz
# Wed, 08 Jul 2020 17:26:32 GMT
ENV HAPROXY_SHA256=3c1a87160eea40e067f1e2813bfe692280a10c455beb17a8ee7fae11e4223274
# Wed, 08 Jul 2020 17:27:25 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(nproc)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& apt-mark auto '.*' > /dev/null 	&& { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; } 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 08 Jul 2020 17:27:26 GMT
STOPSIGNAL SIGUSR1
# Wed, 08 Jul 2020 17:27:26 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Wed, 08 Jul 2020 17:27:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 08 Jul 2020 17:27:26 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:8559a31e96f442f2c7b6da49d6c84705f98a39d8be10b3f5f14821d0ee8417df`  
		Last Modified: Tue, 09 Jun 2020 01:25:50 GMT  
		Size: 27.1 MB (27098265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:750692642e7f89adcaa7fc3412c7ef38f9638b59a36b9411a0ef76456016f584`  
		Last Modified: Wed, 08 Jul 2020 17:29:26 GMT  
		Size: 9.2 MB (9213968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:429cbaf04cbfce8beb545c3603ee6554a8a9a8e5f71296ce62c96a2f43a2d9ed`  
		Last Modified: Wed, 08 Jul 2020 17:29:24 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:latest` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:9bdc3a2a7a3d77d0b8457f7bfcd5ef7ea19f9d49dc19b71bddf173770b928dda
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.7 MB (33651256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d2c89ae9d8a273834e3a8654ed1d739a02e9c19b3c42b9ceb7bbd8541dff386`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 09 Jun 2020 00:51:58 GMT
ADD file:7fde417d1c70a9ef2b4e468f6e2ee4cbd3f340fb2d5b67ede087c81520c95f4a in / 
# Tue, 09 Jun 2020 00:51:59 GMT
CMD ["bash"]
# Wed, 08 Jul 2020 17:48:41 GMT
ENV HAPROXY_VERSION=2.2.0
# Wed, 08 Jul 2020 17:48:41 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.0.tar.gz
# Wed, 08 Jul 2020 17:48:42 GMT
ENV HAPROXY_SHA256=3c1a87160eea40e067f1e2813bfe692280a10c455beb17a8ee7fae11e4223274
# Wed, 08 Jul 2020 17:49:58 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(nproc)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& apt-mark auto '.*' > /dev/null 	&& { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; } 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 08 Jul 2020 17:49:59 GMT
STOPSIGNAL SIGUSR1
# Wed, 08 Jul 2020 17:49:59 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Wed, 08 Jul 2020 17:50:00 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 08 Jul 2020 17:50:01 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:5b11fc09c1a26b11a7df7d593adf43baff53c5cdba71cf8a87ae4a6dd17eb52c`  
		Last Modified: Tue, 09 Jun 2020 00:59:24 GMT  
		Size: 24.8 MB (24837249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f86f187bd1b64990b114e09c7c6e0f0eff9df9b08800f62c10cfc0e5cb6beb5`  
		Last Modified: Wed, 08 Jul 2020 17:55:35 GMT  
		Size: 8.8 MB (8813627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e06de3333a4e2551b6203761406cee4c337b1829e79f6e750523de39ab6caf89`  
		Last Modified: Wed, 08 Jul 2020 17:55:32 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:latest` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:b58a781f5acf7a12d0c57c525860d987b202c06db4dad4985e8f3b27d1c5da8b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31332342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7164e57ec41763c7572b1a024b4dcf912cb5e801a6bb8d5802e952d52987232f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 22 Jul 2020 01:19:50 GMT
ADD file:c47f7b84c9113624f53d9c52e13f649f1e5d739665b5a5a5df6b1d5b5274d71b in / 
# Wed, 22 Jul 2020 01:19:58 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 08:41:38 GMT
ENV HAPROXY_VERSION=2.2.0
# Wed, 22 Jul 2020 08:41:38 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.0.tar.gz
# Wed, 22 Jul 2020 08:41:39 GMT
ENV HAPROXY_SHA256=3c1a87160eea40e067f1e2813bfe692280a10c455beb17a8ee7fae11e4223274
# Wed, 22 Jul 2020 08:42:19 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(nproc)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& apt-mark auto '.*' > /dev/null 	&& { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; } 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 22 Jul 2020 08:42:19 GMT
STOPSIGNAL SIGUSR1
# Wed, 22 Jul 2020 08:42:20 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Wed, 22 Jul 2020 08:42:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Jul 2020 08:42:22 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:0c4667eb56da53c2c07c288a210a70fb8d6089f57ce32a2cd88c2a75ae9ad8af`  
		Last Modified: Wed, 22 Jul 2020 01:40:34 GMT  
		Size: 22.7 MB (22705906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d3047102acec900737f25bd920fb77b5dfa70729e7682d67d3f4f079fdeaf36`  
		Last Modified: Wed, 22 Jul 2020 08:48:23 GMT  
		Size: 8.6 MB (8626057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269455e49e43f5349777fcd9eed70b823edb44f9bef07dde218333f7ddd41c2f`  
		Last Modified: Wed, 22 Jul 2020 08:48:20 GMT  
		Size: 379.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:latest` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:362fc265b1805b1a5577be15bf024a5df59af3bfb628939d4d5ea922a0cf3dd1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.9 MB (34887796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59d5e0c2dfb4130a37bed7bdf2cd99a2630ee057be46d20b1ee8aca20b45ce27`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 22 Jul 2020 00:41:09 GMT
ADD file:1efd5b51a56f36bcf79a1bcea1df36ef28299a42bc11e758f9e49066f2a1f085 in / 
# Wed, 22 Jul 2020 00:41:10 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 05:07:50 GMT
ENV HAPROXY_VERSION=2.2.0
# Wed, 22 Jul 2020 05:07:50 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.0.tar.gz
# Wed, 22 Jul 2020 05:07:51 GMT
ENV HAPROXY_SHA256=3c1a87160eea40e067f1e2813bfe692280a10c455beb17a8ee7fae11e4223274
# Wed, 22 Jul 2020 05:08:44 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(nproc)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& apt-mark auto '.*' > /dev/null 	&& { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; } 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 22 Jul 2020 05:08:46 GMT
STOPSIGNAL SIGUSR1
# Wed, 22 Jul 2020 05:08:54 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Wed, 22 Jul 2020 05:08:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Jul 2020 05:08:59 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:3999339def4d7591a8064bfc698302ae0e29bc5e0557ae392c122e1b3efa9305`  
		Last Modified: Wed, 22 Jul 2020 00:47:42 GMT  
		Size: 25.9 MB (25857826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:255cab3f6de572bb702c9d7f4ab3110152b5261cb4fb8b876eb5bd2cfe447489`  
		Last Modified: Wed, 22 Jul 2020 05:15:06 GMT  
		Size: 9.0 MB (9029590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147444c115b23cb195c7f12ce99f4da81388e5f6262193a49bb08186e9d3dbec`  
		Last Modified: Wed, 22 Jul 2020 05:15:04 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:latest` - linux; 386

```console
$ docker pull haproxy@sha256:1bc2deb3449c6181f8d2b950a07c04656c965b7cb8de508646d30b4bbfbf5a4f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.8 MB (36841798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:226fcc1ee49c66cf63f2c61bd5bb184598a0d32508eec0aba7f9c8cc93a7ec0a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 22 Jul 2020 02:09:15 GMT
ADD file:ee51bd8fcf2e02243de32c0f0e7899acebfa23bdceb783f13feb33c484ee98b8 in / 
# Wed, 22 Jul 2020 02:09:15 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 03:09:14 GMT
ENV HAPROXY_VERSION=2.2.0
# Wed, 22 Jul 2020 03:09:15 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.0.tar.gz
# Wed, 22 Jul 2020 03:09:15 GMT
ENV HAPROXY_SHA256=3c1a87160eea40e067f1e2813bfe692280a10c455beb17a8ee7fae11e4223274
# Wed, 22 Jul 2020 03:10:26 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(nproc)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& apt-mark auto '.*' > /dev/null 	&& { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; } 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 22 Jul 2020 03:10:27 GMT
STOPSIGNAL SIGUSR1
# Wed, 22 Jul 2020 03:10:27 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Wed, 22 Jul 2020 03:10:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Jul 2020 03:10:27 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:75157e9ef5a857d6b02d235e08a164737ad009bae299277f86131063e6204e0b`  
		Last Modified: Wed, 22 Jul 2020 02:15:45 GMT  
		Size: 27.8 MB (27754899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:934239530ec8ddf4b8b65da20809be0700f1ebf639642dcf93106b0ec7c5694a`  
		Last Modified: Wed, 22 Jul 2020 03:16:54 GMT  
		Size: 9.1 MB (9086519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:573a8c70a511356726f510634cd8d6dc840eb925e119dea5ce06930c15afa971`  
		Last Modified: Wed, 22 Jul 2020 03:16:51 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:latest` - linux; mips64le

```console
$ docker pull haproxy@sha256:0ef728b5b906b008573b9b7cb336f81461b5a7cce323798b17b3042da1dda115
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 MB (34545807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dde4613adfea07a9b3ac7d5ba2e1a8e00a4c4a1fee61b3698675966a9f2e6732`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 22 Jul 2020 01:09:52 GMT
ADD file:67401cc8bdd27435a027e4051d2eb03c5012a09274aaae230008279234586dfb in / 
# Wed, 22 Jul 2020 01:09:53 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 01:40:52 GMT
ENV HAPROXY_VERSION=2.2.0
# Wed, 22 Jul 2020 01:40:52 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.0.tar.gz
# Wed, 22 Jul 2020 01:40:52 GMT
ENV HAPROXY_SHA256=3c1a87160eea40e067f1e2813bfe692280a10c455beb17a8ee7fae11e4223274
# Wed, 22 Jul 2020 01:43:53 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(nproc)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& apt-mark auto '.*' > /dev/null 	&& { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; } 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 22 Jul 2020 01:43:53 GMT
STOPSIGNAL SIGUSR1
# Wed, 22 Jul 2020 01:43:53 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Wed, 22 Jul 2020 01:43:54 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Jul 2020 01:43:54 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:2cab09a0ed78d8465b06bc43bf504e7c4ed41f36db2ee9cb181c154d562fc9ff`  
		Last Modified: Wed, 22 Jul 2020 01:16:46 GMT  
		Size: 25.8 MB (25764196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd501af70f647836fd64c2aed280be68c4f86590a944d81a602a40eea710d210`  
		Last Modified: Wed, 22 Jul 2020 01:57:38 GMT  
		Size: 8.8 MB (8781231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae1cef2114ee1d93e28cce73b36c8e56ae1aaca5113d341f030d8e169ea2095e`  
		Last Modified: Wed, 22 Jul 2020 01:57:31 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:latest` - linux; ppc64le

```console
$ docker pull haproxy@sha256:ab90418d63129d81f17164498fcf3941a5b123ab8bf8569c8887d0fe75956a13
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40202458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98fd633fea562ee863f420d7eb5836c34f7c4e974767c38ec9e8b8196555ef95`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 22 Jul 2020 02:16:05 GMT
ADD file:037dec996d9b742fc49f675272aa42ebd31f04226ba3d28836a6556cb61c29e7 in / 
# Wed, 22 Jul 2020 02:16:14 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 06:11:44 GMT
ENV HAPROXY_VERSION=2.2.0
# Wed, 22 Jul 2020 06:11:47 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.0.tar.gz
# Wed, 22 Jul 2020 06:11:50 GMT
ENV HAPROXY_SHA256=3c1a87160eea40e067f1e2813bfe692280a10c455beb17a8ee7fae11e4223274
# Wed, 22 Jul 2020 06:14:32 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(nproc)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& apt-mark auto '.*' > /dev/null 	&& { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; } 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 22 Jul 2020 06:14:36 GMT
STOPSIGNAL SIGUSR1
# Wed, 22 Jul 2020 06:14:38 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Wed, 22 Jul 2020 06:14:42 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Jul 2020 06:14:47 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:d022338f917106731b8902d4c3d7009435a41381c11c8d210bbd6af007569f69`  
		Last Modified: Wed, 22 Jul 2020 02:26:01 GMT  
		Size: 30.5 MB (30524562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e6a5bd2dca2f60cf349bcdfd21138c6c6b492a0f23b594dd84c2a3955ecbc4b`  
		Last Modified: Wed, 22 Jul 2020 06:39:45 GMT  
		Size: 9.7 MB (9677516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6991a97dae08e1a13c73beafd814594dc0d1cdd2dddfd72d8d80d1c4ed628098`  
		Last Modified: Wed, 22 Jul 2020 06:39:41 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:latest` - linux; s390x

```console
$ docker pull haproxy@sha256:9541b5f2cc58ceecb2844ebefce7bced0b1400aa1b637dcde997459ad00496b1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.6 MB (34627322 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0d8eabda54acbe0b30a98b5d89734153d9077c534eecccb510a039a548bd9c7`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 22 Jul 2020 00:42:41 GMT
ADD file:2864b647009a85c176c3aeb2d75843b9336b02a18412124b8a03710df61dc971 in / 
# Wed, 22 Jul 2020 00:42:43 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 01:15:00 GMT
ENV HAPROXY_VERSION=2.2.0
# Wed, 22 Jul 2020 01:15:00 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.0.tar.gz
# Wed, 22 Jul 2020 01:15:00 GMT
ENV HAPROXY_SHA256=3c1a87160eea40e067f1e2813bfe692280a10c455beb17a8ee7fae11e4223274
# Wed, 22 Jul 2020 01:15:27 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(nproc)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& apt-mark auto '.*' > /dev/null 	&& { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; } 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 22 Jul 2020 01:15:28 GMT
STOPSIGNAL SIGUSR1
# Wed, 22 Jul 2020 01:15:28 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Wed, 22 Jul 2020 01:15:28 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Jul 2020 01:15:28 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:71104c8b0e24cdcb6152cf3a5afb2944f578c741e6defa1905768c590598a79a`  
		Last Modified: Wed, 22 Jul 2020 00:45:48 GMT  
		Size: 25.7 MB (25712820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c923e4497c5584c9bf6ba7af38eaffc9ea66df1b0a10086bd75d55efc132a544`  
		Last Modified: Wed, 22 Jul 2020 01:19:06 GMT  
		Size: 8.9 MB (8914122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0050b0612df375609dc260829c6dd2cf823786b05bbfbde7b2cfc7ef4f6c7713`  
		Last Modified: Wed, 22 Jul 2020 01:19:04 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
