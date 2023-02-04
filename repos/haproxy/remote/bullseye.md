## `haproxy:bullseye`

```console
$ docker pull haproxy@sha256:d5a8cd59870899f4f83af27c6e0f31afcc40a494444ecd5b5ec333d81826e233
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

### `haproxy:bullseye` - linux; amd64

```console
$ docker pull haproxy@sha256:1bde77ea8d4489e2902f05090c5100ee9c0f0d2a2cb55148c31c6a7ef8749713
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.6 MB (39622145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9a9dda01072fb27de01a90c14dda10ff0661644663a2832203dc2849312e31d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:44 GMT
ADD file:e2398d0bf516084b2b37ba1bb76b86d56e66999831df692461679fbd6a5d8eb6 in / 
# Wed, 11 Jan 2023 02:34:44 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 05:25:49 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Sat, 21 Jan 2023 00:24:35 GMT
ENV HAPROXY_VERSION=2.7.2
# Sat, 21 Jan 2023 00:24:35 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.7/src/haproxy-2.7.2.tar.gz
# Sat, 21 Jan 2023 00:24:35 GMT
ENV HAPROXY_SHA256=63bc6ec0302d0ebbe1fa769c19606640de834ac8cb07447b80799cb563dc0f3f
# Sat, 21 Jan 2023 00:25:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 21 Jan 2023 00:25:15 GMT
STOPSIGNAL SIGUSR1
# Sat, 21 Jan 2023 00:25:15 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 21 Jan 2023 00:25:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Jan 2023 00:25:16 GMT
USER haproxy
# Sat, 21 Jan 2023 00:25:16 GMT
WORKDIR /var/lib/haproxy
# Sat, 21 Jan 2023 00:25:16 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:8740c948ffd4c816ea7ca963f99ca52f4788baa23f228da9581a9ea2edd3fcd7`  
		Last Modified: Wed, 11 Jan 2023 02:39:07 GMT  
		Size: 31.4 MB (31396972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:388da74d11798c19fd297a8e94a8271bf0db6bd74e25cb04e333f0cdd635fb4f`  
		Last Modified: Wed, 11 Jan 2023 05:31:45 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cbaffeba70dc94b72cbff3b45a1182a42c3d98c6c50708b7eddb323471cd45f`  
		Last Modified: Sat, 21 Jan 2023 00:27:34 GMT  
		Size: 8.2 MB (8223285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a06058dcc4df43f5fff47bd51855750c6a5c4ebb305f78c672a78de59a4bc3f`  
		Last Modified: Sat, 21 Jan 2023 00:27:32 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:bullseye` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:359eddd26b20adae7982bbd366bc1da7ea688bbb8e2177f92c64458f11add055
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36977171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82ec3cc0ba6849d3084b3452ae6051334b4ffb9ea56a93cdde2321c16f0e3633`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 04 Feb 2023 02:46:38 GMT
ADD file:ce468627e54d8d1c839cea8ab62e505f612298fd97d50e189293fcfcc6af03a5 in / 
# Sat, 04 Feb 2023 02:46:38 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 03:54:55 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Sat, 04 Feb 2023 03:55:39 GMT
ENV HAPROXY_VERSION=2.7.2
# Sat, 04 Feb 2023 03:55:39 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.7/src/haproxy-2.7.2.tar.gz
# Sat, 04 Feb 2023 03:55:39 GMT
ENV HAPROXY_SHA256=63bc6ec0302d0ebbe1fa769c19606640de834ac8cb07447b80799cb563dc0f3f
# Sat, 04 Feb 2023 03:56:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 04 Feb 2023 03:56:15 GMT
STOPSIGNAL SIGUSR1
# Sat, 04 Feb 2023 03:56:15 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 04 Feb 2023 03:56:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Feb 2023 03:56:16 GMT
USER haproxy
# Sat, 04 Feb 2023 03:56:16 GMT
WORKDIR /var/lib/haproxy
# Sat, 04 Feb 2023 03:56:16 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:83735a64f458d40820e4310d632e8bb1dc888f6c25114496be3ce431b5f21d5d`  
		Last Modified: Sat, 04 Feb 2023 02:51:43 GMT  
		Size: 28.9 MB (28898637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67887e9006269224a7c47f481d22c35f172f94e31a3c36801ac590d8b2514219`  
		Last Modified: Sat, 04 Feb 2023 04:00:53 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578796f90873cceac845b6c8251bbacc60ed5e5367c6d0ed4d8c2ee37f418096`  
		Last Modified: Sat, 04 Feb 2023 04:01:13 GMT  
		Size: 8.1 MB (8076678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:769e3bd6e9c1693be723301c77eb55faf56670652d99495f952a31277655fada`  
		Last Modified: Sat, 04 Feb 2023 04:01:12 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:bullseye` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:cc43d5b0cf2af69528d9f753480b7579c56d07f64bbb47e2f3861782530f2d5e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 MB (34490461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca9918751e615f2bb504c852331fc8b2eb498634560b2e07b1bbe40201c15642`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 11 Jan 2023 04:00:36 GMT
ADD file:3fb94bfd628f3ebd91db74501bd297a817977cc066664f0fa342442b3352e0be in / 
# Wed, 11 Jan 2023 04:00:37 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 06:24:37 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Sat, 21 Jan 2023 00:58:04 GMT
ENV HAPROXY_VERSION=2.7.2
# Sat, 21 Jan 2023 00:58:04 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.7/src/haproxy-2.7.2.tar.gz
# Sat, 21 Jan 2023 00:58:04 GMT
ENV HAPROXY_SHA256=63bc6ec0302d0ebbe1fa769c19606640de834ac8cb07447b80799cb563dc0f3f
# Sat, 21 Jan 2023 00:58:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 21 Jan 2023 00:58:50 GMT
STOPSIGNAL SIGUSR1
# Sat, 21 Jan 2023 00:58:50 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 21 Jan 2023 00:58:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Jan 2023 00:58:50 GMT
USER haproxy
# Sat, 21 Jan 2023 00:58:51 GMT
WORKDIR /var/lib/haproxy
# Sat, 21 Jan 2023 00:58:51 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:330ad28688ae3fa5f3b241fef3efd076299bec9874e0597b1c16dcf8a165a53d`  
		Last Modified: Wed, 11 Jan 2023 04:07:49 GMT  
		Size: 26.6 MB (26559488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2275ee8ed371a164ee8f7818a8a18f492cc5d05735ea9855619d210fb7dad6`  
		Last Modified: Wed, 11 Jan 2023 06:32:12 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5806f0deaaf712a50672f12765e7a2a3eb379f7131ca0789f991f767fd08841b`  
		Last Modified: Sat, 21 Jan 2023 01:03:48 GMT  
		Size: 7.9 MB (7929112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a289bd8441694af0b0e12e67e9d39c1dfdd14a6eb5cb2aa65bd565d5448fb39b`  
		Last Modified: Sat, 21 Jan 2023 01:03:46 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:bullseye` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:33631f96c53368c8671229f809a406ca44deabd401e72d0feb0d57954333cf06
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.2 MB (38225311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a5b2f2f93609db61bd5d2ae7c8cb81ef1ecec82cdd8005967133665484cc00a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:37 GMT
ADD file:f613775c59ebd3ca219dc6bbad83115eb74bbbc1980ca4b63e7cb8ab3fa364e4 in / 
# Sat, 04 Feb 2023 06:17:37 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 07:57:19 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Sat, 04 Feb 2023 07:57:54 GMT
ENV HAPROXY_VERSION=2.7.2
# Sat, 04 Feb 2023 07:57:54 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.7/src/haproxy-2.7.2.tar.gz
# Sat, 04 Feb 2023 07:57:54 GMT
ENV HAPROXY_SHA256=63bc6ec0302d0ebbe1fa769c19606640de834ac8cb07447b80799cb563dc0f3f
# Sat, 04 Feb 2023 07:58:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 04 Feb 2023 07:58:18 GMT
STOPSIGNAL SIGUSR1
# Sat, 04 Feb 2023 07:58:19 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 04 Feb 2023 07:58:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Feb 2023 07:58:19 GMT
USER haproxy
# Sat, 04 Feb 2023 07:58:19 GMT
WORKDIR /var/lib/haproxy
# Sat, 04 Feb 2023 07:58:19 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:f79f8cc5c20d534298dd6317333f38b7691da6d66e063ff10699727982c852be`  
		Last Modified: Sat, 04 Feb 2023 06:21:25 GMT  
		Size: 30.0 MB (30044792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7857d415d1ad28288e04b6fbe3a678f69cecaff2c6f1e9478c0bb0176f8889`  
		Last Modified: Sat, 04 Feb 2023 08:01:52 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac057073438f4139858d49c811f5f857b9bad5e84a37c1cb90cbfa7c17697b4e`  
		Last Modified: Sat, 04 Feb 2023 08:02:09 GMT  
		Size: 8.2 MB (8178630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a2aa1c3ae5f8b7c460fd838abf5a2e1d02789e19af7e6a250879f56e0cd3d2`  
		Last Modified: Sat, 04 Feb 2023 08:02:08 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:bullseye` - linux; 386

```console
$ docker pull haproxy@sha256:fbf42732afb39c35637226985f12498c79e1eefb98c6109424b574faaa1271bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.4 MB (40369408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a83aaf57bd033e9b2c7cb2add371a12200d2f6b42449b56416d43d45a52cdf0c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 11 Jan 2023 03:16:08 GMT
ADD file:68afc7c49a947a9fb253ffeba9950cdc39e241f8a5cf0133043cfc612447f597 in / 
# Wed, 11 Jan 2023 03:16:08 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 05:25:11 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Sat, 21 Jan 2023 00:40:49 GMT
ENV HAPROXY_VERSION=2.7.2
# Sat, 21 Jan 2023 00:40:50 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.7/src/haproxy-2.7.2.tar.gz
# Sat, 21 Jan 2023 00:40:51 GMT
ENV HAPROXY_SHA256=63bc6ec0302d0ebbe1fa769c19606640de834ac8cb07447b80799cb563dc0f3f
# Sat, 21 Jan 2023 00:41:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 21 Jan 2023 00:41:28 GMT
STOPSIGNAL SIGUSR1
# Sat, 21 Jan 2023 00:41:30 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 21 Jan 2023 00:41:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Jan 2023 00:41:31 GMT
USER haproxy
# Sat, 21 Jan 2023 00:41:32 GMT
WORKDIR /var/lib/haproxy
# Sat, 21 Jan 2023 00:41:33 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:165165b78fad597abd0883f40adcaa0edcfe981a358deea181323680a07b7011`  
		Last Modified: Wed, 11 Jan 2023 03:22:01 GMT  
		Size: 32.4 MB (32375738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:797b3b48eb3b2c367079f9bdc9b2c216f5b1234659a117b052bef2fd0f680779`  
		Last Modified: Wed, 11 Jan 2023 05:33:25 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f1bbb42228e47c4d1a55a76e349820842b29a67752dcf45891291291b690627`  
		Last Modified: Sat, 21 Jan 2023 00:45:25 GMT  
		Size: 8.0 MB (7991929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66fd896d6bc950b8b36e8840f624e61eba895a1b43e7218d8bb57de5d668dc59`  
		Last Modified: Sat, 21 Jan 2023 00:45:24 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:bullseye` - linux; mips64le

```console
$ docker pull haproxy@sha256:9a2e0ab09413a3a697e8492c8b0ae53aaaf7cca050be0a98af461da96c16ecc0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.9 MB (37912765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdbed98d8ee4179eac1fe3ac0c0ce2d02a87405bb12fad8ea527f2b3142d213c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 04 Feb 2023 06:20:15 GMT
ADD file:03d6cf2d45a21e59975a1d17c6ca9fc83bb7a0da235873315c9c7940245beb1e in / 
# Sat, 04 Feb 2023 06:20:19 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 07:35:11 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Sat, 04 Feb 2023 07:39:20 GMT
ENV HAPROXY_VERSION=2.7.2
# Sat, 04 Feb 2023 07:39:23 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.7/src/haproxy-2.7.2.tar.gz
# Sat, 04 Feb 2023 07:39:25 GMT
ENV HAPROXY_SHA256=63bc6ec0302d0ebbe1fa769c19606640de834ac8cb07447b80799cb563dc0f3f
# Sat, 04 Feb 2023 07:42:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 04 Feb 2023 07:42:55 GMT
STOPSIGNAL SIGUSR1
# Sat, 04 Feb 2023 07:42:57 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 04 Feb 2023 07:42:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Feb 2023 07:43:02 GMT
USER haproxy
# Sat, 04 Feb 2023 07:43:04 GMT
WORKDIR /var/lib/haproxy
# Sat, 04 Feb 2023 07:43:07 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:aedd2a952aead0f89a308f23f44377263665bf76192d5542abd66473ea799d44`  
		Last Modified: Sat, 04 Feb 2023 06:28:25 GMT  
		Size: 29.6 MB (29619892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:660d4c7895ab03cc4087c0463ccf3d6817013b6f73295c9dbec5e8b2f9f3b889`  
		Last Modified: Sat, 04 Feb 2023 07:58:47 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75432c335197920c26d9f8dd8421becc9b01bbb8d11ef24d88fab50a5c179c95`  
		Last Modified: Sat, 04 Feb 2023 07:59:12 GMT  
		Size: 8.3 MB (8291124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f4d99a438c91e88c877501c5cebe21ca339fa6a59585cdaa4a3879d303e4e2`  
		Last Modified: Sat, 04 Feb 2023 07:59:06 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:bullseye` - linux; ppc64le

```console
$ docker pull haproxy@sha256:7f3b761279627feaca0a30a6d680ed8ebfe791620bbd2767c87da7364b1e085b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.9 MB (43875389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:361be8551ce1ddf00ca1482a2d6d253fdb084e1a9aee74a9f869fa4cb862dbd1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Wed, 11 Jan 2023 03:49:30 GMT
ADD file:3c7553fb5eda606d574ff6c08bc2213f9e6a68910043fe3087e4c1a04b65a18e in / 
# Wed, 11 Jan 2023 03:49:32 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 04:48:01 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Sat, 21 Jan 2023 00:29:34 GMT
ENV HAPROXY_VERSION=2.7.2
# Sat, 21 Jan 2023 00:29:34 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.7/src/haproxy-2.7.2.tar.gz
# Sat, 21 Jan 2023 00:29:35 GMT
ENV HAPROXY_SHA256=63bc6ec0302d0ebbe1fa769c19606640de834ac8cb07447b80799cb563dc0f3f
# Sat, 21 Jan 2023 00:30:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 21 Jan 2023 00:30:29 GMT
STOPSIGNAL SIGUSR1
# Sat, 21 Jan 2023 00:30:29 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 21 Jan 2023 00:30:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Jan 2023 00:30:30 GMT
USER haproxy
# Sat, 21 Jan 2023 00:30:31 GMT
WORKDIR /var/lib/haproxy
# Sat, 21 Jan 2023 00:30:32 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:bbf81328aca90b7ddb122fc175443f5323674a9e51bbb00d5b1d683ef0b858f4`  
		Last Modified: Wed, 11 Jan 2023 03:55:33 GMT  
		Size: 35.3 MB (35268773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa2392a85792bd7b764b84bcf96f9096ca395c121dbf0f906598cd8eac20060`  
		Last Modified: Wed, 11 Jan 2023 04:56:41 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d540ea08364c78958a6ffd47169fd0d9d8236222021a9db7aa87b8c125eb68e`  
		Last Modified: Sat, 21 Jan 2023 00:34:40 GMT  
		Size: 8.6 MB (8604731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1918168865f81dcfc11a4fc31e4e3b43049413a344452fd21fb2b49d8645808c`  
		Last Modified: Sat, 21 Jan 2023 00:34:37 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:bullseye` - linux; s390x

```console
$ docker pull haproxy@sha256:653548f342999151c758911be89593703328d8748ff3b6e1e79e3ec00fbc9ffe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.8 MB (37836077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a076914e605556ce8dd8febd030297d1be338a626c5ba835e0dc679847e45d8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Sat, 04 Feb 2023 04:06:15 GMT
ADD file:29a3ecb38611dbbb6f45b2d10ad3cee60c0198429376f999e9a397f9c405820e in / 
# Sat, 04 Feb 2023 04:06:17 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 05:10:45 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Sat, 04 Feb 2023 05:11:33 GMT
ENV HAPROXY_VERSION=2.7.2
# Sat, 04 Feb 2023 05:11:34 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.7/src/haproxy-2.7.2.tar.gz
# Sat, 04 Feb 2023 05:11:34 GMT
ENV HAPROXY_SHA256=63bc6ec0302d0ebbe1fa769c19606640de834ac8cb07447b80799cb563dc0f3f
# Sat, 04 Feb 2023 05:12:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Sat, 04 Feb 2023 05:12:07 GMT
STOPSIGNAL SIGUSR1
# Sat, 04 Feb 2023 05:12:07 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Sat, 04 Feb 2023 05:12:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Feb 2023 05:12:07 GMT
USER haproxy
# Sat, 04 Feb 2023 05:12:08 GMT
WORKDIR /var/lib/haproxy
# Sat, 04 Feb 2023 05:12:08 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:7c6fe4d1ef15da79055e0a71952e1a38f799d4f36e9acebdb1ec1512651b39f1`  
		Last Modified: Sat, 04 Feb 2023 04:10:27 GMT  
		Size: 29.6 MB (29629678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca520a29cb99b74e94a405adeeb2bd89dbd03a064edd1fbb587c1221eeba11c`  
		Last Modified: Sat, 04 Feb 2023 05:17:28 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad38b9109bee5f5045ee35d8f48d27db10176e4ae99f7adc05dcfc4cba063759`  
		Last Modified: Sat, 04 Feb 2023 05:17:44 GMT  
		Size: 8.2 MB (8204513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98c113fad3b3cc4352875d15fa0260f483c6133b520bcff04dff4431e91ed353`  
		Last Modified: Sat, 04 Feb 2023 05:17:42 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
