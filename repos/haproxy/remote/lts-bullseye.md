## `haproxy:lts-bullseye`

```console
$ docker pull haproxy@sha256:c9892476376d981bd2d78be05c3e03bd3fe0b2f8e79cbfb4c9bdf18e8271643c
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

### `haproxy:lts-bullseye` - linux; amd64

```console
$ docker pull haproxy@sha256:0dd42da423947fb224d650898bfed099b44c7c4e54c256f540920bad8040ec26
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39452137 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fd0fa7940873ce6ab0d5d981399046f0238ebb422e9a4ed6ace5ff1c682740f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:58 GMT
ADD file:493a5b0c8d2d63a1343258b3f9aa5fcd59a93f44fe26ad9e56b094c3a08fd3be in / 
# Wed, 01 Mar 2023 04:09:59 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 06:56:57 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Mon, 20 Mar 2023 23:42:05 GMT
ENV HAPROXY_VERSION=2.6.11
# Mon, 20 Mar 2023 23:42:05 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.6/src/haproxy-2.6.11.tar.gz
# Mon, 20 Mar 2023 23:42:05 GMT
ENV HAPROXY_SHA256=e0bc430ac407747b077bc88ee6922b4616fa55a9e0f3ec84438dfb055eb9a715
# Mon, 20 Mar 2023 23:42:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Mon, 20 Mar 2023 23:42:37 GMT
STOPSIGNAL SIGUSR1
# Mon, 20 Mar 2023 23:42:37 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 20 Mar 2023 23:42:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 20 Mar 2023 23:42:37 GMT
USER haproxy
# Mon, 20 Mar 2023 23:42:37 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:3f9582a2cbe7197f39185419c0ced2c986389f8fc6aa805e1f5c090eea6511e0`  
		Last Modified: Wed, 01 Mar 2023 04:14:23 GMT  
		Size: 31.4 MB (31411403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f8f79fd20f85521bbd4aa3163a8b6961379938d4b5ac11dc310e2eb66dc54db`  
		Last Modified: Wed, 01 Mar 2023 07:02:59 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ab7c4518e55084f643fbd630add875e968cce8c0db2e874e2e8bb32a2503996`  
		Last Modified: Mon, 20 Mar 2023 23:46:14 GMT  
		Size: 8.0 MB (8038846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e3e77e2862adb88dc39b82da2d6d0b535fb990cd26cddf35af538b74c386b6f`  
		Last Modified: Mon, 20 Mar 2023 23:46:12 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts-bullseye` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:74666ff87ba0c8d0b6f3d726da9973ff8fbb914066037b1150971175cb2cd41f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.8 MB (36847422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3358718174e2be751d4403db3aace793414f2569f252c256957fc77d3e1154f7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 01 Mar 2023 01:48:54 GMT
ADD file:b4fb1081f6eb8a0560d56d5781bbcedaac1453615d56e0943245dca784785ea2 in / 
# Wed, 01 Mar 2023 01:48:54 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 03:05:00 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Tue, 21 Mar 2023 00:05:03 GMT
ENV HAPROXY_VERSION=2.6.11
# Tue, 21 Mar 2023 00:05:03 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.6/src/haproxy-2.6.11.tar.gz
# Tue, 21 Mar 2023 00:05:03 GMT
ENV HAPROXY_SHA256=e0bc430ac407747b077bc88ee6922b4616fa55a9e0f3ec84438dfb055eb9a715
# Tue, 21 Mar 2023 00:05:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Tue, 21 Mar 2023 00:05:32 GMT
STOPSIGNAL SIGUSR1
# Tue, 21 Mar 2023 00:05:32 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Tue, 21 Mar 2023 00:05:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Mar 2023 00:05:32 GMT
USER haproxy
# Tue, 21 Mar 2023 00:05:32 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:3c3af56dbec5913ef8aec0f1ca7112eb5914b4ad346ccd48f836dd7ec0621ba5`  
		Last Modified: Wed, 01 Mar 2023 01:52:57 GMT  
		Size: 28.9 MB (28915776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d4cdee50de2ae555704da915c88a6606c5520650a996dad6b31043b7b6ec27`  
		Last Modified: Wed, 01 Mar 2023 03:09:46 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac4b476a25bc28c09b52ef067b67424346d313a77a2699932a19f952a40ba52d`  
		Last Modified: Tue, 21 Mar 2023 00:13:50 GMT  
		Size: 7.9 MB (7929758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed11cc9961c24215e2dc7e872612355753adfd5611352f3e8dcbe95a3919546`  
		Last Modified: Tue, 21 Mar 2023 00:13:49 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts-bullseye` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:8a7652b9f428a75c44af7eb9fe2d50fc0f45df226e362a2189ade038c14d9d60
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.4 MB (34370485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c793d975bcc08da1c16412b4e37be6f360c6661718d4bfaa022fbc93a804bf3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 01 Mar 2023 01:57:55 GMT
ADD file:182fe91b8976a8871aba0d2ff9d4400a60317c8dec282261ba94247500c8d3dc in / 
# Wed, 01 Mar 2023 01:57:55 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 21:01:42 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Tue, 21 Mar 2023 00:54:35 GMT
ENV HAPROXY_VERSION=2.6.11
# Tue, 21 Mar 2023 00:54:35 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.6/src/haproxy-2.6.11.tar.gz
# Tue, 21 Mar 2023 00:54:35 GMT
ENV HAPROXY_SHA256=e0bc430ac407747b077bc88ee6922b4616fa55a9e0f3ec84438dfb055eb9a715
# Tue, 21 Mar 2023 00:55:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Tue, 21 Mar 2023 00:55:01 GMT
STOPSIGNAL SIGUSR1
# Tue, 21 Mar 2023 00:55:01 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Tue, 21 Mar 2023 00:55:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Mar 2023 00:55:01 GMT
USER haproxy
# Tue, 21 Mar 2023 00:55:01 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:b4770fcf2ef78c1e46693da734476bfaf03cbe1d0b6e0a0f22c2c2e53419e803`  
		Last Modified: Wed, 01 Mar 2023 02:03:02 GMT  
		Size: 26.6 MB (26577290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac653ccdf582fdad89ed0efa8b5ab7af8d74a3fc6228fd90f70d588829c11ab`  
		Last Modified: Wed, 01 Mar 2023 21:11:38 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d96fbdbddb1cbd9438b16b1fc80b1b0b3d5d8766181e159a1ac19bee71127da8`  
		Last Modified: Tue, 21 Mar 2023 00:57:30 GMT  
		Size: 7.8 MB (7791311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e452979649752a4517d994f1d10c9f75ac9476fba67f2a5e8533a0b19bc841`  
		Last Modified: Tue, 21 Mar 2023 00:57:29 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts-bullseye` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:3d0d847a643327fb592e3dbd1b2c4a8154a9a6311c5f4894b958b1b4aa2dce52
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.1 MB (38117128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:415cf82446336ee5e13990858eef313cda4e2fe6917fed1768245723232f95ff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:39 GMT
ADD file:9dc5c6fb6431df80107eddb76fb18256d6f4a06b4b22f9a7c4bcd58476068186 in / 
# Wed, 01 Mar 2023 02:20:39 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:32:19 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Mon, 20 Mar 2023 23:53:13 GMT
ENV HAPROXY_VERSION=2.6.11
# Mon, 20 Mar 2023 23:53:13 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.6/src/haproxy-2.6.11.tar.gz
# Mon, 20 Mar 2023 23:53:13 GMT
ENV HAPROXY_SHA256=e0bc430ac407747b077bc88ee6922b4616fa55a9e0f3ec84438dfb055eb9a715
# Mon, 20 Mar 2023 23:53:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Mon, 20 Mar 2023 23:53:37 GMT
STOPSIGNAL SIGUSR1
# Mon, 20 Mar 2023 23:53:37 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 20 Mar 2023 23:53:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 20 Mar 2023 23:53:37 GMT
USER haproxy
# Mon, 20 Mar 2023 23:53:37 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:66dbba0fb1b568cc3ffd53409ba2f9f82995ab7f80e379338f3f36e4dcd223be`  
		Last Modified: Wed, 01 Mar 2023 02:24:17 GMT  
		Size: 30.1 MB (30062814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a817596583607e51fe5d4edc34f9f272a460a21d5ff59a41314fac04047f3b5`  
		Last Modified: Wed, 01 Mar 2023 04:36:55 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04fb4ccc4f96ab50eb795ce7465b73ea43aebc6e861553134652c475a5b7dbb5`  
		Last Modified: Mon, 20 Mar 2023 23:56:52 GMT  
		Size: 8.1 MB (8052425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae535a92cd120bd1b168572ca3eaf1fb7b651539c6cd1a80650f82698ebffe7`  
		Last Modified: Mon, 20 Mar 2023 23:56:51 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts-bullseye` - linux; 386

```console
$ docker pull haproxy@sha256:ba8929cfe92ce2980e06c9421ed413424440827d533f7bfc8962c23f2e5a8e64
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40216029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe39a7d11a6ef99121c9266e6b637af035335c0889341b033745f322029b44d2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 01 Mar 2023 01:39:14 GMT
ADD file:7ff48f7b36d13400120a726cd394769a4c39e8424877f5b080aeb9da07eacebe in / 
# Wed, 01 Mar 2023 01:39:15 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:29:05 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Mon, 20 Mar 2023 23:50:57 GMT
ENV HAPROXY_VERSION=2.6.11
# Mon, 20 Mar 2023 23:50:57 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.6/src/haproxy-2.6.11.tar.gz
# Mon, 20 Mar 2023 23:50:57 GMT
ENV HAPROXY_SHA256=e0bc430ac407747b077bc88ee6922b4616fa55a9e0f3ec84438dfb055eb9a715
# Mon, 20 Mar 2023 23:51:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Mon, 20 Mar 2023 23:51:52 GMT
STOPSIGNAL SIGUSR1
# Mon, 20 Mar 2023 23:51:52 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 20 Mar 2023 23:51:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 20 Mar 2023 23:51:52 GMT
USER haproxy
# Mon, 20 Mar 2023 23:51:52 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:2b884ef8a2d2b7c2016a8d2926b5b284f2130128ee049cae31a2da609cda7257`  
		Last Modified: Wed, 01 Mar 2023 01:44:44 GMT  
		Size: 32.4 MB (32396138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5dfd81829d4f65db12577875af78f8f988da6aab4cd75f015c5a645221857b`  
		Last Modified: Wed, 01 Mar 2023 02:46:43 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dab819ebe7357b886bc24f69d7b5875a0ca1452a3be7da9b8e3bd9bbf1f11192`  
		Last Modified: Mon, 20 Mar 2023 23:58:38 GMT  
		Size: 7.8 MB (7818004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886149bc854ba54ff0a47cb7383d079339e456f4fd6634428c9f9c5064b95451`  
		Last Modified: Mon, 20 Mar 2023 23:58:37 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts-bullseye` - linux; mips64le

```console
$ docker pull haproxy@sha256:1e11c7da1746cec6c5776e78ad2b50f96b14ed5433b5da0f75d174b11e8d62f6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.8 MB (37791176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b16bf46c2dbb95095549f257f04d9e1d54646be2817537341b83f856dec57344`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 01 Mar 2023 02:10:54 GMT
ADD file:0bcd66a6a099cdb6e018ddc0f00270be93dccd3be6167ce36e9efc99c31549d9 in / 
# Wed, 01 Mar 2023 02:10:59 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 14:42:20 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Tue, 21 Mar 2023 00:27:19 GMT
ENV HAPROXY_VERSION=2.6.11
# Tue, 21 Mar 2023 00:27:22 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.6/src/haproxy-2.6.11.tar.gz
# Tue, 21 Mar 2023 00:27:24 GMT
ENV HAPROXY_SHA256=e0bc430ac407747b077bc88ee6922b4616fa55a9e0f3ec84438dfb055eb9a715
# Tue, 21 Mar 2023 00:30:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Tue, 21 Mar 2023 00:30:51 GMT
STOPSIGNAL SIGUSR1
# Tue, 21 Mar 2023 00:30:53 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Tue, 21 Mar 2023 00:30:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Mar 2023 00:30:58 GMT
USER haproxy
# Tue, 21 Mar 2023 00:31:00 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:89f6b45a7afd174bf0d443156831cacd9e6a26c834ad62610b6db53c731d257f`  
		Last Modified: Wed, 01 Mar 2023 02:18:50 GMT  
		Size: 29.6 MB (29634488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c918b7bec042cd347be0f0164c6f2eba5b49ad24cbdeac986e57694dd0d4bf`  
		Last Modified: Wed, 01 Mar 2023 15:05:54 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:522c5dcd942564fa1890c1480aee6bdfd0ef3f266fe4af88baf1f5b7bbd92f11`  
		Last Modified: Tue, 21 Mar 2023 00:35:54 GMT  
		Size: 8.2 MB (8154944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c3eb469a73867c24041d626f4a2ee8bb15b5dfa6d648b0aa041f4ac22824529`  
		Last Modified: Tue, 21 Mar 2023 00:35:49 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts-bullseye` - linux; ppc64le

```console
$ docker pull haproxy@sha256:e56c07773f292d0cf0aac65a7873e85ebd8a9a37562d85bcb0b2fb1429cfcaac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.7 MB (43733888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93622e48152f7b4a1f1c4e1680e307a12d816b2561cf4344c3c215af1d558547`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 01 Mar 2023 04:47:33 GMT
ADD file:6fdf0b2f8ea4be2d01e25a9d85db8f8c7e3b2a641c9c7665e34f4fad771815e0 in / 
# Wed, 01 Mar 2023 04:47:35 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 07:00:47 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Tue, 21 Mar 2023 00:58:16 GMT
ENV HAPROXY_VERSION=2.6.11
# Tue, 21 Mar 2023 00:58:16 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.6/src/haproxy-2.6.11.tar.gz
# Tue, 21 Mar 2023 00:58:16 GMT
ENV HAPROXY_SHA256=e0bc430ac407747b077bc88ee6922b4616fa55a9e0f3ec84438dfb055eb9a715
# Tue, 21 Mar 2023 00:59:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Tue, 21 Mar 2023 00:59:05 GMT
STOPSIGNAL SIGUSR1
# Tue, 21 Mar 2023 00:59:05 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Tue, 21 Mar 2023 00:59:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Mar 2023 00:59:05 GMT
USER haproxy
# Tue, 21 Mar 2023 00:59:06 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:93ab3a60c2a8cbc1150cb2bd54222db8b79c525c0243534a10d6294ef7ff83ac`  
		Last Modified: Wed, 01 Mar 2023 04:53:54 GMT  
		Size: 35.3 MB (35288103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:261d0def80093db35248b37b075c7e30289f41203906519855d2cc54e27946e8`  
		Last Modified: Wed, 01 Mar 2023 07:12:22 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56036e6cfd3e438012730b932f4318f2af42a598409d4d633d2ed127573df67c`  
		Last Modified: Tue, 21 Mar 2023 01:02:32 GMT  
		Size: 8.4 MB (8443892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4955ef0d9752b686e941a7917f40583f90a996f26883680b660cbd612e0dc162`  
		Last Modified: Tue, 21 Mar 2023 01:02:30 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts-bullseye` - linux; s390x

```console
$ docker pull haproxy@sha256:a6e7e6f4e5590fe6b09a822c4af16591436c10ac3a22eba87ef34f7073936ca2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.7 MB (37697329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22122746048c8dc9215f5a4d2230e21706e92ed8ed252dd99ae597cafc283474`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 01 Mar 2023 02:50:30 GMT
ADD file:01aa3de7444f0716938e0d85522be065193be4ffb6788b3190a0f4fefdbb8d65 in / 
# Wed, 01 Mar 2023 02:50:31 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:05:36 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Mon, 20 Mar 2023 23:58:22 GMT
ENV HAPROXY_VERSION=2.6.11
# Mon, 20 Mar 2023 23:58:22 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.6/src/haproxy-2.6.11.tar.gz
# Mon, 20 Mar 2023 23:58:22 GMT
ENV HAPROXY_SHA256=e0bc430ac407747b077bc88ee6922b4616fa55a9e0f3ec84438dfb055eb9a715
# Mon, 20 Mar 2023 23:58:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Mon, 20 Mar 2023 23:58:54 GMT
STOPSIGNAL SIGUSR1
# Mon, 20 Mar 2023 23:58:54 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 20 Mar 2023 23:58:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 20 Mar 2023 23:58:55 GMT
USER haproxy
# Mon, 20 Mar 2023 23:58:55 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:7b8d78f42e32e7fa234bcf890ae6603acab2881bca68a9d8c429981c7f42b1d6`  
		Last Modified: Wed, 01 Mar 2023 02:54:48 GMT  
		Size: 29.6 MB (29646854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3596b3a647ee326c568e21dd2eaa3996ce3fb324b541a0ae08e0e7fcd167623d`  
		Last Modified: Wed, 01 Mar 2023 04:11:51 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:942f9bb7a69df9ef5260433bc0eba259aa42500cf0e6a91f4fbdcd40dc2b9a59`  
		Last Modified: Tue, 21 Mar 2023 00:03:47 GMT  
		Size: 8.0 MB (8048578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fd3f67af88e62dba274a0b013af5576150f11a0e705cee12ac41f8e0d9a6c8`  
		Last Modified: Tue, 21 Mar 2023 00:03:45 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
