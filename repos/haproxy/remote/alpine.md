## `haproxy:alpine`

```console
$ docker pull haproxy@sha256:fb77781a11df1c966f4c2f6c4ae5e04c938a25b8e2b0a74c797ed09cac1412f3
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
$ docker pull haproxy@sha256:7cc40fe25a496912efa4005a51bafd3437948c53cca3ac2e36ccad448606ae53
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9557598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58af2a59493e4370047ffe193972b14ebf38ee1b8b4cffbb48804dadc65c1835`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 16:21:01 GMT
ENV HAPROXY_VERSION=2.1.5
# Tue, 02 Jun 2020 16:21:01 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.1/src/haproxy-2.1.5.tar.gz
# Tue, 02 Jun 2020 16:21:02 GMT
ENV HAPROXY_SHA256=42174ac5836ab243565b888299ec30115c1259e75872696708528260c6700ea1
# Tue, 02 Jun 2020 16:21:54 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Tue, 02 Jun 2020 16:21:54 GMT
STOPSIGNAL SIGUSR1
# Tue, 02 Jun 2020 16:21:55 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Tue, 02 Jun 2020 16:21:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 02 Jun 2020 16:21:55 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:425c132a4e569cd90775ab9ce89856a8bfd1d736c7c10a76099b36cd3affd086`  
		Last Modified: Tue, 02 Jun 2020 16:23:02 GMT  
		Size: 6.7 MB (6743902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f26c48efe296ebc759e35d521ca7d1aaef5aeb2abebcf7995ead49adf88aa54a`  
		Last Modified: Tue, 02 Jun 2020 16:23:01 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:fded5a0db627afb3271b57875260fca1d2eb661c1855370c90fe2e8f45b6888e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (9020573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:775c0f018b87329076d2ee5a2a6d6f7f077caee07934b7b411890743e1145043`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Tue, 09 Jun 2020 22:16:19 GMT
ENV HAPROXY_VERSION=2.1.7
# Tue, 09 Jun 2020 22:16:19 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.1/src/haproxy-2.1.7.tar.gz
# Tue, 09 Jun 2020 22:16:20 GMT
ENV HAPROXY_SHA256=392e6cf18e75fe7e166102e8c4512942890a0b5ae738f6064faab4687f60a339
# Tue, 09 Jun 2020 22:16:49 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Tue, 09 Jun 2020 22:16:50 GMT
STOPSIGNAL SIGUSR1
# Tue, 09 Jun 2020 22:16:51 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Tue, 09 Jun 2020 22:16:51 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 09 Jun 2020 22:16:52 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a4adb9ee16e7d20fd66f49dec0ed7085ad8ddbb18737ba7a3f40a1ecb93e345`  
		Last Modified: Tue, 09 Jun 2020 22:17:31 GMT  
		Size: 6.4 MB (6400257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac615a4b3216e7b40abea8fa2ed01644d8ca425d83829b4ec9bca83271bb5a61`  
		Last Modified: Tue, 09 Jun 2020 22:17:30 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:5f9b091e59f728c2ce5e649520222d1162b13f92d65a7696015757e9ab7e63ee
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8975732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e089575128e48c8bb5b52bf2f382a526d6d378a611892f77743b7c312adaa78c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 15:59:55 GMT
ENV HAPROXY_VERSION=2.1.5
# Tue, 02 Jun 2020 15:59:55 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.1/src/haproxy-2.1.5.tar.gz
# Tue, 02 Jun 2020 15:59:56 GMT
ENV HAPROXY_SHA256=42174ac5836ab243565b888299ec30115c1259e75872696708528260c6700ea1
# Tue, 02 Jun 2020 16:00:15 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Tue, 02 Jun 2020 16:00:16 GMT
STOPSIGNAL SIGUSR1
# Tue, 02 Jun 2020 16:00:17 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Tue, 02 Jun 2020 16:00:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 02 Jun 2020 16:00:18 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c34db2c0bf055c7be562b5a1dff7e52333daed56c26bfc4771ed96eddb356b9d`  
		Last Modified: Tue, 02 Jun 2020 16:01:46 GMT  
		Size: 6.6 MB (6553289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:601d372a83614052168c7618fccffbb86d84249b067557386d9c7c8d7300027a`  
		Last Modified: Tue, 02 Jun 2020 16:01:41 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:fe0b4ecf0a9c18ad20dc443d14415a0190d6f5f87d2ca9a7e3b6772a16329c4f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.4 MB (9413010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f33ebd48f40e634bb4387b9c3dc4e217deab6faba9f327dfd1d46c4c1d886e5b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Tue, 02 Jun 2020 16:40:56 GMT
ENV HAPROXY_VERSION=2.1.5
# Tue, 02 Jun 2020 16:40:56 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.1/src/haproxy-2.1.5.tar.gz
# Tue, 02 Jun 2020 16:40:57 GMT
ENV HAPROXY_SHA256=42174ac5836ab243565b888299ec30115c1259e75872696708528260c6700ea1
# Tue, 02 Jun 2020 16:41:18 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Tue, 02 Jun 2020 16:41:19 GMT
STOPSIGNAL SIGUSR1
# Tue, 02 Jun 2020 16:41:19 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Tue, 02 Jun 2020 16:41:20 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 02 Jun 2020 16:41:21 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f33284dadf470dfc026b0d44f45224c13c0bccb04a936a5e0f7057ab81a5cb`  
		Last Modified: Tue, 02 Jun 2020 16:42:33 GMT  
		Size: 6.7 MB (6688205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:806ef95fb53827cd7a36a5eb7b98b09472b399c6de1a7ac1d0a3226a9d3ee0ac`  
		Last Modified: Tue, 02 Jun 2020 16:42:30 GMT  
		Size: 381.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:alpine` - linux; 386

```console
$ docker pull haproxy@sha256:9b47e531f461eecd0ed537c53004a2d0ca2c35b55e570613dd0e56531303655c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9321403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27982fc42000c9e689d1f4a4e3dfca6161287f097c4b94972ead24ef81adb65f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:04 GMT
ADD file:63bd8a316cba8c404cc2e32a5120406c24aee8db3224c469a6077b941d900863 in / 
# Thu, 23 Apr 2020 21:16:04 GMT
CMD ["/bin/sh"]
# Wed, 10 Jun 2020 00:30:42 GMT
ENV HAPROXY_VERSION=2.1.7
# Wed, 10 Jun 2020 00:30:43 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.1/src/haproxy-2.1.7.tar.gz
# Wed, 10 Jun 2020 00:30:43 GMT
ENV HAPROXY_SHA256=392e6cf18e75fe7e166102e8c4512942890a0b5ae738f6064faab4687f60a339
# Wed, 10 Jun 2020 00:32:31 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Wed, 10 Jun 2020 00:32:31 GMT
STOPSIGNAL SIGUSR1
# Wed, 10 Jun 2020 00:32:32 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Wed, 10 Jun 2020 00:32:32 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 10 Jun 2020 00:32:32 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:2826c1e79865da7e0da0a993a2a38db61c3911e05b5df617439a86d4deac90fb`  
		Last Modified: Thu, 23 Apr 2020 21:16:32 GMT  
		Size: 2.8 MB (2808418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40cc4e0b604c6748a938c02ac1e07a21a3007bcd2c083afeebf81b672e061eec`  
		Last Modified: Wed, 10 Jun 2020 00:34:03 GMT  
		Size: 6.5 MB (6512605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46d6745c3e106843929e122f52f5fb1d643691a9dc747e914012eb7d2690843c`  
		Last Modified: Wed, 10 Jun 2020 00:34:00 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:29c0280074691782ec3204ca8fe7f3cb7a4d8c7d185b7d62b1e51ef0c68bc9a0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9644258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82c34ced09ee052f8bebc5efe85a92839a6803aadbea837504f6186b81aa8cbc`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 23 Apr 2020 20:39:04 GMT
ADD file:1aaebe252dfb1885e066fcbc84aaa915bae149c3608f19600855ad1d4f7450c1 in / 
# Thu, 23 Apr 2020 20:39:06 GMT
CMD ["/bin/sh"]
# Tue, 09 Jun 2020 22:20:15 GMT
ENV HAPROXY_VERSION=2.1.7
# Tue, 09 Jun 2020 22:20:18 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.1/src/haproxy-2.1.7.tar.gz
# Tue, 09 Jun 2020 22:20:23 GMT
ENV HAPROXY_SHA256=392e6cf18e75fe7e166102e8c4512942890a0b5ae738f6064faab4687f60a339
# Tue, 09 Jun 2020 22:21:15 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Tue, 09 Jun 2020 22:21:31 GMT
STOPSIGNAL SIGUSR1
# Tue, 09 Jun 2020 22:21:36 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Tue, 09 Jun 2020 22:21:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 09 Jun 2020 22:21:55 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:9a8fdc5b698322331ee7eba7dd6f66f3a4e956554db22dd1e834d519415b4f8e`  
		Last Modified: Thu, 23 Apr 2020 20:41:33 GMT  
		Size: 2.8 MB (2821843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c24cc887772f6430d0d19ac2dfbd45c743bb9eeddf2e787573d4528733df6a19`  
		Last Modified: Tue, 09 Jun 2020 22:45:46 GMT  
		Size: 6.8 MB (6822035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b7cfaa612d00c1cd380975ce1adda5771fc4765a0eb802f532b6882bedd8c0f`  
		Last Modified: Tue, 09 Jun 2020 22:45:44 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:alpine` - linux; s390x

```console
$ docker pull haproxy@sha256:db925d82886c0a5a980828163f430a233a83a7b229b60ae01b66e164bdbebf70
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.1 MB (9126034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bae30663f074532aef9c3faacbfd498ae9dd3fc3d64d0260694d3373be6f4a7d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 23 Apr 2020 17:50:57 GMT
ADD file:a59a30c2fd43c9f3b820751a6f5a54688c14440a1ddace1ab255475f46e6ba2d in / 
# Thu, 23 Apr 2020 17:50:58 GMT
CMD ["/bin/sh"]
# Tue, 09 Jun 2020 22:00:46 GMT
ENV HAPROXY_VERSION=2.1.7
# Tue, 09 Jun 2020 22:00:46 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.1/src/haproxy-2.1.7.tar.gz
# Tue, 09 Jun 2020 22:00:47 GMT
ENV HAPROXY_SHA256=392e6cf18e75fe7e166102e8c4512942890a0b5ae738f6064faab4687f60a339
# Tue, 09 Jun 2020 22:01:24 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 		zlib-dev 		&& wget -O haproxy.tar.gz "$HAPROXY_URL" 	&& echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c 	&& mkdir -p /usr/src/haproxy 	&& tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1 	&& rm haproxy.tar.gz 		&& makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_ZLIB=1 				EXTRA_OBJS=" 			contrib/prometheus-exporter/service-prometheus.o 		" 	' 	&& nproc="$(getconf _NPROCESSORS_ONLN)" 	&& eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts" 	&& eval "make -C /usr/src/haproxy install-bin $makeOpts" 		&& mkdir -p /usr/local/etc/haproxy 	&& cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors 	&& rm -rf /usr/src/haproxy 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .haproxy-rundeps $runDeps 	&& apk del --no-network .build-deps
# Tue, 09 Jun 2020 22:01:24 GMT
STOPSIGNAL SIGUSR1
# Tue, 09 Jun 2020 22:01:25 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in / 
# Tue, 09 Jun 2020 22:01:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 09 Jun 2020 22:01:25 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:7184c046fdf17da4c16ca482e5ede36e1f2d41ac8cea9c036e488fd149d6e8e7`  
		Last Modified: Thu, 23 Apr 2020 17:51:38 GMT  
		Size: 2.6 MB (2582859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbe63547717793be03861683b389d90f2511cf9a238080f324401704cf73a20a`  
		Last Modified: Tue, 09 Jun 2020 22:02:30 GMT  
		Size: 6.5 MB (6542795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708cb82e7ca1052d8ff8a6454868e70709ccf1a39f45b024f24e8b2c5be425ee`  
		Last Modified: Tue, 09 Jun 2020 22:02:34 GMT  
		Size: 380.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
