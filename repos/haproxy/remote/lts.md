## `haproxy:lts`

```console
$ docker pull haproxy@sha256:d14e90aec71a44279025e95a4d199436786c3c66c327c0c976dcd389ea15eb48
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
$ docker pull haproxy@sha256:bcca123130d7c23498cf1cd7062f6c34ed98e5aa48c1a3e2f20b3f432dd43a11
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.5 MB (44533947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff19db9c7173b43433cc30e361c4597361bb0b2ffe501f4b416007e6b9c470fc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:38:07 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Tue, 02 May 2023 18:31:16 GMT
ENV HAPROXY_VERSION=2.6.13
# Tue, 02 May 2023 18:31:16 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.6/src/haproxy-2.6.13.tar.gz
# Tue, 02 May 2023 18:31:16 GMT
ENV HAPROXY_SHA256=d69ff5233dbca657132ef280d111222ec1e33f5be1c1937d4e9ff516f63f5243
# Tue, 02 May 2023 18:31:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Tue, 02 May 2023 18:31:50 GMT
STOPSIGNAL SIGUSR1
# Tue, 02 May 2023 18:31:50 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Tue, 02 May 2023 18:31:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 May 2023 18:31:50 GMT
USER haproxy
# Tue, 02 May 2023 18:31:50 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc6f2b5b570ac8cb5b797ab7a36ffcfa9d5c278d45b764607f37d590de4a04f`  
		Last Modified: Wed, 12 Apr 2023 01:43:29 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:941d84d830e99886e83310a9c1845d13ed6129ef52ecdb67afcf7e87e5c3158d`  
		Last Modified: Tue, 02 May 2023 18:35:26 GMT  
		Size: 13.1 MB (13113829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1526e9ff2151360c68d0fb39f7821801033e36fa1ba5742c9f26c53bc67f1fc`  
		Last Modified: Tue, 02 May 2023 18:35:22 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:da496774a60ca312b5f73cbbe39a387e0806f4a0cf142567396c46086c20f32e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.9 MB (36851662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77972008013d17cb90ad2ac32d3f0579d9ed793e831b14737d6bdd7a7827bca7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 02 May 2023 22:48:53 GMT
ADD file:ca82c0d9094c1022a00b5f2157a02e1a9032aafc357a41c76c6b60bd74d25395 in / 
# Tue, 02 May 2023 22:48:53 GMT
CMD ["bash"]
# Wed, 03 May 2023 08:59:54 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Wed, 03 May 2023 09:01:13 GMT
ENV HAPROXY_VERSION=2.6.13
# Wed, 03 May 2023 09:01:14 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.6/src/haproxy-2.6.13.tar.gz
# Wed, 03 May 2023 09:01:14 GMT
ENV HAPROXY_SHA256=d69ff5233dbca657132ef280d111222ec1e33f5be1c1937d4e9ff516f63f5243
# Wed, 03 May 2023 09:01:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 03 May 2023 09:01:44 GMT
STOPSIGNAL SIGUSR1
# Wed, 03 May 2023 09:01:44 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 03 May 2023 09:01:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 May 2023 09:01:45 GMT
USER haproxy
# Wed, 03 May 2023 09:01:45 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:eb6ee5d3f82142e70aca665cea92048b1a46ff1aa5c5be47a04c27a471470c07`  
		Last Modified: Tue, 02 May 2023 22:51:25 GMT  
		Size: 28.9 MB (28903418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da417f762af8426d1f4e7224ccffe481c6619d696bec1f4ee9d3527ff87b1d0e`  
		Last Modified: Wed, 03 May 2023 09:03:41 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcd8cccff45e8bc149bdb48f4462438bb70a2912c9175ed0a2b6d87edfda1393`  
		Last Modified: Wed, 03 May 2023 09:04:14 GMT  
		Size: 7.9 MB (7946360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea3d68c2e3999415fa1d778293559e3707b51fb392f59fa41e33160cc857bb0a`  
		Last Modified: Wed, 03 May 2023 09:04:12 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:7a34cb2e0b2c7a97e29709ab346a6b5f3e54a9903f79ef135a9096f467fc6244
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.3 MB (38294068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cd8e17d6b7c0bb8568c778d63e488618c9b9e37e3ddeca6cfb96b8ddf267503`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 11 Apr 2023 23:59:44 GMT
ADD file:e5f4777456ed4424053e9aa1f3d783f57da094c7a6c6d9d7a2fd315e00b5bbb0 in / 
# Tue, 11 Apr 2023 23:59:44 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:19:56 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Tue, 02 May 2023 19:36:41 GMT
ENV HAPROXY_VERSION=2.6.13
# Tue, 02 May 2023 19:36:41 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.6/src/haproxy-2.6.13.tar.gz
# Tue, 02 May 2023 19:36:41 GMT
ENV HAPROXY_SHA256=d69ff5233dbca657132ef280d111222ec1e33f5be1c1937d4e9ff516f63f5243
# Tue, 02 May 2023 19:37:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Tue, 02 May 2023 19:37:10 GMT
STOPSIGNAL SIGUSR1
# Tue, 02 May 2023 19:37:10 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Tue, 02 May 2023 19:37:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 May 2023 19:37:10 GMT
USER haproxy
# Tue, 02 May 2023 19:37:10 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:99c2a28b4a43ce341eb611e82106b886315f30a250473617f2293828e10d8fff`  
		Last Modified: Wed, 12 Apr 2023 00:03:19 GMT  
		Size: 26.6 MB (26579772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43535115d5b5c81980891656e7d0045e4b5b6d344f658d15e2401c30ceffc9af`  
		Last Modified: Wed, 12 Apr 2023 00:24:45 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4898e395afa8b4e474eba1059d1aa30242e2349329aee25d1aacb331b6b14c57`  
		Last Modified: Tue, 02 May 2023 19:40:10 GMT  
		Size: 11.7 MB (11712412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c04c7e06a09a52eb9b737b446f0eb06db4be4ef32cd27cd22bd841955b9c137`  
		Last Modified: Tue, 02 May 2023 19:40:08 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:c93ba0c0bf63467e2c37d7fff08d688235b39956dd631c4b489edfe61cccf4fc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.4 MB (42408972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a719be1b9c552298e079060ac06b38ea66dc9304de02c7867139a440ae70684`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:49 GMT
ADD file:7b3c55926db26568f849247e80abdec3cfd6642929a40f0bbee95e4cb176051e in / 
# Wed, 12 Apr 2023 00:39:49 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 01:39:12 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Tue, 02 May 2023 19:02:27 GMT
ENV HAPROXY_VERSION=2.6.13
# Tue, 02 May 2023 19:02:27 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.6/src/haproxy-2.6.13.tar.gz
# Tue, 02 May 2023 19:02:27 GMT
ENV HAPROXY_SHA256=d69ff5233dbca657132ef280d111222ec1e33f5be1c1937d4e9ff516f63f5243
# Tue, 02 May 2023 19:02:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Tue, 02 May 2023 19:02:53 GMT
STOPSIGNAL SIGUSR1
# Tue, 02 May 2023 19:02:53 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Tue, 02 May 2023 19:02:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 May 2023 19:02:53 GMT
USER haproxy
# Tue, 02 May 2023 19:02:53 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:ebc3dc5a2d72427c585c8cda7574a75d96e04b9a37572bd3af0bff905abefbb9`  
		Last Modified: Wed, 12 Apr 2023 00:42:35 GMT  
		Size: 30.1 MB (30063826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593e4fdcdd7122019d2f03bf6741ffdf76a42660a73f691226b8e123ac9a588e`  
		Last Modified: Wed, 12 Apr 2023 01:42:59 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ecccbb7103a89d90456f44fe1752849d1555aa5554eb15294c41ea08989ab1`  
		Last Modified: Tue, 02 May 2023 19:05:50 GMT  
		Size: 12.3 MB (12343261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37c0b015eb69ca9a5d66dbd1bf6ba22fbdf33bb04d58a5a0c01721b5e0768367`  
		Last Modified: Tue, 02 May 2023 19:05:49 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; 386

```console
$ docker pull haproxy@sha256:4a9662dd1aeab82778b1a557e81ad7c72e25d0b124077e5916ee425bf3736aa4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.9 MB (44866494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:436625da28edca40b7ccd9d9f26e33bc5eb57a65711ae8d11346fba7b245001e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:01 GMT
ADD file:42fc1b4536cdd6823499b0c94d799e9bfbcb280b7df55d8d6c9f6defd61ecb6e in / 
# Wed, 12 Apr 2023 00:39:01 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 04:26:05 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Tue, 02 May 2023 18:59:55 GMT
ENV HAPROXY_VERSION=2.6.13
# Tue, 02 May 2023 18:59:55 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.6/src/haproxy-2.6.13.tar.gz
# Tue, 02 May 2023 18:59:55 GMT
ENV HAPROXY_SHA256=d69ff5233dbca657132ef280d111222ec1e33f5be1c1937d4e9ff516f63f5243
# Tue, 02 May 2023 19:00:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Tue, 02 May 2023 19:00:54 GMT
STOPSIGNAL SIGUSR1
# Tue, 02 May 2023 19:00:54 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Tue, 02 May 2023 19:00:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 May 2023 19:00:54 GMT
USER haproxy
# Tue, 02 May 2023 19:00:54 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:b2ee1f87789d52ef09851b4e5c9745fb8aceafa107b0d3452f9973f1abe65042`  
		Last Modified: Wed, 12 Apr 2023 00:42:45 GMT  
		Size: 32.4 MB (32398925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a5a233689960826b780db90148677f52527d8ed44d62199ca74de5cbdbfe452`  
		Last Modified: Wed, 12 Apr 2023 04:34:03 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84194671bdde8ab5c401c143ea0a6bb8e03f0ab218f3f73003287add9457ac9e`  
		Last Modified: Tue, 02 May 2023 19:06:12 GMT  
		Size: 12.5 MB (12465684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7f8af2dc61908e4304867907231cf0ddc9f787023e7bd15b0b5f54584a850fc`  
		Last Modified: Tue, 02 May 2023 19:06:10 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; mips64le

```console
$ docker pull haproxy@sha256:f77e8f2cc452f2f02ed9eaf29e29af992439d42636937c042c7046b1da6556e2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.2 MB (42201290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d64723f6a799b3f8b201237cb8383473ee89d15b24e9710561a3e045b9b94f6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 Apr 2023 00:09:59 GMT
ADD file:2f558bb3cf4bc685f98fcdb12200961e3059267213f0caf7686523305967a663 in / 
# Wed, 12 Apr 2023 00:10:03 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 14:46:55 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Tue, 02 May 2023 18:16:15 GMT
ENV HAPROXY_VERSION=2.6.13
# Tue, 02 May 2023 18:16:18 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.6/src/haproxy-2.6.13.tar.gz
# Tue, 02 May 2023 18:16:20 GMT
ENV HAPROXY_SHA256=d69ff5233dbca657132ef280d111222ec1e33f5be1c1937d4e9ff516f63f5243
# Tue, 02 May 2023 18:19:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Tue, 02 May 2023 18:19:46 GMT
STOPSIGNAL SIGUSR1
# Tue, 02 May 2023 18:19:48 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Tue, 02 May 2023 18:19:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 May 2023 18:19:53 GMT
USER haproxy
# Tue, 02 May 2023 18:19:55 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:8b0f62b0d33641c5348fd31abfd06463bdc4213a072d71479a0765756673777b`  
		Last Modified: Wed, 12 Apr 2023 00:17:28 GMT  
		Size: 29.6 MB (29639206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6fd3df26bfe63e36d3a29a9155f3887d397695137ff81ce9a58074ff150c760`  
		Last Modified: Wed, 12 Apr 2023 16:37:53 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e1d8e5a723a3915fb39a986af3eefbc52b2d8eb7db431bb4f91b84d5c0855f`  
		Last Modified: Tue, 02 May 2023 18:25:17 GMT  
		Size: 12.6 MB (12560340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296a683a42750ceb750dd3df236663f5f80d90a034302c07eba8b52e5fa3edf4`  
		Last Modified: Tue, 02 May 2023 18:25:09 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; ppc64le

```console
$ docker pull haproxy@sha256:9edee8b9f19c2687d6f74bb51177e1a6cd2dce11667bc1df2ad78a7ca010a81a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49639257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad0fbd0d246dd423cc0007556b4c30ac4c9e07df9f3917760f6ed6a9f7cff45a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 Apr 2023 00:08:20 GMT
ADD file:63eb52aaff02c15bceabb87a78eb1b36389066ff4774cf8a754160ca7d509816 in / 
# Wed, 12 Apr 2023 00:08:23 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:30:14 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Tue, 02 May 2023 19:09:13 GMT
ENV HAPROXY_VERSION=2.6.13
# Tue, 02 May 2023 19:09:14 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.6/src/haproxy-2.6.13.tar.gz
# Tue, 02 May 2023 19:09:14 GMT
ENV HAPROXY_SHA256=d69ff5233dbca657132ef280d111222ec1e33f5be1c1937d4e9ff516f63f5243
# Tue, 02 May 2023 19:10:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Tue, 02 May 2023 19:10:40 GMT
STOPSIGNAL SIGUSR1
# Tue, 02 May 2023 19:10:40 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Tue, 02 May 2023 19:10:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 May 2023 19:10:42 GMT
USER haproxy
# Tue, 02 May 2023 19:10:43 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:5b41d5ec640939cf684959234ad3b80909268a32bfd520a31c6720a91521c2fa`  
		Last Modified: Wed, 12 Apr 2023 00:13:13 GMT  
		Size: 35.3 MB (35291995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414c4648f800c15eada0ad86034f7c0acb255013717b002aeeee193947ee1d52`  
		Last Modified: Wed, 12 Apr 2023 00:41:50 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b03983366f2df24129dd1f54a349a23b8bcd1e40344db29f78298c6df8a52899`  
		Last Modified: Tue, 02 May 2023 19:15:59 GMT  
		Size: 14.3 MB (14345374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27a06694668e54b0fbd15612983879e1c9adaa995aef5c836a7c757def9ad6f8`  
		Last Modified: Tue, 02 May 2023 19:15:55 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; s390x

```console
$ docker pull haproxy@sha256:56d0e30ff9ed9c3e701cddf06f0ff5faf7c0ca334d1b12a3af6cf54e1119ff7f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.0 MB (42035036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c901f60c9c1c1a73727124e9f1b873726d34eabf1358bae53544553315151bf4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 12 Apr 2023 00:01:00 GMT
ADD file:b6463dba97ba9c0a29bacfafc4d67bc603ab57e80b75e23cd42d7ef4b0f8e6ae in / 
# Wed, 12 Apr 2023 00:01:04 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 00:13:35 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Tue, 02 May 2023 19:04:57 GMT
ENV HAPROXY_VERSION=2.6.13
# Tue, 02 May 2023 19:04:57 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.6/src/haproxy-2.6.13.tar.gz
# Tue, 02 May 2023 19:04:58 GMT
ENV HAPROXY_SHA256=d69ff5233dbca657132ef280d111222ec1e33f5be1c1937d4e9ff516f63f5243
# Tue, 02 May 2023 19:05:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Tue, 02 May 2023 19:05:31 GMT
STOPSIGNAL SIGUSR1
# Tue, 02 May 2023 19:05:31 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Tue, 02 May 2023 19:05:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 May 2023 19:05:31 GMT
USER haproxy
# Tue, 02 May 2023 19:05:31 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:97fe10bc7def58e7938e97e41eec4788ec7a45b6ef2cb1770cec02fa831fd19d`  
		Last Modified: Wed, 12 Apr 2023 00:05:18 GMT  
		Size: 29.7 MB (29653156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007131dfbe10e2851ece1616dcd33f98b0ed70bf550d506f39015ed721daa073`  
		Last Modified: Wed, 12 Apr 2023 00:19:06 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8637d46a53a869a1b037b09ebe675c74daf5978b3e552c5210f99b0c1968e968`  
		Last Modified: Tue, 02 May 2023 19:11:00 GMT  
		Size: 12.4 MB (12379991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8b86ba62793db3ce9a0e63e11655723102e67a57b7a56e4dc8c58f18f60827`  
		Last Modified: Tue, 02 May 2023 19:10:59 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
