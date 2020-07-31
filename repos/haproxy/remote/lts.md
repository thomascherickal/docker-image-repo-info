## `haproxy:lts`

```console
$ docker pull haproxy@sha256:6ff4cd0b552f6758b9bfd132fa4fd1cce45799e00eb3345278fc47a495d0973f
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
$ docker pull haproxy@sha256:a8590dd9ab4c74fdbbcb4d16c825d9496aff06b58e9d9f717a80356e6ddde328
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36318674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88aff958cbc5bf549dcb7d1db07bb0d17359eab3f210f7b72b12021b5312efb0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 22 Jul 2020 02:03:37 GMT
ADD file:6ccb3bbcc69b0d44c48a8ef1bfa08d835444ea13b8a93701bd37d86b81b13ac2 in / 
# Wed, 22 Jul 2020 02:03:37 GMT
CMD ["bash"]
# Thu, 23 Jul 2020 18:36:42 GMT
ENV HAPROXY_VERSION=2.2.1
# Thu, 23 Jul 2020 18:36:42 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.1.tar.gz
# Thu, 23 Jul 2020 18:36:42 GMT
ENV HAPROXY_SHA256=536552af1316807c01de727ad3dac84b3a2f5285db32e9bfdfe234e47ff9d124
# Thu, 23 Jul 2020 18:37:36 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(nproc)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& apt-mark auto '.*' > /dev/null 	&& { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; } 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 23 Jul 2020 18:37:36 GMT
STOPSIGNAL SIGUSR1
# Thu, 23 Jul 2020 18:37:36 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 23 Jul 2020 18:37:36 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 23 Jul 2020 18:37:37 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:6ec8c9369e08152361a01729f2c8a1e7aae898426c6e67267f41894bf9524827`  
		Last Modified: Wed, 22 Jul 2020 02:09:51 GMT  
		Size: 27.1 MB (27098544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1677bc710369f3526f4d0b673623a099bb048a6ff90ddae0e3f642a3c390a0d`  
		Last Modified: Thu, 23 Jul 2020 18:41:18 GMT  
		Size: 9.2 MB (9219750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eae8ba1a6bd79e9432f77833e440889c913435fc5d5b9e51480f7e69f8023ca`  
		Last Modified: Thu, 23 Jul 2020 18:41:16 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:2698de174fda80ca0982f5acfe957bc10dd119e24b61ff1436d44af2ffd4a82d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.7 MB (33656665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1227ee6eea704f70ae5829ab2596f051c6f0e912085692f4486a79d93edb75d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 22 Jul 2020 00:51:01 GMT
ADD file:4ea2d111c970d510f4eccf0fa08caafde1d227fc4c249d67c1b9d99998b0b906 in / 
# Wed, 22 Jul 2020 00:51:04 GMT
CMD ["bash"]
# Fri, 31 Jul 2020 17:48:45 GMT
ENV HAPROXY_VERSION=2.2.2
# Fri, 31 Jul 2020 17:48:45 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.2.tar.gz
# Fri, 31 Jul 2020 17:48:46 GMT
ENV HAPROXY_SHA256=391c705a46c6208a63a67ea842c6600146ca24618531570c89c7915b0c6a54d6
# Fri, 31 Jul 2020 17:49:50 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(nproc)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& apt-mark auto '.*' > /dev/null 	&& { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; } 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 31 Jul 2020 17:49:52 GMT
STOPSIGNAL SIGUSR1
# Fri, 31 Jul 2020 17:49:53 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 31 Jul 2020 17:49:54 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 31 Jul 2020 17:49:55 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:7ae4223cfc253e8d54407ec654ed8fb606352daea8da124f33dacd17626259ad`  
		Last Modified: Wed, 22 Jul 2020 00:58:53 GMT  
		Size: 24.8 MB (24837461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f38a834ddbb3f16a5517296a4ce37c7d7f4eaca1e164e9c22152530a9c76220`  
		Last Modified: Fri, 31 Jul 2020 17:55:02 GMT  
		Size: 8.8 MB (8818824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9707f76df6630bf7fa4dbb3f643d9117934727c92b4434cee57fc9fe87554fc9`  
		Last Modified: Fri, 31 Jul 2020 17:54:59 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:4ea687ae9045873879e0cd1b537369cd84f61ea62e9f11cbce8b3ef300142406
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31342449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b20a82a2ca7d5da091dba91aaaead0dac58e911aae51e7f0a9b01c5f2d537f1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 22 Jul 2020 01:19:50 GMT
ADD file:c47f7b84c9113624f53d9c52e13f649f1e5d739665b5a5a5df6b1d5b5274d71b in / 
# Wed, 22 Jul 2020 01:19:58 GMT
CMD ["bash"]
# Fri, 31 Jul 2020 17:59:16 GMT
ENV HAPROXY_VERSION=2.2.2
# Fri, 31 Jul 2020 17:59:17 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.2.tar.gz
# Fri, 31 Jul 2020 17:59:17 GMT
ENV HAPROXY_SHA256=391c705a46c6208a63a67ea842c6600146ca24618531570c89c7915b0c6a54d6
# Fri, 31 Jul 2020 17:59:57 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(nproc)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& apt-mark auto '.*' > /dev/null 	&& { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; } 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 31 Jul 2020 17:59:58 GMT
STOPSIGNAL SIGUSR1
# Fri, 31 Jul 2020 17:59:58 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 31 Jul 2020 17:59:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 31 Jul 2020 18:00:00 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:0c4667eb56da53c2c07c288a210a70fb8d6089f57ce32a2cd88c2a75ae9ad8af`  
		Last Modified: Wed, 22 Jul 2020 01:40:34 GMT  
		Size: 22.7 MB (22705906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:372d6e6955c2af88c5858661c4eb79c005c1cc43921aec91474e7e62b4295094`  
		Last Modified: Fri, 31 Jul 2020 18:01:41 GMT  
		Size: 8.6 MB (8636163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e440d097d6d512e4fadbaf917560e429f2fa902f28e76f7e0848f57c26fcc11`  
		Last Modified: Fri, 31 Jul 2020 18:01:39 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:233cf4a6effe584b8a7ed95440d3e30c645d0434db8ef857fa34025759fa7e84
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.9 MB (34896185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89d7ac5636ec49f2c9ad68cbbe133e68ab2e07e9624b96edce07bb433328d52b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 22 Jul 2020 00:41:09 GMT
ADD file:1efd5b51a56f36bcf79a1bcea1df36ef28299a42bc11e758f9e49066f2a1f085 in / 
# Wed, 22 Jul 2020 00:41:10 GMT
CMD ["bash"]
# Fri, 31 Jul 2020 17:45:22 GMT
ENV HAPROXY_VERSION=2.2.2
# Fri, 31 Jul 2020 17:45:23 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.2.tar.gz
# Fri, 31 Jul 2020 17:45:23 GMT
ENV HAPROXY_SHA256=391c705a46c6208a63a67ea842c6600146ca24618531570c89c7915b0c6a54d6
# Fri, 31 Jul 2020 17:46:05 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(nproc)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& apt-mark auto '.*' > /dev/null 	&& { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; } 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 31 Jul 2020 17:46:06 GMT
STOPSIGNAL SIGUSR1
# Fri, 31 Jul 2020 17:46:06 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 31 Jul 2020 17:46:07 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 31 Jul 2020 17:46:07 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:3999339def4d7591a8064bfc698302ae0e29bc5e0557ae392c122e1b3efa9305`  
		Last Modified: Wed, 22 Jul 2020 00:47:42 GMT  
		Size: 25.9 MB (25857826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e844fe21d3c33b32e578fc236b3fba46b74ca549e0a8062670f818914974095e`  
		Last Modified: Fri, 31 Jul 2020 17:47:57 GMT  
		Size: 9.0 MB (9037979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d0903a59cb45fbb13bee54aeeed789a78065ba99279a1cbd2205d2af179ffc7`  
		Last Modified: Fri, 31 Jul 2020 17:47:54 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; 386

```console
$ docker pull haproxy@sha256:38fbed97b3a698124e41baeebfc7c0994d76e9c6bcf4110b1317678f959f65ce
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.9 MB (36852672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:732045a0affba5b68a2d3af6052b2b74340a6644f995f7c65dd363dc5cfbc4c8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 22 Jul 2020 02:09:15 GMT
ADD file:ee51bd8fcf2e02243de32c0f0e7899acebfa23bdceb783f13feb33c484ee98b8 in / 
# Wed, 22 Jul 2020 02:09:15 GMT
CMD ["bash"]
# Fri, 31 Jul 2020 17:40:21 GMT
ENV HAPROXY_VERSION=2.2.2
# Fri, 31 Jul 2020 17:40:21 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.2.tar.gz
# Fri, 31 Jul 2020 17:40:21 GMT
ENV HAPROXY_SHA256=391c705a46c6208a63a67ea842c6600146ca24618531570c89c7915b0c6a54d6
# Fri, 31 Jul 2020 17:41:24 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(nproc)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& apt-mark auto '.*' > /dev/null 	&& { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; } 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 31 Jul 2020 17:41:24 GMT
STOPSIGNAL SIGUSR1
# Fri, 31 Jul 2020 17:41:24 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 31 Jul 2020 17:41:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 31 Jul 2020 17:41:25 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:75157e9ef5a857d6b02d235e08a164737ad009bae299277f86131063e6204e0b`  
		Last Modified: Wed, 22 Jul 2020 02:15:45 GMT  
		Size: 27.8 MB (27754899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84bdd7ebefdbafcaca80eb8af8804e1983d54d2474463fbd92c8f1767e64ea2e`  
		Last Modified: Fri, 31 Jul 2020 17:43:37 GMT  
		Size: 9.1 MB (9097393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a7ff35d534ac811235ac2e95f82ee339d82198ee787211f77090b8aec1280b`  
		Last Modified: Fri, 31 Jul 2020 17:43:35 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; mips64le

```console
$ docker pull haproxy@sha256:2ccb6e3d3eb721f203513c634d8d8ac4a7d5b7157725361ec82ac21a474dfab8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.6 MB (34552095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ba84e4b237a8236ae524822aa0cf829ccdbe04a44ef0d9189501c77d29b84cb`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 22 Jul 2020 01:09:52 GMT
ADD file:67401cc8bdd27435a027e4051d2eb03c5012a09274aaae230008279234586dfb in / 
# Wed, 22 Jul 2020 01:09:53 GMT
CMD ["bash"]
# Fri, 31 Jul 2020 18:07:19 GMT
ENV HAPROXY_VERSION=2.2.2
# Fri, 31 Jul 2020 18:07:20 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.2.tar.gz
# Fri, 31 Jul 2020 18:07:20 GMT
ENV HAPROXY_SHA256=391c705a46c6208a63a67ea842c6600146ca24618531570c89c7915b0c6a54d6
# Fri, 31 Jul 2020 18:10:26 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(nproc)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& apt-mark auto '.*' > /dev/null 	&& { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; } 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 31 Jul 2020 18:10:26 GMT
STOPSIGNAL SIGUSR1
# Fri, 31 Jul 2020 18:10:27 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 31 Jul 2020 18:10:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 31 Jul 2020 18:10:27 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:2cab09a0ed78d8465b06bc43bf504e7c4ed41f36db2ee9cb181c154d562fc9ff`  
		Last Modified: Wed, 22 Jul 2020 01:16:46 GMT  
		Size: 25.8 MB (25764196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e6a4db749ab3b4d03a8e3626111079d88c491f869b7ff46adadbc9b1f46373`  
		Last Modified: Fri, 31 Jul 2020 18:11:02 GMT  
		Size: 8.8 MB (8787519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e10434b8883896a9459e12c27500b455fe30ee4279ce7c49b258e05332e3c5f`  
		Last Modified: Fri, 31 Jul 2020 18:10:55 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; ppc64le

```console
$ docker pull haproxy@sha256:7f69c0d530ede29fd38572619d8e47b0cc622278f99ff354be224dbd6c317b65
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40207415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d98a974ff8f260ac7aa986fe293baa6c8c0977b0b0499bb2fdf4bb6d4038411a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 22 Jul 2020 02:16:05 GMT
ADD file:037dec996d9b742fc49f675272aa42ebd31f04226ba3d28836a6556cb61c29e7 in / 
# Wed, 22 Jul 2020 02:16:14 GMT
CMD ["bash"]
# Thu, 23 Jul 2020 20:12:55 GMT
ENV HAPROXY_VERSION=2.2.1
# Thu, 23 Jul 2020 20:13:08 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.1.tar.gz
# Thu, 23 Jul 2020 20:13:18 GMT
ENV HAPROXY_SHA256=536552af1316807c01de727ad3dac84b3a2f5285db32e9bfdfe234e47ff9d124
# Thu, 23 Jul 2020 20:17:40 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(nproc)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& apt-mark auto '.*' > /dev/null 	&& { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; } 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 23 Jul 2020 20:17:45 GMT
STOPSIGNAL SIGUSR1
# Thu, 23 Jul 2020 20:17:50 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Thu, 23 Jul 2020 20:17:58 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 23 Jul 2020 20:18:04 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:d022338f917106731b8902d4c3d7009435a41381c11c8d210bbd6af007569f69`  
		Last Modified: Wed, 22 Jul 2020 02:26:01 GMT  
		Size: 30.5 MB (30524562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca6647d6ac615e6479c078ea9a49be54e95ce6ee55cb02113bae3eca94f412e3`  
		Last Modified: Thu, 23 Jul 2020 20:22:31 GMT  
		Size: 9.7 MB (9682473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a90d4fa11f83e8867c34cc8b46d439050f177bd920dda642815851eeb2a9a79`  
		Last Modified: Thu, 23 Jul 2020 20:22:30 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; s390x

```console
$ docker pull haproxy@sha256:a8cee77a97e99cee3fd35021185fb3c53e956e7b288b958ce5cd56be30d6e8c3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.6 MB (34632333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98f5b0cb214b56f622ff40ddf0dc068d918f20469844a9184ddd1735310d40de`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 22 Jul 2020 00:42:41 GMT
ADD file:2864b647009a85c176c3aeb2d75843b9336b02a18412124b8a03710df61dc971 in / 
# Wed, 22 Jul 2020 00:42:43 GMT
CMD ["bash"]
# Fri, 31 Jul 2020 17:41:50 GMT
ENV HAPROXY_VERSION=2.2.2
# Fri, 31 Jul 2020 17:41:51 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.2/src/haproxy-2.2.2.tar.gz
# Fri, 31 Jul 2020 17:41:51 GMT
ENV HAPROXY_SHA256=391c705a46c6208a63a67ea842c6600146ca24618531570c89c7915b0c6a54d6
# Fri, 31 Jul 2020 17:42:43 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 		zlib1g-dev 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(nproc)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& apt-mark auto '.*' > /dev/null 	&& { [ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; } 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 31 Jul 2020 17:42:45 GMT
STOPSIGNAL SIGUSR1
# Fri, 31 Jul 2020 17:42:45 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Fri, 31 Jul 2020 17:42:46 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 31 Jul 2020 17:42:46 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:71104c8b0e24cdcb6152cf3a5afb2944f578c741e6defa1905768c590598a79a`  
		Last Modified: Wed, 22 Jul 2020 00:45:48 GMT  
		Size: 25.7 MB (25712820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6a28358957279df383cf08800fc2234a4e1cf8f1777bde116781070cf6f5f0`  
		Last Modified: Fri, 31 Jul 2020 17:44:56 GMT  
		Size: 8.9 MB (8919133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399f0b9093614ab636edac84cbaa97af9e98bfc6849bffac4c22b1b47fe9297a`  
		Last Modified: Fri, 31 Jul 2020 17:44:54 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
