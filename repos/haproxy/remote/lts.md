## `haproxy:lts`

```console
$ docker pull haproxy@sha256:d19bc3c72bb56be5ac512d1d0e9518b92795edc45f2b5aab01a0d71541ab19be
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

### `haproxy:lts` - linux; amd64

```console
$ docker pull haproxy@sha256:2ae6d6ec6041889bb13d485bd783afc9b4e37df19cadd264aabc63336619931d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.0 MB (45978892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:842065b5bfbe6ded24b120c18acdbca837ba465f1f6a2b95c89514158cefa306`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Mon, 11 Dec 2023 23:56:16 GMT
ADD file:ac3cd70031d35e46d86b876934946ffc8756de4de065fbc926dce642dac07ff3 in / 
# Mon, 11 Dec 2023 23:56:16 GMT
CMD ["bash"]
# Mon, 11 Dec 2023 23:56:16 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy # buildkit
# Mon, 11 Dec 2023 23:56:16 GMT
ENV HAPROXY_VERSION=2.8.5
# Mon, 11 Dec 2023 23:56:16 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.8/src/haproxy-2.8.5.tar.gz
# Mon, 11 Dec 2023 23:56:16 GMT
ENV HAPROXY_SHA256=3f5459c5a58e0b343a32eaef7ed5bed9d3fc29d8aa9e14b36c92c969fc2a60d9
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
	-	`sha256:af107e978371b6cd6339127a05502c5eacd1e6b0e9eb7b2f4aa7b6fc87e2dd81`  
		Last Modified: Tue, 19 Dec 2023 01:24:59 GMT  
		Size: 29.1 MB (29125963 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ba17d94a27e3e880866807cb379e0607be6acf8c01e22c1c2b3b74f7b27a33b9`  
		Last Modified: Tue, 19 Dec 2023 03:48:03 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:eaf6caed9510d9ef9e592a854459e916d4b90e4e2e28cc94a9b58b76ce6f721d`  
		Last Modified: Tue, 19 Dec 2023 03:48:03 GMT  
		Size: 16.9 MB (16851286 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7c461e24b579793f29fe1584f75abd442803e34ecfd0d4ca7e7e33b8519a2305`  
		Last Modified: Tue, 19 Dec 2023 03:48:03 GMT  
		Size: 449.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `haproxy:lts` - unknown; unknown

```console
$ docker pull haproxy@sha256:43a7e319cf777a06acc7857936eb0c8d851a0ae22736dcc93c5e2a45ffdd7aa4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3057092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18d3ece69bb28c798128e0f098cdd3e868405c0ec3868d3c4b75756210b2f94d`

```dockerfile
```

-	Layers:
	-	`sha256:6bd2759c1c624e82d30e492037de3da17113b5ab1eb41c4d12f9ed49c84a426f`  
		Last Modified: Tue, 19 Dec 2023 03:48:03 GMT  
		Size: 3.0 MB (3037455 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:3fb532275226a0704a670bf5bfa3b9014c5dbfc004854a1d46fc0eea1c95b296`  
		Last Modified: Tue, 19 Dec 2023 03:48:03 GMT  
		Size: 19.6 KB (19637 bytes)  
		MIME: application/vnd.in-toto+json

### `haproxy:lts` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:b6a71c60134cba60fa2a595c87051cd81bb946727e24a2db9aa1cbbeff8cf657
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.8 MB (41815743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff45d2b5f62ed057165dd399ddba0ac2beebdfac6763f936f7a8431454c7d32c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Mon, 11 Dec 2023 23:56:16 GMT
ADD file:9503ab966c9dd707eeccc7c2f633bccc94c199f8714ec4ff2c8b54dde3dbabf9 in / 
# Mon, 11 Dec 2023 23:56:16 GMT
CMD ["bash"]
# Mon, 11 Dec 2023 23:56:16 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy # buildkit
# Mon, 11 Dec 2023 23:56:16 GMT
ENV HAPROXY_VERSION=2.8.5
# Mon, 11 Dec 2023 23:56:16 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.8/src/haproxy-2.8.5.tar.gz
# Mon, 11 Dec 2023 23:56:16 GMT
ENV HAPROXY_SHA256=3f5459c5a58e0b343a32eaef7ed5bed9d3fc29d8aa9e14b36c92c969fc2a60d9
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
	-	`sha256:1ae9a2844c8c70942d2220553689b62e841cc706d77284fbfedbd770080fd699`  
		Last Modified: Tue, 19 Dec 2023 01:58:33 GMT  
		Size: 26.9 MB (26885440 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:29e46dbc80d018f67237ea6331c64f659a7b655cc2f711f63d92bfffd7058b98`  
		Last Modified: Tue, 19 Dec 2023 13:32:42 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e0b138c5c46cb3ec02a5103b5b4037aeacb1c7c8935b82a4c2cc89b0dd2dc662`  
		Last Modified: Tue, 19 Dec 2023 16:00:11 GMT  
		Size: 14.9 MB (14928659 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bb56af1676fec7737392b3ce30ff98029366aa1f4d5a8c290357c5e7db57f10c`  
		Last Modified: Tue, 19 Dec 2023 16:00:11 GMT  
		Size: 450.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `haproxy:lts` - unknown; unknown

```console
$ docker pull haproxy@sha256:f81b61d19b0f477546e546c40867b5a4b208d5b48c9fcd1775eddf08ca299fda
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.4 KB (19353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4244309142bc2c36b2ba39be3f2fd0826cfa06bb8ee402fb218663f761e46cf`

```dockerfile
```

-	Layers:
	-	`sha256:ef6fabf1745ff598cffbac6a47b1ea740abb2a0db8789a379f89bc1ed968c57d`  
		Last Modified: Tue, 19 Dec 2023 16:00:11 GMT  
		Size: 19.4 KB (19353 bytes)  
		MIME: application/vnd.in-toto+json

### `haproxy:lts` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:5a4214eaf8d029d6726e897166c1f50415394f794fcac0f02aed47e80f0d1652
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.1 MB (39106862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:accff93382de2e5b7eb7ddc43ba58112efdcbf44f11fb86c1378a703d4428d62`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Mon, 11 Dec 2023 23:56:16 GMT
ADD file:aef112919e7924ad6da32181b1df5099cd692680c104118da3a24cd4dfe55a1d in / 
# Mon, 11 Dec 2023 23:56:16 GMT
CMD ["bash"]
# Mon, 11 Dec 2023 23:56:16 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy # buildkit
# Mon, 11 Dec 2023 23:56:16 GMT
ENV HAPROXY_VERSION=2.8.5
# Mon, 11 Dec 2023 23:56:16 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.8/src/haproxy-2.8.5.tar.gz
# Mon, 11 Dec 2023 23:56:16 GMT
ENV HAPROXY_SHA256=3f5459c5a58e0b343a32eaef7ed5bed9d3fc29d8aa9e14b36c92c969fc2a60d9
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
	-	`sha256:65ab19615c01a3b542f77fadb3bd27872b6a20cba3e9269fb951de36d8fa6805`  
		Last Modified: Tue, 19 Dec 2023 02:11:52 GMT  
		Size: 24.7 MB (24718157 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:18d1e6d49217dcdd8d29ab6ff2107ef5489e07a023377e9b0543e476a249c76e`  
		Last Modified: Tue, 19 Dec 2023 21:50:54 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:393483fb6299807017aa2dba811576dd3997f10755d9018be13d21cdf5540824`  
		Last Modified: Wed, 20 Dec 2023 00:11:03 GMT  
		Size: 14.4 MB (14387061 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:190807343bde5ee4febd4f050bcfa4651d97498657e5616955acf73fa4222480`  
		Last Modified: Wed, 20 Dec 2023 00:11:02 GMT  
		Size: 449.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `haproxy:lts` - unknown; unknown

```console
$ docker pull haproxy@sha256:a9bd04b65bc107f187dd7a78444865652893295aad3244122df2f3872695654e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3031582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35f008fe92481a94e92298e30352c2bb2dbaec45cbd8ff4a0c55193e0da066d6`

```dockerfile
```

-	Layers:
	-	`sha256:539af439b227db84f22239551ffb6ccf6403635d67fa879118ede1ed9596cbeb`  
		Last Modified: Wed, 20 Dec 2023 00:11:03 GMT  
		Size: 3.0 MB (3012013 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:f74c20659b7a566e0465f2939e00cb5bd076ff0d4f4425babfb84330c98c667d`  
		Last Modified: Wed, 20 Dec 2023 00:11:03 GMT  
		Size: 19.6 KB (19569 bytes)  
		MIME: application/vnd.in-toto+json

### `haproxy:lts` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:8c47c3c64033e6bbfb203d499feb85b005ba716cf9f81e73d6a03117df5d39d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.8 MB (44784217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fc88a43171f5674a3f131a16bf82bab013948eebb648532f86dea708ef89793`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Mon, 11 Dec 2023 23:56:16 GMT
ADD file:262fd7bf0bc26e5d2a229fba52626e22b8a93beac29733acfc60e716c26e689d in / 
# Mon, 11 Dec 2023 23:56:16 GMT
CMD ["bash"]
# Mon, 11 Dec 2023 23:56:16 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy # buildkit
# Mon, 11 Dec 2023 23:56:16 GMT
ENV HAPROXY_VERSION=2.8.5
# Mon, 11 Dec 2023 23:56:16 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.8/src/haproxy-2.8.5.tar.gz
# Mon, 11 Dec 2023 23:56:16 GMT
ENV HAPROXY_SHA256=3f5459c5a58e0b343a32eaef7ed5bed9d3fc29d8aa9e14b36c92c969fc2a60d9
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
	-	`sha256:24e221e92a36ab5b0075dd156b4f2ff095532a9b0927946cf6070bb1bea208b8`  
		Last Modified: Tue, 19 Dec 2023 01:44:38 GMT  
		Size: 29.2 MB (29157269 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:16af36f4e1693c15fac473895e82e43aa472a6f4f6bd59aab5895854a1d44daa`  
		Last Modified: Wed, 20 Dec 2023 09:39:19 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:deffc2e69ef2dac8dcc93cb9ce1df75009ca3030fd1fc2acb4ffa19d69b97e8b`  
		Last Modified: Wed, 20 Dec 2023 09:42:24 GMT  
		Size: 15.6 MB (15625305 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a4a9932410f984a2869fbc4a32611370c2303b5d7a7b1b77734f665c6506a87b`  
		Last Modified: Wed, 20 Dec 2023 09:42:23 GMT  
		Size: 449.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `haproxy:lts` - unknown; unknown

```console
$ docker pull haproxy@sha256:a79a0037eb10e114862f2a1b9b29e2a260a7f4e47c8d335ead275552de0ffeb3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3032118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:546a4f9c70671cb06b98a9beddfb3dc5ee8d078a476c24559403a6426f76ee1a`

```dockerfile
```

-	Layers:
	-	`sha256:4f39d3ddfd2b1355cd5e0c495082cb95bbcaa67601f31ee6d61bf32e0c3737de`  
		Last Modified: Wed, 20 Dec 2023 09:42:23 GMT  
		Size: 3.0 MB (3012634 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:8c2e9d64dcb89be23513f29106ab95d3c68dd36369668d0043e0b1949cf2959b`  
		Last Modified: Wed, 20 Dec 2023 09:42:23 GMT  
		Size: 19.5 KB (19484 bytes)  
		MIME: application/vnd.in-toto+json

### `haproxy:lts` - linux; 386

```console
$ docker pull haproxy@sha256:07b3540f43b2836f8b1af463ebee7bfd341aa466a603359d5d15f23c05b10edf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.2 MB (46223806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:326388d07d8db7cceea1a7d05abff91960f544d7aaf1874c3517a9f536f1f285`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Mon, 11 Dec 2023 23:56:16 GMT
ADD file:6f4083d57ea9644b5a827e67b0725087a15aa428272ec223ab968bf8b4623e42 in / 
# Mon, 11 Dec 2023 23:56:16 GMT
CMD ["bash"]
# Mon, 11 Dec 2023 23:56:16 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy # buildkit
# Mon, 11 Dec 2023 23:56:16 GMT
ENV HAPROXY_VERSION=2.8.5
# Mon, 11 Dec 2023 23:56:16 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.8/src/haproxy-2.8.5.tar.gz
# Mon, 11 Dec 2023 23:56:16 GMT
ENV HAPROXY_SHA256=3f5459c5a58e0b343a32eaef7ed5bed9d3fc29d8aa9e14b36c92c969fc2a60d9
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
	-	`sha256:8d4aad22fb6a12b8cc7a78d338dfb9bc2bd6d621517b374e446f2915833ea883`  
		Last Modified: Tue, 19 Dec 2023 01:43:45 GMT  
		Size: 30.1 MB (30143863 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f07fa4650aec4756a1a7272a29e7cf815bb54462daa8926bf8cead303adea63c`  
		Last Modified: Tue, 19 Dec 2023 03:47:59 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7fb2f4d6d331c57ccf97e9ec3473fe608bf786c1c1192d4f10a8cbd6964589db`  
		Last Modified: Tue, 19 Dec 2023 03:48:03 GMT  
		Size: 16.1 MB (16078303 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3dcb29fb404abac21c73416793f70cfe50fe46fd737f485dd27c53fe38636b5f`  
		Last Modified: Tue, 19 Dec 2023 03:48:03 GMT  
		Size: 448.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `haproxy:lts` - unknown; unknown

```console
$ docker pull haproxy@sha256:b937ba485e3c13d90312e27fe476e2dd4659e4f6dea4d402436d43b062f07bd6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.4 KB (19380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3f31bc20fefee8256e074fbb4877aaf4614d6db43f47ef2f7202b91aab2e00e`

```dockerfile
```

-	Layers:
	-	`sha256:7db10a7400c79516e65ffe9101ab3e93989a28bbafb0a00badc63b891b79ea02`  
		Last Modified: Tue, 19 Dec 2023 03:48:03 GMT  
		Size: 19.4 KB (19380 bytes)  
		MIME: application/vnd.in-toto+json

### `haproxy:lts` - linux; mips64le

```console
$ docker pull haproxy@sha256:e9da97fbad6ef9fb3ce62b63ceecfcdafe823d6c4cc49202006989aceb7750e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.8 MB (44778979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b01970e0427a5e5233a99c5aca738b63d195e4661aecb3f271447a8f9e0c642c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 21 Nov 2023 04:09:50 GMT
ADD file:e093749192323dc72b60a8440ddba26c415586f618b5e107fa264ba5eb2ca7ba in / 
# Tue, 21 Nov 2023 04:09:54 GMT
CMD ["bash"]
# Mon, 11 Dec 2023 23:56:16 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy # buildkit
# Mon, 11 Dec 2023 23:56:16 GMT
ENV HAPROXY_VERSION=2.8.5
# Mon, 11 Dec 2023 23:56:16 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.8/src/haproxy-2.8.5.tar.gz
# Mon, 11 Dec 2023 23:56:16 GMT
ENV HAPROXY_SHA256=3f5459c5a58e0b343a32eaef7ed5bed9d3fc29d8aa9e14b36c92c969fc2a60d9
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
	-	`sha256:ebdff2138fee4a3ec27560ab1353dc51c12c2608ff721f5db3d24104872b702a`  
		Last Modified: Tue, 21 Nov 2023 04:20:35 GMT  
		Size: 29.1 MB (29141984 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d44b3e0124156f133404ff7cf7b849fab508d9164a968d740b37ecf2bafa3969`  
		Last Modified: Wed, 13 Dec 2023 22:59:17 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:09a05013c33f47f1aa2e65b5ac46d52111a8e65a7cae598fd48bf3c541e40ee7`  
		Last Modified: Wed, 13 Dec 2023 23:09:34 GMT  
		Size: 15.6 MB (15635349 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:33a5128c601db623008f87cc5959a7a9f2bb0196556175396e3535bc6d0715f8`  
		Last Modified: Wed, 13 Dec 2023 23:09:32 GMT  
		Size: 450.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `haproxy:lts` - unknown; unknown

```console
$ docker pull haproxy@sha256:d1666134856befb047a9bbdd0157742c69e1f8f45125c15d5b092661f05bddc5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.3 KB (19333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:402c1a2249db5c326855e06dbc872baed0b18818b605177a2fe19f98d95d81a6`

```dockerfile
```

-	Layers:
	-	`sha256:cdfde7e0a1d87073d72d732e7224d835a0bae9c10cf2e148a2d6fed0e42e04cb`  
		Last Modified: Wed, 13 Dec 2023 23:09:32 GMT  
		Size: 19.3 KB (19333 bytes)  
		MIME: application/vnd.in-toto+json

### `haproxy:lts` - linux; ppc64le

```console
$ docker pull haproxy@sha256:4d508391ed170772d54f4b4c7ca8bc9576a0350d4d36514dcc1e19cffe7183da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50460477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7c7c84ccaae03896ff18042b416ab9155eb0b88b9c6f577ee456248abe89ecc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Mon, 11 Dec 2023 23:56:16 GMT
ADD file:ca1db68689e0b0388337ba450ad2c8e79c159c6b78f5aa6d3ff2b89b8d7edc93 in / 
# Mon, 11 Dec 2023 23:56:16 GMT
CMD ["bash"]
# Mon, 11 Dec 2023 23:56:16 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy # buildkit
# Mon, 11 Dec 2023 23:56:16 GMT
ENV HAPROXY_VERSION=2.8.5
# Mon, 11 Dec 2023 23:56:16 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.8/src/haproxy-2.8.5.tar.gz
# Mon, 11 Dec 2023 23:56:16 GMT
ENV HAPROXY_SHA256=3f5459c5a58e0b343a32eaef7ed5bed9d3fc29d8aa9e14b36c92c969fc2a60d9
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
	-	`sha256:fc9b8f5eec3aa37ab3aace05165427479352f290d53904cea87dca6349633a09`  
		Last Modified: Tue, 19 Dec 2023 01:26:19 GMT  
		Size: 33.1 MB (33120558 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f631a9bc37faab082104c7e02f76a7d0e292e3af5f21028f0af639fa4ed45731`  
		Last Modified: Wed, 20 Dec 2023 08:15:48 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4646bec0acecee6379c0bfe6ba69673cdb1b60095c34a6557f8b1a13fc7a15f6`  
		Last Modified: Wed, 20 Dec 2023 08:20:35 GMT  
		Size: 17.3 MB (17338277 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a5bc3009ab46771711fac83500b796cf49cb3a2061397b23770795a425d1f914`  
		Last Modified: Wed, 20 Dec 2023 08:20:34 GMT  
		Size: 449.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `haproxy:lts` - unknown; unknown

```console
$ docker pull haproxy@sha256:a39f21e60e96c9bdfa55fc2973ffada4ccf52fc61a761c91594e2953c318bfdd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3045505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:561f1ab492ef2f49bc16bfee61d262968f207ba7bc6ee2aea204042d25336a82`

```dockerfile
```

-	Layers:
	-	`sha256:862a25e6fe006f9fc93a8f95bde8ef8e7ff1151493ba7f1e53b14f419d6b2221`  
		Last Modified: Wed, 20 Dec 2023 08:20:34 GMT  
		Size: 3.0 MB (3025983 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:73f5acabfbfdfa32d991c4f22558caec4ced4d07cc04e6110439890314e3c722`  
		Last Modified: Wed, 20 Dec 2023 08:20:34 GMT  
		Size: 19.5 KB (19522 bytes)  
		MIME: application/vnd.in-toto+json

### `haproxy:lts` - linux; s390x

```console
$ docker pull haproxy@sha256:81986853deabfa68d3eb7fb1da5b2acd2387f2648cc72ce80b9dcfc2de364180
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.8 MB (42769422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77a813c89f908d6facc5582985ee7f50c5ab3eb31589c0830a8726f2b2f658ad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Mon, 11 Dec 2023 23:56:16 GMT
ADD file:f06f12fa5a93afc3a79ac4371d24b0a471a5a1818cf34c1d90004c8f410914b9 in / 
# Mon, 11 Dec 2023 23:56:16 GMT
CMD ["bash"]
# Mon, 11 Dec 2023 23:56:16 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy # buildkit
# Mon, 11 Dec 2023 23:56:16 GMT
ENV HAPROXY_VERSION=2.8.5
# Mon, 11 Dec 2023 23:56:16 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.8/src/haproxy-2.8.5.tar.gz
# Mon, 11 Dec 2023 23:56:16 GMT
ENV HAPROXY_SHA256=3f5459c5a58e0b343a32eaef7ed5bed9d3fc29d8aa9e14b36c92c969fc2a60d9
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
	-	`sha256:bc6b1888979d3ceb063da848b2034e980e2c2613642159c1e856550b79aa620c`  
		Last Modified: Tue, 19 Dec 2023 01:47:38 GMT  
		Size: 27.5 MB (27491874 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:085ebe9bb8e3d1ab51792ce7ff8056129143d4c419a56ab87d526f87ad58039a`  
		Last Modified: Tue, 19 Dec 2023 10:10:47 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f46cca607f6a67f6d2867d160d76962a8c1f9939cd1a5cf81a6734f90e8f1636`  
		Last Modified: Tue, 19 Dec 2023 15:25:47 GMT  
		Size: 15.3 MB (15275906 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5e18d03b43694831050d052352aec5989f9362675ebda489caa7b2711ef0c83d`  
		Last Modified: Tue, 19 Dec 2023 15:25:46 GMT  
		Size: 448.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `haproxy:lts` - unknown; unknown

```console
$ docker pull haproxy@sha256:c40f5b6733f57a67601b2e192e122546e8b1e2825bdefa78ad40c8166b96e1b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3046474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f3e0c538a80502fd9c97d9fe78bd72e193e781bcd4d3a97a4d5e02eed47820c`

```dockerfile
```

-	Layers:
	-	`sha256:edbc9ab8e6e153ade57c2a46e9ccef99b84d3e88fa9106fcb27f188966de203b`  
		Last Modified: Tue, 19 Dec 2023 15:25:46 GMT  
		Size: 3.0 MB (3027004 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:eec3461c57e1e16c9c8ab8bab06c669d5f6ac5b6131309951bf04e1fb77451df`  
		Last Modified: Tue, 19 Dec 2023 15:25:46 GMT  
		Size: 19.5 KB (19470 bytes)  
		MIME: application/vnd.in-toto+json
