## `haproxy:lts`

```console
$ docker pull haproxy@sha256:1ff3ffe715862915a521402246208cfd0f5cf0abf8e62677046d6858bf9cf249
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
$ docker pull haproxy@sha256:b4b9c33b96a23a94fe369d0828fe53d79c3a7849f783d3029d1440e406eee429
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.4 MB (39422223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dac71ddde48fd829d9c5828c0df8f908c0d9f5269c3632eb0d3ca478a5884c84`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:54 GMT
ADD file:d08e242792caa7f842fcf39a09ad59c97a856660e2013d5aed3e4a29197e9aaa in / 
# Tue, 15 Nov 2022 04:04:54 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 12:38:01 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Mon, 05 Dec 2022 21:27:19 GMT
ENV HAPROXY_VERSION=2.6.7
# Mon, 05 Dec 2022 21:27:20 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.6/src/haproxy-2.6.7.tar.gz
# Mon, 05 Dec 2022 21:27:20 GMT
ENV HAPROXY_SHA256=cff9b8b18a52bfec277f9c1887fac93c18e1b9f3eff48892255a7c6e64528b7d
# Mon, 05 Dec 2022 21:27:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Mon, 05 Dec 2022 21:27:58 GMT
STOPSIGNAL SIGUSR1
# Mon, 05 Dec 2022 21:27:58 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 05 Dec 2022 21:27:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 05 Dec 2022 21:27:58 GMT
USER haproxy
# Mon, 05 Dec 2022 21:27:58 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:a603fa5e3b4127f210503aaa6189abf6286ee5a73deeaab460f8f33ebc6b64e2`  
		Last Modified: Tue, 15 Nov 2022 04:08:47 GMT  
		Size: 31.4 MB (31412630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c83661736dfceff3e877d8f012cb0d2f75a779d9750f8d5e44f7f3d32928f238`  
		Last Modified: Tue, 15 Nov 2022 12:43:55 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f3f0a1c0158172c504eeafe1ff3f766b1a6bd7c4c8008136df9899104d267e`  
		Last Modified: Mon, 05 Dec 2022 21:31:21 GMT  
		Size: 8.0 MB (8007704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:790cdd103b3fb823176697728450dc68b6e514cd8b0559d19fa4f6d742572f40`  
		Last Modified: Mon, 05 Dec 2022 21:31:20 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:30988e2b9ea79b25467a87fe67fb2eb91f5ca97fff69b7b8067832010e98ddae
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.8 MB (36813243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52dccb72a52a793c9522bc54f6ccda3d61a45fee109ead29dedf14885498583f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Nov 2022 01:49:18 GMT
ADD file:1949af7e583a1b54055a421129c32315fc101e53e2cda05da3171ed461bde0a6 in / 
# Tue, 15 Nov 2022 01:49:19 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 10:13:42 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Mon, 05 Dec 2022 20:48:41 GMT
ENV HAPROXY_VERSION=2.6.7
# Mon, 05 Dec 2022 20:48:41 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.6/src/haproxy-2.6.7.tar.gz
# Mon, 05 Dec 2022 20:48:41 GMT
ENV HAPROXY_SHA256=cff9b8b18a52bfec277f9c1887fac93c18e1b9f3eff48892255a7c6e64528b7d
# Mon, 05 Dec 2022 20:49:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Mon, 05 Dec 2022 20:49:14 GMT
STOPSIGNAL SIGUSR1
# Mon, 05 Dec 2022 20:49:14 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 05 Dec 2022 20:49:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 05 Dec 2022 20:49:14 GMT
USER haproxy
# Mon, 05 Dec 2022 20:49:14 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:b56836d864a6d857be3d12242b65962f2a2cf0d77c48cfb85bbbdf9d56a7e93d`  
		Last Modified: Tue, 15 Nov 2022 01:54:26 GMT  
		Size: 28.9 MB (28914126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670a7e7484c3fcbb8bdcf879bbc529d20b4091293c0412adbf80aff0a7474987`  
		Last Modified: Tue, 15 Nov 2022 10:18:37 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cca5e93effa41735f9d26f9dc3a48be7ad6237651c1de7c13a1ce1b6e2ba3b36`  
		Last Modified: Mon, 05 Dec 2022 20:51:45 GMT  
		Size: 7.9 MB (7897262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09aa780925266b35f63c3407e3933bdc48137f9e03a6bd213249819667b9dc22`  
		Last Modified: Mon, 05 Dec 2022 20:51:43 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:6bf8a0ca03786978efd7553e78bfd99ce5178cda6391c3fe65e4516d7541e98c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34336546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1baa1a460c9d8845f8454ee1ac2579924d05fa997d533e8ce9f80d1af7b3d346`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Nov 2022 03:43:25 GMT
ADD file:1b5c939bd2a35667d7fc44c3009a56ed92a932f512a73df1617dec6ccbd6e6b1 in / 
# Tue, 15 Nov 2022 03:43:26 GMT
CMD ["bash"]
# Wed, 16 Nov 2022 09:04:22 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Mon, 05 Dec 2022 21:12:06 GMT
ENV HAPROXY_VERSION=2.6.7
# Mon, 05 Dec 2022 21:12:06 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.6/src/haproxy-2.6.7.tar.gz
# Mon, 05 Dec 2022 21:12:06 GMT
ENV HAPROXY_SHA256=cff9b8b18a52bfec277f9c1887fac93c18e1b9f3eff48892255a7c6e64528b7d
# Mon, 05 Dec 2022 21:12:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Mon, 05 Dec 2022 21:12:38 GMT
STOPSIGNAL SIGUSR1
# Mon, 05 Dec 2022 21:12:38 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 05 Dec 2022 21:12:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 05 Dec 2022 21:12:39 GMT
USER haproxy
# Mon, 05 Dec 2022 21:12:39 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:fd18d0201d0ce0c5e103902d894f5d601fc5dde76688aa7dae786840141d23e4`  
		Last Modified: Tue, 15 Nov 2022 03:50:11 GMT  
		Size: 26.6 MB (26576195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84e76fa915ccc89514803e6a4819ef0235574211bd9797e4e37e624e801f9dfa`  
		Last Modified: Wed, 16 Nov 2022 09:12:22 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:421e7ccfd4a9f7fab4b81f7e4a30704f18f688a3aae07fb8b84b744d05963fc9`  
		Last Modified: Mon, 05 Dec 2022 21:18:52 GMT  
		Size: 7.8 MB (7758494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4e686ad7baa53fb4abb6a1fa605e61e4c835eb01b43e45685fb13a7b3b19ca2`  
		Last Modified: Mon, 05 Dec 2022 21:18:50 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:fd1cbf12f7d401c1a10813cdf84c190673a3e4e4d1c8ee29bee80b8e54acfe98
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.1 MB (38079905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a679e0cafe0ac8a3888f8c366318245a3b7581e969636ecf940703249c5efb6e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:20 GMT
ADD file:1dad2420090b3d6ef5df8d1f7f2878b22f8687b8dba008a63800f6c74b36dee9 in / 
# Tue, 15 Nov 2022 01:41:20 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 06:14:33 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Mon, 05 Dec 2022 20:56:50 GMT
ENV HAPROXY_VERSION=2.6.7
# Mon, 05 Dec 2022 20:56:50 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.6/src/haproxy-2.6.7.tar.gz
# Mon, 05 Dec 2022 20:56:50 GMT
ENV HAPROXY_SHA256=cff9b8b18a52bfec277f9c1887fac93c18e1b9f3eff48892255a7c6e64528b7d
# Mon, 05 Dec 2022 20:57:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Mon, 05 Dec 2022 20:57:18 GMT
STOPSIGNAL SIGUSR1
# Mon, 05 Dec 2022 20:57:18 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 05 Dec 2022 20:57:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 05 Dec 2022 20:57:18 GMT
USER haproxy
# Mon, 05 Dec 2022 20:57:18 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:f3ac85625e767ee0ec42b5a2ef93880251cd973b86f77124c4ed39bccd2f8bf9`  
		Last Modified: Tue, 15 Nov 2022 01:44:35 GMT  
		Size: 30.1 MB (30060605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b6d8e4efc3cf0303cbede1fd2894e9204ca11d1015d4d5704cb58e9b9d5d3f9`  
		Last Modified: Tue, 15 Nov 2022 06:19:10 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be700b0006f2141f9741a1538eb88cfa585f849511d76e189f751f830a23bb9`  
		Last Modified: Mon, 05 Dec 2022 21:00:18 GMT  
		Size: 8.0 MB (8017414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9f9974e331090a2529b23e7aae08627e306e77719bf3ce7f406176ab568bc2`  
		Last Modified: Mon, 05 Dec 2022 21:00:16 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; 386

```console
$ docker pull haproxy@sha256:d9981abfbcca1e3ce8968cfab44c8fe736e0ea80bbd532351ef7c22e3648d75f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40178771 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e28c8c944b1d8b49b0482f496cd71b6676bd627875f02786c0e31263ef93254`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:27 GMT
ADD file:608bec4ba3e2543714da4c5158f3c46a168f63ee69ac3f48bff54474ba9a6f27 in / 
# Tue, 15 Nov 2022 01:41:27 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 07:15:24 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Mon, 05 Dec 2022 20:49:30 GMT
ENV HAPROXY_VERSION=2.6.7
# Mon, 05 Dec 2022 20:49:31 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.6/src/haproxy-2.6.7.tar.gz
# Mon, 05 Dec 2022 20:49:32 GMT
ENV HAPROXY_SHA256=cff9b8b18a52bfec277f9c1887fac93c18e1b9f3eff48892255a7c6e64528b7d
# Mon, 05 Dec 2022 20:50:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Mon, 05 Dec 2022 20:50:06 GMT
STOPSIGNAL SIGUSR1
# Mon, 05 Dec 2022 20:50:08 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 05 Dec 2022 20:50:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 05 Dec 2022 20:50:09 GMT
USER haproxy
# Mon, 05 Dec 2022 20:50:10 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:f6a1e975b34444ecb7c6a2b537403fd6b94d2ff3225944ac2ac3b292466e4078`  
		Last Modified: Tue, 15 Nov 2022 01:47:05 GMT  
		Size: 32.4 MB (32392982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f82e21db04a41c1e28358349f8b3cdde0c3fd6f8d0301301c676dd7039711f2`  
		Last Modified: Tue, 15 Nov 2022 07:23:35 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3910bc4cb5bead48d5a896bfdfd676e80d2e0e93434db090aa1f3ea29ee01dcd`  
		Last Modified: Mon, 05 Dec 2022 20:55:49 GMT  
		Size: 7.8 MB (7784052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88aedc1fff540da3332f4004e0f244fcaf25fc0a2e464c3c6572f2a03fa6ca3e`  
		Last Modified: Mon, 05 Dec 2022 20:55:47 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; mips64le

```console
$ docker pull haproxy@sha256:d643a62817f2592ea755c50f01f9ff97252e3134acffb65689fcccd2cdd93056
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.8 MB (37758172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b50d8e03ccb0615912c1a7c96fb7f9be2b0165e81efcca4a6383b28e1d98373f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Nov 2022 04:13:42 GMT
ADD file:da7bed758c1e8c14583d53792170b6f4133a408ce2966e22ce52905f5c0d55a4 in / 
# Tue, 15 Nov 2022 04:13:46 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 23:43:27 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Tue, 15 Nov 2022 23:47:37 GMT
ENV HAPROXY_VERSION=2.6.6
# Tue, 15 Nov 2022 23:47:39 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.6/src/haproxy-2.6.6.tar.gz
# Tue, 15 Nov 2022 23:47:42 GMT
ENV HAPROXY_SHA256=d0c80c90c04ae79598b58b9749d53787f00f7b515175e7d8203f2796e6a6594d
# Tue, 15 Nov 2022 23:50:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Tue, 15 Nov 2022 23:50:53 GMT
STOPSIGNAL SIGUSR1
# Tue, 15 Nov 2022 23:50:55 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Tue, 15 Nov 2022 23:50:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 23:51:00 GMT
USER haproxy
# Tue, 15 Nov 2022 23:51:02 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:27e2cdb4ebe2b6ee11014db328a4a8a055e3dcee2e275bf3aca6f03b39a09ad5`  
		Last Modified: Tue, 15 Nov 2022 04:21:14 GMT  
		Size: 29.6 MB (29635497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c19145edc1930601b168ceacf3561a59f54375c3954e812d75f040596a0e377d`  
		Last Modified: Wed, 16 Nov 2022 00:02:26 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f8d1742c4b9d7d590be46f77f93d4a72b333a822dcdcc1aa8a452c58d03de88`  
		Last Modified: Wed, 16 Nov 2022 00:02:50 GMT  
		Size: 8.1 MB (8120923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1ddd20cb0ca5b5873f5264b5ad70789940d194fb4fecf95cae74997231ca39`  
		Last Modified: Wed, 16 Nov 2022 00:02:44 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; ppc64le

```console
$ docker pull haproxy@sha256:857e08e3801b6ceaf69c88b610920921469241adbcadf38365d80ef03d9e167d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.7 MB (43702357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc019b9b731fc1674d7b3de18f5abd30525645a6aca72b14f6c7802456365abb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Nov 2022 05:18:45 GMT
ADD file:520926164fdc762143905745329e568c67289232bec450e48645d82a4613dccf in / 
# Tue, 15 Nov 2022 05:18:47 GMT
CMD ["bash"]
# Wed, 16 Nov 2022 02:29:56 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Mon, 05 Dec 2022 21:17:16 GMT
ENV HAPROXY_VERSION=2.6.7
# Mon, 05 Dec 2022 21:17:16 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.6/src/haproxy-2.6.7.tar.gz
# Mon, 05 Dec 2022 21:17:17 GMT
ENV HAPROXY_SHA256=cff9b8b18a52bfec277f9c1887fac93c18e1b9f3eff48892255a7c6e64528b7d
# Mon, 05 Dec 2022 21:18:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Mon, 05 Dec 2022 21:18:02 GMT
STOPSIGNAL SIGUSR1
# Mon, 05 Dec 2022 21:18:03 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 05 Dec 2022 21:18:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 05 Dec 2022 21:18:03 GMT
USER haproxy
# Mon, 05 Dec 2022 21:18:04 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c57913b7d0318ef1a47f0348ce54d9865316776aa1ffb2c7871b1473b3d29407`  
		Last Modified: Tue, 15 Nov 2022 05:24:22 GMT  
		Size: 35.3 MB (35285140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bbb14dc9bdb01a2075bd23b163b1d031a5d8e9e9f126ae5bf96be0f70475872`  
		Last Modified: Wed, 16 Nov 2022 02:37:24 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca3f72c4da376ea87592a3ce353e63c5970262040b0faadac9d5165f461c5f49`  
		Last Modified: Mon, 05 Dec 2022 21:23:19 GMT  
		Size: 8.4 MB (8415330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9e99309230c020289e0d89d176662b1bc31df9aa312b49e5dfcb74e34236bf2`  
		Last Modified: Mon, 05 Dec 2022 21:23:16 GMT  
		Size: 457.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; s390x

```console
$ docker pull haproxy@sha256:16817e75e471caf1d8bf5290625f9ca46bbbf944beb5a25d258e905a60717944
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.7 MB (37661476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c08785ee7f903549716300082909f54e64a0abe299833ad4ab0a090e8813c7e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 15 Nov 2022 01:42:51 GMT
ADD file:af482bbfc85f1f292de8bd5f2751ee2b67ec9e057eab3684f96984f0e4ecf943 in / 
# Tue, 15 Nov 2022 01:42:56 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 13:17:23 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Mon, 05 Dec 2022 20:47:49 GMT
ENV HAPROXY_VERSION=2.6.7
# Mon, 05 Dec 2022 20:47:49 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.6/src/haproxy-2.6.7.tar.gz
# Mon, 05 Dec 2022 20:47:49 GMT
ENV HAPROXY_SHA256=cff9b8b18a52bfec277f9c1887fac93c18e1b9f3eff48892255a7c6e64528b7d
# Mon, 05 Dec 2022 20:48:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Mon, 05 Dec 2022 20:48:20 GMT
STOPSIGNAL SIGUSR1
# Mon, 05 Dec 2022 20:48:20 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Mon, 05 Dec 2022 20:48:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 05 Dec 2022 20:48:21 GMT
USER haproxy
# Mon, 05 Dec 2022 20:48:21 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:a6ad801d746b7bdde3a0ef72107d05694a38101de03b6eed340af802bdf13957`  
		Last Modified: Tue, 15 Nov 2022 01:47:33 GMT  
		Size: 29.6 MB (29643781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3beabbac8d8220cb7b1a7e7a740a6093ace46da9614c60eea0c8550523f8ae7`  
		Last Modified: Tue, 15 Nov 2022 13:30:29 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52dbfb4c8fb2b19fd7349f312648e32bc6e981f7f8dbf19aca371ec4ce65dee6`  
		Last Modified: Mon, 05 Dec 2022 20:53:24 GMT  
		Size: 8.0 MB (8015807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ffb4a954672659dc6e433a6d2392324f74de254a041a2ef7cc8e0bcbceb1044`  
		Last Modified: Mon, 05 Dec 2022 20:53:22 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
