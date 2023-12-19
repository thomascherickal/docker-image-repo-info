## `haproxy:latest`

```console
$ docker pull haproxy@sha256:6fc1a1dafffdb5590338363e0e74acadbafc6a8534bb7e4aab4595fad122a3a3
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

### `haproxy:latest` - linux; amd64

```console
$ docker pull haproxy@sha256:c8f4701f92b6de0a07bcaf4bcced3d0c3013aebf2c8f600a033f0b99d156588d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.3 MB (46295939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:480a95428f35c55fb2b74fba5ede7b800b033275b14606598e036924c8500bcf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 15 Dec 2023 18:13:27 GMT
ADD file:ac3cd70031d35e46d86b876934946ffc8756de4de065fbc926dce642dac07ff3 in / 
# Fri, 15 Dec 2023 18:13:27 GMT
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
	-	`sha256:af107e978371b6cd6339127a05502c5eacd1e6b0e9eb7b2f4aa7b6fc87e2dd81`  
		Last Modified: Tue, 19 Dec 2023 01:24:59 GMT  
		Size: 29.1 MB (29125963 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2158e837605b7ba429bdf70f832840865431a84c21f259ba5b75eaaf8b246bdd`  
		Last Modified: Tue, 19 Dec 2023 03:48:00 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f1d8787a236ae74c0a43872e6467347af51d6ee57f4c4cee7f5418a222b831ce`  
		Last Modified: Tue, 19 Dec 2023 03:48:01 GMT  
		Size: 17.2 MB (17168337 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:be6a8ed45611be9bab8fc13840714a3f470b1f803062e641dd6245d95b526250`  
		Last Modified: Tue, 19 Dec 2023 03:48:00 GMT  
		Size: 448.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `haproxy:latest` - unknown; unknown

```console
$ docker pull haproxy@sha256:b366e75746495d857fa7904412be88b91c7675bcd965c5c588fb8545324cfff1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3057088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07e7e0ef1261fa23f691ab8f4ad088b8d66a11e9ba193b346d31cbc719cbd030`

```dockerfile
```

-	Layers:
	-	`sha256:232f5c0285bd5a2874499e8e1306d1ab8cd067bb644a6d3b24369905a8c5ca6a`  
		Last Modified: Tue, 19 Dec 2023 03:48:00 GMT  
		Size: 3.0 MB (3037453 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:f341e63d441a08fea9269e66ab637bcf568ef2e6aa9fc914208f466d4fb68ca2`  
		Last Modified: Tue, 19 Dec 2023 03:48:00 GMT  
		Size: 19.6 KB (19635 bytes)  
		MIME: application/vnd.in-toto+json

### `haproxy:latest` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:9f1fa2bcded3c81ca92875937ccc924837e0396ff790331abd788c66c51c9a2c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.2 MB (42171430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e39072ec2c530f619eb523e0d2492362a7cd05ea861c8514e9a9ceb0170cb326`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 15 Dec 2023 18:13:27 GMT
ADD file:9503ab966c9dd707eeccc7c2f633bccc94c199f8714ec4ff2c8b54dde3dbabf9 in / 
# Fri, 15 Dec 2023 18:13:27 GMT
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
	-	`sha256:1ae9a2844c8c70942d2220553689b62e841cc706d77284fbfedbd770080fd699`  
		Last Modified: Tue, 19 Dec 2023 01:58:33 GMT  
		Size: 26.9 MB (26885440 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:29e46dbc80d018f67237ea6331c64f659a7b655cc2f711f63d92bfffd7058b98`  
		Last Modified: Tue, 19 Dec 2023 13:32:42 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:79488a33d3ca2e588d22f5b26c80cbd0ac33b29dd95230630656f5ba7e0d6627`  
		Last Modified: Tue, 19 Dec 2023 15:55:33 GMT  
		Size: 15.3 MB (15284346 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3c8de719d8c2fd1a32b66933329562929e9384503913db143378cecb3ee94994`  
		Last Modified: Tue, 19 Dec 2023 15:55:32 GMT  
		Size: 450.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `haproxy:latest` - unknown; unknown

```console
$ docker pull haproxy@sha256:0458b09e34dc39c85c30b3610c7f2158ef04788ebaa15e8fb4ee278280fe9310
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.4 KB (19352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:757eee56494bc1f78237f44ccf8c0e3a7d64d7a5d679b12b751b63bfb80ad859`

```dockerfile
```

-	Layers:
	-	`sha256:183a84480fcd716acbb33ab012f876356650fcdf26e76ad18097edffeb081053`  
		Last Modified: Tue, 19 Dec 2023 15:55:32 GMT  
		Size: 19.4 KB (19352 bytes)  
		MIME: application/vnd.in-toto+json

### `haproxy:latest` - linux; arm variant v7

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

### `haproxy:latest` - unknown; unknown

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

### `haproxy:latest` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:9088c39f08c31095629ad20b9526dac4dadf025f14d9ba88c35cb1d1c866b88b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.2 MB (45185337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:277b46d7152e755ee195b2b23fc33e9b0d9692884662bbd7a59ddb4c87cfa4b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:06 GMT
ADD file:869c7d0747a17c53715581a2e862992eb8516c7f45f167821dfa80966a4870d1 in / 
# Tue, 21 Nov 2023 06:27:06 GMT
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
	-	`sha256:2c6d21737d8318aa15c4cc838475029a5efc36c0429e3d8da80d97d0b96d9aaf`  
		Last Modified: Tue, 21 Nov 2023 06:30:30 GMT  
		Size: 29.2 MB (29179277 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cf6288c418af0a13c3069d6ec38e11c277c8f5f584c19250da321fd2c14f2c40`  
		Last Modified: Wed, 13 Dec 2023 23:06:02 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9e842dc21844ba79df913b486251bc5c4b4878c63fb16f2a15ded550bcc7bedf`  
		Last Modified: Sat, 16 Dec 2023 00:36:25 GMT  
		Size: 16.0 MB (16004417 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4c059ccdbbe3c6e1d7ebd868ea44999cee6eff2afeacdf0c686f2c8c8ae509da`  
		Last Modified: Sat, 16 Dec 2023 00:36:24 GMT  
		Size: 449.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `haproxy:latest` - unknown; unknown

```console
$ docker pull haproxy@sha256:9ba198b4cf6962ad88858d6bb898fb24531daf76101b965ad4b60f8bd7daf950
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3032034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa7fcb5f43a0826dbe238487356f3694f5da5177bc787a2494a8d5d1ffa8148d`

```dockerfile
```

-	Layers:
	-	`sha256:d0088d4730647e5308c634ca0569641588aa2cdcd6dd5c843962779aeb27af44`  
		Last Modified: Sat, 16 Dec 2023 00:36:25 GMT  
		Size: 3.0 MB (3012552 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:bb78b563c78f2a9946d6192e7e0343bc5083822c78741ff91e630758f7c45c5b`  
		Last Modified: Sat, 16 Dec 2023 00:36:24 GMT  
		Size: 19.5 KB (19482 bytes)  
		MIME: application/vnd.in-toto+json

### `haproxy:latest` - linux; 386

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

### `haproxy:latest` - unknown; unknown

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

### `haproxy:latest` - linux; mips64le

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

### `haproxy:latest` - unknown; unknown

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

### `haproxy:latest` - linux; ppc64le

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

### `haproxy:latest` - unknown; unknown

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

### `haproxy:latest` - linux; s390x

```console
$ docker pull haproxy@sha256:ffd712a55ecdf086689e47bb196d742c69cc4a9183f13e19cc24850ac46aee73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43128553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:871d97bcb090ccc22ec703522cdae24adf762cfd916512776de9401b47f5aed2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Fri, 15 Dec 2023 18:13:27 GMT
ADD file:f06f12fa5a93afc3a79ac4371d24b0a471a5a1818cf34c1d90004c8f410914b9 in / 
# Fri, 15 Dec 2023 18:13:27 GMT
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
	-	`sha256:bc6b1888979d3ceb063da848b2034e980e2c2613642159c1e856550b79aa620c`  
		Last Modified: Tue, 19 Dec 2023 01:47:38 GMT  
		Size: 27.5 MB (27491874 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:085ebe9bb8e3d1ab51792ce7ff8056129143d4c419a56ab87d526f87ad58039a`  
		Last Modified: Tue, 19 Dec 2023 10:10:47 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:276c5d5500c33615be03e7c5c4360f839241235cc0f37d092847e311eb0b695b`  
		Last Modified: Tue, 19 Dec 2023 15:09:21 GMT  
		Size: 15.6 MB (15635034 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ed07eca07286c6f9b09f9b99857c74b56fb146dc7cb9e25a32cd8a380051c5bf`  
		Last Modified: Tue, 19 Dec 2023 15:09:21 GMT  
		Size: 451.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `haproxy:latest` - unknown; unknown

```console
$ docker pull haproxy@sha256:b9b58459800776506929bb93727f6d5ab62d76d9fae501377c8d6f02116d6898
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.0 MB (3046470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7db24deb1360a515e4140708f3708880c2bb3d4e392b9f97e3b973cd0208cf06`

```dockerfile
```

-	Layers:
	-	`sha256:eef42e67b4d095cc900e1ac206517f055fd789ada60e92ba6c374eef105e09f0`  
		Last Modified: Tue, 19 Dec 2023 15:09:20 GMT  
		Size: 3.0 MB (3027002 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:042d70e0ee38975d7565c21e1de7edd331dff5ad93a2170c38ad74133fc4ebce`  
		Last Modified: Tue, 19 Dec 2023 15:09:20 GMT  
		Size: 19.5 KB (19468 bytes)  
		MIME: application/vnd.in-toto+json
