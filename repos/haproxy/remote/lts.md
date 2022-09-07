## `haproxy:lts`

```console
$ docker pull haproxy@sha256:22148fc702410d4a6ec3f802db1d559205466dc4bb0d9b5fcff200ce5c67b6ff
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
$ docker pull haproxy@sha256:2a2380c698fcd4cf36c67ee718514d4d96f2dc26eeca64a624b9f3e94657b8fb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.4 MB (39369610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aeca1769e9d572682e4e29a564a28f389668646982d0f198d6af1651d386535b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:42:20 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Tue, 23 Aug 2022 02:43:02 GMT
ENV HAPROXY_VERSION=2.6.4
# Tue, 23 Aug 2022 02:43:02 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.6/src/haproxy-2.6.4.tar.gz
# Tue, 23 Aug 2022 02:43:03 GMT
ENV HAPROXY_SHA256=f07d67ada2ff3a999fed4e34459c0489536331a549665ac90cb6a8df91f4a289
# Tue, 23 Aug 2022 02:43:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Tue, 23 Aug 2022 02:43:36 GMT
STOPSIGNAL SIGUSR1
# Tue, 23 Aug 2022 02:43:36 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Tue, 23 Aug 2022 02:43:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 Aug 2022 02:43:36 GMT
USER haproxy
# Tue, 23 Aug 2022 02:43:36 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f0bdc50f17a71122f59ebfede271ed6c0e711cf6625b717e21eeb110e693e7e`  
		Last Modified: Tue, 23 Aug 2022 02:48:05 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29483803b38accf49bc44053069a078d070ac80c641b07743235d7d9ce8ec697`  
		Last Modified: Tue, 23 Aug 2022 02:48:22 GMT  
		Size: 8.0 MB (7986236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:624a7a879e60e13828e0a9c76794162cfcfe3924bc3a7e1c0372879dec4e6873`  
		Last Modified: Tue, 23 Aug 2022 02:48:21 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:8feeee80dbcaff58810eadbbd85837d524082424de8fb775f32cd8e71bb4bbde
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.8 MB (36807485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e29b14b289832c7099a66c964d8cd92c2c09f9b36f321ffe8b1600a679bebc93`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 23 Aug 2022 01:17:14 GMT
ADD file:83fb076a50e935419eb0db2bd97477d7ed5f16aaac4c8cc35a4a69ac612df327 in / 
# Tue, 23 Aug 2022 01:17:14 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 10:17:53 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Wed, 07 Sep 2022 19:49:45 GMT
ENV HAPROXY_VERSION=2.6.5
# Wed, 07 Sep 2022 19:49:45 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.6/src/haproxy-2.6.5.tar.gz
# Wed, 07 Sep 2022 19:49:45 GMT
ENV HAPROXY_SHA256=ce9e19ebfcdd43e51af8a6090f1df8d512d972ddf742fa648a643bbb19056605
# Wed, 07 Sep 2022 19:51:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 07 Sep 2022 19:51:28 GMT
STOPSIGNAL SIGUSR1
# Wed, 07 Sep 2022 19:51:28 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 07 Sep 2022 19:51:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Sep 2022 19:51:28 GMT
USER haproxy
# Wed, 07 Sep 2022 19:51:28 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:74eb5afab626122970f8620ac001fcc4a200725acb05519b85aba47a38bf1016`  
		Last Modified: Tue, 23 Aug 2022 01:22:44 GMT  
		Size: 28.9 MB (28917250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d6064050485adfecd7d2172356fd43bc9903af9230769bc5ca6fa804867161`  
		Last Modified: Tue, 23 Aug 2022 10:26:40 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7401e1548a07832e48afd43ff6f51271ecb61293168dbe60c85424fdbfdd0c02`  
		Last Modified: Wed, 07 Sep 2022 19:53:17 GMT  
		Size: 7.9 MB (7888350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c785d2057824faeb1015386e9806e77c7a829b0315a8cdbfa658c909b8d4aa0b`  
		Last Modified: Wed, 07 Sep 2022 19:53:15 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:eb7836d4b8f906f50ad1a9a900ce8a626d31d45e8459358a3dd5a0b6bbadfbfa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34316988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b418e4330c3a7dadfe6ce9084edca7a4412cc08e19983a0231868dcec7fd4e6c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 23 Aug 2022 01:43:01 GMT
ADD file:4cd1b4287674228db28402a76aa4f241740585448be48b5b15068d275ee9eb84 in / 
# Tue, 23 Aug 2022 01:43:01 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 17:26:21 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Tue, 23 Aug 2022 17:28:36 GMT
ENV HAPROXY_VERSION=2.6.4
# Tue, 23 Aug 2022 17:28:36 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.6/src/haproxy-2.6.4.tar.gz
# Tue, 23 Aug 2022 17:28:36 GMT
ENV HAPROXY_SHA256=f07d67ada2ff3a999fed4e34459c0489536331a549665ac90cb6a8df91f4a289
# Tue, 23 Aug 2022 17:30:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Tue, 23 Aug 2022 17:30:29 GMT
STOPSIGNAL SIGUSR1
# Tue, 23 Aug 2022 17:30:29 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Tue, 23 Aug 2022 17:30:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 Aug 2022 17:30:30 GMT
USER haproxy
# Tue, 23 Aug 2022 17:30:30 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:051ba72559abd0cf65b34b75605580f58636ec3cb994f97de317632a85d82761`  
		Last Modified: Tue, 23 Aug 2022 01:50:05 GMT  
		Size: 26.6 MB (26571732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1891a9c3c6b13a17b2bcefa8cd589d2b24a5a5d93cebf6fc59d93b4d1e811a48`  
		Last Modified: Tue, 23 Aug 2022 17:43:55 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e2999eaee891381f01eb00ca95cde590cdc30a3129194c392b364450613fc6e`  
		Last Modified: Tue, 23 Aug 2022 17:44:30 GMT  
		Size: 7.7 MB (7743371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc9b8ef9c0acd753dc34ed59dde61a43cff372d310a066c7d6486ab4f51dd01`  
		Last Modified: Tue, 23 Aug 2022 17:44:28 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:15b930c31f45fbbf03d361f635f840a87c0c764ff2a66a9dceb5fef31838cacd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.1 MB (38066888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d757dbf327ad17d701a408173c7bcf136f7e2e2d2f19aaa1cde8562f941bd040`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 12:51:34 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Wed, 07 Sep 2022 19:59:51 GMT
ENV HAPROXY_VERSION=2.6.5
# Wed, 07 Sep 2022 19:59:52 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.6/src/haproxy-2.6.5.tar.gz
# Wed, 07 Sep 2022 19:59:53 GMT
ENV HAPROXY_SHA256=ce9e19ebfcdd43e51af8a6090f1df8d512d972ddf742fa648a643bbb19056605
# Wed, 07 Sep 2022 20:00:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 07 Sep 2022 20:00:21 GMT
STOPSIGNAL SIGUSR1
# Wed, 07 Sep 2022 20:00:23 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 07 Sep 2022 20:00:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Sep 2022 20:00:24 GMT
USER haproxy
# Wed, 07 Sep 2022 20:00:25 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0da65b843aa2c627fa0f13b6992646c25657e03c89432c4433e1430ca4d6bb00`  
		Last Modified: Tue, 23 Aug 2022 12:59:03 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5772bf4206239ebbdf0aca1b21453daf4e3f14a7fb15634e45cd8dd409d00d9`  
		Last Modified: Wed, 07 Sep 2022 20:04:36 GMT  
		Size: 8.0 MB (8001358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:816c9dc5660bd61a33a93d8bddbb001650f4ac80e1becc1e4443bbb3917ee31b`  
		Last Modified: Wed, 07 Sep 2022 20:04:34 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; 386

```console
$ docker pull haproxy@sha256:97dd6d39a800e15e1d6add403ea50d8a6d8fc97cc414de0fdc99e1413bf2ff4f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40158824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f0cc80b3943ef7b4dfc0ed017b2b9d66950384c4da701c8058b9ac81f1c6fc5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 23 Aug 2022 01:02:40 GMT
ADD file:5ca62c98116941aaa64ec72afb689a088c46f75a3e83d5b0d4e58d65ec905ccd in / 
# Tue, 23 Aug 2022 01:02:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:06:50 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Wed, 07 Sep 2022 19:45:03 GMT
ENV HAPROXY_VERSION=2.6.5
# Wed, 07 Sep 2022 19:45:04 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.6/src/haproxy-2.6.5.tar.gz
# Wed, 07 Sep 2022 19:45:05 GMT
ENV HAPROXY_SHA256=ce9e19ebfcdd43e51af8a6090f1df8d512d972ddf742fa648a643bbb19056605
# Wed, 07 Sep 2022 19:45:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 07 Sep 2022 19:45:39 GMT
STOPSIGNAL SIGUSR1
# Wed, 07 Sep 2022 19:45:41 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 07 Sep 2022 19:45:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Sep 2022 19:45:42 GMT
USER haproxy
# Wed, 07 Sep 2022 19:45:43 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:6b3cb4a05a891d9d8a87a2bd7247b16f79832a9d4afbad3ff5068f6fc2ba1560`  
		Last Modified: Tue, 23 Aug 2022 01:08:25 GMT  
		Size: 32.4 MB (32387317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ec3212ecd546048965b80c98e469cdfba40f8cc9cbdc615c429566fc4408f2`  
		Last Modified: Tue, 23 Aug 2022 03:15:04 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0977581c75aebf5b7ab3a0b51cae8c804ae2a306760f5c66dfdaa377c649379`  
		Last Modified: Wed, 07 Sep 2022 19:50:10 GMT  
		Size: 7.8 MB (7769761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff386ca7e1f36c207b3a84416790e7db436ea4b133eb7006c46e3b31c0785c56`  
		Last Modified: Wed, 07 Sep 2022 19:50:09 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; mips64le

```console
$ docker pull haproxy@sha256:e5411fe1e9f111ce3f8e9dc69f151391a10a1ee3feb761f038af58d995313443
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.7 MB (37744131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf5a4aa3cca6695d387552f45e4a865c20e7ac68b35d7d3e35c94200de702619`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 23 Aug 2022 00:11:17 GMT
ADD file:37d58e8a76488fed0f1ebafd3ee993569a3c611b3a5d93400485783112b71386 in / 
# Tue, 23 Aug 2022 00:11:22 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:40:26 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Tue, 23 Aug 2022 00:44:23 GMT
ENV HAPROXY_VERSION=2.6.4
# Tue, 23 Aug 2022 00:44:25 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.6/src/haproxy-2.6.4.tar.gz
# Tue, 23 Aug 2022 00:44:28 GMT
ENV HAPROXY_SHA256=f07d67ada2ff3a999fed4e34459c0489536331a549665ac90cb6a8df91f4a289
# Tue, 23 Aug 2022 00:47:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Tue, 23 Aug 2022 00:47:50 GMT
STOPSIGNAL SIGUSR1
# Tue, 23 Aug 2022 00:47:52 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Tue, 23 Aug 2022 00:47:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 Aug 2022 00:47:57 GMT
USER haproxy
# Tue, 23 Aug 2022 00:47:59 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:0e8d4fbcc8d2fc93de0170727f6e48b6fc7ec8931443fbda8a8cd154dc6f7d36`  
		Last Modified: Tue, 23 Aug 2022 00:19:35 GMT  
		Size: 29.6 MB (29639012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4f7b39531cea15882f044ccec63accc32985c2231f07d11866cbcab4328fe6`  
		Last Modified: Tue, 23 Aug 2022 01:00:11 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ec7501cb207bae5ad640e247eda8d282c28b6fec1e58d692a2aa8ca7fb34de`  
		Last Modified: Tue, 23 Aug 2022 01:00:37 GMT  
		Size: 8.1 MB (8103368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ea9bfeb4b972d4a6a84bfed97ac276c584ae192ad7a44251fba157491041dbb`  
		Last Modified: Tue, 23 Aug 2022 01:00:31 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; ppc64le

```console
$ docker pull haproxy@sha256:840aafb02677163ccd2d442ff7465dcbb9ca217aba64dd7d954b0f1a01b3c1ad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.7 MB (43672786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04be90821c6633e5fa3e9389735dabf76639853f0f20a501dacdb977261ad4f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 23 Aug 2022 01:24:52 GMT
ADD file:d35213360d726a18e220276d33f245115c3e94a321addaa4c9127488368b0203 in / 
# Tue, 23 Aug 2022 01:24:54 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:15:55 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Tue, 23 Aug 2022 02:16:59 GMT
ENV HAPROXY_VERSION=2.6.4
# Tue, 23 Aug 2022 02:16:59 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.6/src/haproxy-2.6.4.tar.gz
# Tue, 23 Aug 2022 02:17:00 GMT
ENV HAPROXY_SHA256=f07d67ada2ff3a999fed4e34459c0489536331a549665ac90cb6a8df91f4a289
# Tue, 23 Aug 2022 02:17:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Tue, 23 Aug 2022 02:17:45 GMT
STOPSIGNAL SIGUSR1
# Tue, 23 Aug 2022 02:17:45 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Tue, 23 Aug 2022 02:17:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 Aug 2022 02:17:46 GMT
USER haproxy
# Tue, 23 Aug 2022 02:17:46 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:698954eda09d38dd1ccc9ce777b1f6bc7f7473fc6c4c3eb634acc8d035a42eae`  
		Last Modified: Tue, 23 Aug 2022 01:30:36 GMT  
		Size: 35.3 MB (35284280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:293c33ae226ef8fddafb119fce3d663a17dad2b98196d676cfc1b247a93cb4bf`  
		Last Modified: Tue, 23 Aug 2022 02:23:48 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0f6a0068d23bcde196559f7d8f836e6623100c8a0e00afa2de23ee827f08b3`  
		Last Modified: Tue, 23 Aug 2022 02:24:15 GMT  
		Size: 8.4 MB (8386618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b26bab886e458c0d79cb29a2e3927a36b0d0880803bb00f813a78960b75326c4`  
		Last Modified: Tue, 23 Aug 2022 02:24:13 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; s390x

```console
$ docker pull haproxy@sha256:3a7eaefc4d8038300c89d2a9052f843691c037b2f8f8637a12f969854c87559e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.7 MB (37651235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d0ef64682645c8fe79f3e5e5bffda0545b482e96e39d04f7836697a289a8a93`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 23 Aug 2022 00:54:01 GMT
ADD file:7e494cf2e639edf0f0ce27e06887b8488570da37c5fce0a889687622d8cd443e in / 
# Tue, 23 Aug 2022 00:54:03 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 10:02:55 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Wed, 07 Sep 2022 19:53:05 GMT
ENV HAPROXY_VERSION=2.6.5
# Wed, 07 Sep 2022 19:53:05 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.6/src/haproxy-2.6.5.tar.gz
# Wed, 07 Sep 2022 19:53:05 GMT
ENV HAPROXY_SHA256=ce9e19ebfcdd43e51af8a6090f1df8d512d972ddf742fa648a643bbb19056605
# Wed, 07 Sep 2022 19:53:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 07 Sep 2022 19:53:33 GMT
STOPSIGNAL SIGUSR1
# Wed, 07 Sep 2022 19:53:33 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 07 Sep 2022 19:53:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 07 Sep 2022 19:53:33 GMT
USER haproxy
# Wed, 07 Sep 2022 19:53:34 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:1c2e5a5a3305e50395bba8974e6c201849f83c07fb0ad036111055f59157c7ff`  
		Last Modified: Tue, 23 Aug 2022 01:04:36 GMT  
		Size: 29.7 MB (29650094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1b011d7778a4af3d0878673e3591d4db6e49968668a8c858e5b43678163db90`  
		Last Modified: Tue, 23 Aug 2022 10:09:14 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97c828defd90815f2dc38b33fadc10ce7f5954d325d2b5f8df105291ec92ba36`  
		Last Modified: Wed, 07 Sep 2022 19:57:24 GMT  
		Size: 8.0 MB (7999256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d06563efdac2425aa1fc199edb055f11db508cd0484c8101a7bcf07c8d7845`  
		Last Modified: Wed, 07 Sep 2022 19:57:23 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
