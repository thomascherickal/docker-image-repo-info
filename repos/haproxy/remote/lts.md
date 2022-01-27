## `haproxy:lts`

```console
$ docker pull haproxy@sha256:abece3921a71c72df05773316e6c359eea81777a16ae1754b86bdfd8c9641d3f
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
$ docker pull haproxy@sha256:59da0e1e9513534e40816b85eae8bbbc88e703a43a8d77d712181c1e509857c1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.2 MB (39152835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56e6b650bb9175219513b4e478e0c8e03140d6f53f1e06d4ca16e1a034d40cf1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:35 GMT
ADD file:90495c24c897ec47982e200f732f8be3109fcd791691ddffae0756898f91024f in / 
# Wed, 26 Jan 2022 01:40:36 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 08:07:17 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Wed, 26 Jan 2022 08:09:39 GMT
ENV HAPROXY_VERSION=2.4.12
# Wed, 26 Jan 2022 08:09:40 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.12.tar.gz
# Wed, 26 Jan 2022 08:09:40 GMT
ENV HAPROXY_SHA256=6984a94466739e5e8188949a3d1731634087226a12aada8bf6f81f9d316ca4f3
# Wed, 26 Jan 2022 08:10:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 26 Jan 2022 08:10:39 GMT
STOPSIGNAL SIGUSR1
# Wed, 26 Jan 2022 08:10:39 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 26 Jan 2022 08:10:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 08:10:39 GMT
USER haproxy
# Wed, 26 Jan 2022 08:10:40 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:5eb5b503b37671af16371272f9c5313a3e82f1d0756e14506704489ad9900803`  
		Last Modified: Wed, 26 Jan 2022 01:46:39 GMT  
		Size: 31.4 MB (31366257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96465204a9121a482dba9ac47053f89357b2acb86376009c41285cd516c39147`  
		Last Modified: Wed, 26 Jan 2022 08:16:13 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5406cf6b5606bf53108275c23f1f674d531d10e6ddb7fb59cc97488101d08694`  
		Last Modified: Wed, 26 Jan 2022 08:16:58 GMT  
		Size: 7.8 MB (7784693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f9cd871bb51db9dd25f30c95f1ac2ae02bfcbcfbbc3f4c83fa2fbcdb1ff3bac`  
		Last Modified: Wed, 26 Jan 2022 08:16:56 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:eba487859466c15e40a864411234cec5210c1cceea3dba6c8a68c1f51f0fcff1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.6 MB (36607751 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03f967a918d7cc442b0e9335c099e377d84b15d21ada9362b80e1df8a328e596`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:57 GMT
ADD file:4ccea3cb033595f7bd9896126e94a8a19199b987bedd87b3c0700d8b29baa1fb in / 
# Wed, 26 Jan 2022 01:41:58 GMT
CMD ["bash"]
# Thu, 27 Jan 2022 02:35:06 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Thu, 27 Jan 2022 02:37:40 GMT
ENV HAPROXY_VERSION=2.4.12
# Thu, 27 Jan 2022 02:37:40 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.12.tar.gz
# Thu, 27 Jan 2022 02:37:40 GMT
ENV HAPROXY_SHA256=6984a94466739e5e8188949a3d1731634087226a12aada8bf6f81f9d316ca4f3
# Thu, 27 Jan 2022 02:38:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 27 Jan 2022 02:38:38 GMT
STOPSIGNAL SIGUSR1
# Thu, 27 Jan 2022 02:38:39 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 27 Jan 2022 02:38:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jan 2022 02:38:39 GMT
USER haproxy
# Thu, 27 Jan 2022 02:38:40 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:247ff78919074ec9db7cccd537dd6eb4d7e2788013b7ef07443e345d91c8a588`  
		Last Modified: Wed, 26 Jan 2022 01:57:36 GMT  
		Size: 28.9 MB (28909638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44e5d20fe5d9970d48350ff308cab28c025ffd98ad425d89da7ea9ed2f800a45`  
		Last Modified: Thu, 27 Jan 2022 02:46:31 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b1cffc1b1620aa8d3f26d68904bd4f769dcc682b2444a072657ab37f0cac3e`  
		Last Modified: Thu, 27 Jan 2022 02:47:34 GMT  
		Size: 7.7 MB (7696223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c29efd4bc55c23b7c8891b951d010445aa8c2b053aa789310eb01ba10554e11`  
		Last Modified: Thu, 27 Jan 2022 02:47:29 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:307791797cd5fa71ded1c30fc7dcee2d9de64655f24c2b6e8ba2abb49972bd4d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34126598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb7081dd135e1faf1c787560b6672d11fb786a1e3402f667257d8a4d1537849d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:08 GMT
ADD file:7f27f5b43b7cb04e509fe145266d9bdeacfcacb024cafac32e57ef1c831d5ea7 in / 
# Wed, 26 Jan 2022 01:42:09 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:31:48 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Wed, 26 Jan 2022 02:34:38 GMT
ENV HAPROXY_VERSION=2.4.12
# Wed, 26 Jan 2022 02:34:38 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.12.tar.gz
# Wed, 26 Jan 2022 02:34:39 GMT
ENV HAPROXY_SHA256=6984a94466739e5e8188949a3d1731634087226a12aada8bf6f81f9d316ca4f3
# Wed, 26 Jan 2022 02:35:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 26 Jan 2022 02:35:34 GMT
STOPSIGNAL SIGUSR1
# Wed, 26 Jan 2022 02:35:34 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 26 Jan 2022 02:35:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 02:35:35 GMT
USER haproxy
# Wed, 26 Jan 2022 02:35:36 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:aaef1f1162ec03e01b5b955d41da400544ec2374093ae3dbc330ab2bb36df3e1`  
		Last Modified: Wed, 26 Jan 2022 01:57:59 GMT  
		Size: 26.6 MB (26564933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0602ad1ae7f3b207731c569c474289181c2bb551e22622129c2329f200c597ba`  
		Last Modified: Wed, 26 Jan 2022 02:46:07 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd5667abcdc1d0b55f1a25a7c15e835d736c8d90cf21cd378d37634da10e268f`  
		Last Modified: Wed, 26 Jan 2022 02:47:30 GMT  
		Size: 7.6 MB (7559781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5238d5becf7c16935acdba614253dc6b5772153a1540f243607af6a73ba121d`  
		Last Modified: Wed, 26 Jan 2022 02:47:26 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:8ec14095c57d2b1aff2259ce8e062d67c9ad308886f1b8b98a2fcd5ee9df7212
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.9 MB (37904815 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8cd6f6be7a80234faea1b43eff63b4132e257682153ddffc91032fcd33e548c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:31 GMT
ADD file:0ec6f47a8857bf8e6cef71ed8f864be7ce1790ff6ed04fd4201e7dbde4728d3a in / 
# Wed, 26 Jan 2022 01:42:31 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 04:05:26 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Wed, 26 Jan 2022 04:07:03 GMT
ENV HAPROXY_VERSION=2.4.12
# Wed, 26 Jan 2022 04:07:04 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.12.tar.gz
# Wed, 26 Jan 2022 04:07:05 GMT
ENV HAPROXY_SHA256=6984a94466739e5e8188949a3d1731634087226a12aada8bf6f81f9d316ca4f3
# Wed, 26 Jan 2022 04:07:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 26 Jan 2022 04:07:35 GMT
STOPSIGNAL SIGUSR1
# Wed, 26 Jan 2022 04:07:37 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 26 Jan 2022 04:07:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 04:07:38 GMT
USER haproxy
# Wed, 26 Jan 2022 04:07:39 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:8998bd30e6a1204d13403045766edbe14f941b52087465f5d140ab63c8b113bf`  
		Last Modified: Wed, 26 Jan 2022 01:49:04 GMT  
		Size: 30.1 MB (30056774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:610b62b47697e69f6743a6a999f1f794f61484ab499feb9dca129a7f128a9d68`  
		Last Modified: Wed, 26 Jan 2022 04:12:49 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d17c8cd2bd48615d884b35c4b3563b2062bbcd5a739ac4354a56b0aa5a7e6e`  
		Last Modified: Wed, 26 Jan 2022 04:13:38 GMT  
		Size: 7.8 MB (7846297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0511890281403e2682eebe91680c4ac19367a7807f88bf1cc8275fa549e02a5`  
		Last Modified: Wed, 26 Jan 2022 04:13:36 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; 386

```console
$ docker pull haproxy@sha256:39421a8b870cbd7b50b979b9a7ebde408cb3aa473a97860c43f683c5ffddb5f6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.9 MB (39936883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28d3fe4d88428ae610af5dc9ef842a35ecef217ed43c69b7a81e4a286810e8fb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 26 Jan 2022 01:39:55 GMT
ADD file:876ebf07c65841f4840842086c883af48e07386964fe6d643ba193895ec2a582 in / 
# Wed, 26 Jan 2022 01:39:56 GMT
CMD ["bash"]
# Thu, 27 Jan 2022 03:45:22 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Thu, 27 Jan 2022 03:49:21 GMT
ENV HAPROXY_VERSION=2.4.12
# Thu, 27 Jan 2022 03:49:22 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.12.tar.gz
# Thu, 27 Jan 2022 03:49:23 GMT
ENV HAPROXY_SHA256=6984a94466739e5e8188949a3d1731634087226a12aada8bf6f81f9d316ca4f3
# Thu, 27 Jan 2022 03:51:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 27 Jan 2022 03:51:27 GMT
STOPSIGNAL SIGUSR1
# Thu, 27 Jan 2022 03:51:28 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 27 Jan 2022 03:51:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Jan 2022 03:51:29 GMT
USER haproxy
# Thu, 27 Jan 2022 03:51:29 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:86933886b1754aba091548cf031a9bca88cdce9bb4fc1f28bb38b61594c2c2c7`  
		Last Modified: Wed, 26 Jan 2022 01:48:57 GMT  
		Size: 32.4 MB (32377406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7b43951bf7f23397c9f48567e8bd06579a27ba0a61a71d46e3fa115ec7f9a8`  
		Last Modified: Thu, 27 Jan 2022 04:06:45 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf1cbe2d0aaf68691c389f2c2b79fdec8f14811f01946e37c844c6d8718a5686`  
		Last Modified: Thu, 27 Jan 2022 04:07:58 GMT  
		Size: 7.6 MB (7557594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48895a44964adf8fa1e1d9be235d1f7aae87343fd5ec9209503225dab732ab4a`  
		Last Modified: Thu, 27 Jan 2022 04:07:55 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; mips64le

```console
$ docker pull haproxy@sha256:b5831334c6a2058b6541512d8e9fda26e8dee69c50ee77bbaa9e4065a93b26db
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.6 MB (37556186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9adf9fd520d17054a7040a7efd242e154ec9545ab9dd0567671363da20b47fa5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:45 GMT
ADD file:61767027a5ab46afbcd4079d200abe8d663326adc96fa28ca8c8955a06d9322e in / 
# Wed, 26 Jan 2022 01:42:46 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:48:02 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Wed, 26 Jan 2022 02:53:29 GMT
ENV HAPROXY_VERSION=2.4.12
# Wed, 26 Jan 2022 02:53:30 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.12.tar.gz
# Wed, 26 Jan 2022 02:53:30 GMT
ENV HAPROXY_SHA256=6984a94466739e5e8188949a3d1731634087226a12aada8bf6f81f9d316ca4f3
# Wed, 26 Jan 2022 02:56:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 26 Jan 2022 02:56:04 GMT
STOPSIGNAL SIGUSR1
# Wed, 26 Jan 2022 02:56:04 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 26 Jan 2022 02:56:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 02:56:05 GMT
USER haproxy
# Wed, 26 Jan 2022 02:56:05 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:266e7d2b59483859eaa1711d2afeb25ea4458eeb36b3e909372930db1f834d7f`  
		Last Modified: Wed, 26 Jan 2022 01:51:23 GMT  
		Size: 29.6 MB (29632834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fb05aa9e5c9f174904584616623f4f44d6bfcda93b7c9cbbe16cc35a59d08b4`  
		Last Modified: Wed, 26 Jan 2022 03:06:03 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f2b103a85e7f5f5b34e4addad96f780e65ea73e47963920ef74c6c9247f34b`  
		Last Modified: Wed, 26 Jan 2022 03:06:54 GMT  
		Size: 7.9 MB (7921490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a289c2081ddc2f62a31e920f0287952aa4676313fa8f6cf0ca968a2e886af744`  
		Last Modified: Wed, 26 Jan 2022 03:06:48 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; ppc64le

```console
$ docker pull haproxy@sha256:83bf6e313bc6d7aa79411e7604809912356b31a08a7715c4443db0c183f617b0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.5 MB (43455928 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:888eb37f4c69afa00c2d033d316e6a2f388e581edad3cbe2175915e2a2aba167`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 26 Jan 2022 01:46:51 GMT
ADD file:c03f34c221e57fa5cb625c166d1db9f72d6ba2fa17a3c41a5d04d6875d098949 in / 
# Wed, 26 Jan 2022 01:46:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 21:49:01 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Wed, 26 Jan 2022 21:54:57 GMT
ENV HAPROXY_VERSION=2.4.12
# Wed, 26 Jan 2022 21:54:59 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.12.tar.gz
# Wed, 26 Jan 2022 21:55:02 GMT
ENV HAPROXY_SHA256=6984a94466739e5e8188949a3d1731634087226a12aada8bf6f81f9d316ca4f3
# Wed, 26 Jan 2022 21:57:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 26 Jan 2022 21:57:27 GMT
STOPSIGNAL SIGUSR1
# Wed, 26 Jan 2022 21:57:29 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 26 Jan 2022 21:57:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 21:57:34 GMT
USER haproxy
# Wed, 26 Jan 2022 21:57:35 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:3149ee4a73508a4c39107d64a3fdc1b021626a22a0ac95e62fa0cea49ab77fba`  
		Last Modified: Wed, 26 Jan 2022 01:57:01 GMT  
		Size: 35.3 MB (35273030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f240b089c677f543ff7306f127f06945707e2944c32b207bde0f45eaf89111a6`  
		Last Modified: Wed, 26 Jan 2022 22:12:03 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1c286ad5d2f0542ac6e462a1061c88b28792c8a670d937503bf83ed3ce8af0`  
		Last Modified: Wed, 26 Jan 2022 22:12:58 GMT  
		Size: 8.2 MB (8181003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74366ad85491005d9f717a0f67a3f1b66a9236830c77aa54a4aafd5dab872682`  
		Last Modified: Wed, 26 Jan 2022 22:12:57 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; s390x

```console
$ docker pull haproxy@sha256:12b2568a3a74adec90cc72bcf37d7c22acad68851d4a5fefde1e31bba252c1ef
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.5 MB (37480135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51f789f7e1caa6ccc415f4ba12ded07671b2df6d0903dcbf3dea294423602904`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:13 GMT
ADD file:03b224b82f458b08d3b5071e42b67915a3db309332c0fc9229db7cf1148bc1b5 in / 
# Wed, 26 Jan 2022 01:41:15 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:59:07 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Wed, 26 Jan 2022 03:00:40 GMT
ENV HAPROXY_VERSION=2.4.12
# Wed, 26 Jan 2022 03:00:40 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.12.tar.gz
# Wed, 26 Jan 2022 03:00:41 GMT
ENV HAPROXY_SHA256=6984a94466739e5e8188949a3d1731634087226a12aada8bf6f81f9d316ca4f3
# Wed, 26 Jan 2022 03:01:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 26 Jan 2022 03:01:11 GMT
STOPSIGNAL SIGUSR1
# Wed, 26 Jan 2022 03:01:11 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 26 Jan 2022 03:01:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Jan 2022 03:01:12 GMT
USER haproxy
# Wed, 26 Jan 2022 03:01:12 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:70bed29526f8483937e4d2540d19256d30786007c7c321e717e00d2e74700380`  
		Last Modified: Wed, 26 Jan 2022 01:46:57 GMT  
		Size: 29.6 MB (29647071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7abe581dbf0f516610497c16908f5357455f1e5c2a7e5a4f4db725742caffaa`  
		Last Modified: Wed, 26 Jan 2022 03:06:23 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46634d88c02ad6bfcfe5652dcb00fe3b1315668997a6a4d9880631d9879488c6`  
		Last Modified: Wed, 26 Jan 2022 03:07:01 GMT  
		Size: 7.8 MB (7831178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ece4a817601137eae6a5dd3a0ff8e669a8cf919302014dbb5f4a5b507e9a06`  
		Last Modified: Wed, 26 Jan 2022 03:07:00 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
