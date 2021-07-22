## `haproxy:alpine`

```console
$ docker pull haproxy@sha256:278afc7563fcb5d498201d0093f9c700e659628677604bc15a82e3abba175799
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `haproxy:alpine` - linux; amd64

```console
$ docker pull haproxy@sha256:8819f159761cf992682ccb1267ab52e4b086a332e2baed24df18ff51bf49bd6a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.1 MB (10128308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7a37d8a7b2f124598b023e74621914426f81ab8b4f8e01d74cfbee1dd62ef0f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:19:37 GMT
ADD file:f278386b0cef68136129f5f58c52445590a417b624d62bca158d4dc926c340df in / 
# Tue, 15 Jun 2021 22:19:37 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 02:48:50 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 18:34:10 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 08 Jul 2021 18:34:10 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 08 Jul 2021 18:34:10 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 08 Jul 2021 18:35:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 08 Jul 2021 18:35:12 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 18:35:12 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 18:35:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 18:35:13 GMT
USER haproxy
# Thu, 08 Jul 2021 18:35:13 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:5843afab387455b37944e709ee8c78d7520df80f8d01cf7f861aae63beeddb6b`  
		Last Modified: Tue, 15 Jun 2021 22:20:04 GMT  
		Size: 2.8 MB (2811478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7834d945b9e597e693f56fb0f9847718c1732b738a2f4956ab2c1b66c289d90`  
		Last Modified: Sat, 26 Jun 2021 02:56:43 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddff1cb6bb6da9a692c61843d46abe17a215c726bb13d570212777a87398a3d9`  
		Last Modified: Thu, 08 Jul 2021 18:38:36 GMT  
		Size: 7.3 MB (7315186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee55c5b3ebb2b318c44f2635d4eea44eadfd079d55d0b8c5a6918b8aa9d5b1dc`  
		Last Modified: Thu, 08 Jul 2021 18:38:34 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:alpine` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:b79f0c78bc069755084556b3bd897a39780d24fe70b909b7c119d53f9a6bbc01
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9912733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05e37a7293c9eccbd033a7a1a38aa77387373ba82f719cbcc400dec92a69aad3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:26 GMT
ADD file:c80bc2b093cbc0fc466582ef21cbed377de9fa874aedbf320079525ddacd1200 in / 
# Tue, 15 Jun 2021 22:57:26 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 02:02:51 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 19:07:43 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 08 Jul 2021 19:07:44 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 08 Jul 2021 19:07:44 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 08 Jul 2021 19:08:13 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 08 Jul 2021 19:08:13 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 19:08:14 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 19:08:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 19:08:15 GMT
USER haproxy
# Thu, 08 Jul 2021 19:08:15 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:b4c9a0924271af3466de27804af26420eb58da1466e7eaaba127d178b380fea3`  
		Last Modified: Tue, 15 Jun 2021 22:58:47 GMT  
		Size: 2.6 MB (2624382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85fa2947d9cc2655af4fd4aa21641629e791bcaf309a7095db77d309ddd05dfa`  
		Last Modified: Sat, 26 Jun 2021 02:08:45 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a9ab1152df106ecaf9c67a2a14b91a15581a3b86248b43604172b704b71167`  
		Last Modified: Thu, 08 Jul 2021 19:11:00 GMT  
		Size: 7.3 MB (7286705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc34702136897eee4ca8c94845af335a66311b8b8a57a5f1c40292b913ef9f72`  
		Last Modified: Thu, 08 Jul 2021 19:10:56 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:alpine` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:b318934bc8973f8f73ad46a1c4f1c097899f57cdba1f6bff40285760584a684c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9631368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c900ed3b5e7e8ae25ede6582344b41bf064d26e831bdf4bfd385861422503a3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 23:15:05 GMT
ADD file:416a8b507abdc6bdcb22997a4be0a4170796c3f9f77e315b2dbff2b0a212bc68 in / 
# Tue, 15 Jun 2021 23:15:06 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 05:27:42 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 21:29:41 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 08 Jul 2021 21:29:42 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 08 Jul 2021 21:29:42 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 08 Jul 2021 21:30:19 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 08 Jul 2021 21:30:20 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 21:30:21 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 21:30:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 21:30:22 GMT
USER haproxy
# Thu, 08 Jul 2021 21:30:22 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:136482bf81d1fa351b424ebb8c7e34d15f2c5ed3fc0b66b544b8312bda3d52d9`  
		Last Modified: Tue, 15 Jun 2021 23:16:40 GMT  
		Size: 2.4 MB (2427917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5464af225bd487370319e7125fb2769222c5c7371d1be737936169d2e5b01c`  
		Last Modified: Sat, 26 Jun 2021 05:35:56 GMT  
		Size: 1.2 KB (1196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f903498f8e23244ca6430d647dd5515930d69394f19d017d07930d288ca6580`  
		Last Modified: Thu, 08 Jul 2021 21:36:22 GMT  
		Size: 7.2 MB (7201807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a0d8812e6df331ba2d781cc1fc08c2e4ddad2bb05b762b0eb737308a1205d5`  
		Last Modified: Thu, 08 Jul 2021 21:36:18 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:alpine` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:c17729aebb94fdae2758381c550a8866ce8856237ce1892a6fba9d0cdadd7c5b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.1 MB (10133906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b500e8260787f1a0bcdc19f790686cd272d751cdd28f848f01eb2f054c700341`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 21:44:56 GMT
ADD file:6797caacbfe41bfe44000b39ed017016c6fcc492b3d6557cdaba88536df6c876 in / 
# Tue, 15 Jun 2021 21:44:56 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 02:13:15 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 19:02:27 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 08 Jul 2021 19:02:27 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 08 Jul 2021 19:02:27 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 08 Jul 2021 19:03:26 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 08 Jul 2021 19:03:26 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 19:03:27 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 19:03:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 19:03:27 GMT
USER haproxy
# Thu, 08 Jul 2021 19:03:27 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:58ab47519297212468320b23b8100fc1b2b96e8d342040806ae509a778a0a07a`  
		Last Modified: Tue, 15 Jun 2021 21:46:03 GMT  
		Size: 2.7 MB (2709626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb8dc96e2a4b7f90ae2dbfca981fe199966b64e3426ca1f742499d46ad1aa357`  
		Last Modified: Sat, 26 Jun 2021 02:21:19 GMT  
		Size: 1.2 KB (1197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b367d065849fc1a609fb169119e94047ed3a2b475932bb292bff5b6cc45a1f`  
		Last Modified: Thu, 08 Jul 2021 19:07:30 GMT  
		Size: 7.4 MB (7422635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60cf6675a5a8e39f65c07f8553ab269ab83f947cbfa20da77e6da66ca033969e`  
		Last Modified: Thu, 08 Jul 2021 19:07:28 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:alpine` - linux; 386

```console
$ docker pull haproxy@sha256:01a8472d10c0512c1950dad3ae7472f99767eeaa8f0bbbb3aa53813d35961ab0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (9998434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e50005241013c0fb9d14f539c88cbf5dd3ebfec6c0498014c4a70a002cbe3d48`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 21:38:30 GMT
ADD file:3b0fe1454491bb05e218b090fd461f2fd39546aa4a53eb3f953ee8eae149ac57 in / 
# Tue, 15 Jun 2021 21:38:30 GMT
CMD ["/bin/sh"]
# Sat, 26 Jun 2021 01:39:05 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 19:03:09 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 08 Jul 2021 19:03:09 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 08 Jul 2021 19:03:09 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 08 Jul 2021 19:04:25 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 08 Jul 2021 19:04:25 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 19:04:25 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 19:04:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 19:04:26 GMT
USER haproxy
# Thu, 08 Jul 2021 19:04:26 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:be21df321efb39c5daf3151073ebff7688e15ea6cd5158878bc9559a5db76ac6`  
		Last Modified: Tue, 15 Jun 2021 21:39:16 GMT  
		Size: 2.8 MB (2820718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc6fe536c8e50a97873c166db7d3b669842dec91d85ce73433028b3b198a1c4`  
		Last Modified: Sat, 26 Jun 2021 01:49:46 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:832c00757ee7003ebca753eff8d4c6af86ebcf09efecec8e1171e550c8fc816f`  
		Last Modified: Thu, 08 Jul 2021 19:08:59 GMT  
		Size: 7.2 MB (7176071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85e6578d15134f65f8b977b9e7c9322e6281b3c765978ce760142c0bac7197ad`  
		Last Modified: Thu, 08 Jul 2021 19:08:57 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:alpine` - linux; ppc64le

```console
$ docker pull haproxy@sha256:8371490329ce959d92d6d6bca900a6702869e800fbd8c4a80438da13efa8b696
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.6 MB (10556641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5510c2e0b44e02d587dd27e62dd07ef69cc51b3e43f00927403e3c29eb34cfc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Jun 2021 22:27:00 GMT
ADD file:0075aad7a94f0496483442bb2d9fdaa13e9c23087b90638d014b4bc263aa3861 in / 
# Tue, 15 Jun 2021 22:27:03 GMT
CMD ["/bin/sh"]
# Fri, 16 Jul 2021 20:17:57 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Fri, 16 Jul 2021 20:19:42 GMT
ENV HAPROXY_VERSION=2.4.2
# Fri, 16 Jul 2021 20:19:48 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Fri, 16 Jul 2021 20:19:51 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 22 Jul 2021 03:04:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 22 Jul 2021 03:04:47 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 03:04:50 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 03:04:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 03:04:59 GMT
USER haproxy
# Thu, 22 Jul 2021 03:05:04 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:baf144cfb66ebe9df1969f3b90f1c448beff98edc84de1ccb5d6346195a070d4`  
		Last Modified: Tue, 15 Jun 2021 22:27:38 GMT  
		Size: 2.8 MB (2810478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e907663c9428bbbb731a221721c606bad29e54dac6f0dda85d6aa3175a725e`  
		Last Modified: Thu, 22 Jul 2021 03:40:16 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25fed8e719bd522b435fea4d6999c2ecffeb38e8288458cea40c3ecfa9131656`  
		Last Modified: Thu, 22 Jul 2021 03:40:53 GMT  
		Size: 7.7 MB (7744514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c45ecd590d1194b07f22c1e98348800abd5fdc2592d5c85e8fd5413acc1f29`  
		Last Modified: Thu, 22 Jul 2021 03:40:50 GMT  
		Size: 450.0 B  
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
