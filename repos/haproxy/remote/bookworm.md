## `haproxy:bookworm`

```console
$ docker pull haproxy@sha256:098af53aab6dea259f722d698c4d2068d952c40e7035642b9a36efb96c5b4cd8
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 16
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v5
	-	unknown; unknown
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown
	-	linux; mips64le
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `haproxy:bookworm` - linux; amd64

```console
$ docker pull haproxy@sha256:488bba7aa0bc1315458ee1ae38e1fdc448d3725b4d8e522ddd23e652a9dcd6fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.3 MB (46322295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7b500699a224e5f02e2aa308de296433c036725ecebaf924c47b99986828a8a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:37 GMT
ADD file:d261a6f6921593f1e0b3f472ab1b1822e2c6deb0b369200f0b3370556bfad017 in / 
# Tue, 21 Nov 2023 05:21:37 GMT
CMD ["bash"]
# Fri, 15 Dec 2023 18:13:27 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy # buildkit
# Fri, 15 Dec 2023 18:13:27 GMT
ENV HAPROXY_VERSION=2.9.1
# Fri, 15 Dec 2023 18:13:27 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.9/src/haproxy-2.9.1.tar.gz
# Fri, 15 Dec 2023 18:13:27 GMT
ENV HAPROXY_SHA256=d5801c772aab9c43f40964b7b33b4388d14b5b45750be4d2671785863cdb9f1c
# Fri, 15 Dec 2023 18:13:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v # buildkit
# Fri, 15 Dec 2023 18:13:27 GMT
STOPSIGNAL SIGUSR1
# Fri, 15 Dec 2023 18:13:27 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 15 Dec 2023 18:13:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 15 Dec 2023 18:13:27 GMT
USER haproxy
# Fri, 15 Dec 2023 18:13:27 GMT
WORKDIR /var/lib/haproxy
# Fri, 15 Dec 2023 18:13:27 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:1f7ce2fa46ab3942feabee654933948821303a5a821789dddab2d8c3df59e227`  
		Last Modified: Tue, 21 Nov 2023 05:25:58 GMT  
		Size: 29.1 MB (29149908 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:49005ac079ee266ed146a0e4a7c31eefa22d00c64e77de0863fffca1e97b7634`  
		Last Modified: Sat, 16 Dec 2023 00:17:40 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a15a33e475170cbc02c0d430f2d6ee86df2dacd06c9e4c51aa2bab24dfba9a11`  
		Last Modified: Sat, 16 Dec 2023 00:17:40 GMT  
		Size: 17.2 MB (17170747 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:eadfeb75011fe7da652d9a51541854ec33bcaae902518b195965d360b527c73e`  
		Last Modified: Sat, 16 Dec 2023 00:17:40 GMT  
		Size: 450.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `haproxy:bookworm` - unknown; unknown

```console
$ docker pull haproxy@sha256:21ba06dd8e3dc0064971b92422c68f1ebc3eb95a7e28743233eca132527046ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3057008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c2cd8938310a7d706658a3b186edb8f0540d868c85228a9f491651ab8ccf164`

```dockerfile
```

-	Layers:
	-	`sha256:47d64e39b6ea0555149ea2e838e53b824554ee053ea843a8b474491fb51adbbc`  
		Last Modified: Sat, 16 Dec 2023 00:17:40 GMT  
		Size: 3.0 MB (3037373 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:51d302ee0c3fce1f1f987c7957016ee5cd535c5fe92c5d383dfcabf51bc441a9`  
		Last Modified: Sat, 16 Dec 2023 00:17:40 GMT  
		Size: 19.6 KB (19635 bytes)  
		MIME: application/vnd.in-toto+json

### `haproxy:bookworm` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:47bed7fdf8ccd65a74e64e69f348e88c3cdb5ebc0f8906a0ef89572c62efb281
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.2 MB (42211388 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a47b73947b18386042c869318b616fe5580af1dcb7cfa13da90224512458bbe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 21 Nov 2023 05:00:51 GMT
ADD file:1ae8e5ac45b11d01083680b765e1fcfef9f7938f89d6f424572126fa946d8cdf in / 
# Tue, 21 Nov 2023 05:00:52 GMT
CMD ["bash"]
# Fri, 15 Dec 2023 18:13:27 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy # buildkit
# Fri, 15 Dec 2023 18:13:27 GMT
ENV HAPROXY_VERSION=2.9.1
# Fri, 15 Dec 2023 18:13:27 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.9/src/haproxy-2.9.1.tar.gz
# Fri, 15 Dec 2023 18:13:27 GMT
ENV HAPROXY_SHA256=d5801c772aab9c43f40964b7b33b4388d14b5b45750be4d2671785863cdb9f1c
# Fri, 15 Dec 2023 18:13:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v # buildkit
# Fri, 15 Dec 2023 18:13:27 GMT
STOPSIGNAL SIGUSR1
# Fri, 15 Dec 2023 18:13:27 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 15 Dec 2023 18:13:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 15 Dec 2023 18:13:27 GMT
USER haproxy
# Fri, 15 Dec 2023 18:13:27 GMT
WORKDIR /var/lib/haproxy
# Fri, 15 Dec 2023 18:13:27 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:f476aef5b6e1122850e68c81ef06fc2df17e968961b060483b4d2fb33018aae3`  
		Last Modified: Tue, 21 Nov 2023 05:03:55 GMT  
		Size: 26.9 MB (26922153 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d8aefe895d3d4324e43b84f8c3e269de047afe014846b16bed21ddcb1d9dd713`  
		Last Modified: Wed, 13 Dec 2023 22:55:07 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a0a8e3cf8b3ec5fd633e63500dfa52ce26c08ffb7c40b54d4f44e25375cb7862`  
		Last Modified: Sat, 16 Dec 2023 00:20:57 GMT  
		Size: 15.3 MB (15287590 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dea1cfadc6453d498881c18c065dcf91ef2fd40f1dfc545f9a8876630eb85056`  
		Last Modified: Sat, 16 Dec 2023 00:20:56 GMT  
		Size: 449.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `haproxy:bookworm` - unknown; unknown

```console
$ docker pull haproxy@sha256:176df3f8909ea17a4a7b71b2361e62fbcc8e8c9aa19a06aa6a4185e4248087e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.4 KB (19352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b39ceb6eff1ceb2fa4d25e228623004b585c5d072ce3c45d78cb2b365d53f06`

```dockerfile
```

-	Layers:
	-	`sha256:c442a82f4819bc6b921e74510a1e51e3df75aaa9fbfb0ed148c19d11c6ca2ab0`  
		Last Modified: Sat, 16 Dec 2023 00:20:56 GMT  
		Size: 19.4 KB (19352 bytes)  
		MIME: application/vnd.in-toto+json

### `haproxy:bookworm` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:8f0e41eca7590c4c566ab953b2b732d67efa9b651f6fe62ed864b6843b95e76f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39499094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f48a98c38fef7a9c1d4721e6285e0b66500aa50d34cbdf0eab65b2a288aa40a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 21 Nov 2023 03:57:43 GMT
ADD file:b693944382a95fa47622fde77eb98f0cdeafa40261e7334bd355e00f650b6632 in / 
# Tue, 21 Nov 2023 03:57:43 GMT
CMD ["bash"]
# Fri, 15 Dec 2023 18:13:27 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy # buildkit
# Fri, 15 Dec 2023 18:13:27 GMT
ENV HAPROXY_VERSION=2.9.1
# Fri, 15 Dec 2023 18:13:27 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.9/src/haproxy-2.9.1.tar.gz
# Fri, 15 Dec 2023 18:13:27 GMT
ENV HAPROXY_SHA256=d5801c772aab9c43f40964b7b33b4388d14b5b45750be4d2671785863cdb9f1c
# Fri, 15 Dec 2023 18:13:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v # buildkit
# Fri, 15 Dec 2023 18:13:27 GMT
STOPSIGNAL SIGUSR1
# Fri, 15 Dec 2023 18:13:27 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 15 Dec 2023 18:13:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 15 Dec 2023 18:13:27 GMT
USER haproxy
# Fri, 15 Dec 2023 18:13:27 GMT
WORKDIR /var/lib/haproxy
# Fri, 15 Dec 2023 18:13:27 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:b4ce590529bbcf84326048a22fce76fcfcb5c60af5519debd7935a74c1e9126e`  
		Last Modified: Tue, 21 Nov 2023 04:01:50 GMT  
		Size: 24.7 MB (24748925 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c1fb8e4a403cba6d91c3d502a36c0fb3bf163db98d6ad2aadd4a9a47216e3349`  
		Last Modified: Wed, 13 Dec 2023 23:04:14 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0339c04f565f964335ce2bdb52901d9011aac15df635f8b0578ad896ed36232d`  
		Last Modified: Sat, 16 Dec 2023 00:32:54 GMT  
		Size: 14.7 MB (14748525 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b694cbe162eb9ace960ba1a46fbbc332b1e8708ee8c05a31bc3eaf1cd64e35b2`  
		Last Modified: Sat, 16 Dec 2023 00:32:53 GMT  
		Size: 449.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `haproxy:bookworm` - unknown; unknown

```console
$ docker pull haproxy@sha256:03cd6644e7e3341992455535c3c1bdb353a3c4becd2367d1d08517566c0e307a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3031498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3d100bfbbf1ba80e015d15452a0b4d3020b400b8aa9df46d8b2086a2751d4a1`

```dockerfile
```

-	Layers:
	-	`sha256:b544457979baa501046f87f7b9a29a55daa0676cc480238d09ecbf074bb591d9`  
		Last Modified: Sat, 16 Dec 2023 00:32:53 GMT  
		Size: 3.0 MB (3011931 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:1c3a780b8ee288d46b63ac924e2aa3a79b342f30ca4389f710f25f1473e6eef6`  
		Last Modified: Sat, 16 Dec 2023 00:32:53 GMT  
		Size: 19.6 KB (19567 bytes)  
		MIME: application/vnd.in-toto+json

### `haproxy:bookworm` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:a4df7d0a276955b17cc26cfe952bb4069a8f53188ab1a6d1d1caeba260ed98bb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.2 MB (45182119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a01b003b1a9f7ec8cdfd5a5d53d6e224fecb2939081d48b4ac139638215d6f0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:06 GMT
ADD file:869c7d0747a17c53715581a2e862992eb8516c7f45f167821dfa80966a4870d1 in / 
# Tue, 21 Nov 2023 06:27:06 GMT
CMD ["bash"]
# Mon, 11 Dec 2023 23:56:16 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy # buildkit
# Mon, 11 Dec 2023 23:56:16 GMT
ENV HAPROXY_VERSION=2.9.0
# Mon, 11 Dec 2023 23:56:16 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.9/src/haproxy-2.9.0.tar.gz
# Mon, 11 Dec 2023 23:56:16 GMT
ENV HAPROXY_SHA256=fba18acd1a46337fe20ae07c816c2496c8602b80a1bc9ff3768d4caa5fb80eab
# Mon, 11 Dec 2023 23:56:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v # buildkit
# Mon, 11 Dec 2023 23:56:16 GMT
STOPSIGNAL SIGUSR1
# Mon, 11 Dec 2023 23:56:16 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 11 Dec 2023 23:56:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Dec 2023 23:56:16 GMT
USER haproxy
# Mon, 11 Dec 2023 23:56:16 GMT
WORKDIR /var/lib/haproxy
# Mon, 11 Dec 2023 23:56:16 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:2c6d21737d8318aa15c4cc838475029a5efc36c0429e3d8da80d97d0b96d9aaf`  
		Last Modified: Tue, 21 Nov 2023 06:30:30 GMT  
		Size: 29.2 MB (29179277 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cf6288c418af0a13c3069d6ec38e11c277c8f5f584c19250da321fd2c14f2c40`  
		Last Modified: Wed, 13 Dec 2023 23:06:02 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:59831c6a8beac00e6973691b9fdb69a2d253d9ff34056c8a454a1272447b568f`  
		Last Modified: Wed, 13 Dec 2023 23:06:51 GMT  
		Size: 16.0 MB (16001197 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a550ffa48b09d94811204fff2d4011d9627dc844f972be4c3bae39d9c3414c55`  
		Last Modified: Wed, 13 Dec 2023 23:06:50 GMT  
		Size: 451.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `haproxy:bookworm` - unknown; unknown

```console
$ docker pull haproxy@sha256:e5646db8422c8788e05ee44dd472453536534a867ee3516d73123ea9b956d4c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3032034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae3f4332163e459cec20e9db85c683e6c2d1c04ad50b90ffe9644ad8bd62beae`

```dockerfile
```

-	Layers:
	-	`sha256:8f1229b4bf55a6b489b0c1caf81dced3bf75faa1096f45c2dd80db5f5467fa1d`  
		Last Modified: Wed, 13 Dec 2023 23:06:51 GMT  
		Size: 3.0 MB (3012552 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:0118d25aef8fa32a4fe0763e89187050d9d4bab3087618fad8c06b6f075e0274`  
		Last Modified: Wed, 13 Dec 2023 23:06:50 GMT  
		Size: 19.5 KB (19482 bytes)  
		MIME: application/vnd.in-toto+json

### `haproxy:bookworm` - linux; 386

```console
$ docker pull haproxy@sha256:78badbe4f6d9218c3c9d796185df3f7b01d3a21ef5b0d38cf9a608bb2577e8b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.6 MB (46564282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22d8a901b4c92f7591c12c52e1cd6318bd30060beac190faf6acfb1bacb3aad9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 21 Nov 2023 04:39:53 GMT
ADD file:930e1b9d85b6927c4d3046f7c75de2f3bfc6ec29100c314d0ab2b780ea30e962 in / 
# Tue, 21 Nov 2023 04:39:53 GMT
CMD ["bash"]
# Fri, 15 Dec 2023 18:13:27 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy # buildkit
# Fri, 15 Dec 2023 18:13:27 GMT
ENV HAPROXY_VERSION=2.9.1
# Fri, 15 Dec 2023 18:13:27 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.9/src/haproxy-2.9.1.tar.gz
# Fri, 15 Dec 2023 18:13:27 GMT
ENV HAPROXY_SHA256=d5801c772aab9c43f40964b7b33b4388d14b5b45750be4d2671785863cdb9f1c
# Fri, 15 Dec 2023 18:13:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v # buildkit
# Fri, 15 Dec 2023 18:13:27 GMT
STOPSIGNAL SIGUSR1
# Fri, 15 Dec 2023 18:13:27 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 15 Dec 2023 18:13:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 15 Dec 2023 18:13:27 GMT
USER haproxy
# Fri, 15 Dec 2023 18:13:27 GMT
WORKDIR /var/lib/haproxy
# Fri, 15 Dec 2023 18:13:27 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c0734eabce8885d8904dbd11b77aa97c2d2b04bc8e2af9e89d47c4bda590dd8e`  
		Last Modified: Tue, 21 Nov 2023 04:44:34 GMT  
		Size: 30.2 MB (30164109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:661b6c13acf500b8252c207bc17e8a35df633143e19b3c5d17373e7e18718ccd`  
		Last Modified: Sat, 16 Dec 2023 00:17:56 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ad633a146fcb6e7da84732d6e0f5668e76387038d7624c60d3e408aa7e696bce`  
		Last Modified: Sat, 16 Dec 2023 00:17:57 GMT  
		Size: 16.4 MB (16398533 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0b536ca22ff00ecd405fe631eef64c73eea9ff5d9bd88842595ab901193bab6c`  
		Last Modified: Sat, 16 Dec 2023 00:17:56 GMT  
		Size: 449.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `haproxy:bookworm` - unknown; unknown

```console
$ docker pull haproxy@sha256:6d450f939f1c67e32c7a7919bef8e8bd15c39f9e982dc1cffaf98d39bdaa7403
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.4 KB (19379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba2f5348c427ae5131105442e351395a00b2cdf4884d4d416a62d2d8a6daae3f`

```dockerfile
```

-	Layers:
	-	`sha256:f0318cf699004bc5e7730bb8afb12f05d8e17823724b32161ee63ac7cdac9652`  
		Last Modified: Sat, 16 Dec 2023 00:17:56 GMT  
		Size: 19.4 KB (19379 bytes)  
		MIME: application/vnd.in-toto+json

### `haproxy:bookworm` - linux; mips64le

```console
$ docker pull haproxy@sha256:36dea2f127a0340787fd792a13877fef2b239dd3cf7db3abb8281827e0e69b34
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.1 MB (45135143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a85ca92577d55d67ed9f49b2dad5e89bdc0f10b7fd36e43d795e50c3c6c8755`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 21 Nov 2023 04:09:50 GMT
ADD file:e093749192323dc72b60a8440ddba26c415586f618b5e107fa264ba5eb2ca7ba in / 
# Tue, 21 Nov 2023 04:09:54 GMT
CMD ["bash"]
# Fri, 15 Dec 2023 18:13:27 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy # buildkit
# Fri, 15 Dec 2023 18:13:27 GMT
ENV HAPROXY_VERSION=2.9.1
# Fri, 15 Dec 2023 18:13:27 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.9/src/haproxy-2.9.1.tar.gz
# Fri, 15 Dec 2023 18:13:27 GMT
ENV HAPROXY_SHA256=d5801c772aab9c43f40964b7b33b4388d14b5b45750be4d2671785863cdb9f1c
# Fri, 15 Dec 2023 18:13:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v # buildkit
# Fri, 15 Dec 2023 18:13:27 GMT
STOPSIGNAL SIGUSR1
# Fri, 15 Dec 2023 18:13:27 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 15 Dec 2023 18:13:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 15 Dec 2023 18:13:27 GMT
USER haproxy
# Fri, 15 Dec 2023 18:13:27 GMT
WORKDIR /var/lib/haproxy
# Fri, 15 Dec 2023 18:13:27 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:ebdff2138fee4a3ec27560ab1353dc51c12c2608ff721f5db3d24104872b702a`  
		Last Modified: Tue, 21 Nov 2023 04:20:35 GMT  
		Size: 29.1 MB (29141984 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d44b3e0124156f133404ff7cf7b849fab508d9164a968d740b37ecf2bafa3969`  
		Last Modified: Wed, 13 Dec 2023 22:59:17 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:994e49bc03056a687e66436536d3b542f5f94a36aef0d96e8be9c0a12bb4b2a6`  
		Last Modified: Sat, 16 Dec 2023 00:24:53 GMT  
		Size: 16.0 MB (15991512 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8743cfffbc48038738559a29b39feeca432a2fac69fdfb335d888064296afa38`  
		Last Modified: Sat, 16 Dec 2023 00:24:51 GMT  
		Size: 451.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `haproxy:bookworm` - unknown; unknown

```console
$ docker pull haproxy@sha256:cae00d8f73d8960d5d57c2ad464e4636a0b2f667a9bc03185883f9f93caf1ba7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.3 KB (19331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7ccd79f9277a7b7f6b0f47f0f30ea8d4a64a975eda40dedcfecab544cd20f4b`

```dockerfile
```

-	Layers:
	-	`sha256:f9481745835ebb9e409ed145409383ccd9b20e84e026a4650828fdae08824841`  
		Last Modified: Sat, 16 Dec 2023 00:24:51 GMT  
		Size: 19.3 KB (19331 bytes)  
		MIME: application/vnd.in-toto+json

### `haproxy:bookworm` - linux; ppc64le

```console
$ docker pull haproxy@sha256:f00266c2b8544299863a32abda14eda8b9393906f9402b1c5e9e0f5958468bc1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.8 MB (50846844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc7184f9d2c596b28198cc6dae4a8a9718ba4fe8c74ef2db24fb6452834fe664`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:14 GMT
ADD file:8b22a531b6611a1e63dfc20e4e2931592e2d821bd4b64c4b2810bb9a36640c02 in / 
# Tue, 21 Nov 2023 04:24:16 GMT
CMD ["bash"]
# Fri, 15 Dec 2023 18:13:27 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy # buildkit
# Fri, 15 Dec 2023 18:13:27 GMT
ENV HAPROXY_VERSION=2.9.1
# Fri, 15 Dec 2023 18:13:27 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.9/src/haproxy-2.9.1.tar.gz
# Fri, 15 Dec 2023 18:13:27 GMT
ENV HAPROXY_SHA256=d5801c772aab9c43f40964b7b33b4388d14b5b45750be4d2671785863cdb9f1c
# Fri, 15 Dec 2023 18:13:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v # buildkit
# Fri, 15 Dec 2023 18:13:27 GMT
STOPSIGNAL SIGUSR1
# Fri, 15 Dec 2023 18:13:27 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 15 Dec 2023 18:13:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 15 Dec 2023 18:13:27 GMT
USER haproxy
# Fri, 15 Dec 2023 18:13:27 GMT
WORKDIR /var/lib/haproxy
# Fri, 15 Dec 2023 18:13:27 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:c570d04e61d8e35a3c8f12179d048d701451f97f9cf2099ea3e3738512dbf062`  
		Last Modified: Tue, 21 Nov 2023 04:28:58 GMT  
		Size: 33.1 MB (33141607 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:acda6a68d9288a7bdea706c59122a9090ea2272b125fd07bc3d77cfaa4328f3c`  
		Last Modified: Wed, 13 Dec 2023 23:06:07 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6662a4d14442f328068a8b69720f9d627372536bf6d36f227ed39dc0a1a01eb6`  
		Last Modified: Sat, 16 Dec 2023 00:29:42 GMT  
		Size: 17.7 MB (17703585 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:21d8f1a814146e56cbbc5723299eeaaafe8901a557edb8297bd5d8c9bf729caf`  
		Last Modified: Sat, 16 Dec 2023 00:29:41 GMT  
		Size: 451.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `haproxy:bookworm` - unknown; unknown

```console
$ docker pull haproxy@sha256:3e2a691b3e37145433debec61695478582a0e371cc27584ef643eee7716c727b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3045418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d127ec493ac4d782a34a23dec221a6566466b05f071739de08dbabb1a95a19c`

```dockerfile
```

-	Layers:
	-	`sha256:b6eba0d0ffc92899d931a67ca7997f006cf039852c5494d210b893e000e99b40`  
		Last Modified: Sat, 16 Dec 2023 00:29:41 GMT  
		Size: 3.0 MB (3025901 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:a77f86070ecb657325092ef08f3645803971729e49b0edbb0fb0daa0700a3360`  
		Last Modified: Sat, 16 Dec 2023 00:29:41 GMT  
		Size: 19.5 KB (19517 bytes)  
		MIME: application/vnd.in-toto+json

### `haproxy:bookworm` - linux; s390x

```console
$ docker pull haproxy@sha256:aea6dc515011a012680678ca9e252522d26d93342d198bb1565e816c3f72d2f8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43151912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffe990db52d4429298e32e310a0318a6b2aa8c5d07a1bfa88b1e0038f6766367`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 21 Nov 2023 05:04:35 GMT
ADD file:c33fa9fdde73983850798b6eb1cd062e0398109d1d773e6a937fead7475c8efc in / 
# Tue, 21 Nov 2023 05:04:41 GMT
CMD ["bash"]
# Mon, 11 Dec 2023 23:56:16 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy # buildkit
# Mon, 11 Dec 2023 23:56:16 GMT
ENV HAPROXY_VERSION=2.9.0
# Mon, 11 Dec 2023 23:56:16 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.9/src/haproxy-2.9.0.tar.gz
# Mon, 11 Dec 2023 23:56:16 GMT
ENV HAPROXY_SHA256=fba18acd1a46337fe20ae07c816c2496c8602b80a1bc9ff3768d4caa5fb80eab
# Mon, 11 Dec 2023 23:56:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v # buildkit
# Mon, 11 Dec 2023 23:56:16 GMT
STOPSIGNAL SIGUSR1
# Mon, 11 Dec 2023 23:56:16 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 11 Dec 2023 23:56:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 Dec 2023 23:56:16 GMT
USER haproxy
# Mon, 11 Dec 2023 23:56:16 GMT
WORKDIR /var/lib/haproxy
# Mon, 11 Dec 2023 23:56:16 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:6daa625e5a040476e253e7acd0befa74254a4865ec836d6334a544d82a21d4be`  
		Last Modified: Tue, 21 Nov 2023 05:10:21 GMT  
		Size: 27.5 MB (27512885 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9e1298c459693ebf8ee348c82fe82bec5c7f181a85eaefc3efa1cec1cb4df825`  
		Last Modified: Wed, 13 Dec 2023 22:56:02 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8619515d365401ce96b567626855423c5ed82f4e6b22723ec6e8c74ddcf3f845`  
		Last Modified: Wed, 13 Dec 2023 22:57:10 GMT  
		Size: 15.6 MB (15637382 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:98262e38c394ee48cfe5b46d17f9383d752a84e4673292f4df87a2cedd1fa8db`  
		Last Modified: Wed, 13 Dec 2023 22:57:10 GMT  
		Size: 450.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `haproxy:bookworm` - unknown; unknown

```console
$ docker pull haproxy@sha256:cbe822c6810394f80b913b0a2dd7521ea5c1c64e2fb50fcc56550f10275b18d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3046387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab6872504b863b5555060447a6fd944d68a3126c6bb2f85c7088da6a10fe8916`

```dockerfile
```

-	Layers:
	-	`sha256:25d1fb5321c39c5d8e0bc99cd1f0b3c1b54f9f6c383bb2db6059227067a0d317`  
		Last Modified: Wed, 13 Dec 2023 22:57:10 GMT  
		Size: 3.0 MB (3026922 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:533bad01988a33aaac065e18c848de941c0f8417991046dd666759eb3b7c3db8`  
		Last Modified: Wed, 13 Dec 2023 22:57:10 GMT  
		Size: 19.5 KB (19465 bytes)  
		MIME: application/vnd.in-toto+json
