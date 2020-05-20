## `haproxy:lts`

```console
$ docker pull haproxy@sha256:7ab994f69b67953e020b8c299178fb59fb1c61a8c84d2a7ece97f2bfc64926d4
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
$ docker pull haproxy@sha256:08f9f6c6c9227fe5a87dcdd4cf9fa3c5ca53f39f13dd2bdb97cf4cf3268f6d8c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.7 MB (35745184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d0cff4aa4194a32495c2de87a0363d342986ebde7207946524adc77e877caef`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 15 May 2020 06:28:44 GMT
ADD file:7780c81c33e6cc5b6261af4a6c611cce0f39dec3131009bb297e65f12020c150 in / 
# Fri, 15 May 2020 06:28:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 18:48:42 GMT
ENV HAPROXY_VERSION=2.0.14
# Fri, 15 May 2020 18:48:42 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.14.tar.gz
# Fri, 15 May 2020 18:48:43 GMT
ENV HAPROXY_SHA256=552a708b8b6efd0f241f5d9fd7ad4168d37ce17cdb6dcb6239c2e519f0a63c75
# Fri, 15 May 2020 18:49:42 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(nproc)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& apt-mark auto '.*' > /dev/null 	&& { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; } 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 15 May 2020 18:49:42 GMT
STOPSIGNAL SIGUSR1
# Fri, 15 May 2020 18:49:43 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 15 May 2020 18:49:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 15 May 2020 18:49:43 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:afb6ec6fdc1c3ba04f7a56db32c5ff5ff38962dc4cd0ffdef5beaa0ce2eb77e2`  
		Last Modified: Fri, 15 May 2020 06:37:39 GMT  
		Size: 27.1 MB (27098756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df20592471a1d42e829ddfd2e29b76a9fd60a9194a47ff4a77680b9dbb5b65d`  
		Last Modified: Fri, 15 May 2020 18:55:29 GMT  
		Size: 8.6 MB (8646048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee4106b219c8e157c29607945c1031e8f6c877718d3b868ccefc50135e13aae`  
		Last Modified: Fri, 15 May 2020 18:55:26 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:9c1083697ea037e691e050c83d6673d89bc0cbe50fa399d972e2de16c6deda1f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32969540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4057f9ad8eae865f3ff39bef230089a5ef780bb0bde2513e01b0d8a3cf99165`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 14 May 2020 22:38:03 GMT
ADD file:cbd01ff8d2e40a25bcdb13dc19ffe124c2927b491997dc1c57d4f2c2a308e279 in / 
# Thu, 14 May 2020 22:38:05 GMT
CMD ["bash"]
# Fri, 15 May 2020 03:27:31 GMT
ENV HAPROXY_VERSION=2.0.14
# Fri, 15 May 2020 03:27:32 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.14.tar.gz
# Fri, 15 May 2020 03:27:33 GMT
ENV HAPROXY_SHA256=552a708b8b6efd0f241f5d9fd7ad4168d37ce17cdb6dcb6239c2e519f0a63c75
# Fri, 15 May 2020 03:28:15 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(nproc)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& apt-mark auto '.*' > /dev/null 	&& { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; } 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 15 May 2020 03:28:16 GMT
STOPSIGNAL SIGUSR1
# Fri, 15 May 2020 03:28:17 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 15 May 2020 03:28:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 15 May 2020 03:28:18 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:24d81022117207b0239d8a8023ca1724b7dde38cb08ce5b9199f59d475d1e600`  
		Last Modified: Thu, 14 May 2020 22:46:51 GMT  
		Size: 24.8 MB (24838470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79618e2c556d3c48fa5e72ccb25a8f23195115d4748906ea4e867a6d5bb7e7e9`  
		Last Modified: Fri, 15 May 2020 03:36:52 GMT  
		Size: 8.1 MB (8130689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ba8e9d1ba2fe15516bbec2bbcb513d5d710642512b785f03a7c76711813e61`  
		Last Modified: Fri, 15 May 2020 03:36:50 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:8bf781c7c25c798d1e29a8a5b66b6c2e5659e66d33978bd8d822f1ff1c341d17
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.8 MB (30783616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a061749fa065f22122ace2b3ef45204c0243a50ad72b1e3b084ea4cca50a5900`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 15 May 2020 01:00:06 GMT
ADD file:e3f9a454eccb40b4d7bf1dcc17ec29589a007ac67545d1cb5b6fa213c872c8f2 in / 
# Fri, 15 May 2020 01:00:07 GMT
CMD ["bash"]
# Fri, 15 May 2020 10:09:11 GMT
ENV HAPROXY_VERSION=2.0.14
# Fri, 15 May 2020 10:09:12 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.14.tar.gz
# Fri, 15 May 2020 10:09:13 GMT
ENV HAPROXY_SHA256=552a708b8b6efd0f241f5d9fd7ad4168d37ce17cdb6dcb6239c2e519f0a63c75
# Fri, 15 May 2020 10:09:54 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(nproc)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& apt-mark auto '.*' > /dev/null 	&& { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; } 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 15 May 2020 10:09:55 GMT
STOPSIGNAL SIGUSR1
# Fri, 15 May 2020 10:09:57 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 15 May 2020 10:09:58 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 15 May 2020 10:09:59 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:e41e28500352be59188c3d871a4b5a3f594350b860a9a36ed5808a35920bdae4`  
		Last Modified: Fri, 15 May 2020 01:11:21 GMT  
		Size: 22.7 MB (22705925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e936496d73da33664d867f9d030d7d65aceee4945141cf40b7ec007a12b6e875`  
		Last Modified: Fri, 15 May 2020 10:15:31 GMT  
		Size: 8.1 MB (8077311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90336fd29a80d4567b2d86d04c13b28707a129751cffe2c2d511e67363e88916`  
		Last Modified: Fri, 15 May 2020 10:15:29 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:a047ce57d59cca9273d46b5d50f4bf9ab298f708d75b9f3a5bbd10297cd14cdf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34339771 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02bf6d92896f8b67fcf227a09c3d060d7fa2a5510274d483bd7b84661ec90dd0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 15 May 2020 12:44:06 GMT
ADD file:b305c1792102142f183d3084026f0fc6be3ddf8d1959b32f0a5d22d35eebcd15 in / 
# Fri, 15 May 2020 12:44:07 GMT
CMD ["bash"]
# Fri, 15 May 2020 20:51:57 GMT
ENV HAPROXY_VERSION=2.0.14
# Fri, 15 May 2020 20:51:58 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.14.tar.gz
# Fri, 15 May 2020 20:51:59 GMT
ENV HAPROXY_SHA256=552a708b8b6efd0f241f5d9fd7ad4168d37ce17cdb6dcb6239c2e519f0a63c75
# Fri, 15 May 2020 20:52:49 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(nproc)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& apt-mark auto '.*' > /dev/null 	&& { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; } 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 15 May 2020 20:52:50 GMT
STOPSIGNAL SIGUSR1
# Fri, 15 May 2020 20:52:51 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 15 May 2020 20:52:52 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 15 May 2020 20:52:53 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:8a7e1e68c24e5cac20ef26d29505c58456b561c431f0c683b66d1a0943f40dd4`  
		Last Modified: Fri, 15 May 2020 12:53:36 GMT  
		Size: 25.9 MB (25857195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb12b1ab764e809599e2346e55e8c4ee993e4f2f0805e49bc52be08ed846fbfe`  
		Last Modified: Fri, 15 May 2020 21:02:29 GMT  
		Size: 8.5 MB (8482196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00b5364b6b417ddf6b8965f35e1b17a39c6ba1e814d57eb3442fad43b7aece57`  
		Last Modified: Fri, 15 May 2020 21:02:24 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; 386

```console
$ docker pull haproxy@sha256:d5ab0c91b39e89a37e4726d79328c82497d5f82365c7fd4a068d73f085448434
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.2 MB (36189780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8887b768add5520d6b334d6b4c16c1ae01322186fa728f22be96d5f04f18cebf`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 15 May 2020 07:07:55 GMT
ADD file:0c3b44c83914e95e4604999a86af05023cdd2b2f795e71d737e428fae4a7e0ac in / 
# Fri, 15 May 2020 07:07:56 GMT
CMD ["bash"]
# Fri, 15 May 2020 17:41:04 GMT
ENV HAPROXY_VERSION=2.0.14
# Fri, 15 May 2020 17:41:04 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.14.tar.gz
# Fri, 15 May 2020 17:41:04 GMT
ENV HAPROXY_SHA256=552a708b8b6efd0f241f5d9fd7ad4168d37ce17cdb6dcb6239c2e519f0a63c75
# Fri, 15 May 2020 17:42:10 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(nproc)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& apt-mark auto '.*' > /dev/null 	&& { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; } 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 15 May 2020 17:42:10 GMT
STOPSIGNAL SIGUSR1
# Fri, 15 May 2020 17:42:11 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 15 May 2020 17:42:11 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 15 May 2020 17:42:11 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:a5695130085a13212b02bf2645a52af5b41dd13e6dc9b29e2d7f357e1525aa48`  
		Last Modified: Fri, 15 May 2020 07:18:14 GMT  
		Size: 27.8 MB (27754922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e77a862f56d7fb6211fc0b26abb96a8805e98cda3885ad03eb5ce9b52c6c52`  
		Last Modified: Fri, 15 May 2020 17:47:12 GMT  
		Size: 8.4 MB (8434478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ddecd96dbcee6c9ee28d6e9cee447904a80d5e2b6cd8999c7bba20c577c0d87`  
		Last Modified: Fri, 15 May 2020 17:47:10 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; mips64le

```console
$ docker pull haproxy@sha256:215d9379cb2f8d16eb5b3de66a6dbfb96da81fa942606cdcb7736cf700f1bdf6
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33868342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e47e20dd90a4064c9db20772f82ab6bb833db27e1ce71d1cacdbe0be53bbce8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 15 May 2020 04:48:19 GMT
ADD file:1163d3a5831eb58d132b66b60303169816e7bd8289f19caaac1157179a95f6f9 in / 
# Fri, 15 May 2020 04:48:19 GMT
CMD ["bash"]
# Fri, 15 May 2020 15:09:17 GMT
ENV HAPROXY_VERSION=2.0.14
# Fri, 15 May 2020 15:09:17 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.14.tar.gz
# Fri, 15 May 2020 15:09:18 GMT
ENV HAPROXY_SHA256=552a708b8b6efd0f241f5d9fd7ad4168d37ce17cdb6dcb6239c2e519f0a63c75
# Fri, 15 May 2020 15:12:04 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(nproc)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& apt-mark auto '.*' > /dev/null 	&& { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; } 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 15 May 2020 15:12:04 GMT
STOPSIGNAL SIGUSR1
# Fri, 15 May 2020 15:12:04 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 15 May 2020 15:12:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 15 May 2020 15:12:05 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:d22357c747999d33ec7501da2c05aa9e95079ebddefbcb326976c5ed5b176b3f`  
		Last Modified: Fri, 15 May 2020 04:57:10 GMT  
		Size: 25.8 MB (25764292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbcfc25d569054d0a29b45c4343c8f6dea399575e9732d60e1ef5d9e7dcca437`  
		Last Modified: Fri, 15 May 2020 15:22:17 GMT  
		Size: 8.1 MB (8103669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b5b4c7a0fe8e8f14aac980862ec3e3923ffd3b0a7ec0c9722ed3ce3c76c272`  
		Last Modified: Fri, 15 May 2020 15:22:10 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; ppc64le

```console
$ docker pull haproxy@sha256:723b64553c5ac577ac3d117909c9c6826903828bd7fce5b7e5ca9cf1ccdc6c96
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.4 MB (39431985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0eca74a1db5ae2865c44c90c0cd39326c83eb2a7e8e2ced8efc902204147a9a1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 16 May 2020 17:14:59 GMT
ADD file:b2656a1711bd47585595ae2927cfd4ec00eb903d193583d945b6d60f0a2691bb in / 
# Sat, 16 May 2020 17:15:04 GMT
CMD ["bash"]
# Wed, 20 May 2020 17:24:47 GMT
ENV HAPROXY_VERSION=2.0.14
# Wed, 20 May 2020 17:24:54 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.14.tar.gz
# Wed, 20 May 2020 17:24:59 GMT
ENV HAPROXY_SHA256=552a708b8b6efd0f241f5d9fd7ad4168d37ce17cdb6dcb6239c2e519f0a63c75
# Wed, 20 May 2020 17:28:25 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(nproc)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& apt-mark auto '.*' > /dev/null 	&& { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; } 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 20 May 2020 17:28:32 GMT
STOPSIGNAL SIGUSR1
# Wed, 20 May 2020 17:28:38 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Wed, 20 May 2020 17:28:42 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 20 May 2020 17:28:46 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:034d508ed7647e7139951a435acc95e0124f50c984670d0e53b4f5ba25cf6ed1`  
		Last Modified: Sat, 16 May 2020 18:31:49 GMT  
		Size: 30.5 MB (30524456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf18d40b81bb7f0e602dc13a2e44de18abbfbbe463e6c9910df5b39ca41a4db`  
		Last Modified: Wed, 20 May 2020 17:44:52 GMT  
		Size: 8.9 MB (8907149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c979bb612938b7391591464789ac088f8cfeb6e2f46d727aad0289dc4b2791`  
		Last Modified: Wed, 20 May 2020 17:44:49 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; s390x

```console
$ docker pull haproxy@sha256:d65d1dfa88c08d297875eac3ba5315c36d1ac6709472391380fe53acaacfb99b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33910139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db43a3151c8bd3bf6b480da143e534951bb31c099f17e11afe22f7f3a0fba39d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 14 May 2020 23:06:40 GMT
ADD file:a29e647b8dccf726d8610d8c599d6727d6145426f9374720b985fc9be9ac906c in / 
# Thu, 14 May 2020 23:06:41 GMT
CMD ["bash"]
# Fri, 15 May 2020 04:35:47 GMT
ENV HAPROXY_VERSION=2.0.14
# Fri, 15 May 2020 04:35:47 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.0/src/haproxy-2.0.14.tar.gz
# Fri, 15 May 2020 04:35:48 GMT
ENV HAPROXY_SHA256=552a708b8b6efd0f241f5d9fd7ad4168d37ce17cdb6dcb6239c2e519f0a63c75
# Fri, 15 May 2020 04:36:43 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(nproc)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& apt-mark auto '.*' > /dev/null 	&& { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; } 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 15 May 2020 04:36:44 GMT
STOPSIGNAL SIGUSR1
# Fri, 15 May 2020 04:36:45 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 15 May 2020 04:36:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 15 May 2020 04:36:46 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:bdb298e230dde60bfce8a476ae8ea8988828f7ec9f5452f38f46102a609f57c1`  
		Last Modified: Thu, 14 May 2020 23:11:24 GMT  
		Size: 25.7 MB (25712933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca5c0707e185018717b02972c2482d80fc9a2bd0ce68525d96f1888ec03ea9fe`  
		Last Modified: Fri, 15 May 2020 04:40:04 GMT  
		Size: 8.2 MB (8196825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f5f8cc373e730c82079da138785ea33a09466d6cb7048560661c02b0eea7e0`  
		Last Modified: Fri, 15 May 2020 04:40:08 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
