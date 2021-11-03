## `haproxy:lts-alpine3.14`

```console
$ docker pull haproxy@sha256:2468e789fdc9ea107d81f9f207a3cecf215c09a6131eac42e391809263c6b9fa
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

### `haproxy:lts-alpine3.14` - linux; amd64

```console
$ docker pull haproxy@sha256:8a489da287b945995ff4cb082b3cc65be8dafe486339a2b970fcb7b638ee2072
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.2 MB (10153380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d0267cf98b435e7bbc9a4e6d34ae3167cd32f37e8f28db01a344c3b81f39039`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 09 Oct 2021 00:21:39 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Wed, 03 Nov 2021 19:25:19 GMT
ENV HAPROXY_VERSION=2.4.8
# Wed, 03 Nov 2021 19:25:19 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.8.tar.gz
# Wed, 03 Nov 2021 19:25:19 GMT
ENV HAPROXY_SHA256=e3e4c1ad293bc25e8d8790cc5e45133213dda008bfd0228bf3077259b32ebaa5
# Wed, 03 Nov 2021 19:26:19 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 03 Nov 2021 19:26:19 GMT
STOPSIGNAL SIGUSR1
# Wed, 03 Nov 2021 19:26:19 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 03 Nov 2021 19:26:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 Nov 2021 19:26:20 GMT
USER haproxy
# Wed, 03 Nov 2021 19:26:20 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5febe5707f58c68676cb93a91b42eb1d1ff52d34ff313d13654797f29215efce`  
		Last Modified: Sat, 09 Oct 2021 00:34:07 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b16eee6aa24e790a15f072d59852ebac4d6f982883e987de8446951b3cc0dae7`  
		Last Modified: Wed, 03 Nov 2021 19:28:39 GMT  
		Size: 7.3 MB (7337201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fcab1d1f802783b7358695e9c0d300541844d9bffd10a12341b6015e4378b0d`  
		Last Modified: Wed, 03 Nov 2021 19:28:38 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts-alpine3.14` - linux; arm variant v6

```console
$ docker pull haproxy@sha256:6fea9f4adaccb2ba0e79b865f608e30c404fefe4a5a4ebb71b83b5eb870eb600
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.9 MB (9941444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1d49799e82ae103f310b02f2b191e499a3eeb2877109fb861f95b81f65cd173`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Sat, 09 Oct 2021 01:21:28 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Wed, 03 Nov 2021 19:59:54 GMT
ENV HAPROXY_VERSION=2.4.8
# Wed, 03 Nov 2021 19:59:55 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.8.tar.gz
# Wed, 03 Nov 2021 19:59:55 GMT
ENV HAPROXY_SHA256=e3e4c1ad293bc25e8d8790cc5e45133213dda008bfd0228bf3077259b32ebaa5
# Wed, 03 Nov 2021 20:00:22 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 03 Nov 2021 20:00:23 GMT
STOPSIGNAL SIGUSR1
# Wed, 03 Nov 2021 20:00:23 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 03 Nov 2021 20:00:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 Nov 2021 20:00:24 GMT
USER haproxy
# Wed, 03 Nov 2021 20:00:24 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0020eebb0929212f3cb1582e2aa1d49e079bf7373d97dd02e587597b8d530b34`  
		Last Modified: Sat, 09 Oct 2021 01:28:36 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57cdddfbc5ed7439da1c97e65152ceae1a7296ff82c59fa41360540a02beb18a`  
		Last Modified: Wed, 03 Nov 2021 20:04:24 GMT  
		Size: 7.3 MB (7312266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b0bc7b95e57aaf02b761e88229812b48822413146e2fb749288b4496941eed`  
		Last Modified: Wed, 03 Nov 2021 20:04:19 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts-alpine3.14` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:cfc4a572c2e40a9ce95fbed693b87d12088a1adb674a376dc2256e0a7ca2283c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.6 MB (9649859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:464dbf1d5261462de60f0d06d0813837a8811ae5aaefaed4272ac8e391830574`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Mon, 11 Oct 2021 16:16:42 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Mon, 11 Oct 2021 16:18:40 GMT
ENV HAPROXY_VERSION=2.4.7
# Mon, 11 Oct 2021 16:18:41 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.7.tar.gz
# Mon, 11 Oct 2021 16:18:41 GMT
ENV HAPROXY_SHA256=52af97f72f22ffd8a7a995fafc696291d37818feda50a23caef7dc0622421845
# Mon, 11 Oct 2021 16:19:07 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Mon, 11 Oct 2021 16:19:08 GMT
STOPSIGNAL SIGUSR1
# Mon, 11 Oct 2021 16:19:08 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 11 Oct 2021 16:19:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Oct 2021 16:19:09 GMT
USER haproxy
# Mon, 11 Oct 2021 16:19:10 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:832ba97c9f776dc6fcc764450f300cbd615a787e9a11a846b31a8927fcd8abbd`  
		Last Modified: Mon, 11 Oct 2021 16:33:52 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02a426298d73233ed09b950e99d38f83959128490de159d218010bc822643f6`  
		Last Modified: Mon, 11 Oct 2021 16:35:01 GMT  
		Size: 7.2 MB (7217710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a857a9aca3cdcc30f74d000e25125b39ae3da09d64993337a744d1a899ffeed`  
		Last Modified: Mon, 11 Oct 2021 16:34:57 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:11dfb8c6915e78457d5840f51180c6c2cca7f5a57b1a0eb2cd5de6b34caacd8d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.1 MB (10149084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:016e75c9fe71c7868ec036b17e05a334a22f21176b5394dfc67d86d42dba5d9d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Mon, 18 Oct 2021 22:07:13 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Wed, 03 Nov 2021 19:58:03 GMT
ENV HAPROXY_VERSION=2.4.8
# Wed, 03 Nov 2021 19:58:04 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.8.tar.gz
# Wed, 03 Nov 2021 19:58:05 GMT
ENV HAPROXY_SHA256=e3e4c1ad293bc25e8d8790cc5e45133213dda008bfd0228bf3077259b32ebaa5
# Wed, 03 Nov 2021 19:58:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 03 Nov 2021 19:58:43 GMT
STOPSIGNAL SIGUSR1
# Wed, 03 Nov 2021 19:58:45 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 03 Nov 2021 19:58:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 Nov 2021 19:58:46 GMT
USER haproxy
# Wed, 03 Nov 2021 19:58:47 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:544aa59f81a5014823210bf6f29377dfdda7d34c82c93d8ae32f4127c5d6ea2a`  
		Last Modified: Mon, 18 Oct 2021 22:17:51 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd6da97d02fe1f33552e1c157ef47e0f21a9f5033234acb1ddaeebc8fb44280d`  
		Last Modified: Wed, 03 Nov 2021 20:02:40 GMT  
		Size: 7.4 MB (7435553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dd806ca85804a905011d0daa3fd0762ba8c719b14c25567b58a53329e246299`  
		Last Modified: Wed, 03 Nov 2021 20:02:38 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts-alpine3.14` - linux; 386

```console
$ docker pull haproxy@sha256:5efde1df0e7d24ca6376edcb325ea7f78dc20b0483d970fefd13fb5ba32010f0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (10014351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb5096c2736347b49da16d6ea27ee36b0ecbda0df30319a689e5c10175bbfe02`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 27 Aug 2021 17:38:29 GMT
ADD file:42a7bc5a08b546b47049dd0f89ae4e7a8c86342f87000f39ade3ff52916a6c2e in / 
# Fri, 27 Aug 2021 17:38:30 GMT
CMD ["/bin/sh"]
# Sat, 09 Oct 2021 00:40:51 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Sat, 09 Oct 2021 00:43:39 GMT
ENV HAPROXY_VERSION=2.4.7
# Sat, 09 Oct 2021 00:43:39 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.7.tar.gz
# Sat, 09 Oct 2021 00:43:39 GMT
ENV HAPROXY_SHA256=52af97f72f22ffd8a7a995fafc696291d37818feda50a23caef7dc0622421845
# Sat, 09 Oct 2021 00:45:00 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Sat, 09 Oct 2021 00:45:01 GMT
STOPSIGNAL SIGUSR1
# Sat, 09 Oct 2021 00:45:01 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 09 Oct 2021 00:45:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 09 Oct 2021 00:45:01 GMT
USER haproxy
# Sat, 09 Oct 2021 00:45:02 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:b11ae9fc5d8a106cfed3a6f6c75e5b5b5797c566fac4411622b4055df6541286`  
		Last Modified: Fri, 27 Aug 2021 17:39:18 GMT  
		Size: 2.8 MB (2822857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ce5336d0e41d5d47198312c6837dd025cf7efe7465b5698b196644481cbfb9`  
		Last Modified: Sat, 09 Oct 2021 00:58:55 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e907e0f589fb47af83d50eb3e725f23f616899b737b03cb8ee72e4b07b6aafd`  
		Last Modified: Sat, 09 Oct 2021 00:59:47 GMT  
		Size: 7.2 MB (7189761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfb3708ca11da8a93ed031377a5bc6b9c5068786374d9bb24c94b0ae82a28a17`  
		Last Modified: Sat, 09 Oct 2021 00:59:46 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts-alpine3.14` - linux; ppc64le

```console
$ docker pull haproxy@sha256:7a38378b4bce8d42e3fd2fd8371d704810a73b465bc1d2227a42210d4412c526
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.6 MB (10570259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:203b64265b79fe03fb30f0fa6304031806d6723c72998e3de9c595668fafe9b8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 27 Aug 2021 19:39:54 GMT
ADD file:d213c56ffc24a5051e8060fd0fec1a0520367c10d88ab16321c36336b6c66098 in / 
# Fri, 27 Aug 2021 19:39:59 GMT
CMD ["/bin/sh"]
# Sat, 09 Oct 2021 00:20:35 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Sat, 09 Oct 2021 00:26:06 GMT
ENV HAPROXY_VERSION=2.4.7
# Sat, 09 Oct 2021 00:26:09 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.7.tar.gz
# Sat, 09 Oct 2021 00:26:11 GMT
ENV HAPROXY_SHA256=52af97f72f22ffd8a7a995fafc696291d37818feda50a23caef7dc0622421845
# Sat, 09 Oct 2021 00:26:57 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Sat, 09 Oct 2021 00:27:01 GMT
STOPSIGNAL SIGUSR1
# Sat, 09 Oct 2021 00:27:03 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 09 Oct 2021 00:27:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 09 Oct 2021 00:27:07 GMT
USER haproxy
# Sat, 09 Oct 2021 00:27:11 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:63da8ca98f7b4b94381aed56862a60aecf355d9428b9aeb7c61d5bd017100c18`  
		Last Modified: Fri, 27 Aug 2021 19:41:06 GMT  
		Size: 2.8 MB (2812284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2cb7f4863d3b35c18d80e77dc9d56f0070e7ef01a179431232eba634468aace`  
		Last Modified: Sat, 09 Oct 2021 00:56:52 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03f6c2e1ceee811c075982623f161e5df69404aca653368a0d8dbf4369a578e`  
		Last Modified: Sat, 09 Oct 2021 00:57:47 GMT  
		Size: 7.8 MB (7756238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1090a335e8fd7ba183bc8c208f5837beb8fe4a045efc694ee7bd06b4dc34c915`  
		Last Modified: Sat, 09 Oct 2021 00:57:45 GMT  
		Size: 450.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts-alpine3.14` - linux; s390x

```console
$ docker pull haproxy@sha256:5904315305b65757ebb6f0c68f7d86fae5ef1d4d72a45fbac6ac6976b74e8ef1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **10.0 MB (9962040 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7ee39cdd4aff65faf2154318380a6643e9efbfbb20b28bf373c8ea0ee253d96`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 27 Aug 2021 17:41:29 GMT
ADD file:9b40ee281e8797067fb2ae207c406084cb81593090338a8b7cb09ade52168daa in / 
# Fri, 27 Aug 2021 17:41:30 GMT
CMD ["/bin/sh"]
# Sat, 09 Oct 2021 00:42:13 GMT
RUN set -eux; 	addgroup --gid 99 --system haproxy; 	adduser 		--disabled-password 		--home /var/lib/haproxy 		--ingroup haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Wed, 03 Nov 2021 19:47:47 GMT
ENV HAPROXY_VERSION=2.4.8
# Wed, 03 Nov 2021 19:47:47 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.8.tar.gz
# Wed, 03 Nov 2021 19:47:48 GMT
ENV HAPROXY_SHA256=e3e4c1ad293bc25e8d8790cc5e45133213dda008bfd0228bf3077259b32ebaa5
# Wed, 03 Nov 2021 19:48:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gcc 		libc-dev 		linux-headers 		lua5.3-dev 		make 		openssl 		openssl-dev 		pcre2-dev 		readline-dev 		tar 	; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-musl 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 LUA_LIB=/usr/lib/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 		nproc="$(getconf _NPROCESSORS_ONLN)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .haproxy-rundeps $runDeps; 	apk del --no-network .build-deps; 		haproxy -v
# Wed, 03 Nov 2021 19:48:22 GMT
STOPSIGNAL SIGUSR1
# Wed, 03 Nov 2021 19:48:22 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 03 Nov 2021 19:48:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 Nov 2021 19:48:22 GMT
USER haproxy
# Wed, 03 Nov 2021 19:48:22 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:da14cb6b6dc946dbb2d84386bcaca84e2d46f650767cd11bdb3331ec9d623988`  
		Last Modified: Fri, 27 Aug 2021 17:42:25 GMT  
		Size: 2.6 MB (2603464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61599e3be6ec225e0618ca5f974f39e03242aeb50f3ef84f05fb52d087399fb1`  
		Last Modified: Sat, 09 Oct 2021 00:52:10 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3469b0102fe3c8718335a894c16389ba2dfde2a3ab20e5c215ac814968012656`  
		Last Modified: Wed, 03 Nov 2021 19:52:26 GMT  
		Size: 7.4 MB (7356847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb36e7eaeb41fb3db0c523972ab9081380f27e4acf7a683535370fc64efedb5a`  
		Last Modified: Wed, 03 Nov 2021 19:52:24 GMT  
		Size: 449.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
