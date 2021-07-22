## `haproxy:lts`

```console
$ docker pull haproxy@sha256:0b604e2d9b0366e304d89393dd42651698bbbc2d588b65155b6aabaf4995ba00
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
$ docker pull haproxy@sha256:52aa1ec7d5d0b74f20d4e5c03c8f7561ead3db8931e0b733d6007b397a2d3880
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.3 MB (37295916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d784089a656dab7a82fd06ce515c7a5f2865055cc3d9422c8795a07300428f07`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 06:19:17 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 18:33:10 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 08 Jul 2021 18:33:10 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 08 Jul 2021 18:33:10 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 08 Jul 2021 18:34:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 08 Jul 2021 18:34:02 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 18:34:02 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 18:34:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 18:34:03 GMT
USER haproxy
# Thu, 08 Jul 2021 18:34:03 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91332cb81883405a321c1a2d2144bdd0aef8d1c69f90fdf0cf219982161b6e6e`  
		Last Modified: Wed, 23 Jun 2021 06:29:07 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6373e07bfb885e35a6bd53edfdc9040601b27fc0961fe6129588015b2096db20`  
		Last Modified: Thu, 08 Jul 2021 18:38:19 GMT  
		Size: 10.1 MB (10148233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a5b51f2be69ce74243979e96aaae4a74e55466e342bcd0bb697a2b1e62d59b`  
		Last Modified: Thu, 08 Jul 2021 18:38:18 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:2f24bc20c43df5eb2b7e5ffc0e95674782b29896f65a1226bc2adff0b3d68e0a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34665575 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed1196ca984d9efa3ec3c4f779f012f0662a9586517f0c0e041612416ff4fbc8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 22 Jun 2021 23:50:09 GMT
ADD file:78d4ced31112d85490c684f350aceeebfc72a804262c7ad3e033257e3894f5c4 in / 
# Tue, 22 Jun 2021 23:50:11 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:15:11 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 18:58:15 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 08 Jul 2021 18:58:16 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 08 Jul 2021 18:58:16 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 08 Jul 2021 18:59:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 08 Jul 2021 18:59:09 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 18:59:10 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 18:59:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 18:59:10 GMT
USER haproxy
# Thu, 08 Jul 2021 18:59:11 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:532d6df30af5174ac6e1b379c32b8f464d44651ac060376a560c4a76a87704a7`  
		Last Modified: Wed, 23 Jun 2021 00:01:46 GMT  
		Size: 24.9 MB (24878945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48649e3d7de4cd80d3a9a34c725a2935be904ff90e99ea6c8e4bb6e1e7a4eeb7`  
		Last Modified: Wed, 23 Jun 2021 05:24:11 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ee3e06cb1904b6bc00db8565860713531b542e6ef7389f534e96705484113d`  
		Last Modified: Thu, 08 Jul 2021 19:02:21 GMT  
		Size: 9.8 MB (9784805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b6869880a0636c536ab6434a503f73fbe4faa5d871d3ae25f498d9995adc0f3`  
		Last Modified: Thu, 08 Jul 2021 19:02:15 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:7b6339c2dff4e7a1d7bbb7c72bc74cf2072bf95ff20841bd1c3392db483209b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.4 MB (32372088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9405b9497ca1234f5dd526dab824511329f7053f2f2b6766f2a64e2c9734d7bb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:31 GMT
ADD file:8d200a3bbe985ff355343675c5555852f27550a9e367969df6bc98034efb8fd4 in / 
# Wed, 23 Jun 2021 00:20:31 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:21:41 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 21:28:35 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 08 Jul 2021 21:28:36 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 08 Jul 2021 21:28:37 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 08 Jul 2021 21:29:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 08 Jul 2021 21:29:24 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 21:29:25 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 21:29:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 21:29:26 GMT
USER haproxy
# Thu, 08 Jul 2021 21:29:26 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:8452be1adf00f91570fe21a8e61aaf4c12e014daf67d7de65d984f4e8ecca2f1`  
		Last Modified: Wed, 23 Jun 2021 00:31:49 GMT  
		Size: 22.7 MB (22746055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed1c9c92d0076fd4bf40503e3f47102509a5b99d182f4dd9e81e64d0a7e0b8a`  
		Last Modified: Wed, 23 Jun 2021 05:35:48 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b090e05bfe544bc62f527dcf70dd8799d4180499bcedf6d5a8ffa14c7a75b31d`  
		Last Modified: Thu, 08 Jul 2021 21:35:57 GMT  
		Size: 9.6 MB (9624206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9cdb9eefea684230e2e659f2753469d8df08683a747d1a8d95dc6da0954cb60`  
		Last Modified: Thu, 08 Jul 2021 21:35:52 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:ecddae360d89e478a3ca8575fe6902f41f5bce6d136ffa9d002979696533aed9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35942280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b004550c7f1e6363193435537a32221dc4e6ce0bb68cea61b3c97378b6362064`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:40 GMT
ADD file:beee00b59da720f68e12e2ba2a8134207c80c777ddb4ceb03c71e3e4c3f51c93 in / 
# Tue, 22 Jun 2021 23:49:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 03:19:31 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 19:01:35 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 08 Jul 2021 19:01:35 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 08 Jul 2021 19:01:35 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 08 Jul 2021 19:02:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 08 Jul 2021 19:02:18 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 19:02:18 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 19:02:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 19:02:18 GMT
USER haproxy
# Thu, 08 Jul 2021 19:02:18 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:448f6bf000e31217a7c202c659b03b7f8ac8d3ae6b03ef7a2f8339be2f00ff4a`  
		Last Modified: Tue, 22 Jun 2021 23:55:25 GMT  
		Size: 25.9 MB (25914993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b05ad81dc8a7d67656235988f0e5fb72c374c7d8df44c105b91d712e06c4ac`  
		Last Modified: Wed, 23 Jun 2021 03:26:16 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076876a81ee03b4e5250b7a31318f330ccf4ea3eeef84cecafdc1a92b4803062`  
		Last Modified: Thu, 08 Jul 2021 19:07:11 GMT  
		Size: 10.0 MB (10025457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:277cf44e1cd25ac34ef95ef8bc0084be15c5d80b5fd94d6b8ba385807423dce0`  
		Last Modified: Thu, 08 Jul 2021 19:07:08 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; 386

```console
$ docker pull haproxy@sha256:ef1c5085a09fe3d0028e256643a9453a2b853f34cf360c895fdc418095a9525a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.8 MB (37792502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87c94a82fd63b1e3cbd90c3cca2b24076d38dcdfd88fc0b5f9367719bd84cbdd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 22 Jun 2021 23:39:35 GMT
ADD file:48f656ac6733911048b3de850490438d0233b3badc11861fca62062d4edfaf40 in / 
# Tue, 22 Jun 2021 23:39:35 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:23:13 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 08 Jul 2021 19:01:56 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 08 Jul 2021 19:01:56 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 08 Jul 2021 19:01:56 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 08 Jul 2021 19:02:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 08 Jul 2021 19:02:57 GMT
STOPSIGNAL SIGUSR1
# Thu, 08 Jul 2021 19:02:57 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 08 Jul 2021 19:02:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Jul 2021 19:02:58 GMT
USER haproxy
# Thu, 08 Jul 2021 19:02:58 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:33af2dcb865e65d53cdeb843b67a0ef62151fa32df292293e7c6b0eb728ac5ac`  
		Last Modified: Tue, 22 Jun 2021 23:46:23 GMT  
		Size: 27.8 MB (27797411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a6e4d42b23996eb7d8a1baa85ee19828c2667fd4a2dca6eb1040b266680e9f`  
		Last Modified: Wed, 23 Jun 2021 00:32:00 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c640aece6fea8db01bc9744204c373af3285d4d3b15911631fdc1508b30fe28f`  
		Last Modified: Thu, 08 Jul 2021 19:08:39 GMT  
		Size: 10.0 MB (9993262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e1e627dabfcf736ac7f517f394391e6eeb0fa52347a5f92cee7310d00c35fac`  
		Last Modified: Thu, 08 Jul 2021 19:08:38 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; mips64le

```console
$ docker pull haproxy@sha256:0831d16085b3616dd56baae5d2b16911f5df76ff3643f6ed0cc9206bcdd1b0ef
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.6 MB (35582649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a67c72bc16cd3442d99818a1691f620bb8fba803aa322938bf1f76185d160ae9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 22 Jul 2021 00:09:45 GMT
ADD file:1f77b9001c4977ba733be674fc5eb4b85130f1dea8a7b39d545b70f9c107695f in / 
# Thu, 22 Jul 2021 00:09:46 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:07:49 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 22 Jul 2021 01:10:29 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 22 Jul 2021 01:10:29 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 22 Jul 2021 01:10:30 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 22 Jul 2021 01:12:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 22 Jul 2021 01:12:58 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 01:12:58 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 01:12:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 01:12:59 GMT
USER haproxy
# Thu, 22 Jul 2021 01:12:59 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:99ee621d0b0485e9de65aa19604aa2453d19ea7fc86b22c5b77c1bab74e3cb42`  
		Last Modified: Thu, 22 Jul 2021 00:16:11 GMT  
		Size: 25.8 MB (25812771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f444627794f98947a9df95ec5d19b2a1cd6c151ed438982b1dc0b89f5eaf19e`  
		Last Modified: Thu, 22 Jul 2021 01:24:39 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529ec01a3a5cb58c3aa92432192c7025a9df5ac852a7e1606269d172da56dd54`  
		Last Modified: Thu, 22 Jul 2021 01:25:03 GMT  
		Size: 9.8 MB (9768048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0dc46dbff91be84b369de7651cd4d1d725a03b3d65bfef0a41478894b38fe2`  
		Last Modified: Thu, 22 Jul 2021 01:24:56 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; ppc64le

```console
$ docker pull haproxy@sha256:0265c0700be024578a661ef439408b91cfa73fef6b763a58ddad4d78fdbc51db
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.2 MB (41213069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae16a408d428d4d0a7ed8262d6b984676689a578932f9ff1a168c726b85fb6e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 22 Jul 2021 00:19:04 GMT
ADD file:3a6bd6ce3eff98b88a13de5d0f26cff0b026f876674204dbad6f84fafcf145b1 in / 
# Thu, 22 Jul 2021 00:19:13 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 02:52:46 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 22 Jul 2021 02:59:40 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 22 Jul 2021 02:59:52 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 22 Jul 2021 03:00:03 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 22 Jul 2021 03:03:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 22 Jul 2021 03:03:39 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 03:03:41 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 03:03:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 03:03:48 GMT
USER haproxy
# Thu, 22 Jul 2021 03:03:52 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:1130517d52da84a09f9465006bddab5e49afd398860890eab6274fd0bff32371`  
		Last Modified: Thu, 22 Jul 2021 00:27:49 GMT  
		Size: 30.6 MB (30553709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251bf3fe1d4bbe9c27e393cd8ddc550b56cec90eb916bf9bec24d657c9f6556f`  
		Last Modified: Thu, 22 Jul 2021 03:40:01 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f4b7133364510c1fc0f847a528a441235df0500c39d8318c3557708a9ea74fa`  
		Last Modified: Thu, 22 Jul 2021 03:40:33 GMT  
		Size: 10.7 MB (10657533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1244f9b6844b16203e11b9ed8754bed5a0289f1a3b6bd59d295e18b9fca91bc`  
		Last Modified: Thu, 22 Jul 2021 03:40:30 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; s390x

```console
$ docker pull haproxy@sha256:2f711e846e54ca0e3063a51b841c4291dc0a07925552f9feab60e56ceeb54a8b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.6 MB (35587765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:123ac19f2aeb23d953a63211cc6c840f267890f19ee5a8db61abaed33280a5b5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Thu, 22 Jul 2021 00:42:45 GMT
ADD file:1ab999eb6f80d8ce91ce3a173e23fd2710f2779117bba29037eaa82aadcbf6ed in / 
# Thu, 22 Jul 2021 00:42:48 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:30:19 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy
# Thu, 22 Jul 2021 01:31:40 GMT
ENV HAPROXY_VERSION=2.4.2
# Thu, 22 Jul 2021 01:31:40 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.2.tar.gz
# Thu, 22 Jul 2021 01:31:40 GMT
ENV HAPROXY_SHA256=edf9788f7f3411498e3d7b21777036b4dc14183e95c8e2ce7577baa0ea4ea2aa
# Thu, 22 Jul 2021 01:32:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 22 Jul 2021 01:32:21 GMT
STOPSIGNAL SIGUSR1
# Thu, 22 Jul 2021 01:32:21 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 22 Jul 2021 01:32:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Jul 2021 01:32:22 GMT
USER haproxy
# Thu, 22 Jul 2021 01:32:22 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:7a50fdd85ff244c1465e71c51354d055e3df0b90ff5faad28cc22d9ecde9daf3`  
		Last Modified: Thu, 22 Jul 2021 00:48:13 GMT  
		Size: 25.8 MB (25760761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05fb34d1ed21b67502665114a7ae60445472fc7bafa620bbf6c79b7df85a01d4`  
		Last Modified: Thu, 22 Jul 2021 01:39:54 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509cd29cce72fe3b56df141c72bd9ac7c85aafc2da6d1596ec7e29ef8e10db0f`  
		Last Modified: Thu, 22 Jul 2021 01:40:05 GMT  
		Size: 9.8 MB (9825173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b04c9d12d457a528c260ddcaaecc8d44f66fb72fb0a54770d3011ba16f8433`  
		Last Modified: Thu, 22 Jul 2021 01:40:04 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
