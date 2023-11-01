## `haproxy:lts`

```console
$ docker pull haproxy@sha256:575373e9443fc46e29f7fc19aae82b5c9b60a01543b7e80681f82803a5c8ceb9
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
$ docker pull haproxy@sha256:5e2b156122dd34992ddd73026eb4cd57cbadbed5c30bdc704d0465986e0f8023
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.1 MB (40105314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77b6e95477bbdd2b87f31e84a7d6da419ca5cbbad441842c9f33ef254aa18232`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:11 GMT
ADD file:5fb15e28ab9cd52a4c1371f9273d159579710f4efb955c1e6d76c0403e36967c in / 
# Wed, 01 Nov 2023 00:21:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:50:13 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Wed, 01 Nov 2023 01:50:55 GMT
ENV HAPROXY_VERSION=2.8.3
# Wed, 01 Nov 2023 01:50:55 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.8/src/haproxy-2.8.3.tar.gz
# Wed, 01 Nov 2023 01:50:56 GMT
ENV HAPROXY_SHA256=9ecc6ffe67a977d1ed279107bbdab790d73ae2a626bc38eee23fa1f6786a759e
# Wed, 01 Nov 2023 01:51:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 01 Nov 2023 01:51:30 GMT
STOPSIGNAL SIGUSR1
# Wed, 01 Nov 2023 01:51:30 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 01 Nov 2023 01:51:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Nov 2023 01:51:31 GMT
USER haproxy
# Wed, 01 Nov 2023 01:51:31 GMT
WORKDIR /var/lib/haproxy
# Wed, 01 Nov 2023 01:51:31 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:0bc8ff246cb8ff91066742f8f7ded40397e7aaaa925200b7bec5382d1ffcd6a0`  
		Last Modified: Wed, 01 Nov 2023 00:26:12 GMT  
		Size: 31.4 MB (31417915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a4f3b076c5c9d318d63b69119dc6c39b5300faaa18b3bc54ba75ae301e05dc`  
		Last Modified: Wed, 01 Nov 2023 01:55:49 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a833e28a0ec676d8b7828ede184fe502d078fc792ab7d2de7cad88ec2f3af1db`  
		Last Modified: Wed, 01 Nov 2023 01:56:08 GMT  
		Size: 8.7 MB (8685509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133f911c2d6fe2ac25b95b35e06eb51d38c0cc74822bed10e4b5aa540e5a62d6`  
		Last Modified: Wed, 01 Nov 2023 01:56:06 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:ae179e0e6213e74ce6a6b01ace6b71c567f8f727e70ad9580e46ceae2ca07e14
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.5 MB (37493228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:828d35bac93fc49669fc5bda69a29c722f6418839049661c463642515afdcd65`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 01 Nov 2023 00:48:47 GMT
ADD file:ccc4159f30855826069fec59b14fe886384e5373119e7f382b6faf66f22fb6c6 in / 
# Wed, 01 Nov 2023 00:48:48 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:11:15 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Wed, 01 Nov 2023 01:12:03 GMT
ENV HAPROXY_VERSION=2.8.3
# Wed, 01 Nov 2023 01:12:03 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.8/src/haproxy-2.8.3.tar.gz
# Wed, 01 Nov 2023 01:12:03 GMT
ENV HAPROXY_SHA256=9ecc6ffe67a977d1ed279107bbdab790d73ae2a626bc38eee23fa1f6786a759e
# Wed, 01 Nov 2023 01:12:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 01 Nov 2023 01:12:37 GMT
STOPSIGNAL SIGUSR1
# Wed, 01 Nov 2023 01:12:37 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 01 Nov 2023 01:12:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Nov 2023 01:12:37 GMT
USER haproxy
# Wed, 01 Nov 2023 01:12:37 GMT
WORKDIR /var/lib/haproxy
# Wed, 01 Nov 2023 01:12:38 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:42b20947607fb3d0005c8f3e1da41d53f7e4b3187e4a4bed890c7e9207a1ae03`  
		Last Modified: Wed, 01 Nov 2023 00:52:14 GMT  
		Size: 28.9 MB (28921182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:064788dc196ef4d51d149d1f79fa57c7e49344aef49d696cdf265e4d6f217f3a`  
		Last Modified: Wed, 01 Nov 2023 01:15:33 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9e1051a07b51d3835fa5ab9100da9777f3c85efc5672325b1c799242fa87919`  
		Last Modified: Wed, 01 Nov 2023 01:15:50 GMT  
		Size: 8.6 MB (8570161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c7c9ce4f7b5402424937b3376585caf6196dd0c6aab021d3730cadb09a3e681`  
		Last Modified: Wed, 01 Nov 2023 01:15:48 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:4bbc3b77f3baedf1d9bff79b19fc77206d02a03fa9a3343d710d371dc9f47386
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.0 MB (35001299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59b047dd18b123a7057be73c2a856187edb7e50bbf5520499faf3a8f255a5223`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 01 Nov 2023 00:58:11 GMT
ADD file:a3549614d47152536aaaab630a86d95aaa87b0426b18583391506978eaaa1fb9 in / 
# Wed, 01 Nov 2023 00:58:11 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:05:33 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Wed, 01 Nov 2023 02:06:30 GMT
ENV HAPROXY_VERSION=2.8.3
# Wed, 01 Nov 2023 02:06:30 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.8/src/haproxy-2.8.3.tar.gz
# Wed, 01 Nov 2023 02:06:30 GMT
ENV HAPROXY_SHA256=9ecc6ffe67a977d1ed279107bbdab790d73ae2a626bc38eee23fa1f6786a759e
# Wed, 01 Nov 2023 02:07:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 01 Nov 2023 02:07:11 GMT
STOPSIGNAL SIGUSR1
# Wed, 01 Nov 2023 02:07:11 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 01 Nov 2023 02:07:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Nov 2023 02:07:12 GMT
USER haproxy
# Wed, 01 Nov 2023 02:07:12 GMT
WORKDIR /var/lib/haproxy
# Wed, 01 Nov 2023 02:07:12 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:e016a2def3c8dd02deb4368b431cae20718048a580ddc06a33258cee60ced40f`  
		Last Modified: Wed, 01 Nov 2023 01:02:57 GMT  
		Size: 26.6 MB (26578924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:601dd048b9231a17035bb156472de9f0fe58e298d8f39739740d5416aa66c4ed`  
		Last Modified: Wed, 01 Nov 2023 02:11:17 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae48302f01c3db12526f080380aeca43e565f40426ef454416d1d5b814c3df6d`  
		Last Modified: Wed, 01 Nov 2023 02:11:34 GMT  
		Size: 8.4 MB (8420491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f88ff2167e7a0e03ae51338259cc1a0d02b28bcdc6b013b765745067a1a9d764`  
		Last Modified: Wed, 01 Nov 2023 02:11:33 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:dfc124fdca2c2f706d3da24138dec6ba870e5015aa5059cb387d7230b2273365
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.7 MB (38732037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cdcb725bf6c99060d6a950c3a93a81af195e2b716b9e0312cafe52311c39904`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:55 GMT
ADD file:99dc83e8bb8c67d9179a265fb750c76f73fa660e13e938b6cd613be653cd077e in / 
# Wed, 01 Nov 2023 00:39:56 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 03:28:04 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Wed, 01 Nov 2023 03:28:38 GMT
ENV HAPROXY_VERSION=2.8.3
# Wed, 01 Nov 2023 03:28:38 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.8/src/haproxy-2.8.3.tar.gz
# Wed, 01 Nov 2023 03:28:38 GMT
ENV HAPROXY_SHA256=9ecc6ffe67a977d1ed279107bbdab790d73ae2a626bc38eee23fa1f6786a759e
# Wed, 01 Nov 2023 03:29:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 01 Nov 2023 03:29:04 GMT
STOPSIGNAL SIGUSR1
# Wed, 01 Nov 2023 03:29:04 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 01 Nov 2023 03:29:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Nov 2023 03:29:04 GMT
USER haproxy
# Wed, 01 Nov 2023 03:29:05 GMT
WORKDIR /var/lib/haproxy
# Wed, 01 Nov 2023 03:29:05 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:6e498137f0ed1053c364a5c8a688616b4abee72496a0b97cc71ea5e603565070`  
		Last Modified: Wed, 01 Nov 2023 00:43:46 GMT  
		Size: 30.1 MB (30063905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e405c425f043d12e27353c5ddccd99bc901b1e50a803565a241db1de55ed7ef9`  
		Last Modified: Wed, 01 Nov 2023 03:32:17 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e277d1c718d92edcab24cb0d353e00724b9e92589687dab0b5f2dbd1f4b4d40e`  
		Last Modified: Wed, 01 Nov 2023 03:32:35 GMT  
		Size: 8.7 MB (8666243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b5e717c0185dc061dd61b39685d2bbc0b1255722fe351214c33f9c86d728354`  
		Last Modified: Wed, 01 Nov 2023 03:32:33 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; 386

```console
$ docker pull haproxy@sha256:7d4af3d1693147d6a358cab2f8b92cd7f00dd3ae8081b9b2e3f830dec9353cbf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.8 MB (40840985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:648c9ba06cf8b8d7d6653b5328c9078a1fc5a896a586e9e1de4762351d65f6a3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:18 GMT
ADD file:67f223c9c48e525a23fb110e4c105d7128dcac0c10f32c38f98ea84a21d2bd00 in / 
# Wed, 01 Nov 2023 00:39:19 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:05:07 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Wed, 01 Nov 2023 01:06:17 GMT
ENV HAPROXY_VERSION=2.8.3
# Wed, 01 Nov 2023 01:06:17 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.8/src/haproxy-2.8.3.tar.gz
# Wed, 01 Nov 2023 01:06:17 GMT
ENV HAPROXY_SHA256=9ecc6ffe67a977d1ed279107bbdab790d73ae2a626bc38eee23fa1f6786a759e
# Wed, 01 Nov 2023 01:07:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 01 Nov 2023 01:07:20 GMT
STOPSIGNAL SIGUSR1
# Wed, 01 Nov 2023 01:07:20 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 01 Nov 2023 01:07:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Nov 2023 01:07:20 GMT
USER haproxy
# Wed, 01 Nov 2023 01:07:20 GMT
WORKDIR /var/lib/haproxy
# Wed, 01 Nov 2023 01:07:20 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:bc6810e8fe9346a3caaff984163b789d12b6964a15a2029e384143ca19fef5ad`  
		Last Modified: Wed, 01 Nov 2023 00:44:14 GMT  
		Size: 32.4 MB (32402692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a0f2c99a7373d9ad7bf6e1874c617b11a5ca7b3bd152e3ba8b3bdecfa0e3b07`  
		Last Modified: Wed, 01 Nov 2023 01:13:46 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:312902175d532f96f8fffac9259d8c7b4ee9aa6285022aa4e6445f2b158e0fb8`  
		Last Modified: Wed, 01 Nov 2023 01:14:04 GMT  
		Size: 8.4 MB (8436411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec47fe962a8196e91f6cbd5b24ab61eb03c79af0f51107de0501412b4b130d6`  
		Last Modified: Wed, 01 Nov 2023 01:14:02 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; mips64le

```console
$ docker pull haproxy@sha256:b2e71626d688794ce7b9289d2f635802010a0f90e12a96b21461076a5ff7d7bd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.4 MB (38405557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb73635c2991effabdf0d19a185a0b62c269f20ae8094d774813b7d607235b55`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 01 Nov 2023 01:10:15 GMT
ADD file:c58b99b54270e537286dd7f2ffb13d5a6a1a8ab45c0620c538634014259387e4 in / 
# Wed, 01 Nov 2023 01:10:19 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 06:13:49 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Wed, 01 Nov 2023 06:18:15 GMT
ENV HAPROXY_VERSION=2.8.3
# Wed, 01 Nov 2023 06:18:17 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.8/src/haproxy-2.8.3.tar.gz
# Wed, 01 Nov 2023 06:18:20 GMT
ENV HAPROXY_SHA256=9ecc6ffe67a977d1ed279107bbdab790d73ae2a626bc38eee23fa1f6786a759e
# Wed, 01 Nov 2023 06:21:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 01 Nov 2023 06:21:59 GMT
STOPSIGNAL SIGUSR1
# Wed, 01 Nov 2023 06:22:01 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 01 Nov 2023 06:22:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Nov 2023 06:22:06 GMT
USER haproxy
# Wed, 01 Nov 2023 06:22:09 GMT
WORKDIR /var/lib/haproxy
# Wed, 01 Nov 2023 06:22:12 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c1d7e544711cc24ab1d89506dc11ffa6ff48b21690c7e1d7afff5f1871b8f5fe`  
		Last Modified: Wed, 01 Nov 2023 01:21:13 GMT  
		Size: 29.6 MB (29635977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4168887e865928808cb93b81bd41f66385c76f80fefba2d7e250be05a962bc63`  
		Last Modified: Wed, 01 Nov 2023 06:38:18 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:300e03bd7dbb598acd1a6d6e0a3fddcd05a2ca1907c3883e0d00566e877ab989`  
		Last Modified: Wed, 01 Nov 2023 06:38:43 GMT  
		Size: 8.8 MB (8767833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5699123197578d4e716ea97729fd92cd21c7abca605bd0f685f2fd9157599461`  
		Last Modified: Wed, 01 Nov 2023 06:38:38 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; ppc64le

```console
$ docker pull haproxy@sha256:b74b002b4e4d35707d5c2a69b36af7dc1b555a3ab5f11bb3123b8d99ae4959b0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.4 MB (44406343 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:768416531b1a1e5bb15ac8e2a56c619a212dfaabe279e6e5daeda90b0a9780d3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 01 Nov 2023 00:22:09 GMT
ADD file:a935b2993c62bfb1ade6ba0ffcf1f955422f6f76c63a723877d4bca5bb2aff7b in / 
# Wed, 01 Nov 2023 00:22:11 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:31:30 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Wed, 01 Nov 2023 02:32:42 GMT
ENV HAPROXY_VERSION=2.8.3
# Wed, 01 Nov 2023 02:32:42 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.8/src/haproxy-2.8.3.tar.gz
# Wed, 01 Nov 2023 02:32:42 GMT
ENV HAPROXY_SHA256=9ecc6ffe67a977d1ed279107bbdab790d73ae2a626bc38eee23fa1f6786a759e
# Wed, 01 Nov 2023 02:33:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 01 Nov 2023 02:33:45 GMT
STOPSIGNAL SIGUSR1
# Wed, 01 Nov 2023 02:33:45 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 01 Nov 2023 02:33:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Nov 2023 02:33:46 GMT
USER haproxy
# Wed, 01 Nov 2023 02:33:47 GMT
WORKDIR /var/lib/haproxy
# Wed, 01 Nov 2023 02:33:47 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c4a0eee30f72e7c0e9938500fbc7f30b5eb02d04d49bfe7f18a17af1a6d82f81`  
		Last Modified: Wed, 01 Nov 2023 00:26:59 GMT  
		Size: 35.3 MB (35293810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d80491e17f3c6c4bd6b9662d03a4d236aebd3421edafbef52dd2aa654990957`  
		Last Modified: Wed, 01 Nov 2023 02:38:52 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8e22f8dfee3abbeb1705494b6d827994498849de9f1febb5bbf4ccd4e28213f`  
		Last Modified: Wed, 01 Nov 2023 02:39:10 GMT  
		Size: 9.1 MB (9110646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c0a6999a334f0c1031af4b3cb71a280a63e9c1b59df1b6d9c56fe64446b6a90`  
		Last Modified: Wed, 01 Nov 2023 02:39:08 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; s390x

```console
$ docker pull haproxy@sha256:6e1fee3aff7fd62264e7129ae1445b010e38ccc5eea147ae9e8113d1949c719b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.4 MB (38357008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db5324a46105002cdee1aea57006b39940a4670446cceefa5663cd15658b3a37`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 11 Oct 2023 17:50:58 GMT
ADD file:0cfc89fea6da8404b2bccfb0c408dde9e7497e8a93304c4ced9e51bd2b3a319a in / 
# Wed, 11 Oct 2023 17:51:00 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 23:28:56 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Wed, 11 Oct 2023 23:29:45 GMT
ENV HAPROXY_VERSION=2.8.3
# Wed, 11 Oct 2023 23:29:46 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.8/src/haproxy-2.8.3.tar.gz
# Wed, 11 Oct 2023 23:29:46 GMT
ENV HAPROXY_SHA256=9ecc6ffe67a977d1ed279107bbdab790d73ae2a626bc38eee23fa1f6786a759e
# Wed, 11 Oct 2023 23:30:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 11 Oct 2023 23:30:18 GMT
STOPSIGNAL SIGUSR1
# Wed, 11 Oct 2023 23:30:18 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 11 Oct 2023 23:30:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Oct 2023 23:30:18 GMT
USER haproxy
# Wed, 11 Oct 2023 23:30:18 GMT
WORKDIR /var/lib/haproxy
# Wed, 11 Oct 2023 23:30:19 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:a12df18f4c86c0f825c6b30eb023dc9f30ba0de34f6b97dca708a7247f4f6c49`  
		Last Modified: Wed, 11 Oct 2023 17:57:36 GMT  
		Size: 29.7 MB (29656917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb749962e7c2d0a0927c127a9cfd9844a6e598f90552f7bbe9362677be4a5654`  
		Last Modified: Wed, 11 Oct 2023 23:34:27 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:200c8ec03a61f0604dbe5b9cc51e35ed1fa1378a99cf1568c912216f71feb9ae`  
		Last Modified: Wed, 11 Oct 2023 23:35:21 GMT  
		Size: 8.7 MB (8698206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751705ca552a3d4ae4abd8c88f6df13fc075cc6e0404e011fcf42e2c9f74707f`  
		Last Modified: Wed, 11 Oct 2023 23:35:20 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
