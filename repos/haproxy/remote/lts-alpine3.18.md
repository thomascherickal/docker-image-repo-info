## `haproxy:lts-alpine3.18`

```console
$ docker pull haproxy@sha256:b5b399179deae535a4e5cc5dded44882678d97613997aa7dedf743228b39379a
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

### `haproxy:lts-alpine3.18` - linux; amd64

```console
$ docker pull haproxy@sha256:a68b5dca2bd9391ae7a0bf66b4563b5fe283e78d14b8d45bbe37da45923ef490
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.6 MB (11618788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be9780305ef0ad618a20d7a1118c601f52fe2515c34dc7768119d4a352e9addf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Thu, 30 Nov 2023 23:25:11 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Thu, 07 Dec 2023 22:20:39 GMT
ENV HAPROXY_VERSION=2.8.5
# Thu, 07 Dec 2023 22:20:39 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.8/src/haproxy-2.8.5.tar.gz
# Thu, 07 Dec 2023 22:20:39 GMT
ENV HAPROXY_SHA256=3f5459c5a58e0b343a32eaef7ed5bed9d3fc29d8aa9e14b36c92c969fc2a60d9
# Thu, 07 Dec 2023 22:21:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 07 Dec 2023 22:21:13 GMT
STOPSIGNAL SIGUSR1
# Thu, 07 Dec 2023 22:21:13 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 07 Dec 2023 22:21:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 22:21:13 GMT
USER haproxy
# Thu, 07 Dec 2023 22:21:13 GMT
WORKDIR /var/lib/haproxy
# Thu, 07 Dec 2023 22:21:13 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:572bea91dd40620e8bc09d573976c57083e9e8bbcb9e6063ee07acb0efb06fd8`  
		Last Modified: Thu, 30 Nov 2023 23:30:20 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5036d9216c97040382b1ae535c66629e16a760a4a69df2907c22fd6eb87bab59`  
		Last Modified: Thu, 07 Dec 2023 22:24:00 GMT  
		Size: 8.2 MB (8214632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ea847506da06120749583f338579801950733cb8043157237117bbb1ba97649`  
		Last Modified: Thu, 07 Dec 2023 22:23:59 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts-alpine3.18` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:63a58e30faacf854d99ae46b30754bdcee8daa414ce3e9ee7dd3637c0bda38cb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.2 MB (11182943 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:387447634438967ed768c116510dfc35ddaff4abcc99aa38a85cb00ef5228f28`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 01:04:12 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Thu, 07 Dec 2023 21:49:21 GMT
ENV HAPROXY_VERSION=2.8.5
# Thu, 07 Dec 2023 21:49:21 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.8/src/haproxy-2.8.5.tar.gz
# Thu, 07 Dec 2023 21:49:21 GMT
ENV HAPROXY_SHA256=3f5459c5a58e0b343a32eaef7ed5bed9d3fc29d8aa9e14b36c92c969fc2a60d9
# Thu, 07 Dec 2023 21:49:56 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 07 Dec 2023 21:49:56 GMT
STOPSIGNAL SIGUSR1
# Thu, 07 Dec 2023 21:49:56 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 07 Dec 2023 21:49:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 21:49:56 GMT
USER haproxy
# Thu, 07 Dec 2023 21:49:56 GMT
WORKDIR /var/lib/haproxy
# Thu, 07 Dec 2023 21:49:56 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22df07beba8c71182164f4602773af46842bd9060889cb7975848b7b2c36b4f`  
		Last Modified: Fri, 01 Dec 2023 01:08:00 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed1404cb6dab5c76854f23b9d416baccd3770d31da19ec516cf37f4a6f90385`  
		Last Modified: Thu, 07 Dec 2023 21:50:57 GMT  
		Size: 8.0 MB (8034342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:480ffe0ebe8693b54e14ba52e2d9ea1207e0e0a1a8fb7dbe9acee936acdac139`  
		Last Modified: Thu, 07 Dec 2023 21:50:56 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts-alpine3.18` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:73a4858092bb3e305a10489df4a0cd9893e26d79a2b2879f39c2548bbb507c0b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.8 MB (10827928 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:141a14ada5e9d97c529eecafa6a37628d17b97fd46a6ce00bf13e9577d1282fb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Thu, 30 Nov 2023 22:51:19 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Thu, 07 Dec 2023 21:58:10 GMT
ENV HAPROXY_VERSION=2.8.5
# Thu, 07 Dec 2023 21:58:10 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.8/src/haproxy-2.8.5.tar.gz
# Thu, 07 Dec 2023 21:58:10 GMT
ENV HAPROXY_SHA256=3f5459c5a58e0b343a32eaef7ed5bed9d3fc29d8aa9e14b36c92c969fc2a60d9
# Thu, 07 Dec 2023 21:58:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 07 Dec 2023 21:58:34 GMT
STOPSIGNAL SIGUSR1
# Thu, 07 Dec 2023 21:58:34 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 07 Dec 2023 21:58:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 21:58:34 GMT
USER haproxy
# Thu, 07 Dec 2023 21:58:35 GMT
WORKDIR /var/lib/haproxy
# Thu, 07 Dec 2023 21:58:35 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540d0df0fe33ad5c81369405e8247bf0a99a0d0b872e5c3c6f39726de7a9362f`  
		Last Modified: Thu, 30 Nov 2023 22:55:27 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10098e06fbe3229d9bd5ef3afaeb35eeabc8a1b323a19b34c4aaff7e1af68a98`  
		Last Modified: Thu, 07 Dec 2023 22:00:56 GMT  
		Size: 7.9 MB (7925192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b16988f07dd7dda626267efa2c8ed17cd2f2c7cd507d70cbfc91f2bbbce0029`  
		Last Modified: Thu, 07 Dec 2023 22:00:55 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:dafd2c3db222a5e645538a2499ad7c8c29e2f4ef734e36e87a7de33b03f1d513
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.5 MB (11466667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ea6715ff7dfa47022a04a0bf96a21d6bfcbf1d07d5f7dba4f9768078acddea9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 06:55:29 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Thu, 07 Dec 2023 21:40:16 GMT
ENV HAPROXY_VERSION=2.8.5
# Thu, 07 Dec 2023 21:40:16 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.8/src/haproxy-2.8.5.tar.gz
# Thu, 07 Dec 2023 21:40:16 GMT
ENV HAPROXY_SHA256=3f5459c5a58e0b343a32eaef7ed5bed9d3fc29d8aa9e14b36c92c969fc2a60d9
# Thu, 07 Dec 2023 21:40:38 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 07 Dec 2023 21:40:38 GMT
STOPSIGNAL SIGUSR1
# Thu, 07 Dec 2023 21:40:38 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 07 Dec 2023 21:40:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 21:40:38 GMT
USER haproxy
# Thu, 07 Dec 2023 21:40:38 GMT
WORKDIR /var/lib/haproxy
# Thu, 07 Dec 2023 21:40:39 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48d6cf1687a848ba43d731d0b9848a4167c71d6eda7fd0f2c9e58b3c1bf3f365`  
		Last Modified: Fri, 01 Dec 2023 06:59:01 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d7e2b1bf0d810bcf3d18387bb24e4d65b5942f21a5ed7dbf56fa8b389e3ebc5`  
		Last Modified: Thu, 07 Dec 2023 21:42:44 GMT  
		Size: 8.1 MB (8131907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6676ab7edc3229e97fb64a629c973e2d19a6a62284b78c65a3321c3b891680e`  
		Last Modified: Thu, 07 Dec 2023 21:42:43 GMT  
		Size: 445.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts-alpine3.18` - linux; 386

```console
$ docker pull haproxy@sha256:70e179177ce1097a3561d70de10e7a0c5f7087164900461da9db7d032525abf4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.2 MB (11223117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5be1d15c8c6c9dfba967ea4fd88406b668472b08fbe9490d4eb974eb37d31be6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 01 Dec 2023 02:03:44 GMT
ADD file:92902088cd15ed8f5dca2f7fc6570fb4e4824fac8b09e091c88e96bbd0ca814b in / 
# Fri, 01 Dec 2023 02:03:44 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:48:06 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Thu, 07 Dec 2023 21:39:51 GMT
ENV HAPROXY_VERSION=2.8.5
# Thu, 07 Dec 2023 21:39:51 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.8/src/haproxy-2.8.5.tar.gz
# Thu, 07 Dec 2023 21:39:51 GMT
ENV HAPROXY_SHA256=3f5459c5a58e0b343a32eaef7ed5bed9d3fc29d8aa9e14b36c92c969fc2a60d9
# Thu, 07 Dec 2023 21:41:00 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 07 Dec 2023 21:41:00 GMT
STOPSIGNAL SIGUSR1
# Thu, 07 Dec 2023 21:41:01 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 07 Dec 2023 21:41:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 21:41:01 GMT
USER haproxy
# Thu, 07 Dec 2023 21:41:01 GMT
WORKDIR /var/lib/haproxy
# Thu, 07 Dec 2023 21:41:01 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:4966a8bd129b0a6adf93dc295a8fbe8f665d3194a684a5ce199c1c3596dbf3d9`  
		Last Modified: Fri, 01 Dec 2023 02:04:18 GMT  
		Size: 3.2 MB (3238831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a717fffac8faeb1f473b0e9d6029f86572f1bf51aaff2b8b63e9e964d17b0b51`  
		Last Modified: Fri, 01 Dec 2023 08:57:30 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a284f6060f66c94cff38e2a7f0e731184cc5d9b056ef6b7244183a0a767ec91d`  
		Last Modified: Thu, 07 Dec 2023 21:44:58 GMT  
		Size: 8.0 MB (7982554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318ff17b9e5881f45e2c497862e6ff58ceb00fb97812d1cfefd0980033d782ad`  
		Last Modified: Thu, 07 Dec 2023 21:44:56 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts-alpine3.18` - linux; ppc64le

```console
$ docker pull haproxy@sha256:bdb7f8689f7e6f9660343b11082f1f9c8575ea38acab1117f2b13c947132f020
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.9 MB (11903733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b088fffcbbd2a4e57396a0bb87ef31d8edd6ddd1072c2d8899f9901df187bf1a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 30 Nov 2023 23:19:04 GMT
ADD file:3450a1687b552498a987f87cb844b7f597c7181d7c3d31943d7b3036d5300d5e in / 
# Thu, 30 Nov 2023 23:19:05 GMT
CMD ["/bin/sh"]
# Thu, 30 Nov 2023 23:25:51 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Thu, 07 Dec 2023 22:20:40 GMT
ENV HAPROXY_VERSION=2.8.5
# Thu, 07 Dec 2023 22:20:40 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.8/src/haproxy-2.8.5.tar.gz
# Thu, 07 Dec 2023 22:20:40 GMT
ENV HAPROXY_SHA256=3f5459c5a58e0b343a32eaef7ed5bed9d3fc29d8aa9e14b36c92c969fc2a60d9
# Thu, 07 Dec 2023 22:21:01 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 07 Dec 2023 22:21:01 GMT
STOPSIGNAL SIGUSR1
# Thu, 07 Dec 2023 22:21:01 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 07 Dec 2023 22:21:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 22:21:02 GMT
USER haproxy
# Thu, 07 Dec 2023 22:21:02 GMT
WORKDIR /var/lib/haproxy
# Thu, 07 Dec 2023 22:21:03 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:4e13780adf2776477b14ef9c0f4f563f820a2fde166d472218037b979e84d31a`  
		Last Modified: Thu, 30 Nov 2023 23:20:01 GMT  
		Size: 3.3 MB (3348322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:208e590beab001d2a5a178f6f6977a380b03535ae3a7625b9d282bc148609157`  
		Last Modified: Thu, 30 Nov 2023 23:34:37 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e5d27bdf4be1bb8a92168bc9bc7aef669e20ee41c9ea6e97d95d3c17a61770`  
		Last Modified: Thu, 07 Dec 2023 22:23:46 GMT  
		Size: 8.6 MB (8553675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3be58aae668f87bc6c77399dfb049620c01c7ad61095b723bac2cf8179865d76`  
		Last Modified: Thu, 07 Dec 2023 22:23:45 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts-alpine3.18` - linux; s390x

```console
$ docker pull haproxy@sha256:50af24f5719ed809acb8435cdb6f4e41b4b229c353f9ddac11478ce077462c28
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.3 MB (11295051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a16ecec2d4e5f9452efdf56774210d8eef4f03deee146ebd9590a975cc87a71a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:08 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Thu, 30 Nov 2023 22:42:09 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 07:48:25 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Thu, 07 Dec 2023 21:43:32 GMT
ENV HAPROXY_VERSION=2.8.5
# Thu, 07 Dec 2023 21:43:32 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.8/src/haproxy-2.8.5.tar.gz
# Thu, 07 Dec 2023 21:43:32 GMT
ENV HAPROXY_SHA256=3f5459c5a58e0b343a32eaef7ed5bed9d3fc29d8aa9e14b36c92c969fc2a60d9
# Thu, 07 Dec 2023 21:44:20 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 07 Dec 2023 21:44:23 GMT
STOPSIGNAL SIGUSR1
# Thu, 07 Dec 2023 21:44:23 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 07 Dec 2023 21:44:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 21:44:23 GMT
USER haproxy
# Thu, 07 Dec 2023 21:44:24 GMT
WORKDIR /var/lib/haproxy
# Thu, 07 Dec 2023 21:44:24 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24f860f48f223eeee85484a28de069538b16ec903cffd99b431a0b132eacab39`  
		Last Modified: Fri, 01 Dec 2023 07:54:29 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56bdc760cca0e8650e98a7a44fde7beb9ae8c5f5d3d9d47702f9d7a23c9808ea`  
		Last Modified: Thu, 07 Dec 2023 21:47:49 GMT  
		Size: 8.1 MB (8075863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bb60c9ee1d9e2fb8ec945954d4ea24c50ba2539bd24eab62ebd98fc2c57d8e6`  
		Last Modified: Thu, 07 Dec 2023 21:47:48 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
