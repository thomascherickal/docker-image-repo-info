## `haproxy:alpine3.15`

```console
$ docker pull haproxy@sha256:18086ebbc6c749c8c7b190d5766439ef857ec567f41c48e50e6102c97546375a
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

### `haproxy:alpine3.15` - linux; amd64

```console
$ docker pull haproxy@sha256:82300ab35482dd937662f6c7635894a57141d5362245a8801d0e2b40d28ec5f9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.3 MB (10316839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a1686873de9f6000c7490c8d88b3f56db000302dee78d4b368c145fd8bad406`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 17 Mar 2022 04:01:58 GMT
ADD file:cf4b631a115c2bbfbd81cad2d3041bceb64a8136aac92ba8a63b6c51d60af764 in / 
# Thu, 17 Mar 2022 04:01:59 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 11:32:10 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Thu, 17 Mar 2022 11:34:42 GMT
ENV HAPROXY_VERSION=2.5.5
# Thu, 17 Mar 2022 11:34:42 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/haproxy-2.5.5.tar.gz
# Thu, 17 Mar 2022 11:34:42 GMT
ENV HAPROXY_SHA256=063c4845cdb2d76f292ef44d9c0117a853d8d10ae5d9615b406b14a4d74fe4b9
# Thu, 17 Mar 2022 11:35:57 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 17 Mar 2022 11:35:57 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Mar 2022 11:35:57 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 17 Mar 2022 11:35:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 11:35:58 GMT
USER haproxy
# Thu, 17 Mar 2022 11:35:58 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:3d243047344378e9b7136d552d48feb7ea8b6fe14ce0990e0cc011d5e369626a`  
		Last Modified: Thu, 17 Mar 2022 04:02:41 GMT  
		Size: 2.8 MB (2812636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:675afd8dab16be3a9708952f9037b5b507ceeab54723cdecf8b1c3b23d1d46d7`  
		Last Modified: Thu, 17 Mar 2022 11:50:35 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f46bde4af7a9c51da510dea9d759c59cfa14f0518c58cc7e8fd6b0a4a66d26`  
		Last Modified: Thu, 17 Mar 2022 11:51:11 GMT  
		Size: 7.5 MB (7502476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:783ed07876893591ab56046d8ceeb81c881b16f02a612684d6dc4b483814aed9`  
		Last Modified: Thu, 17 Mar 2022 11:51:10 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:alpine3.15` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:b915635773cfb0f11a74225d599a04d99fa3cd6c6f87bd952811ded8909bc89a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.1 MB (10070755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40c7010f2168baaef7c61b45b1140d63a7a24f664f4fbe963bc2728a34e0de5f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 17 Mar 2022 02:26:45 GMT
ADD file:9c8618405ef54d562132919ffe49c862d014b402e0e4813b87bf01574fa04c0e in / 
# Thu, 17 Mar 2022 02:26:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 05:54:56 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Thu, 17 Mar 2022 05:55:39 GMT
ENV HAPROXY_VERSION=2.5.5
# Thu, 17 Mar 2022 05:55:39 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/haproxy-2.5.5.tar.gz
# Thu, 17 Mar 2022 05:55:40 GMT
ENV HAPROXY_SHA256=063c4845cdb2d76f292ef44d9c0117a853d8d10ae5d9615b406b14a4d74fe4b9
# Thu, 17 Mar 2022 05:56:06 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 17 Mar 2022 05:56:06 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Mar 2022 05:56:06 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 17 Mar 2022 05:56:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 05:56:07 GMT
USER haproxy
# Thu, 17 Mar 2022 05:56:08 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:787f016efa9bc7812361be134f731e845b97fba19169cf3615e7048c0412380e`  
		Last Modified: Thu, 17 Mar 2022 02:28:24 GMT  
		Size: 2.6 MB (2624973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:630f34f77a332e516e594a42e5771436581fbc01c3a0b7ca579db51699e6249f`  
		Last Modified: Thu, 17 Mar 2022 06:02:12 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3700025c7b406382f89e5454658ec7d1592c17e87ce08f9da7dc7537d704a420`  
		Last Modified: Thu, 17 Mar 2022 06:02:40 GMT  
		Size: 7.4 MB (7444052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:947d4f420b57cec0fed4fdf1fb6248065851ad51d9ae2870743a803928417513`  
		Last Modified: Thu, 17 Mar 2022 06:02:35 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:alpine3.15` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:ae1cc691632eb7f4da7c772dbfb961b6c901c55b03b392baddf0bac3cdb4076a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.8 MB (9795631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15d11b443e3d761369f346a84f1e1219acb819d8116cdf425b78050bc1c91b87`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 17 Mar 2022 09:26:34 GMT
ADD file:01e87d7f83dfb32fd8a1b7b889b923432c2e0516d79a4196e01ad0ad15e33d68 in / 
# Thu, 17 Mar 2022 09:26:35 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 21:11:38 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Thu, 17 Mar 2022 21:13:32 GMT
ENV HAPROXY_VERSION=2.5.5
# Thu, 17 Mar 2022 21:13:32 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/haproxy-2.5.5.tar.gz
# Thu, 17 Mar 2022 21:13:33 GMT
ENV HAPROXY_SHA256=063c4845cdb2d76f292ef44d9c0117a853d8d10ae5d9615b406b14a4d74fe4b9
# Thu, 17 Mar 2022 21:13:58 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 17 Mar 2022 21:13:59 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Mar 2022 21:13:59 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 17 Mar 2022 21:14:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 21:14:00 GMT
USER haproxy
# Thu, 17 Mar 2022 21:14:01 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:205cbce5da6d59acc17b2db4c1af7903ca3497b99d4bedb94ef66ace17303808`  
		Last Modified: Thu, 17 Mar 2022 09:28:11 GMT  
		Size: 2.4 MB (2427136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43d33da3c6781aced6c5cb11162bfedbd4f95d2946f556e59de44835b669b474`  
		Last Modified: Thu, 17 Mar 2022 21:28:28 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00c28ba4c339b3cd36715cc470365f594a757f6ec90b12ebdc3a6fbe03ab7444`  
		Last Modified: Thu, 17 Mar 2022 21:29:33 GMT  
		Size: 7.4 MB (7366761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f3ebe75133d4f494d2603cf061b5e630955dc7ed7675ff11c54eb1ca82c57f`  
		Last Modified: Thu, 17 Mar 2022 21:29:29 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:alpine3.15` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:f2f72e6a7a50ecdedbda5b8019b12522593bcbd253c578a603ecb78d52fd1111
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.3 MB (10300982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ed3af8fd565842047725108354b93b67e2109f5b0bca26f1ba6257417d22b37`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 17 Mar 2022 03:19:52 GMT
ADD file:cd7d91362950471ca4678cf3833dc47119ab519dea51424c847bbbb21e1649d4 in / 
# Thu, 17 Mar 2022 03:19:52 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 10:55:59 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Thu, 17 Mar 2022 10:57:25 GMT
ENV HAPROXY_VERSION=2.5.5
# Thu, 17 Mar 2022 10:57:26 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/haproxy-2.5.5.tar.gz
# Thu, 17 Mar 2022 10:57:27 GMT
ENV HAPROXY_SHA256=063c4845cdb2d76f292ef44d9c0117a853d8d10ae5d9615b406b14a4d74fe4b9
# Thu, 17 Mar 2022 10:57:54 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 17 Mar 2022 10:57:54 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Mar 2022 10:57:56 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 17 Mar 2022 10:57:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 10:57:57 GMT
USER haproxy
# Thu, 17 Mar 2022 10:57:58 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:148d739a8e6b9342daa1f5b428d3a3c6118f340f21df28c16e06f918ef150147`  
		Last Modified: Thu, 17 Mar 2022 03:20:45 GMT  
		Size: 2.7 MB (2714807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4be66db9c61a991cea994c1b06c9d816528a445cd38aed2036949c9dd6e473dd`  
		Last Modified: Thu, 17 Mar 2022 11:07:06 GMT  
		Size: 1.3 KB (1254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ab8652162be346a065fb074ab75e17b793e9cec2ba9c7e5f0869911a33b310`  
		Last Modified: Thu, 17 Mar 2022 11:07:47 GMT  
		Size: 7.6 MB (7584472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3870bec3797438c747eaccb39413b5212957f205b6e4e75a38045a06e41ecc2d`  
		Last Modified: Thu, 17 Mar 2022 11:07:46 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:alpine3.15` - linux; 386

```console
$ docker pull haproxy@sha256:1968a1b77a7fdb6c672db7def81d46acc44b78a93eed84028540295bc6983541
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.1 MB (10148517 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fb166a0df74cbd0adc544d4c9ff1b3f888d97ed5879e0550058e8f3df598cff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 17 Mar 2022 08:13:03 GMT
ADD file:22216bc654d9177244235f242fa83cae3b283b3c145cad7ccf11c0d29f5f0ff2 in / 
# Thu, 17 Mar 2022 08:13:03 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 16:57:33 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Thu, 17 Mar 2022 16:59:45 GMT
ENV HAPROXY_VERSION=2.5.5
# Thu, 17 Mar 2022 16:59:45 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/haproxy-2.5.5.tar.gz
# Thu, 17 Mar 2022 16:59:45 GMT
ENV HAPROXY_SHA256=063c4845cdb2d76f292ef44d9c0117a853d8d10ae5d9615b406b14a4d74fe4b9
# Thu, 17 Mar 2022 17:00:50 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 17 Mar 2022 17:00:51 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Mar 2022 17:00:51 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 17 Mar 2022 17:00:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 17:00:51 GMT
USER haproxy
# Thu, 17 Mar 2022 17:00:51 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:93317a1f65ec94b67aefe728a598022610246404e3a68d391c76cd0e5244a2a0`  
		Last Modified: Thu, 17 Mar 2022 08:13:56 GMT  
		Size: 2.8 MB (2821789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f68adde4f2f02524f245ee81cd8cc4ae7266ef56addee397dffc5a733443b8`  
		Last Modified: Thu, 17 Mar 2022 17:14:22 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e816afa37d11a3c761ca6ae92e1e87da0737d4ec44309fa6ba56c45440b9133`  
		Last Modified: Thu, 17 Mar 2022 17:15:13 GMT  
		Size: 7.3 MB (7325003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a6ebdaa53d5a801959fcf495897e1e7aba68a72417024fe38e00fdf9130535`  
		Last Modified: Thu, 17 Mar 2022 17:15:12 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:alpine3.15` - linux; ppc64le

```console
$ docker pull haproxy@sha256:1e6b81124e1d28ca2e4f0aebbc59fd19ae704af3755fdfb9623123c69dc37bb5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.7 MB (10744111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ba903a64084594e3c383ef02631655100976130167225fd740a4a3c64ed0cdc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 17 Mar 2022 11:14:04 GMT
ADD file:ddc94e1e084c05807db26adcc95b47a137fa47fb391e75998b338ada65e00c1c in / 
# Thu, 17 Mar 2022 11:14:09 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 23:47:22 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Thu, 17 Mar 2022 23:53:55 GMT
ENV HAPROXY_VERSION=2.5.5
# Thu, 17 Mar 2022 23:54:00 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/haproxy-2.5.5.tar.gz
# Thu, 17 Mar 2022 23:54:03 GMT
ENV HAPROXY_SHA256=063c4845cdb2d76f292ef44d9c0117a853d8d10ae5d9615b406b14a4d74fe4b9
# Thu, 17 Mar 2022 23:54:49 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 17 Mar 2022 23:54:55 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Mar 2022 23:54:57 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 17 Mar 2022 23:55:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 23:55:03 GMT
USER haproxy
# Thu, 17 Mar 2022 23:55:09 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:eef85fcc847498263d979ef7ec75680d05e90815eb83a9ec4db135b990c0d8b8`  
		Last Modified: Thu, 17 Mar 2022 11:15:15 GMT  
		Size: 2.8 MB (2814051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b148fb71385e6874faf6e02ca7c82c412e346ef236ca4027081adb0fea8186`  
		Last Modified: Fri, 18 Mar 2022 00:30:29 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3040627860f4ea1fe467d4784ef1f61ea409d231150c4fa38046c2d8ecc61f02`  
		Last Modified: Fri, 18 Mar 2022 00:31:20 GMT  
		Size: 7.9 MB (7928324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7ab5bdf47b7ca47b1e59f8d8a54a54c8967455e9662c9cab3bad3e67084e6a`  
		Last Modified: Fri, 18 Mar 2022 00:31:19 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:alpine3.15` - linux; s390x

```console
$ docker pull haproxy@sha256:25dd0b071ce090c6d27d8accb5975f75c4e7c0849a6359d8e06fc7a68d9eb639
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.1 MB (10109939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f32e8deced0c435caf16056df25152e349efbd77d3c1e0d9f2f5cf187e5ca69a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 17 Mar 2022 03:04:28 GMT
ADD file:f623c69acb1859b41ef29e8f20f4e6c7072d9c6d7210d745afc615251bfe418f in / 
# Thu, 17 Mar 2022 03:04:28 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 08:10:57 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Thu, 17 Mar 2022 08:12:18 GMT
ENV HAPROXY_VERSION=2.5.5
# Thu, 17 Mar 2022 08:12:18 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.5/src/haproxy-2.5.5.tar.gz
# Thu, 17 Mar 2022 08:12:18 GMT
ENV HAPROXY_SHA256=063c4845cdb2d76f292ef44d9c0117a853d8d10ae5d9615b406b14a4d74fe4b9
# Thu, 17 Mar 2022 08:12:49 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Thu, 17 Mar 2022 08:12:49 GMT
STOPSIGNAL SIGUSR1
# Thu, 17 Mar 2022 08:12:50 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 17 Mar 2022 08:12:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 08:12:50 GMT
USER haproxy
# Thu, 17 Mar 2022 08:12:50 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:d51040c5bfbf434887bfed2557335a411e6ef760d04cc178d455d1c3ec1b721c`  
		Last Modified: Thu, 17 Mar 2022 03:05:26 GMT  
		Size: 2.6 MB (2601715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5d1764618b7322967211467ec4152b6e3f10de2669c225c694d1af732930c2`  
		Last Modified: Thu, 17 Mar 2022 08:21:33 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ebf81bca3fba11c1b3492c55b6ce4769304982d71fb2e8661c90f2a24d28fb2`  
		Last Modified: Thu, 17 Mar 2022 08:22:01 GMT  
		Size: 7.5 MB (7506496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc1ab77d482b7546df3a560e61801bb086bbc084e9f68837cb007b7f80c2c247`  
		Last Modified: Thu, 17 Mar 2022 08:22:00 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
