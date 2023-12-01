<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `memcached`

-	[`memcached:1`](#memcached1)
-	[`memcached:1-alpine`](#memcached1-alpine)
-	[`memcached:1-alpine3.18`](#memcached1-alpine318)
-	[`memcached:1-bookworm`](#memcached1-bookworm)
-	[`memcached:1.6`](#memcached16)
-	[`memcached:1.6-alpine`](#memcached16-alpine)
-	[`memcached:1.6-alpine3.18`](#memcached16-alpine318)
-	[`memcached:1.6-bookworm`](#memcached16-bookworm)
-	[`memcached:1.6.22`](#memcached1622)
-	[`memcached:1.6.22-alpine`](#memcached1622-alpine)
-	[`memcached:1.6.22-alpine3.18`](#memcached1622-alpine318)
-	[`memcached:1.6.22-bookworm`](#memcached1622-bookworm)
-	[`memcached:alpine`](#memcachedalpine)
-	[`memcached:alpine3.18`](#memcachedalpine318)
-	[`memcached:bookworm`](#memcachedbookworm)
-	[`memcached:latest`](#memcachedlatest)

## `memcached:1`

```console
$ docker pull memcached@sha256:e86e92011ac296d084a8f12dc414c01952d86b7711dfc936fbd325f342581631
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 15
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v5
	-	unknown; unknown
	-	linux; arm variant v7
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

### `memcached:1` - linux; amd64

```console
$ docker pull memcached@sha256:7b0480ab945f960f703af2f286b02a7b620eb4f772e25a2a1374e0c7d32f46de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.8 MB (38815745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f65c7b1a196aa7dfe9520f598f699d5846d6ff0eed117a36ca216302174a1bb1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:d261a6f6921593f1e0b3f472ab1b1822e2c6deb0b369200f0b3370556bfad017 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1f7ce2fa46ab3942feabee654933948821303a5a821789dddab2d8c3df59e227`  
		Last Modified: Tue, 21 Nov 2023 05:25:58 GMT  
		Size: 29.1 MB (29149908 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3606f7d6f784848f3e26f4bc5fae3dde08d65681dbaba232236ac8855cddb881`  
		Last Modified: Tue, 21 Nov 2023 06:19:50 GMT  
		Size: 1.1 KB (1110 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d9e66f47c0a00f0a833454718ca9dc6504f38c45944b5ebf43ccac532dc520b6`  
		Last Modified: Tue, 21 Nov 2023 06:19:50 GMT  
		Size: 2.5 MB (2488339 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:26e0a53c88ab99ad6e23fbb12147cce82e922e4141af56338b4ec01c2ead2b07`  
		Last Modified: Tue, 21 Nov 2023 06:19:50 GMT  
		Size: 7.2 MB (7175988 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:afc0db62c179dab7a3fc4ff6848e150c3315896846d827282affab08909d6e23`  
		Last Modified: Tue, 21 Nov 2023 06:19:50 GMT  
		Size: 281.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7af609a76aa9ed2d446da8865870d0e2b3bff46785783284d956d755a714899b`  
		Last Modified: Tue, 21 Nov 2023 06:19:50 GMT  
		Size: 119.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1` - unknown; unknown

```console
$ docker pull memcached@sha256:cb387d9a91a709e6a4193c58df1f36753dbc6c13b9788d741d6dd92ee262ea52
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3078549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3b5853b03b272d3ad2682a093fbc3b2ffd577e3c9fe01f926b5963b333208cd`

```dockerfile
```

-	Layers:
	-	`sha256:9630a5bf61090e535bcf3b7ad1349332584446ea948e10119e025a65fad57d26`  
		Last Modified: Tue, 21 Nov 2023 06:19:50 GMT  
		Size: 3.1 MB (3056780 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:a2ef4829ccc1863c60fdfcf41590326d17bfbdef204a7d37664c92bec494942b`  
		Last Modified: Tue, 21 Nov 2023 06:19:50 GMT  
		Size: 21.8 KB (21769 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1` - linux; arm variant v5

```console
$ docker pull memcached@sha256:c5fbea0a198cb4ae068e4761d5d1abab499e4ebc80275be6b7d797196cf3db54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34849973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b72ee44b42eca798309f6aa48ed2af9feca23c5eb64e5be38fa2536110b12ce`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:1ae8e5ac45b11d01083680b765e1fcfef9f7938f89d6f424572126fa946d8cdf in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f476aef5b6e1122850e68c81ef06fc2df17e968961b060483b4d2fb33018aae3`  
		Last Modified: Tue, 21 Nov 2023 05:03:55 GMT  
		Size: 26.9 MB (26922153 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:26dadbdb945a22546f6b2c171d0bededff72d7598719ab8f3877f67129e21730`  
		Last Modified: Tue, 21 Nov 2023 16:18:13 GMT  
		Size: 1.1 KB (1109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:44f46f0b8b7c11e6cd53e82541f819c66da246b152155fff8ce762f98c25219f`  
		Last Modified: Tue, 21 Nov 2023 16:18:14 GMT  
		Size: 2.1 MB (2089268 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:639e86d18160b654876d404a88b437cea26de29151122dfe8cbed9947f1b7b10`  
		Last Modified: Tue, 21 Nov 2023 16:18:14 GMT  
		Size: 5.8 MB (5837040 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7b963217677ca57533744aee2b331f059fbb6882f27abe2cc976462604e7b560`  
		Last Modified: Tue, 21 Nov 2023 16:18:15 GMT  
		Size: 283.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ac3a1fa5d4b6c48ea8ce4c375a197047f1480fbfb37c316b7d730d026d261219`  
		Last Modified: Tue, 21 Nov 2023 16:18:15 GMT  
		Size: 120.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1` - unknown; unknown

```console
$ docker pull memcached@sha256:cd008d8c4d507d73b5f0153ed880e81e86a53741b480bbf6b1d318510e83a288
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.7 KB (21695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85e0f40569066724c087be3d901d5c5d984043271b56a33dec281e36032017f0`

```dockerfile
```

-	Layers:
	-	`sha256:2eff64dde44b4be85375aed8309f5d20476ca81876607d799b56c31addee0cb8`  
		Last Modified: Tue, 21 Nov 2023 16:18:13 GMT  
		Size: 21.7 KB (21695 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1` - linux; arm variant v7

```console
$ docker pull memcached@sha256:2841be0a36134563966c09a6ed68b21053d20342ec8736cf92763c28077ead43
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28094215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cf74ffa940dd93988fc0beb6698c5796563c82a40b7dd668153969f64d2e6ca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 09 Feb 2023 06:12:09 GMT
ADD file:5f1a343224e8486690bd90dd1e50c8d84b3d770c51bb6829544e5cf650c0419c in / 
# Thu, 09 Feb 2023 06:12:10 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 07:52:31 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 09 Feb 2023 07:52:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:52:35 GMT
ENV MEMCACHED_VERSION=1.6.18
# Thu, 09 Feb 2023 07:52:35 GMT
ENV MEMCACHED_SHA1=be16909bb75ab972ee5fe438312501de01c4725a
# Thu, 09 Feb 2023 07:55:44 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 09 Feb 2023 07:55:44 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 09 Feb 2023 07:55:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 09 Feb 2023 07:55:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Feb 2023 07:55:44 GMT
USER memcache
# Thu, 09 Feb 2023 07:55:45 GMT
EXPOSE 11211
# Thu, 09 Feb 2023 07:55:45 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:e7318f6106ad75d7d482ae9dddf4d927b0872ef3ddb6e1330aa691fc8d17279e`  
		Last Modified: Thu, 09 Feb 2023 06:19:19 GMT  
		Size: 26.6 MB (26577666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de49d9d72daf1680b5f1b9532dd2eb0162829f36c8db9669935462636fbf99d9`  
		Last Modified: Thu, 09 Feb 2023 08:06:11 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0beac9d5bcac946f8c54c72b8a9c136914b1aa7a5fe2b8c3df4c7d8858ea6559`  
		Last Modified: Thu, 09 Feb 2023 08:06:11 GMT  
		Size: 312.1 KB (312088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4c9e5a265394e4c0f357779e6195a4e82d767a3691a0e77d427e56651c3e54a`  
		Last Modified: Thu, 09 Feb 2023 08:06:11 GMT  
		Size: 1.2 MB (1199163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ea82ad892fe1ae8623d84e32c8c027087cda8aa49e40d4546ed6942e471c60`  
		Last Modified: Thu, 09 Feb 2023 08:06:11 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2ae3bcdc0d114ba49a67df022b6f7215fc87f1f50e64939fcfbbec4eaadee5`  
		Last Modified: Thu, 09 Feb 2023 08:06:11 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:dd556de8d6e6b81c51ba9120fa924fbb7fae427468d82db9f2b3db124f9ac0b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.7 MB (37711361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f05ec0c73b4afc866c99864d86b1c66deb5d8bda84bf2cc78e1e763e0ed6a263`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:869c7d0747a17c53715581a2e862992eb8516c7f45f167821dfa80966a4870d1 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2c6d21737d8318aa15c4cc838475029a5efc36c0429e3d8da80d97d0b96d9aaf`  
		Last Modified: Tue, 21 Nov 2023 06:30:30 GMT  
		Size: 29.2 MB (29179277 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fa3a18531b093eb1a543ad01b2a54d4692f59bba8d49ea9793b3ff09e528cd93`  
		Last Modified: Wed, 22 Nov 2023 11:50:41 GMT  
		Size: 1.1 KB (1109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:395fd5be77a2adb2c1b863f9ba2c664074aacb120f379bbb0f45cda74cc09cf4`  
		Last Modified: Wed, 22 Nov 2023 11:50:41 GMT  
		Size: 2.3 MB (2345987 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1dbcb5e891e054cd85f29e62fff856117d8cb919630be0c7473b520168b8c261`  
		Last Modified: Wed, 22 Nov 2023 11:50:41 GMT  
		Size: 6.2 MB (6184583 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2654df736cfb30e0097cca6a637ae794285396f6e2b87031636c8056b66baed0`  
		Last Modified: Wed, 22 Nov 2023 11:50:41 GMT  
		Size: 283.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e54ea6c3f7f45d9ed3f003bcf9e0a717c342daae58d330fef355e712d15b732`  
		Last Modified: Wed, 22 Nov 2023 11:50:42 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1` - unknown; unknown

```console
$ docker pull memcached@sha256:2b5053d245e0312a77b7827553fcf09a6b19a0bf825a7016a4125713ad0d814f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3053591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e04bc647daea7fbb746cd418f19740162bd910826c366cdcc3549c3888ad5e1b`

```dockerfile
```

-	Layers:
	-	`sha256:f04377bb8fcfc3a24c1a36aa0bdf9b2d9272b7a60e82a88b66e2bb0645703c07`  
		Last Modified: Wed, 22 Nov 2023 11:50:41 GMT  
		Size: 3.0 MB (3031971 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:601cddda9e5f7f3a82cfc305051ac3c1fc5f65a9722e4dbe06363cc8b6ea68be`  
		Last Modified: Wed, 22 Nov 2023 11:50:41 GMT  
		Size: 21.6 KB (21620 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1` - linux; 386

```console
$ docker pull memcached@sha256:fa9dba8086765d68f2feecfc2ac08fb29c019597d09943bb480227e6cba87666
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.3 MB (39294993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93047050e75b6d4d64adb8a7c8f68cb118bad27ca9dc772120e251b174752cf9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:0c94521fdd9c0a4fdeeb9aad23e68cd053fba0dcd7c3af550aefa79377816e31 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:98bdfce9af831c2a0d0bfcca812d0039cd1666986550f552b4b4c625bd5aa31c`  
		Last Modified: Wed, 01 Nov 2023 00:43:26 GMT  
		Size: 30.2 MB (30164042 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1b647d4b10cf20ac5807101c7d0380701be684aa82f5c01ec41f674b5ef23d42`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 1.1 KB (1109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b61c058003459de4911c2901b2d799b03de754a1b9e64ffbe21a04992e962e62`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 2.5 MB (2492501 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:810b6db64df2fcc8f76941cdac75093cf35bd72ac3cd1fa5eb664e74c1f67cd8`  
		Last Modified: Wed, 01 Nov 2023 01:06:50 GMT  
		Size: 6.6 MB (6636937 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dbb899942df4149bd5fae8bac6e295285ec80f82d621f2b29c931ee348491cfb`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 282.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4a8530160ab232c37c0ddcbf5e3a731d835d378d1382843957f6c2a73b2b5be6`  
		Last Modified: Wed, 01 Nov 2023 01:06:50 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1` - unknown; unknown

```console
$ docker pull memcached@sha256:dd7ce9519c31365127142232df2ed0b285e9acc03cd77c23c838bf932165def8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 KB (21498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eef82c92e07c11a92c337806d01cfb1c6cdc7a16608dcf304a38de34d2ef1dbb`

```dockerfile
```

-	Layers:
	-	`sha256:c0d9dd22513f8d3e791e1796d7ef1906e57c798c92dd35d0be9cf2eaecec5954`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 21.5 KB (21498 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1` - linux; mips64le

```console
$ docker pull memcached@sha256:a7c198db1b0856aff4b1514137e473ea30bce2ef22f0192cfdce7e2e44f2a863
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.6 MB (37588022 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1654ec4454e597d7e7cb6a7d97e98208de241a3dfafc5e0532b9561eac91f013`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:e093749192323dc72b60a8440ddba26c415586f618b5e107fa264ba5eb2ca7ba in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:ebdff2138fee4a3ec27560ab1353dc51c12c2608ff721f5db3d24104872b702a`  
		Last Modified: Tue, 21 Nov 2023 04:20:35 GMT  
		Size: 29.1 MB (29141984 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:50b1ffce24cec457fe1757715d60bd669145e5babade7c57143c4b665a55389e`  
		Last Modified: Thu, 23 Nov 2023 01:10:58 GMT  
		Size: 1.1 KB (1112 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:893c712c491a058aada36756e9f176b6c6c2f3a2b3adf0cd94b896c8198ec3ee`  
		Last Modified: Thu, 23 Nov 2023 01:10:59 GMT  
		Size: 1.9 MB (1937483 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0b8443254952572331df084976853329b69a4348b3c620bb073b5c89fb943b2b`  
		Last Modified: Thu, 23 Nov 2023 01:10:59 GMT  
		Size: 6.5 MB (6507036 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:904bfc5c5c0923edd9be421332402b224bfcd49053bc9b3fae6173383f5cd395`  
		Last Modified: Thu, 23 Nov 2023 01:10:59 GMT  
		Size: 285.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c265216ad3407dbc99903d96423b3a2314bc48cc0118911d150a6bb087ff7d85`  
		Last Modified: Thu, 23 Nov 2023 01:11:00 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1` - unknown; unknown

```console
$ docker pull memcached@sha256:e2fcd32899d09ff06793849927220bea14475e64f085972afbc1f3af74dc209b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.7 KB (21656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf1c2028769aa20a3e529d0f85c8144ba6b099f74cda0dfca2272b7831d2d7a5`

```dockerfile
```

-	Layers:
	-	`sha256:75bab713cb94cdececf4c3879050737e7cb4bbb6206daa071ea001692b53d659`  
		Last Modified: Thu, 23 Nov 2023 01:10:58 GMT  
		Size: 21.7 KB (21656 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1` - linux; ppc64le

```console
$ docker pull memcached@sha256:d8d106a88d6a15fadf738e59a6dcfc3942f11c7a2d19b7473abce66af7f4d19c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.0 MB (43030916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85da4ca798d44fc951b843ec85c410207ecc3c56af6d1bf7c321c91266d54e1b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:8b22a531b6611a1e63dfc20e4e2931592e2d821bd4b64c4b2810bb9a36640c02 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c570d04e61d8e35a3c8f12179d048d701451f97f9cf2099ea3e3738512dbf062`  
		Last Modified: Tue, 21 Nov 2023 04:28:58 GMT  
		Size: 33.1 MB (33141607 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bcd0cf90a66e23cd3d72b99e7d36129b0e846407a07c30031b0c1e4ba115cd30`  
		Last Modified: Tue, 21 Nov 2023 23:46:47 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5e4166a0e033df4117b469f840c6f5527e87dbd13c582c0b50c182b4bb3ead79`  
		Last Modified: Tue, 21 Nov 2023 23:46:47 GMT  
		Size: 2.7 MB (2698215 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:947b7328e0db59b9870fe9c6d6b7fc4e8a8f1fef3d2a36064fe3d60f5314652d`  
		Last Modified: Tue, 21 Nov 2023 23:46:48 GMT  
		Size: 7.2 MB (7189577 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f011f72796530a711f1de9d543435299d02ed3636e4cd28aee1fa493fbc2bf4`  
		Last Modified: Tue, 21 Nov 2023 23:46:47 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9d27046f19e474530b87e1d0b429e9d85f403210dd3d91bf60d8303fef03af96`  
		Last Modified: Tue, 21 Nov 2023 23:46:48 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1` - unknown; unknown

```console
$ docker pull memcached@sha256:4269af6aa39a29d6dca352659fbf04b7d1bb4e65151e63a3ffcf2749d853597e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3067036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6e9626f30d490d2014e9fbb19add0b6ac0f63c8f4af2082d04750fea7ec35ff`

```dockerfile
```

-	Layers:
	-	`sha256:70759e1722d82b89de5c0d71ba2050ecc9f29d95ee758369044a1fc79026a546`  
		Last Modified: Tue, 21 Nov 2023 23:46:47 GMT  
		Size: 3.0 MB (3045366 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:4f34d59241ff06b2bd0cb8239d96be938e1e13470264898863f307f84ab275b6`  
		Last Modified: Tue, 21 Nov 2023 23:46:47 GMT  
		Size: 21.7 KB (21670 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1` - linux; s390x

```console
$ docker pull memcached@sha256:312625a69b30a0a0371060c62ec97a621d587675e55a8ced694303d8a7015d30
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.7 MB (35745726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13ebe1c7df28f24c49c7dc749c55574a0a51a84e31dcff380e6caa5441fca944`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:c33fa9fdde73983850798b6eb1cd062e0398109d1d773e6a937fead7475c8efc in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6daa625e5a040476e253e7acd0befa74254a4865ec836d6334a544d82a21d4be`  
		Last Modified: Tue, 21 Nov 2023 05:10:21 GMT  
		Size: 27.5 MB (27512885 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:410539cfd307a2626bf5520b21d1cff0d4c8a336ebea36ed08878d81eca92847`  
		Last Modified: Tue, 21 Nov 2023 15:56:02 GMT  
		Size: 1.1 KB (1109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1ba4cc4f8ba1aa1865931fde910e1ebac220aea9a207eff2f2556bc289a513d3`  
		Last Modified: Tue, 21 Nov 2023 15:56:03 GMT  
		Size: 2.2 MB (2152517 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a47325d5bddeb006ca8a01a6239f747f4ed2c21fd6a28226bdfe46d1981d8962`  
		Last Modified: Tue, 21 Nov 2023 15:56:03 GMT  
		Size: 6.1 MB (6078811 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:32f889bfd6f6b6b2d773abb9f72f86fe0c7469d2a271e5bd209a3eb9b1c61dea`  
		Last Modified: Tue, 21 Nov 2023 15:56:04 GMT  
		Size: 283.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:56ce84d34f650bc21b164be1bb375a2b43c761943b4d06497991ceca18be1009`  
		Last Modified: Tue, 21 Nov 2023 15:56:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1` - unknown; unknown

```console
$ docker pull memcached@sha256:b070f08010996b181adf3fbb4b9004e0d125115bf1380df8c4ddb96a99827218
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3068089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:307228ea8d7a2ce5fee0e1c4c36745e1c0244aa6d316102bde5b655af1bedd24`

```dockerfile
```

-	Layers:
	-	`sha256:640994e8299bce5ed690d70d55a1bc2035868614a169e4cda3391dafb76e9469`  
		Last Modified: Tue, 21 Nov 2023 15:56:03 GMT  
		Size: 3.0 MB (3046321 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:1893b50125646067935dd81f10c259d7b0c3b7cf2f42c81abe2b0f93e45f4250`  
		Last Modified: Tue, 21 Nov 2023 15:56:03 GMT  
		Size: 21.8 KB (21768 bytes)  
		MIME: application/vnd.in-toto+json

## `memcached:1-alpine`

```console
$ docker pull memcached@sha256:e8191559af396cda215a055e31a07bfc8178241854fa20f9e2cd32e4f1f5169e
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 11
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `memcached:1-alpine` - linux; amd64

```console
$ docker pull memcached@sha256:f85dfa7d8ec9dc1b785c37ccf6dfa62bca5fec355c32ddf7957116376863284a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4471146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f687f33554b696db4e2422b52d11bd36b20649d152ca63d20848c83b0679237f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["/bin/sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN apk add --no-cache libsasl # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ce5e53c5eb3023b585266ac7ee39c0b268a83b4e16556b72f52bd67e39f596be`  
		Last Modified: Fri, 01 Dec 2023 00:14:01 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e958dac8143e41701702904f092ab10b8682434d3d88e5af758dafaeb3317428`  
		Last Modified: Fri, 01 Dec 2023 00:14:01 GMT  
		Size: 108.0 KB (107998 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:61dfbf83553658c4ab4a5ae4477150c88a3f30da8309b9cfefdc185b3764e501`  
		Last Modified: Fri, 01 Dec 2023 00:14:01 GMT  
		Size: 959.1 KB (959085 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8b397213e2806c5c7c6aca6c20bc2f69362c9f6204c5d3947eaaf870176d9a36`  
		Last Modified: Fri, 01 Dec 2023 00:14:01 GMT  
		Size: 277.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8c404d1dff37be469e83d35363176296e0129304273844e38a69edbd6861f08c`  
		Last Modified: Fri, 01 Dec 2023 00:14:02 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-alpine` - unknown; unknown

```console
$ docker pull memcached@sha256:6a508d9bd488a6e6f8bbaae93d8ff14548111b267a7440f64edec96b04f8a3cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 KB (97008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fdbf48b2b61dd467eec02ffd7b0e996989023a93d9ecbc7a655a0755362c38a`

```dockerfile
```

-	Layers:
	-	`sha256:5c3e16fb5448bac47fadf2a80df72f13e831b463525dc9823da6c85f1770bf69`  
		Last Modified: Fri, 01 Dec 2023 00:14:01 GMT  
		Size: 78.1 KB (78055 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:1d5f7cf7dffd0d16953251b75fd8b7224aae91e57357d5af853c41398d72a5f7`  
		Last Modified: Fri, 01 Dec 2023 00:14:01 GMT  
		Size: 19.0 KB (18953 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1-alpine` - linux; arm variant v7

```console
$ docker pull memcached@sha256:79a5646a0c845a791f36017fda3292281b48295b06c53f13d62c9f94237d4731
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3960292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2afac0e49af3ce3f1769abe11a29f8f5610c6a736d8c5b6c7b9770c8d8e94e91`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 06:43:29 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 17 Dec 2020 06:43:31 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Thu, 17 Dec 2020 06:43:33 GMT
ENV MEMCACHED_VERSION=1.6.9
# Thu, 17 Dec 2020 06:43:35 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Thu, 17 Dec 2020 06:46:32 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 17 Dec 2020 06:46:33 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Dec 2020 06:46:35 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Dec 2020 06:46:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 06:46:36 GMT
USER memcache
# Thu, 17 Dec 2020 06:46:38 GMT
EXPOSE 11211
# Thu, 17 Dec 2020 06:46:39 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68564bbfc09f153688e942bf54d5375d1e27f3507c0bed6b038c2ac8ce095aa5`  
		Last Modified: Thu, 17 Dec 2020 06:46:58 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cac3a91edee49d0b08a25706ae86059bed89941a08b496e72ef092e57c4ecb3`  
		Last Modified: Thu, 17 Dec 2020 06:46:58 GMT  
		Size: 13.8 KB (13825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf16e9bb942ec42a35a792beab65aea843209e7bdde7e856499b9fc85f93bc4e`  
		Last Modified: Thu, 17 Dec 2020 06:46:58 GMT  
		Size: 1.5 MB (1537248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc15394239bd0c083e1b6df806aa5ffeb8b9cc7e80113afc2959721de49f90d1`  
		Last Modified: Thu, 17 Dec 2020 06:46:58 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482f0eb571548eae5720c652ff7da13558e56a8722dc9932cf7eb1ef3eb33acb`  
		Last Modified: Thu, 17 Dec 2020 06:46:58 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:e9673caac3d318f89edf7ca6eaba8910416292f12f0f0abbf3d862a8b5af88ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4406434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a4e56736197b019e201b69449a358660e6806d076b61fd473dbcbb11caf5197`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["/bin/sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN apk add --no-cache libsasl # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4962e560ef629491acb51e64b06a5ee52545098f8403705778786a404e81434b`  
		Last Modified: Fri, 01 Dec 2023 15:25:24 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d4b10238ba82be69f174742e8ae9cd6e4484f32dce6eeb40dcbe3c5a4e0a1480`  
		Last Modified: Fri, 01 Dec 2023 15:25:24 GMT  
		Size: 124.1 KB (124087 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:276ae0cb4d4371459c3116e0453691ac59cdd9a6d649cb27bb3d3a090ef10fbf`  
		Last Modified: Fri, 01 Dec 2023 15:25:24 GMT  
		Size: 947.7 KB (947670 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:315ab34d41c816b04b8d07e4b7db199c17340b3b882b52819a0564f6be31a04c`  
		Last Modified: Fri, 01 Dec 2023 15:25:24 GMT  
		Size: 278.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:024d99cdc8f15c63cc478d1850db680f8c0dfae1ea2a5bca55e41fb0db12d020`  
		Last Modified: Fri, 01 Dec 2023 15:25:25 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-alpine` - unknown; unknown

```console
$ docker pull memcached@sha256:91dac18281e4a194ee9756cf2652c70b2fb0bd2ba9d26c5c86d44c762d111821
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.9 KB (96880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3590bb02748f6b9e8a22ef90e7b41976bcb90189d98a78beae80f5aab1cd1cf4`

```dockerfile
```

-	Layers:
	-	`sha256:605a9d206d49d790bef9ce82c45179355571f37a91c5730ca6f59a03e13c0c76`  
		Last Modified: Fri, 01 Dec 2023 15:25:24 GMT  
		Size: 78.1 KB (78074 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:95803ef4905954256ae922386b3196bdafabd328ecd648b88ed7d8c13ec3b640`  
		Last Modified: Fri, 01 Dec 2023 15:25:24 GMT  
		Size: 18.8 KB (18806 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1-alpine` - linux; 386

```console
$ docker pull memcached@sha256:c281c55fd61946d53161839c584fb2bab1e6701155ad4b32c816d6ab0dc21a08
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4692614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c2fd98aa81c35c4a5fa9401b2f61ac48a2632d3b4b4baacc4b7982b10310097`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 28 Sep 2023 20:38:19 GMT
ADD file:8402753f294e403e92353bd65c86a6428c960be5116c0a15484b663a84f66fcd in / 
# Thu, 28 Sep 2023 20:38:20 GMT
CMD ["/bin/sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN apk add --no-cache libsasl # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:dc95107ad2a031a015320bb397f73ec151d738127175b31ad643120697dc7e90`  
		Last Modified: Thu, 28 Sep 2023 20:39:32 GMT  
		Size: 3.2 MB (3235757 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4951068162aca253cfa98ba4876636d5f13870e8ae9df08734f097bb6291e163`  
		Last Modified: Wed, 18 Oct 2023 01:04:05 GMT  
		Size: 1.2 KB (1246 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:50e4c32dd77b7a60c60be859a9848c50b3da8b95360dea46acf070797f48ab2a`  
		Last Modified: Wed, 18 Oct 2023 01:04:05 GMT  
		Size: 109.5 KB (109458 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:77aecf5d85dda7360aa3010357b83f206e1873aa4df6de5692c0c39dbf083c2a`  
		Last Modified: Wed, 18 Oct 2023 01:04:06 GMT  
		Size: 1.3 MB (1345750 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:99e49c7a1306cd1125b7dbc332a0b1b47b2408c77e975df11b090c0ab5599be3`  
		Last Modified: Wed, 18 Oct 2023 01:04:06 GMT  
		Size: 281.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:68c5ecf5461e2d137f2c403e26fe6e0532a5ecf0eedcd77a5b18254c82b9a075`  
		Last Modified: Wed, 18 Oct 2023 01:04:07 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-alpine` - unknown; unknown

```console
$ docker pull memcached@sha256:f0efd827c59fd288434c24a501d257456e82560b34d98f97cfe8b132454e28b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 KB (18687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea78294aafd9f308a52d310f899433de63e91eaac550b4ace8c1b8647774c7b8`

```dockerfile
```

-	Layers:
	-	`sha256:8c15fbe468a3b1236cadb64627426b8e2cb8bb71fddd26e10cdc44abd3b3519c`  
		Last Modified: Wed, 18 Oct 2023 01:04:05 GMT  
		Size: 18.7 KB (18687 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:bae49b5a412b4535ebab987425356a20af16fc1ce70c38e18f6aa6572cac522d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4460245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b845ad70056a07d2adbebdc425879a4eb74152c886dae5d8e5496c6114cd3cda`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:3450a1687b552498a987f87cb844b7f597c7181d7c3d31943d7b3036d5300d5e in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["/bin/sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN apk add --no-cache libsasl # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:4e13780adf2776477b14ef9c0f4f563f820a2fde166d472218037b979e84d31a`  
		Last Modified: Thu, 30 Nov 2023 23:20:01 GMT  
		Size: 3.3 MB (3348322 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a33c280bf18f1bba1782f90d468941796634b74c44d9aae4c406162114520e9a`  
		Last Modified: Fri, 01 Dec 2023 12:01:06 GMT  
		Size: 1.2 KB (1247 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a54d91525051bf65bd807cac3c6f1a685ac2fc6ec7f763df97c18a3ca4b6dde0`  
		Last Modified: Fri, 01 Dec 2023 12:01:07 GMT  
		Size: 123.9 KB (123864 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:73f73a883ca0c1147533ae5085475dee29244e8ef06b0455c52afa6ab50c3023`  
		Last Modified: Fri, 01 Dec 2023 12:01:07 GMT  
		Size: 986.4 KB (986410 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:183bb794a2f98d5b2192b311c4b597c47ee4ee0bb405558f67827c8afaf0b8d3`  
		Last Modified: Fri, 01 Dec 2023 12:01:07 GMT  
		Size: 280.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:556988ad767ddefdfb131bbf239cceba01e60b197c0893287ee0f6274e54a0c8`  
		Last Modified: Fri, 01 Dec 2023 12:01:08 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-alpine` - unknown; unknown

```console
$ docker pull memcached@sha256:df95592ada35b125fd73982e23f99a4fc3820ab083e12870f4edb179935ec44d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.3 KB (95332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67d44fe1dc00fdfaba957619ac6567e2ba40c2bad9a422ffb5287bb160b01fe7`

```dockerfile
```

-	Layers:
	-	`sha256:4a7a9ea74e3391f7a0e156b244eb474f674d42637b77983cfd9c92b23701d5ce`  
		Last Modified: Fri, 01 Dec 2023 12:01:06 GMT  
		Size: 76.5 KB (76477 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:671ec9ab176a20a138f0a3e238976e619a6f3011f598148b2cadd4c167721f81`  
		Last Modified: Fri, 01 Dec 2023 12:01:07 GMT  
		Size: 18.9 KB (18855 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1-alpine` - linux; s390x

```console
$ docker pull memcached@sha256:7af81a585082ce3ca180a3fac82a30bb37a43973123841b2dec30e5d096be8cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4285472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b785f0d9bb74e0e2b4f8772ce85a7b23cfc2e2f8dbb7ad428517b68cca17de38`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["/bin/sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN apk add --no-cache libsasl # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a7b34c58047c2f1ded65320321066565e57ddd2ed65156bde99267b8e575bf63`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:036bb49faad29b98ef9de81de4441efa5208c00e72ccea2b631c7b1c283f072d`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 112.8 KB (112781 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c1da6195feb453292bec9ae13a8968a7fbc7b611793ac2bc13df3614b514db3f`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 953.6 KB (953590 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a43896e685e7c2e1e51c75c1ed262d1c57940abdc2e68d74301201c9aa8ebdfe`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 281.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:928e080b9c3b24e2e655bd62e483670acb3c5508648e5a2784a6bebb4d252367`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-alpine` - unknown; unknown

```console
$ docker pull memcached@sha256:89eda6fd40656e7c2d5de572e4bdfbd821a333eb1067170caf9074dcbc141515
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.2 KB (95207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e34e69a75d4acd1221e6dd87a6f96bcf43e52e6ebaba333e1e4cc57d391f048`

```dockerfile
```

-	Layers:
	-	`sha256:c5dd02fe5ddfbc8ce715e0e666a98ae24e73371a2a8dee859d796538f4cf0618`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 76.4 KB (76419 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:13692e9f247d60b0cd5d0d4c0ccb23a86437ea348414e8548639ba89b5e4b65a`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 18.8 KB (18788 bytes)  
		MIME: application/vnd.in-toto+json

## `memcached:1-alpine3.18`

```console
$ docker pull memcached@sha256:93a9ff5ab97a213a027913f59bf902a118fa9750f88dbd4d513ebd920428820e
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 10
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `memcached:1-alpine3.18` - linux; amd64

```console
$ docker pull memcached@sha256:f85dfa7d8ec9dc1b785c37ccf6dfa62bca5fec355c32ddf7957116376863284a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4471146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f687f33554b696db4e2422b52d11bd36b20649d152ca63d20848c83b0679237f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["/bin/sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN apk add --no-cache libsasl # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ce5e53c5eb3023b585266ac7ee39c0b268a83b4e16556b72f52bd67e39f596be`  
		Last Modified: Fri, 01 Dec 2023 00:14:01 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e958dac8143e41701702904f092ab10b8682434d3d88e5af758dafaeb3317428`  
		Last Modified: Fri, 01 Dec 2023 00:14:01 GMT  
		Size: 108.0 KB (107998 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:61dfbf83553658c4ab4a5ae4477150c88a3f30da8309b9cfefdc185b3764e501`  
		Last Modified: Fri, 01 Dec 2023 00:14:01 GMT  
		Size: 959.1 KB (959085 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8b397213e2806c5c7c6aca6c20bc2f69362c9f6204c5d3947eaaf870176d9a36`  
		Last Modified: Fri, 01 Dec 2023 00:14:01 GMT  
		Size: 277.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8c404d1dff37be469e83d35363176296e0129304273844e38a69edbd6861f08c`  
		Last Modified: Fri, 01 Dec 2023 00:14:02 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-alpine3.18` - unknown; unknown

```console
$ docker pull memcached@sha256:6a508d9bd488a6e6f8bbaae93d8ff14548111b267a7440f64edec96b04f8a3cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 KB (97008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fdbf48b2b61dd467eec02ffd7b0e996989023a93d9ecbc7a655a0755362c38a`

```dockerfile
```

-	Layers:
	-	`sha256:5c3e16fb5448bac47fadf2a80df72f13e831b463525dc9823da6c85f1770bf69`  
		Last Modified: Fri, 01 Dec 2023 00:14:01 GMT  
		Size: 78.1 KB (78055 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:1d5f7cf7dffd0d16953251b75fd8b7224aae91e57357d5af853c41398d72a5f7`  
		Last Modified: Fri, 01 Dec 2023 00:14:01 GMT  
		Size: 19.0 KB (18953 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:e9673caac3d318f89edf7ca6eaba8910416292f12f0f0abbf3d862a8b5af88ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4406434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a4e56736197b019e201b69449a358660e6806d076b61fd473dbcbb11caf5197`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["/bin/sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN apk add --no-cache libsasl # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4962e560ef629491acb51e64b06a5ee52545098f8403705778786a404e81434b`  
		Last Modified: Fri, 01 Dec 2023 15:25:24 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d4b10238ba82be69f174742e8ae9cd6e4484f32dce6eeb40dcbe3c5a4e0a1480`  
		Last Modified: Fri, 01 Dec 2023 15:25:24 GMT  
		Size: 124.1 KB (124087 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:276ae0cb4d4371459c3116e0453691ac59cdd9a6d649cb27bb3d3a090ef10fbf`  
		Last Modified: Fri, 01 Dec 2023 15:25:24 GMT  
		Size: 947.7 KB (947670 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:315ab34d41c816b04b8d07e4b7db199c17340b3b882b52819a0564f6be31a04c`  
		Last Modified: Fri, 01 Dec 2023 15:25:24 GMT  
		Size: 278.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:024d99cdc8f15c63cc478d1850db680f8c0dfae1ea2a5bca55e41fb0db12d020`  
		Last Modified: Fri, 01 Dec 2023 15:25:25 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-alpine3.18` - unknown; unknown

```console
$ docker pull memcached@sha256:91dac18281e4a194ee9756cf2652c70b2fb0bd2ba9d26c5c86d44c762d111821
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.9 KB (96880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3590bb02748f6b9e8a22ef90e7b41976bcb90189d98a78beae80f5aab1cd1cf4`

```dockerfile
```

-	Layers:
	-	`sha256:605a9d206d49d790bef9ce82c45179355571f37a91c5730ca6f59a03e13c0c76`  
		Last Modified: Fri, 01 Dec 2023 15:25:24 GMT  
		Size: 78.1 KB (78074 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:95803ef4905954256ae922386b3196bdafabd328ecd648b88ed7d8c13ec3b640`  
		Last Modified: Fri, 01 Dec 2023 15:25:24 GMT  
		Size: 18.8 KB (18806 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1-alpine3.18` - linux; 386

```console
$ docker pull memcached@sha256:c281c55fd61946d53161839c584fb2bab1e6701155ad4b32c816d6ab0dc21a08
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4692614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c2fd98aa81c35c4a5fa9401b2f61ac48a2632d3b4b4baacc4b7982b10310097`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 28 Sep 2023 20:38:19 GMT
ADD file:8402753f294e403e92353bd65c86a6428c960be5116c0a15484b663a84f66fcd in / 
# Thu, 28 Sep 2023 20:38:20 GMT
CMD ["/bin/sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN apk add --no-cache libsasl # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:dc95107ad2a031a015320bb397f73ec151d738127175b31ad643120697dc7e90`  
		Last Modified: Thu, 28 Sep 2023 20:39:32 GMT  
		Size: 3.2 MB (3235757 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4951068162aca253cfa98ba4876636d5f13870e8ae9df08734f097bb6291e163`  
		Last Modified: Wed, 18 Oct 2023 01:04:05 GMT  
		Size: 1.2 KB (1246 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:50e4c32dd77b7a60c60be859a9848c50b3da8b95360dea46acf070797f48ab2a`  
		Last Modified: Wed, 18 Oct 2023 01:04:05 GMT  
		Size: 109.5 KB (109458 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:77aecf5d85dda7360aa3010357b83f206e1873aa4df6de5692c0c39dbf083c2a`  
		Last Modified: Wed, 18 Oct 2023 01:04:06 GMT  
		Size: 1.3 MB (1345750 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:99e49c7a1306cd1125b7dbc332a0b1b47b2408c77e975df11b090c0ab5599be3`  
		Last Modified: Wed, 18 Oct 2023 01:04:06 GMT  
		Size: 281.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:68c5ecf5461e2d137f2c403e26fe6e0532a5ecf0eedcd77a5b18254c82b9a075`  
		Last Modified: Wed, 18 Oct 2023 01:04:07 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-alpine3.18` - unknown; unknown

```console
$ docker pull memcached@sha256:f0efd827c59fd288434c24a501d257456e82560b34d98f97cfe8b132454e28b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 KB (18687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea78294aafd9f308a52d310f899433de63e91eaac550b4ace8c1b8647774c7b8`

```dockerfile
```

-	Layers:
	-	`sha256:8c15fbe468a3b1236cadb64627426b8e2cb8bb71fddd26e10cdc44abd3b3519c`  
		Last Modified: Wed, 18 Oct 2023 01:04:05 GMT  
		Size: 18.7 KB (18687 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1-alpine3.18` - linux; ppc64le

```console
$ docker pull memcached@sha256:bae49b5a412b4535ebab987425356a20af16fc1ce70c38e18f6aa6572cac522d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4460245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b845ad70056a07d2adbebdc425879a4eb74152c886dae5d8e5496c6114cd3cda`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:3450a1687b552498a987f87cb844b7f597c7181d7c3d31943d7b3036d5300d5e in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["/bin/sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN apk add --no-cache libsasl # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:4e13780adf2776477b14ef9c0f4f563f820a2fde166d472218037b979e84d31a`  
		Last Modified: Thu, 30 Nov 2023 23:20:01 GMT  
		Size: 3.3 MB (3348322 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a33c280bf18f1bba1782f90d468941796634b74c44d9aae4c406162114520e9a`  
		Last Modified: Fri, 01 Dec 2023 12:01:06 GMT  
		Size: 1.2 KB (1247 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a54d91525051bf65bd807cac3c6f1a685ac2fc6ec7f763df97c18a3ca4b6dde0`  
		Last Modified: Fri, 01 Dec 2023 12:01:07 GMT  
		Size: 123.9 KB (123864 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:73f73a883ca0c1147533ae5085475dee29244e8ef06b0455c52afa6ab50c3023`  
		Last Modified: Fri, 01 Dec 2023 12:01:07 GMT  
		Size: 986.4 KB (986410 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:183bb794a2f98d5b2192b311c4b597c47ee4ee0bb405558f67827c8afaf0b8d3`  
		Last Modified: Fri, 01 Dec 2023 12:01:07 GMT  
		Size: 280.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:556988ad767ddefdfb131bbf239cceba01e60b197c0893287ee0f6274e54a0c8`  
		Last Modified: Fri, 01 Dec 2023 12:01:08 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-alpine3.18` - unknown; unknown

```console
$ docker pull memcached@sha256:df95592ada35b125fd73982e23f99a4fc3820ab083e12870f4edb179935ec44d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.3 KB (95332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67d44fe1dc00fdfaba957619ac6567e2ba40c2bad9a422ffb5287bb160b01fe7`

```dockerfile
```

-	Layers:
	-	`sha256:4a7a9ea74e3391f7a0e156b244eb474f674d42637b77983cfd9c92b23701d5ce`  
		Last Modified: Fri, 01 Dec 2023 12:01:06 GMT  
		Size: 76.5 KB (76477 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:671ec9ab176a20a138f0a3e238976e619a6f3011f598148b2cadd4c167721f81`  
		Last Modified: Fri, 01 Dec 2023 12:01:07 GMT  
		Size: 18.9 KB (18855 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1-alpine3.18` - linux; s390x

```console
$ docker pull memcached@sha256:7af81a585082ce3ca180a3fac82a30bb37a43973123841b2dec30e5d096be8cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4285472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b785f0d9bb74e0e2b4f8772ce85a7b23cfc2e2f8dbb7ad428517b68cca17de38`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["/bin/sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN apk add --no-cache libsasl # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a7b34c58047c2f1ded65320321066565e57ddd2ed65156bde99267b8e575bf63`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:036bb49faad29b98ef9de81de4441efa5208c00e72ccea2b631c7b1c283f072d`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 112.8 KB (112781 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c1da6195feb453292bec9ae13a8968a7fbc7b611793ac2bc13df3614b514db3f`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 953.6 KB (953590 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a43896e685e7c2e1e51c75c1ed262d1c57940abdc2e68d74301201c9aa8ebdfe`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 281.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:928e080b9c3b24e2e655bd62e483670acb3c5508648e5a2784a6bebb4d252367`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-alpine3.18` - unknown; unknown

```console
$ docker pull memcached@sha256:89eda6fd40656e7c2d5de572e4bdfbd821a333eb1067170caf9074dcbc141515
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.2 KB (95207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e34e69a75d4acd1221e6dd87a6f96bcf43e52e6ebaba333e1e4cc57d391f048`

```dockerfile
```

-	Layers:
	-	`sha256:c5dd02fe5ddfbc8ce715e0e666a98ae24e73371a2a8dee859d796538f4cf0618`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 76.4 KB (76419 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:13692e9f247d60b0cd5d0d4c0ccb23a86437ea348414e8548639ba89b5e4b65a`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 18.8 KB (18788 bytes)  
		MIME: application/vnd.in-toto+json

## `memcached:1-bookworm`

```console
$ docker pull memcached@sha256:9ed83da692bea50f7d0466186e0a2b527c047993805b98c99c1794bceb27d0e8
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 14
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v5
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

### `memcached:1-bookworm` - linux; amd64

```console
$ docker pull memcached@sha256:7b0480ab945f960f703af2f286b02a7b620eb4f772e25a2a1374e0c7d32f46de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.8 MB (38815745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f65c7b1a196aa7dfe9520f598f699d5846d6ff0eed117a36ca216302174a1bb1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:d261a6f6921593f1e0b3f472ab1b1822e2c6deb0b369200f0b3370556bfad017 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1f7ce2fa46ab3942feabee654933948821303a5a821789dddab2d8c3df59e227`  
		Last Modified: Tue, 21 Nov 2023 05:25:58 GMT  
		Size: 29.1 MB (29149908 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3606f7d6f784848f3e26f4bc5fae3dde08d65681dbaba232236ac8855cddb881`  
		Last Modified: Tue, 21 Nov 2023 06:19:50 GMT  
		Size: 1.1 KB (1110 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d9e66f47c0a00f0a833454718ca9dc6504f38c45944b5ebf43ccac532dc520b6`  
		Last Modified: Tue, 21 Nov 2023 06:19:50 GMT  
		Size: 2.5 MB (2488339 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:26e0a53c88ab99ad6e23fbb12147cce82e922e4141af56338b4ec01c2ead2b07`  
		Last Modified: Tue, 21 Nov 2023 06:19:50 GMT  
		Size: 7.2 MB (7175988 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:afc0db62c179dab7a3fc4ff6848e150c3315896846d827282affab08909d6e23`  
		Last Modified: Tue, 21 Nov 2023 06:19:50 GMT  
		Size: 281.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7af609a76aa9ed2d446da8865870d0e2b3bff46785783284d956d755a714899b`  
		Last Modified: Tue, 21 Nov 2023 06:19:50 GMT  
		Size: 119.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:cb387d9a91a709e6a4193c58df1f36753dbc6c13b9788d741d6dd92ee262ea52
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3078549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3b5853b03b272d3ad2682a093fbc3b2ffd577e3c9fe01f926b5963b333208cd`

```dockerfile
```

-	Layers:
	-	`sha256:9630a5bf61090e535bcf3b7ad1349332584446ea948e10119e025a65fad57d26`  
		Last Modified: Tue, 21 Nov 2023 06:19:50 GMT  
		Size: 3.1 MB (3056780 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:a2ef4829ccc1863c60fdfcf41590326d17bfbdef204a7d37664c92bec494942b`  
		Last Modified: Tue, 21 Nov 2023 06:19:50 GMT  
		Size: 21.8 KB (21769 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1-bookworm` - linux; arm variant v5

```console
$ docker pull memcached@sha256:c5fbea0a198cb4ae068e4761d5d1abab499e4ebc80275be6b7d797196cf3db54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34849973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b72ee44b42eca798309f6aa48ed2af9feca23c5eb64e5be38fa2536110b12ce`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:1ae8e5ac45b11d01083680b765e1fcfef9f7938f89d6f424572126fa946d8cdf in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f476aef5b6e1122850e68c81ef06fc2df17e968961b060483b4d2fb33018aae3`  
		Last Modified: Tue, 21 Nov 2023 05:03:55 GMT  
		Size: 26.9 MB (26922153 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:26dadbdb945a22546f6b2c171d0bededff72d7598719ab8f3877f67129e21730`  
		Last Modified: Tue, 21 Nov 2023 16:18:13 GMT  
		Size: 1.1 KB (1109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:44f46f0b8b7c11e6cd53e82541f819c66da246b152155fff8ce762f98c25219f`  
		Last Modified: Tue, 21 Nov 2023 16:18:14 GMT  
		Size: 2.1 MB (2089268 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:639e86d18160b654876d404a88b437cea26de29151122dfe8cbed9947f1b7b10`  
		Last Modified: Tue, 21 Nov 2023 16:18:14 GMT  
		Size: 5.8 MB (5837040 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7b963217677ca57533744aee2b331f059fbb6882f27abe2cc976462604e7b560`  
		Last Modified: Tue, 21 Nov 2023 16:18:15 GMT  
		Size: 283.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ac3a1fa5d4b6c48ea8ce4c375a197047f1480fbfb37c316b7d730d026d261219`  
		Last Modified: Tue, 21 Nov 2023 16:18:15 GMT  
		Size: 120.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:cd008d8c4d507d73b5f0153ed880e81e86a53741b480bbf6b1d318510e83a288
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.7 KB (21695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85e0f40569066724c087be3d901d5c5d984043271b56a33dec281e36032017f0`

```dockerfile
```

-	Layers:
	-	`sha256:2eff64dde44b4be85375aed8309f5d20476ca81876607d799b56c31addee0cb8`  
		Last Modified: Tue, 21 Nov 2023 16:18:13 GMT  
		Size: 21.7 KB (21695 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1-bookworm` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:dd556de8d6e6b81c51ba9120fa924fbb7fae427468d82db9f2b3db124f9ac0b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.7 MB (37711361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f05ec0c73b4afc866c99864d86b1c66deb5d8bda84bf2cc78e1e763e0ed6a263`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:869c7d0747a17c53715581a2e862992eb8516c7f45f167821dfa80966a4870d1 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2c6d21737d8318aa15c4cc838475029a5efc36c0429e3d8da80d97d0b96d9aaf`  
		Last Modified: Tue, 21 Nov 2023 06:30:30 GMT  
		Size: 29.2 MB (29179277 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fa3a18531b093eb1a543ad01b2a54d4692f59bba8d49ea9793b3ff09e528cd93`  
		Last Modified: Wed, 22 Nov 2023 11:50:41 GMT  
		Size: 1.1 KB (1109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:395fd5be77a2adb2c1b863f9ba2c664074aacb120f379bbb0f45cda74cc09cf4`  
		Last Modified: Wed, 22 Nov 2023 11:50:41 GMT  
		Size: 2.3 MB (2345987 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1dbcb5e891e054cd85f29e62fff856117d8cb919630be0c7473b520168b8c261`  
		Last Modified: Wed, 22 Nov 2023 11:50:41 GMT  
		Size: 6.2 MB (6184583 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2654df736cfb30e0097cca6a637ae794285396f6e2b87031636c8056b66baed0`  
		Last Modified: Wed, 22 Nov 2023 11:50:41 GMT  
		Size: 283.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e54ea6c3f7f45d9ed3f003bcf9e0a717c342daae58d330fef355e712d15b732`  
		Last Modified: Wed, 22 Nov 2023 11:50:42 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:2b5053d245e0312a77b7827553fcf09a6b19a0bf825a7016a4125713ad0d814f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3053591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e04bc647daea7fbb746cd418f19740162bd910826c366cdcc3549c3888ad5e1b`

```dockerfile
```

-	Layers:
	-	`sha256:f04377bb8fcfc3a24c1a36aa0bdf9b2d9272b7a60e82a88b66e2bb0645703c07`  
		Last Modified: Wed, 22 Nov 2023 11:50:41 GMT  
		Size: 3.0 MB (3031971 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:601cddda9e5f7f3a82cfc305051ac3c1fc5f65a9722e4dbe06363cc8b6ea68be`  
		Last Modified: Wed, 22 Nov 2023 11:50:41 GMT  
		Size: 21.6 KB (21620 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1-bookworm` - linux; 386

```console
$ docker pull memcached@sha256:fa9dba8086765d68f2feecfc2ac08fb29c019597d09943bb480227e6cba87666
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.3 MB (39294993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93047050e75b6d4d64adb8a7c8f68cb118bad27ca9dc772120e251b174752cf9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:0c94521fdd9c0a4fdeeb9aad23e68cd053fba0dcd7c3af550aefa79377816e31 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:98bdfce9af831c2a0d0bfcca812d0039cd1666986550f552b4b4c625bd5aa31c`  
		Last Modified: Wed, 01 Nov 2023 00:43:26 GMT  
		Size: 30.2 MB (30164042 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1b647d4b10cf20ac5807101c7d0380701be684aa82f5c01ec41f674b5ef23d42`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 1.1 KB (1109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b61c058003459de4911c2901b2d799b03de754a1b9e64ffbe21a04992e962e62`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 2.5 MB (2492501 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:810b6db64df2fcc8f76941cdac75093cf35bd72ac3cd1fa5eb664e74c1f67cd8`  
		Last Modified: Wed, 01 Nov 2023 01:06:50 GMT  
		Size: 6.6 MB (6636937 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dbb899942df4149bd5fae8bac6e295285ec80f82d621f2b29c931ee348491cfb`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 282.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4a8530160ab232c37c0ddcbf5e3a731d835d378d1382843957f6c2a73b2b5be6`  
		Last Modified: Wed, 01 Nov 2023 01:06:50 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:dd7ce9519c31365127142232df2ed0b285e9acc03cd77c23c838bf932165def8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 KB (21498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eef82c92e07c11a92c337806d01cfb1c6cdc7a16608dcf304a38de34d2ef1dbb`

```dockerfile
```

-	Layers:
	-	`sha256:c0d9dd22513f8d3e791e1796d7ef1906e57c798c92dd35d0be9cf2eaecec5954`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 21.5 KB (21498 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1-bookworm` - linux; mips64le

```console
$ docker pull memcached@sha256:a7c198db1b0856aff4b1514137e473ea30bce2ef22f0192cfdce7e2e44f2a863
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.6 MB (37588022 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1654ec4454e597d7e7cb6a7d97e98208de241a3dfafc5e0532b9561eac91f013`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:e093749192323dc72b60a8440ddba26c415586f618b5e107fa264ba5eb2ca7ba in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:ebdff2138fee4a3ec27560ab1353dc51c12c2608ff721f5db3d24104872b702a`  
		Last Modified: Tue, 21 Nov 2023 04:20:35 GMT  
		Size: 29.1 MB (29141984 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:50b1ffce24cec457fe1757715d60bd669145e5babade7c57143c4b665a55389e`  
		Last Modified: Thu, 23 Nov 2023 01:10:58 GMT  
		Size: 1.1 KB (1112 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:893c712c491a058aada36756e9f176b6c6c2f3a2b3adf0cd94b896c8198ec3ee`  
		Last Modified: Thu, 23 Nov 2023 01:10:59 GMT  
		Size: 1.9 MB (1937483 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0b8443254952572331df084976853329b69a4348b3c620bb073b5c89fb943b2b`  
		Last Modified: Thu, 23 Nov 2023 01:10:59 GMT  
		Size: 6.5 MB (6507036 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:904bfc5c5c0923edd9be421332402b224bfcd49053bc9b3fae6173383f5cd395`  
		Last Modified: Thu, 23 Nov 2023 01:10:59 GMT  
		Size: 285.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c265216ad3407dbc99903d96423b3a2314bc48cc0118911d150a6bb087ff7d85`  
		Last Modified: Thu, 23 Nov 2023 01:11:00 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:e2fcd32899d09ff06793849927220bea14475e64f085972afbc1f3af74dc209b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.7 KB (21656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf1c2028769aa20a3e529d0f85c8144ba6b099f74cda0dfca2272b7831d2d7a5`

```dockerfile
```

-	Layers:
	-	`sha256:75bab713cb94cdececf4c3879050737e7cb4bbb6206daa071ea001692b53d659`  
		Last Modified: Thu, 23 Nov 2023 01:10:58 GMT  
		Size: 21.7 KB (21656 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1-bookworm` - linux; ppc64le

```console
$ docker pull memcached@sha256:d8d106a88d6a15fadf738e59a6dcfc3942f11c7a2d19b7473abce66af7f4d19c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.0 MB (43030916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85da4ca798d44fc951b843ec85c410207ecc3c56af6d1bf7c321c91266d54e1b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:8b22a531b6611a1e63dfc20e4e2931592e2d821bd4b64c4b2810bb9a36640c02 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c570d04e61d8e35a3c8f12179d048d701451f97f9cf2099ea3e3738512dbf062`  
		Last Modified: Tue, 21 Nov 2023 04:28:58 GMT  
		Size: 33.1 MB (33141607 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bcd0cf90a66e23cd3d72b99e7d36129b0e846407a07c30031b0c1e4ba115cd30`  
		Last Modified: Tue, 21 Nov 2023 23:46:47 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5e4166a0e033df4117b469f840c6f5527e87dbd13c582c0b50c182b4bb3ead79`  
		Last Modified: Tue, 21 Nov 2023 23:46:47 GMT  
		Size: 2.7 MB (2698215 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:947b7328e0db59b9870fe9c6d6b7fc4e8a8f1fef3d2a36064fe3d60f5314652d`  
		Last Modified: Tue, 21 Nov 2023 23:46:48 GMT  
		Size: 7.2 MB (7189577 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f011f72796530a711f1de9d543435299d02ed3636e4cd28aee1fa493fbc2bf4`  
		Last Modified: Tue, 21 Nov 2023 23:46:47 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9d27046f19e474530b87e1d0b429e9d85f403210dd3d91bf60d8303fef03af96`  
		Last Modified: Tue, 21 Nov 2023 23:46:48 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:4269af6aa39a29d6dca352659fbf04b7d1bb4e65151e63a3ffcf2749d853597e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3067036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6e9626f30d490d2014e9fbb19add0b6ac0f63c8f4af2082d04750fea7ec35ff`

```dockerfile
```

-	Layers:
	-	`sha256:70759e1722d82b89de5c0d71ba2050ecc9f29d95ee758369044a1fc79026a546`  
		Last Modified: Tue, 21 Nov 2023 23:46:47 GMT  
		Size: 3.0 MB (3045366 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:4f34d59241ff06b2bd0cb8239d96be938e1e13470264898863f307f84ab275b6`  
		Last Modified: Tue, 21 Nov 2023 23:46:47 GMT  
		Size: 21.7 KB (21670 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1-bookworm` - linux; s390x

```console
$ docker pull memcached@sha256:312625a69b30a0a0371060c62ec97a621d587675e55a8ced694303d8a7015d30
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.7 MB (35745726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13ebe1c7df28f24c49c7dc749c55574a0a51a84e31dcff380e6caa5441fca944`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:c33fa9fdde73983850798b6eb1cd062e0398109d1d773e6a937fead7475c8efc in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6daa625e5a040476e253e7acd0befa74254a4865ec836d6334a544d82a21d4be`  
		Last Modified: Tue, 21 Nov 2023 05:10:21 GMT  
		Size: 27.5 MB (27512885 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:410539cfd307a2626bf5520b21d1cff0d4c8a336ebea36ed08878d81eca92847`  
		Last Modified: Tue, 21 Nov 2023 15:56:02 GMT  
		Size: 1.1 KB (1109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1ba4cc4f8ba1aa1865931fde910e1ebac220aea9a207eff2f2556bc289a513d3`  
		Last Modified: Tue, 21 Nov 2023 15:56:03 GMT  
		Size: 2.2 MB (2152517 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a47325d5bddeb006ca8a01a6239f747f4ed2c21fd6a28226bdfe46d1981d8962`  
		Last Modified: Tue, 21 Nov 2023 15:56:03 GMT  
		Size: 6.1 MB (6078811 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:32f889bfd6f6b6b2d773abb9f72f86fe0c7469d2a271e5bd209a3eb9b1c61dea`  
		Last Modified: Tue, 21 Nov 2023 15:56:04 GMT  
		Size: 283.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:56ce84d34f650bc21b164be1bb375a2b43c761943b4d06497991ceca18be1009`  
		Last Modified: Tue, 21 Nov 2023 15:56:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:b070f08010996b181adf3fbb4b9004e0d125115bf1380df8c4ddb96a99827218
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3068089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:307228ea8d7a2ce5fee0e1c4c36745e1c0244aa6d316102bde5b655af1bedd24`

```dockerfile
```

-	Layers:
	-	`sha256:640994e8299bce5ed690d70d55a1bc2035868614a169e4cda3391dafb76e9469`  
		Last Modified: Tue, 21 Nov 2023 15:56:03 GMT  
		Size: 3.0 MB (3046321 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:1893b50125646067935dd81f10c259d7b0c3b7cf2f42c81abe2b0f93e45f4250`  
		Last Modified: Tue, 21 Nov 2023 15:56:03 GMT  
		Size: 21.8 KB (21768 bytes)  
		MIME: application/vnd.in-toto+json

## `memcached:1.6`

```console
$ docker pull memcached@sha256:e86e92011ac296d084a8f12dc414c01952d86b7711dfc936fbd325f342581631
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 15
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v5
	-	unknown; unknown
	-	linux; arm variant v7
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

### `memcached:1.6` - linux; amd64

```console
$ docker pull memcached@sha256:7b0480ab945f960f703af2f286b02a7b620eb4f772e25a2a1374e0c7d32f46de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.8 MB (38815745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f65c7b1a196aa7dfe9520f598f699d5846d6ff0eed117a36ca216302174a1bb1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:d261a6f6921593f1e0b3f472ab1b1822e2c6deb0b369200f0b3370556bfad017 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1f7ce2fa46ab3942feabee654933948821303a5a821789dddab2d8c3df59e227`  
		Last Modified: Tue, 21 Nov 2023 05:25:58 GMT  
		Size: 29.1 MB (29149908 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3606f7d6f784848f3e26f4bc5fae3dde08d65681dbaba232236ac8855cddb881`  
		Last Modified: Tue, 21 Nov 2023 06:19:50 GMT  
		Size: 1.1 KB (1110 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d9e66f47c0a00f0a833454718ca9dc6504f38c45944b5ebf43ccac532dc520b6`  
		Last Modified: Tue, 21 Nov 2023 06:19:50 GMT  
		Size: 2.5 MB (2488339 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:26e0a53c88ab99ad6e23fbb12147cce82e922e4141af56338b4ec01c2ead2b07`  
		Last Modified: Tue, 21 Nov 2023 06:19:50 GMT  
		Size: 7.2 MB (7175988 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:afc0db62c179dab7a3fc4ff6848e150c3315896846d827282affab08909d6e23`  
		Last Modified: Tue, 21 Nov 2023 06:19:50 GMT  
		Size: 281.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7af609a76aa9ed2d446da8865870d0e2b3bff46785783284d956d755a714899b`  
		Last Modified: Tue, 21 Nov 2023 06:19:50 GMT  
		Size: 119.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6` - unknown; unknown

```console
$ docker pull memcached@sha256:cb387d9a91a709e6a4193c58df1f36753dbc6c13b9788d741d6dd92ee262ea52
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3078549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3b5853b03b272d3ad2682a093fbc3b2ffd577e3c9fe01f926b5963b333208cd`

```dockerfile
```

-	Layers:
	-	`sha256:9630a5bf61090e535bcf3b7ad1349332584446ea948e10119e025a65fad57d26`  
		Last Modified: Tue, 21 Nov 2023 06:19:50 GMT  
		Size: 3.1 MB (3056780 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:a2ef4829ccc1863c60fdfcf41590326d17bfbdef204a7d37664c92bec494942b`  
		Last Modified: Tue, 21 Nov 2023 06:19:50 GMT  
		Size: 21.8 KB (21769 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6` - linux; arm variant v5

```console
$ docker pull memcached@sha256:c5fbea0a198cb4ae068e4761d5d1abab499e4ebc80275be6b7d797196cf3db54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34849973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b72ee44b42eca798309f6aa48ed2af9feca23c5eb64e5be38fa2536110b12ce`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:1ae8e5ac45b11d01083680b765e1fcfef9f7938f89d6f424572126fa946d8cdf in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f476aef5b6e1122850e68c81ef06fc2df17e968961b060483b4d2fb33018aae3`  
		Last Modified: Tue, 21 Nov 2023 05:03:55 GMT  
		Size: 26.9 MB (26922153 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:26dadbdb945a22546f6b2c171d0bededff72d7598719ab8f3877f67129e21730`  
		Last Modified: Tue, 21 Nov 2023 16:18:13 GMT  
		Size: 1.1 KB (1109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:44f46f0b8b7c11e6cd53e82541f819c66da246b152155fff8ce762f98c25219f`  
		Last Modified: Tue, 21 Nov 2023 16:18:14 GMT  
		Size: 2.1 MB (2089268 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:639e86d18160b654876d404a88b437cea26de29151122dfe8cbed9947f1b7b10`  
		Last Modified: Tue, 21 Nov 2023 16:18:14 GMT  
		Size: 5.8 MB (5837040 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7b963217677ca57533744aee2b331f059fbb6882f27abe2cc976462604e7b560`  
		Last Modified: Tue, 21 Nov 2023 16:18:15 GMT  
		Size: 283.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ac3a1fa5d4b6c48ea8ce4c375a197047f1480fbfb37c316b7d730d026d261219`  
		Last Modified: Tue, 21 Nov 2023 16:18:15 GMT  
		Size: 120.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6` - unknown; unknown

```console
$ docker pull memcached@sha256:cd008d8c4d507d73b5f0153ed880e81e86a53741b480bbf6b1d318510e83a288
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.7 KB (21695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85e0f40569066724c087be3d901d5c5d984043271b56a33dec281e36032017f0`

```dockerfile
```

-	Layers:
	-	`sha256:2eff64dde44b4be85375aed8309f5d20476ca81876607d799b56c31addee0cb8`  
		Last Modified: Tue, 21 Nov 2023 16:18:13 GMT  
		Size: 21.7 KB (21695 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6` - linux; arm variant v7

```console
$ docker pull memcached@sha256:2841be0a36134563966c09a6ed68b21053d20342ec8736cf92763c28077ead43
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28094215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cf74ffa940dd93988fc0beb6698c5796563c82a40b7dd668153969f64d2e6ca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 09 Feb 2023 06:12:09 GMT
ADD file:5f1a343224e8486690bd90dd1e50c8d84b3d770c51bb6829544e5cf650c0419c in / 
# Thu, 09 Feb 2023 06:12:10 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 07:52:31 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 09 Feb 2023 07:52:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:52:35 GMT
ENV MEMCACHED_VERSION=1.6.18
# Thu, 09 Feb 2023 07:52:35 GMT
ENV MEMCACHED_SHA1=be16909bb75ab972ee5fe438312501de01c4725a
# Thu, 09 Feb 2023 07:55:44 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 09 Feb 2023 07:55:44 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 09 Feb 2023 07:55:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 09 Feb 2023 07:55:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Feb 2023 07:55:44 GMT
USER memcache
# Thu, 09 Feb 2023 07:55:45 GMT
EXPOSE 11211
# Thu, 09 Feb 2023 07:55:45 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:e7318f6106ad75d7d482ae9dddf4d927b0872ef3ddb6e1330aa691fc8d17279e`  
		Last Modified: Thu, 09 Feb 2023 06:19:19 GMT  
		Size: 26.6 MB (26577666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de49d9d72daf1680b5f1b9532dd2eb0162829f36c8db9669935462636fbf99d9`  
		Last Modified: Thu, 09 Feb 2023 08:06:11 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0beac9d5bcac946f8c54c72b8a9c136914b1aa7a5fe2b8c3df4c7d8858ea6559`  
		Last Modified: Thu, 09 Feb 2023 08:06:11 GMT  
		Size: 312.1 KB (312088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4c9e5a265394e4c0f357779e6195a4e82d767a3691a0e77d427e56651c3e54a`  
		Last Modified: Thu, 09 Feb 2023 08:06:11 GMT  
		Size: 1.2 MB (1199163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ea82ad892fe1ae8623d84e32c8c027087cda8aa49e40d4546ed6942e471c60`  
		Last Modified: Thu, 09 Feb 2023 08:06:11 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2ae3bcdc0d114ba49a67df022b6f7215fc87f1f50e64939fcfbbec4eaadee5`  
		Last Modified: Thu, 09 Feb 2023 08:06:11 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:dd556de8d6e6b81c51ba9120fa924fbb7fae427468d82db9f2b3db124f9ac0b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.7 MB (37711361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f05ec0c73b4afc866c99864d86b1c66deb5d8bda84bf2cc78e1e763e0ed6a263`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:869c7d0747a17c53715581a2e862992eb8516c7f45f167821dfa80966a4870d1 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2c6d21737d8318aa15c4cc838475029a5efc36c0429e3d8da80d97d0b96d9aaf`  
		Last Modified: Tue, 21 Nov 2023 06:30:30 GMT  
		Size: 29.2 MB (29179277 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fa3a18531b093eb1a543ad01b2a54d4692f59bba8d49ea9793b3ff09e528cd93`  
		Last Modified: Wed, 22 Nov 2023 11:50:41 GMT  
		Size: 1.1 KB (1109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:395fd5be77a2adb2c1b863f9ba2c664074aacb120f379bbb0f45cda74cc09cf4`  
		Last Modified: Wed, 22 Nov 2023 11:50:41 GMT  
		Size: 2.3 MB (2345987 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1dbcb5e891e054cd85f29e62fff856117d8cb919630be0c7473b520168b8c261`  
		Last Modified: Wed, 22 Nov 2023 11:50:41 GMT  
		Size: 6.2 MB (6184583 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2654df736cfb30e0097cca6a637ae794285396f6e2b87031636c8056b66baed0`  
		Last Modified: Wed, 22 Nov 2023 11:50:41 GMT  
		Size: 283.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e54ea6c3f7f45d9ed3f003bcf9e0a717c342daae58d330fef355e712d15b732`  
		Last Modified: Wed, 22 Nov 2023 11:50:42 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6` - unknown; unknown

```console
$ docker pull memcached@sha256:2b5053d245e0312a77b7827553fcf09a6b19a0bf825a7016a4125713ad0d814f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3053591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e04bc647daea7fbb746cd418f19740162bd910826c366cdcc3549c3888ad5e1b`

```dockerfile
```

-	Layers:
	-	`sha256:f04377bb8fcfc3a24c1a36aa0bdf9b2d9272b7a60e82a88b66e2bb0645703c07`  
		Last Modified: Wed, 22 Nov 2023 11:50:41 GMT  
		Size: 3.0 MB (3031971 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:601cddda9e5f7f3a82cfc305051ac3c1fc5f65a9722e4dbe06363cc8b6ea68be`  
		Last Modified: Wed, 22 Nov 2023 11:50:41 GMT  
		Size: 21.6 KB (21620 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6` - linux; 386

```console
$ docker pull memcached@sha256:fa9dba8086765d68f2feecfc2ac08fb29c019597d09943bb480227e6cba87666
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.3 MB (39294993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93047050e75b6d4d64adb8a7c8f68cb118bad27ca9dc772120e251b174752cf9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:0c94521fdd9c0a4fdeeb9aad23e68cd053fba0dcd7c3af550aefa79377816e31 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:98bdfce9af831c2a0d0bfcca812d0039cd1666986550f552b4b4c625bd5aa31c`  
		Last Modified: Wed, 01 Nov 2023 00:43:26 GMT  
		Size: 30.2 MB (30164042 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1b647d4b10cf20ac5807101c7d0380701be684aa82f5c01ec41f674b5ef23d42`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 1.1 KB (1109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b61c058003459de4911c2901b2d799b03de754a1b9e64ffbe21a04992e962e62`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 2.5 MB (2492501 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:810b6db64df2fcc8f76941cdac75093cf35bd72ac3cd1fa5eb664e74c1f67cd8`  
		Last Modified: Wed, 01 Nov 2023 01:06:50 GMT  
		Size: 6.6 MB (6636937 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dbb899942df4149bd5fae8bac6e295285ec80f82d621f2b29c931ee348491cfb`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 282.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4a8530160ab232c37c0ddcbf5e3a731d835d378d1382843957f6c2a73b2b5be6`  
		Last Modified: Wed, 01 Nov 2023 01:06:50 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6` - unknown; unknown

```console
$ docker pull memcached@sha256:dd7ce9519c31365127142232df2ed0b285e9acc03cd77c23c838bf932165def8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 KB (21498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eef82c92e07c11a92c337806d01cfb1c6cdc7a16608dcf304a38de34d2ef1dbb`

```dockerfile
```

-	Layers:
	-	`sha256:c0d9dd22513f8d3e791e1796d7ef1906e57c798c92dd35d0be9cf2eaecec5954`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 21.5 KB (21498 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6` - linux; mips64le

```console
$ docker pull memcached@sha256:a7c198db1b0856aff4b1514137e473ea30bce2ef22f0192cfdce7e2e44f2a863
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.6 MB (37588022 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1654ec4454e597d7e7cb6a7d97e98208de241a3dfafc5e0532b9561eac91f013`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:e093749192323dc72b60a8440ddba26c415586f618b5e107fa264ba5eb2ca7ba in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:ebdff2138fee4a3ec27560ab1353dc51c12c2608ff721f5db3d24104872b702a`  
		Last Modified: Tue, 21 Nov 2023 04:20:35 GMT  
		Size: 29.1 MB (29141984 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:50b1ffce24cec457fe1757715d60bd669145e5babade7c57143c4b665a55389e`  
		Last Modified: Thu, 23 Nov 2023 01:10:58 GMT  
		Size: 1.1 KB (1112 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:893c712c491a058aada36756e9f176b6c6c2f3a2b3adf0cd94b896c8198ec3ee`  
		Last Modified: Thu, 23 Nov 2023 01:10:59 GMT  
		Size: 1.9 MB (1937483 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0b8443254952572331df084976853329b69a4348b3c620bb073b5c89fb943b2b`  
		Last Modified: Thu, 23 Nov 2023 01:10:59 GMT  
		Size: 6.5 MB (6507036 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:904bfc5c5c0923edd9be421332402b224bfcd49053bc9b3fae6173383f5cd395`  
		Last Modified: Thu, 23 Nov 2023 01:10:59 GMT  
		Size: 285.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c265216ad3407dbc99903d96423b3a2314bc48cc0118911d150a6bb087ff7d85`  
		Last Modified: Thu, 23 Nov 2023 01:11:00 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6` - unknown; unknown

```console
$ docker pull memcached@sha256:e2fcd32899d09ff06793849927220bea14475e64f085972afbc1f3af74dc209b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.7 KB (21656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf1c2028769aa20a3e529d0f85c8144ba6b099f74cda0dfca2272b7831d2d7a5`

```dockerfile
```

-	Layers:
	-	`sha256:75bab713cb94cdececf4c3879050737e7cb4bbb6206daa071ea001692b53d659`  
		Last Modified: Thu, 23 Nov 2023 01:10:58 GMT  
		Size: 21.7 KB (21656 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6` - linux; ppc64le

```console
$ docker pull memcached@sha256:d8d106a88d6a15fadf738e59a6dcfc3942f11c7a2d19b7473abce66af7f4d19c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.0 MB (43030916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85da4ca798d44fc951b843ec85c410207ecc3c56af6d1bf7c321c91266d54e1b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:8b22a531b6611a1e63dfc20e4e2931592e2d821bd4b64c4b2810bb9a36640c02 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c570d04e61d8e35a3c8f12179d048d701451f97f9cf2099ea3e3738512dbf062`  
		Last Modified: Tue, 21 Nov 2023 04:28:58 GMT  
		Size: 33.1 MB (33141607 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bcd0cf90a66e23cd3d72b99e7d36129b0e846407a07c30031b0c1e4ba115cd30`  
		Last Modified: Tue, 21 Nov 2023 23:46:47 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5e4166a0e033df4117b469f840c6f5527e87dbd13c582c0b50c182b4bb3ead79`  
		Last Modified: Tue, 21 Nov 2023 23:46:47 GMT  
		Size: 2.7 MB (2698215 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:947b7328e0db59b9870fe9c6d6b7fc4e8a8f1fef3d2a36064fe3d60f5314652d`  
		Last Modified: Tue, 21 Nov 2023 23:46:48 GMT  
		Size: 7.2 MB (7189577 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f011f72796530a711f1de9d543435299d02ed3636e4cd28aee1fa493fbc2bf4`  
		Last Modified: Tue, 21 Nov 2023 23:46:47 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9d27046f19e474530b87e1d0b429e9d85f403210dd3d91bf60d8303fef03af96`  
		Last Modified: Tue, 21 Nov 2023 23:46:48 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6` - unknown; unknown

```console
$ docker pull memcached@sha256:4269af6aa39a29d6dca352659fbf04b7d1bb4e65151e63a3ffcf2749d853597e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3067036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6e9626f30d490d2014e9fbb19add0b6ac0f63c8f4af2082d04750fea7ec35ff`

```dockerfile
```

-	Layers:
	-	`sha256:70759e1722d82b89de5c0d71ba2050ecc9f29d95ee758369044a1fc79026a546`  
		Last Modified: Tue, 21 Nov 2023 23:46:47 GMT  
		Size: 3.0 MB (3045366 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:4f34d59241ff06b2bd0cb8239d96be938e1e13470264898863f307f84ab275b6`  
		Last Modified: Tue, 21 Nov 2023 23:46:47 GMT  
		Size: 21.7 KB (21670 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6` - linux; s390x

```console
$ docker pull memcached@sha256:312625a69b30a0a0371060c62ec97a621d587675e55a8ced694303d8a7015d30
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.7 MB (35745726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13ebe1c7df28f24c49c7dc749c55574a0a51a84e31dcff380e6caa5441fca944`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:c33fa9fdde73983850798b6eb1cd062e0398109d1d773e6a937fead7475c8efc in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6daa625e5a040476e253e7acd0befa74254a4865ec836d6334a544d82a21d4be`  
		Last Modified: Tue, 21 Nov 2023 05:10:21 GMT  
		Size: 27.5 MB (27512885 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:410539cfd307a2626bf5520b21d1cff0d4c8a336ebea36ed08878d81eca92847`  
		Last Modified: Tue, 21 Nov 2023 15:56:02 GMT  
		Size: 1.1 KB (1109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1ba4cc4f8ba1aa1865931fde910e1ebac220aea9a207eff2f2556bc289a513d3`  
		Last Modified: Tue, 21 Nov 2023 15:56:03 GMT  
		Size: 2.2 MB (2152517 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a47325d5bddeb006ca8a01a6239f747f4ed2c21fd6a28226bdfe46d1981d8962`  
		Last Modified: Tue, 21 Nov 2023 15:56:03 GMT  
		Size: 6.1 MB (6078811 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:32f889bfd6f6b6b2d773abb9f72f86fe0c7469d2a271e5bd209a3eb9b1c61dea`  
		Last Modified: Tue, 21 Nov 2023 15:56:04 GMT  
		Size: 283.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:56ce84d34f650bc21b164be1bb375a2b43c761943b4d06497991ceca18be1009`  
		Last Modified: Tue, 21 Nov 2023 15:56:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6` - unknown; unknown

```console
$ docker pull memcached@sha256:b070f08010996b181adf3fbb4b9004e0d125115bf1380df8c4ddb96a99827218
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3068089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:307228ea8d7a2ce5fee0e1c4c36745e1c0244aa6d316102bde5b655af1bedd24`

```dockerfile
```

-	Layers:
	-	`sha256:640994e8299bce5ed690d70d55a1bc2035868614a169e4cda3391dafb76e9469`  
		Last Modified: Tue, 21 Nov 2023 15:56:03 GMT  
		Size: 3.0 MB (3046321 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:1893b50125646067935dd81f10c259d7b0c3b7cf2f42c81abe2b0f93e45f4250`  
		Last Modified: Tue, 21 Nov 2023 15:56:03 GMT  
		Size: 21.8 KB (21768 bytes)  
		MIME: application/vnd.in-toto+json

## `memcached:1.6-alpine`

```console
$ docker pull memcached@sha256:e8191559af396cda215a055e31a07bfc8178241854fa20f9e2cd32e4f1f5169e
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 11
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `memcached:1.6-alpine` - linux; amd64

```console
$ docker pull memcached@sha256:f85dfa7d8ec9dc1b785c37ccf6dfa62bca5fec355c32ddf7957116376863284a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4471146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f687f33554b696db4e2422b52d11bd36b20649d152ca63d20848c83b0679237f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["/bin/sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN apk add --no-cache libsasl # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ce5e53c5eb3023b585266ac7ee39c0b268a83b4e16556b72f52bd67e39f596be`  
		Last Modified: Fri, 01 Dec 2023 00:14:01 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e958dac8143e41701702904f092ab10b8682434d3d88e5af758dafaeb3317428`  
		Last Modified: Fri, 01 Dec 2023 00:14:01 GMT  
		Size: 108.0 KB (107998 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:61dfbf83553658c4ab4a5ae4477150c88a3f30da8309b9cfefdc185b3764e501`  
		Last Modified: Fri, 01 Dec 2023 00:14:01 GMT  
		Size: 959.1 KB (959085 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8b397213e2806c5c7c6aca6c20bc2f69362c9f6204c5d3947eaaf870176d9a36`  
		Last Modified: Fri, 01 Dec 2023 00:14:01 GMT  
		Size: 277.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8c404d1dff37be469e83d35363176296e0129304273844e38a69edbd6861f08c`  
		Last Modified: Fri, 01 Dec 2023 00:14:02 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6-alpine` - unknown; unknown

```console
$ docker pull memcached@sha256:6a508d9bd488a6e6f8bbaae93d8ff14548111b267a7440f64edec96b04f8a3cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 KB (97008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fdbf48b2b61dd467eec02ffd7b0e996989023a93d9ecbc7a655a0755362c38a`

```dockerfile
```

-	Layers:
	-	`sha256:5c3e16fb5448bac47fadf2a80df72f13e831b463525dc9823da6c85f1770bf69`  
		Last Modified: Fri, 01 Dec 2023 00:14:01 GMT  
		Size: 78.1 KB (78055 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:1d5f7cf7dffd0d16953251b75fd8b7224aae91e57357d5af853c41398d72a5f7`  
		Last Modified: Fri, 01 Dec 2023 00:14:01 GMT  
		Size: 19.0 KB (18953 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6-alpine` - linux; arm variant v7

```console
$ docker pull memcached@sha256:79a5646a0c845a791f36017fda3292281b48295b06c53f13d62c9f94237d4731
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3960292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2afac0e49af3ce3f1769abe11a29f8f5610c6a736d8c5b6c7b9770c8d8e94e91`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 06:43:29 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 17 Dec 2020 06:43:31 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Thu, 17 Dec 2020 06:43:33 GMT
ENV MEMCACHED_VERSION=1.6.9
# Thu, 17 Dec 2020 06:43:35 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Thu, 17 Dec 2020 06:46:32 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 17 Dec 2020 06:46:33 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Dec 2020 06:46:35 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Dec 2020 06:46:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 06:46:36 GMT
USER memcache
# Thu, 17 Dec 2020 06:46:38 GMT
EXPOSE 11211
# Thu, 17 Dec 2020 06:46:39 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68564bbfc09f153688e942bf54d5375d1e27f3507c0bed6b038c2ac8ce095aa5`  
		Last Modified: Thu, 17 Dec 2020 06:46:58 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cac3a91edee49d0b08a25706ae86059bed89941a08b496e72ef092e57c4ecb3`  
		Last Modified: Thu, 17 Dec 2020 06:46:58 GMT  
		Size: 13.8 KB (13825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf16e9bb942ec42a35a792beab65aea843209e7bdde7e856499b9fc85f93bc4e`  
		Last Modified: Thu, 17 Dec 2020 06:46:58 GMT  
		Size: 1.5 MB (1537248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc15394239bd0c083e1b6df806aa5ffeb8b9cc7e80113afc2959721de49f90d1`  
		Last Modified: Thu, 17 Dec 2020 06:46:58 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482f0eb571548eae5720c652ff7da13558e56a8722dc9932cf7eb1ef3eb33acb`  
		Last Modified: Thu, 17 Dec 2020 06:46:58 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:e9673caac3d318f89edf7ca6eaba8910416292f12f0f0abbf3d862a8b5af88ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4406434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a4e56736197b019e201b69449a358660e6806d076b61fd473dbcbb11caf5197`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["/bin/sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN apk add --no-cache libsasl # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4962e560ef629491acb51e64b06a5ee52545098f8403705778786a404e81434b`  
		Last Modified: Fri, 01 Dec 2023 15:25:24 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d4b10238ba82be69f174742e8ae9cd6e4484f32dce6eeb40dcbe3c5a4e0a1480`  
		Last Modified: Fri, 01 Dec 2023 15:25:24 GMT  
		Size: 124.1 KB (124087 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:276ae0cb4d4371459c3116e0453691ac59cdd9a6d649cb27bb3d3a090ef10fbf`  
		Last Modified: Fri, 01 Dec 2023 15:25:24 GMT  
		Size: 947.7 KB (947670 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:315ab34d41c816b04b8d07e4b7db199c17340b3b882b52819a0564f6be31a04c`  
		Last Modified: Fri, 01 Dec 2023 15:25:24 GMT  
		Size: 278.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:024d99cdc8f15c63cc478d1850db680f8c0dfae1ea2a5bca55e41fb0db12d020`  
		Last Modified: Fri, 01 Dec 2023 15:25:25 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6-alpine` - unknown; unknown

```console
$ docker pull memcached@sha256:91dac18281e4a194ee9756cf2652c70b2fb0bd2ba9d26c5c86d44c762d111821
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.9 KB (96880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3590bb02748f6b9e8a22ef90e7b41976bcb90189d98a78beae80f5aab1cd1cf4`

```dockerfile
```

-	Layers:
	-	`sha256:605a9d206d49d790bef9ce82c45179355571f37a91c5730ca6f59a03e13c0c76`  
		Last Modified: Fri, 01 Dec 2023 15:25:24 GMT  
		Size: 78.1 KB (78074 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:95803ef4905954256ae922386b3196bdafabd328ecd648b88ed7d8c13ec3b640`  
		Last Modified: Fri, 01 Dec 2023 15:25:24 GMT  
		Size: 18.8 KB (18806 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6-alpine` - linux; 386

```console
$ docker pull memcached@sha256:c281c55fd61946d53161839c584fb2bab1e6701155ad4b32c816d6ab0dc21a08
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4692614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c2fd98aa81c35c4a5fa9401b2f61ac48a2632d3b4b4baacc4b7982b10310097`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 28 Sep 2023 20:38:19 GMT
ADD file:8402753f294e403e92353bd65c86a6428c960be5116c0a15484b663a84f66fcd in / 
# Thu, 28 Sep 2023 20:38:20 GMT
CMD ["/bin/sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN apk add --no-cache libsasl # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:dc95107ad2a031a015320bb397f73ec151d738127175b31ad643120697dc7e90`  
		Last Modified: Thu, 28 Sep 2023 20:39:32 GMT  
		Size: 3.2 MB (3235757 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4951068162aca253cfa98ba4876636d5f13870e8ae9df08734f097bb6291e163`  
		Last Modified: Wed, 18 Oct 2023 01:04:05 GMT  
		Size: 1.2 KB (1246 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:50e4c32dd77b7a60c60be859a9848c50b3da8b95360dea46acf070797f48ab2a`  
		Last Modified: Wed, 18 Oct 2023 01:04:05 GMT  
		Size: 109.5 KB (109458 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:77aecf5d85dda7360aa3010357b83f206e1873aa4df6de5692c0c39dbf083c2a`  
		Last Modified: Wed, 18 Oct 2023 01:04:06 GMT  
		Size: 1.3 MB (1345750 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:99e49c7a1306cd1125b7dbc332a0b1b47b2408c77e975df11b090c0ab5599be3`  
		Last Modified: Wed, 18 Oct 2023 01:04:06 GMT  
		Size: 281.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:68c5ecf5461e2d137f2c403e26fe6e0532a5ecf0eedcd77a5b18254c82b9a075`  
		Last Modified: Wed, 18 Oct 2023 01:04:07 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6-alpine` - unknown; unknown

```console
$ docker pull memcached@sha256:f0efd827c59fd288434c24a501d257456e82560b34d98f97cfe8b132454e28b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 KB (18687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea78294aafd9f308a52d310f899433de63e91eaac550b4ace8c1b8647774c7b8`

```dockerfile
```

-	Layers:
	-	`sha256:8c15fbe468a3b1236cadb64627426b8e2cb8bb71fddd26e10cdc44abd3b3519c`  
		Last Modified: Wed, 18 Oct 2023 01:04:05 GMT  
		Size: 18.7 KB (18687 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:bae49b5a412b4535ebab987425356a20af16fc1ce70c38e18f6aa6572cac522d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4460245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b845ad70056a07d2adbebdc425879a4eb74152c886dae5d8e5496c6114cd3cda`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:3450a1687b552498a987f87cb844b7f597c7181d7c3d31943d7b3036d5300d5e in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["/bin/sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN apk add --no-cache libsasl # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:4e13780adf2776477b14ef9c0f4f563f820a2fde166d472218037b979e84d31a`  
		Last Modified: Thu, 30 Nov 2023 23:20:01 GMT  
		Size: 3.3 MB (3348322 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a33c280bf18f1bba1782f90d468941796634b74c44d9aae4c406162114520e9a`  
		Last Modified: Fri, 01 Dec 2023 12:01:06 GMT  
		Size: 1.2 KB (1247 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a54d91525051bf65bd807cac3c6f1a685ac2fc6ec7f763df97c18a3ca4b6dde0`  
		Last Modified: Fri, 01 Dec 2023 12:01:07 GMT  
		Size: 123.9 KB (123864 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:73f73a883ca0c1147533ae5085475dee29244e8ef06b0455c52afa6ab50c3023`  
		Last Modified: Fri, 01 Dec 2023 12:01:07 GMT  
		Size: 986.4 KB (986410 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:183bb794a2f98d5b2192b311c4b597c47ee4ee0bb405558f67827c8afaf0b8d3`  
		Last Modified: Fri, 01 Dec 2023 12:01:07 GMT  
		Size: 280.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:556988ad767ddefdfb131bbf239cceba01e60b197c0893287ee0f6274e54a0c8`  
		Last Modified: Fri, 01 Dec 2023 12:01:08 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6-alpine` - unknown; unknown

```console
$ docker pull memcached@sha256:df95592ada35b125fd73982e23f99a4fc3820ab083e12870f4edb179935ec44d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.3 KB (95332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67d44fe1dc00fdfaba957619ac6567e2ba40c2bad9a422ffb5287bb160b01fe7`

```dockerfile
```

-	Layers:
	-	`sha256:4a7a9ea74e3391f7a0e156b244eb474f674d42637b77983cfd9c92b23701d5ce`  
		Last Modified: Fri, 01 Dec 2023 12:01:06 GMT  
		Size: 76.5 KB (76477 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:671ec9ab176a20a138f0a3e238976e619a6f3011f598148b2cadd4c167721f81`  
		Last Modified: Fri, 01 Dec 2023 12:01:07 GMT  
		Size: 18.9 KB (18855 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6-alpine` - linux; s390x

```console
$ docker pull memcached@sha256:7af81a585082ce3ca180a3fac82a30bb37a43973123841b2dec30e5d096be8cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4285472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b785f0d9bb74e0e2b4f8772ce85a7b23cfc2e2f8dbb7ad428517b68cca17de38`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["/bin/sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN apk add --no-cache libsasl # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a7b34c58047c2f1ded65320321066565e57ddd2ed65156bde99267b8e575bf63`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:036bb49faad29b98ef9de81de4441efa5208c00e72ccea2b631c7b1c283f072d`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 112.8 KB (112781 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c1da6195feb453292bec9ae13a8968a7fbc7b611793ac2bc13df3614b514db3f`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 953.6 KB (953590 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a43896e685e7c2e1e51c75c1ed262d1c57940abdc2e68d74301201c9aa8ebdfe`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 281.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:928e080b9c3b24e2e655bd62e483670acb3c5508648e5a2784a6bebb4d252367`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6-alpine` - unknown; unknown

```console
$ docker pull memcached@sha256:89eda6fd40656e7c2d5de572e4bdfbd821a333eb1067170caf9074dcbc141515
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.2 KB (95207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e34e69a75d4acd1221e6dd87a6f96bcf43e52e6ebaba333e1e4cc57d391f048`

```dockerfile
```

-	Layers:
	-	`sha256:c5dd02fe5ddfbc8ce715e0e666a98ae24e73371a2a8dee859d796538f4cf0618`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 76.4 KB (76419 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:13692e9f247d60b0cd5d0d4c0ccb23a86437ea348414e8548639ba89b5e4b65a`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 18.8 KB (18788 bytes)  
		MIME: application/vnd.in-toto+json

## `memcached:1.6-alpine3.18`

```console
$ docker pull memcached@sha256:93a9ff5ab97a213a027913f59bf902a118fa9750f88dbd4d513ebd920428820e
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 10
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `memcached:1.6-alpine3.18` - linux; amd64

```console
$ docker pull memcached@sha256:f85dfa7d8ec9dc1b785c37ccf6dfa62bca5fec355c32ddf7957116376863284a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4471146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f687f33554b696db4e2422b52d11bd36b20649d152ca63d20848c83b0679237f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["/bin/sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN apk add --no-cache libsasl # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ce5e53c5eb3023b585266ac7ee39c0b268a83b4e16556b72f52bd67e39f596be`  
		Last Modified: Fri, 01 Dec 2023 00:14:01 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e958dac8143e41701702904f092ab10b8682434d3d88e5af758dafaeb3317428`  
		Last Modified: Fri, 01 Dec 2023 00:14:01 GMT  
		Size: 108.0 KB (107998 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:61dfbf83553658c4ab4a5ae4477150c88a3f30da8309b9cfefdc185b3764e501`  
		Last Modified: Fri, 01 Dec 2023 00:14:01 GMT  
		Size: 959.1 KB (959085 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8b397213e2806c5c7c6aca6c20bc2f69362c9f6204c5d3947eaaf870176d9a36`  
		Last Modified: Fri, 01 Dec 2023 00:14:01 GMT  
		Size: 277.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8c404d1dff37be469e83d35363176296e0129304273844e38a69edbd6861f08c`  
		Last Modified: Fri, 01 Dec 2023 00:14:02 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6-alpine3.18` - unknown; unknown

```console
$ docker pull memcached@sha256:6a508d9bd488a6e6f8bbaae93d8ff14548111b267a7440f64edec96b04f8a3cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 KB (97008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fdbf48b2b61dd467eec02ffd7b0e996989023a93d9ecbc7a655a0755362c38a`

```dockerfile
```

-	Layers:
	-	`sha256:5c3e16fb5448bac47fadf2a80df72f13e831b463525dc9823da6c85f1770bf69`  
		Last Modified: Fri, 01 Dec 2023 00:14:01 GMT  
		Size: 78.1 KB (78055 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:1d5f7cf7dffd0d16953251b75fd8b7224aae91e57357d5af853c41398d72a5f7`  
		Last Modified: Fri, 01 Dec 2023 00:14:01 GMT  
		Size: 19.0 KB (18953 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:e9673caac3d318f89edf7ca6eaba8910416292f12f0f0abbf3d862a8b5af88ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4406434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a4e56736197b019e201b69449a358660e6806d076b61fd473dbcbb11caf5197`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["/bin/sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN apk add --no-cache libsasl # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4962e560ef629491acb51e64b06a5ee52545098f8403705778786a404e81434b`  
		Last Modified: Fri, 01 Dec 2023 15:25:24 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d4b10238ba82be69f174742e8ae9cd6e4484f32dce6eeb40dcbe3c5a4e0a1480`  
		Last Modified: Fri, 01 Dec 2023 15:25:24 GMT  
		Size: 124.1 KB (124087 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:276ae0cb4d4371459c3116e0453691ac59cdd9a6d649cb27bb3d3a090ef10fbf`  
		Last Modified: Fri, 01 Dec 2023 15:25:24 GMT  
		Size: 947.7 KB (947670 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:315ab34d41c816b04b8d07e4b7db199c17340b3b882b52819a0564f6be31a04c`  
		Last Modified: Fri, 01 Dec 2023 15:25:24 GMT  
		Size: 278.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:024d99cdc8f15c63cc478d1850db680f8c0dfae1ea2a5bca55e41fb0db12d020`  
		Last Modified: Fri, 01 Dec 2023 15:25:25 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6-alpine3.18` - unknown; unknown

```console
$ docker pull memcached@sha256:91dac18281e4a194ee9756cf2652c70b2fb0bd2ba9d26c5c86d44c762d111821
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.9 KB (96880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3590bb02748f6b9e8a22ef90e7b41976bcb90189d98a78beae80f5aab1cd1cf4`

```dockerfile
```

-	Layers:
	-	`sha256:605a9d206d49d790bef9ce82c45179355571f37a91c5730ca6f59a03e13c0c76`  
		Last Modified: Fri, 01 Dec 2023 15:25:24 GMT  
		Size: 78.1 KB (78074 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:95803ef4905954256ae922386b3196bdafabd328ecd648b88ed7d8c13ec3b640`  
		Last Modified: Fri, 01 Dec 2023 15:25:24 GMT  
		Size: 18.8 KB (18806 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6-alpine3.18` - linux; 386

```console
$ docker pull memcached@sha256:c281c55fd61946d53161839c584fb2bab1e6701155ad4b32c816d6ab0dc21a08
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4692614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c2fd98aa81c35c4a5fa9401b2f61ac48a2632d3b4b4baacc4b7982b10310097`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 28 Sep 2023 20:38:19 GMT
ADD file:8402753f294e403e92353bd65c86a6428c960be5116c0a15484b663a84f66fcd in / 
# Thu, 28 Sep 2023 20:38:20 GMT
CMD ["/bin/sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN apk add --no-cache libsasl # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:dc95107ad2a031a015320bb397f73ec151d738127175b31ad643120697dc7e90`  
		Last Modified: Thu, 28 Sep 2023 20:39:32 GMT  
		Size: 3.2 MB (3235757 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4951068162aca253cfa98ba4876636d5f13870e8ae9df08734f097bb6291e163`  
		Last Modified: Wed, 18 Oct 2023 01:04:05 GMT  
		Size: 1.2 KB (1246 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:50e4c32dd77b7a60c60be859a9848c50b3da8b95360dea46acf070797f48ab2a`  
		Last Modified: Wed, 18 Oct 2023 01:04:05 GMT  
		Size: 109.5 KB (109458 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:77aecf5d85dda7360aa3010357b83f206e1873aa4df6de5692c0c39dbf083c2a`  
		Last Modified: Wed, 18 Oct 2023 01:04:06 GMT  
		Size: 1.3 MB (1345750 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:99e49c7a1306cd1125b7dbc332a0b1b47b2408c77e975df11b090c0ab5599be3`  
		Last Modified: Wed, 18 Oct 2023 01:04:06 GMT  
		Size: 281.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:68c5ecf5461e2d137f2c403e26fe6e0532a5ecf0eedcd77a5b18254c82b9a075`  
		Last Modified: Wed, 18 Oct 2023 01:04:07 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6-alpine3.18` - unknown; unknown

```console
$ docker pull memcached@sha256:f0efd827c59fd288434c24a501d257456e82560b34d98f97cfe8b132454e28b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 KB (18687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea78294aafd9f308a52d310f899433de63e91eaac550b4ace8c1b8647774c7b8`

```dockerfile
```

-	Layers:
	-	`sha256:8c15fbe468a3b1236cadb64627426b8e2cb8bb71fddd26e10cdc44abd3b3519c`  
		Last Modified: Wed, 18 Oct 2023 01:04:05 GMT  
		Size: 18.7 KB (18687 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6-alpine3.18` - linux; ppc64le

```console
$ docker pull memcached@sha256:bae49b5a412b4535ebab987425356a20af16fc1ce70c38e18f6aa6572cac522d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4460245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b845ad70056a07d2adbebdc425879a4eb74152c886dae5d8e5496c6114cd3cda`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:3450a1687b552498a987f87cb844b7f597c7181d7c3d31943d7b3036d5300d5e in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["/bin/sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN apk add --no-cache libsasl # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:4e13780adf2776477b14ef9c0f4f563f820a2fde166d472218037b979e84d31a`  
		Last Modified: Thu, 30 Nov 2023 23:20:01 GMT  
		Size: 3.3 MB (3348322 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a33c280bf18f1bba1782f90d468941796634b74c44d9aae4c406162114520e9a`  
		Last Modified: Fri, 01 Dec 2023 12:01:06 GMT  
		Size: 1.2 KB (1247 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a54d91525051bf65bd807cac3c6f1a685ac2fc6ec7f763df97c18a3ca4b6dde0`  
		Last Modified: Fri, 01 Dec 2023 12:01:07 GMT  
		Size: 123.9 KB (123864 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:73f73a883ca0c1147533ae5085475dee29244e8ef06b0455c52afa6ab50c3023`  
		Last Modified: Fri, 01 Dec 2023 12:01:07 GMT  
		Size: 986.4 KB (986410 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:183bb794a2f98d5b2192b311c4b597c47ee4ee0bb405558f67827c8afaf0b8d3`  
		Last Modified: Fri, 01 Dec 2023 12:01:07 GMT  
		Size: 280.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:556988ad767ddefdfb131bbf239cceba01e60b197c0893287ee0f6274e54a0c8`  
		Last Modified: Fri, 01 Dec 2023 12:01:08 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6-alpine3.18` - unknown; unknown

```console
$ docker pull memcached@sha256:df95592ada35b125fd73982e23f99a4fc3820ab083e12870f4edb179935ec44d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.3 KB (95332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67d44fe1dc00fdfaba957619ac6567e2ba40c2bad9a422ffb5287bb160b01fe7`

```dockerfile
```

-	Layers:
	-	`sha256:4a7a9ea74e3391f7a0e156b244eb474f674d42637b77983cfd9c92b23701d5ce`  
		Last Modified: Fri, 01 Dec 2023 12:01:06 GMT  
		Size: 76.5 KB (76477 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:671ec9ab176a20a138f0a3e238976e619a6f3011f598148b2cadd4c167721f81`  
		Last Modified: Fri, 01 Dec 2023 12:01:07 GMT  
		Size: 18.9 KB (18855 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6-alpine3.18` - linux; s390x

```console
$ docker pull memcached@sha256:7af81a585082ce3ca180a3fac82a30bb37a43973123841b2dec30e5d096be8cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4285472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b785f0d9bb74e0e2b4f8772ce85a7b23cfc2e2f8dbb7ad428517b68cca17de38`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["/bin/sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN apk add --no-cache libsasl # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a7b34c58047c2f1ded65320321066565e57ddd2ed65156bde99267b8e575bf63`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:036bb49faad29b98ef9de81de4441efa5208c00e72ccea2b631c7b1c283f072d`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 112.8 KB (112781 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c1da6195feb453292bec9ae13a8968a7fbc7b611793ac2bc13df3614b514db3f`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 953.6 KB (953590 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a43896e685e7c2e1e51c75c1ed262d1c57940abdc2e68d74301201c9aa8ebdfe`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 281.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:928e080b9c3b24e2e655bd62e483670acb3c5508648e5a2784a6bebb4d252367`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6-alpine3.18` - unknown; unknown

```console
$ docker pull memcached@sha256:89eda6fd40656e7c2d5de572e4bdfbd821a333eb1067170caf9074dcbc141515
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.2 KB (95207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e34e69a75d4acd1221e6dd87a6f96bcf43e52e6ebaba333e1e4cc57d391f048`

```dockerfile
```

-	Layers:
	-	`sha256:c5dd02fe5ddfbc8ce715e0e666a98ae24e73371a2a8dee859d796538f4cf0618`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 76.4 KB (76419 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:13692e9f247d60b0cd5d0d4c0ccb23a86437ea348414e8548639ba89b5e4b65a`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 18.8 KB (18788 bytes)  
		MIME: application/vnd.in-toto+json

## `memcached:1.6-bookworm`

```console
$ docker pull memcached@sha256:9ed83da692bea50f7d0466186e0a2b527c047993805b98c99c1794bceb27d0e8
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 14
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v5
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

### `memcached:1.6-bookworm` - linux; amd64

```console
$ docker pull memcached@sha256:7b0480ab945f960f703af2f286b02a7b620eb4f772e25a2a1374e0c7d32f46de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.8 MB (38815745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f65c7b1a196aa7dfe9520f598f699d5846d6ff0eed117a36ca216302174a1bb1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:d261a6f6921593f1e0b3f472ab1b1822e2c6deb0b369200f0b3370556bfad017 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1f7ce2fa46ab3942feabee654933948821303a5a821789dddab2d8c3df59e227`  
		Last Modified: Tue, 21 Nov 2023 05:25:58 GMT  
		Size: 29.1 MB (29149908 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3606f7d6f784848f3e26f4bc5fae3dde08d65681dbaba232236ac8855cddb881`  
		Last Modified: Tue, 21 Nov 2023 06:19:50 GMT  
		Size: 1.1 KB (1110 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d9e66f47c0a00f0a833454718ca9dc6504f38c45944b5ebf43ccac532dc520b6`  
		Last Modified: Tue, 21 Nov 2023 06:19:50 GMT  
		Size: 2.5 MB (2488339 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:26e0a53c88ab99ad6e23fbb12147cce82e922e4141af56338b4ec01c2ead2b07`  
		Last Modified: Tue, 21 Nov 2023 06:19:50 GMT  
		Size: 7.2 MB (7175988 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:afc0db62c179dab7a3fc4ff6848e150c3315896846d827282affab08909d6e23`  
		Last Modified: Tue, 21 Nov 2023 06:19:50 GMT  
		Size: 281.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7af609a76aa9ed2d446da8865870d0e2b3bff46785783284d956d755a714899b`  
		Last Modified: Tue, 21 Nov 2023 06:19:50 GMT  
		Size: 119.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:cb387d9a91a709e6a4193c58df1f36753dbc6c13b9788d741d6dd92ee262ea52
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3078549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3b5853b03b272d3ad2682a093fbc3b2ffd577e3c9fe01f926b5963b333208cd`

```dockerfile
```

-	Layers:
	-	`sha256:9630a5bf61090e535bcf3b7ad1349332584446ea948e10119e025a65fad57d26`  
		Last Modified: Tue, 21 Nov 2023 06:19:50 GMT  
		Size: 3.1 MB (3056780 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:a2ef4829ccc1863c60fdfcf41590326d17bfbdef204a7d37664c92bec494942b`  
		Last Modified: Tue, 21 Nov 2023 06:19:50 GMT  
		Size: 21.8 KB (21769 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6-bookworm` - linux; arm variant v5

```console
$ docker pull memcached@sha256:c5fbea0a198cb4ae068e4761d5d1abab499e4ebc80275be6b7d797196cf3db54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34849973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b72ee44b42eca798309f6aa48ed2af9feca23c5eb64e5be38fa2536110b12ce`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:1ae8e5ac45b11d01083680b765e1fcfef9f7938f89d6f424572126fa946d8cdf in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f476aef5b6e1122850e68c81ef06fc2df17e968961b060483b4d2fb33018aae3`  
		Last Modified: Tue, 21 Nov 2023 05:03:55 GMT  
		Size: 26.9 MB (26922153 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:26dadbdb945a22546f6b2c171d0bededff72d7598719ab8f3877f67129e21730`  
		Last Modified: Tue, 21 Nov 2023 16:18:13 GMT  
		Size: 1.1 KB (1109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:44f46f0b8b7c11e6cd53e82541f819c66da246b152155fff8ce762f98c25219f`  
		Last Modified: Tue, 21 Nov 2023 16:18:14 GMT  
		Size: 2.1 MB (2089268 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:639e86d18160b654876d404a88b437cea26de29151122dfe8cbed9947f1b7b10`  
		Last Modified: Tue, 21 Nov 2023 16:18:14 GMT  
		Size: 5.8 MB (5837040 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7b963217677ca57533744aee2b331f059fbb6882f27abe2cc976462604e7b560`  
		Last Modified: Tue, 21 Nov 2023 16:18:15 GMT  
		Size: 283.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ac3a1fa5d4b6c48ea8ce4c375a197047f1480fbfb37c316b7d730d026d261219`  
		Last Modified: Tue, 21 Nov 2023 16:18:15 GMT  
		Size: 120.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:cd008d8c4d507d73b5f0153ed880e81e86a53741b480bbf6b1d318510e83a288
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.7 KB (21695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85e0f40569066724c087be3d901d5c5d984043271b56a33dec281e36032017f0`

```dockerfile
```

-	Layers:
	-	`sha256:2eff64dde44b4be85375aed8309f5d20476ca81876607d799b56c31addee0cb8`  
		Last Modified: Tue, 21 Nov 2023 16:18:13 GMT  
		Size: 21.7 KB (21695 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6-bookworm` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:dd556de8d6e6b81c51ba9120fa924fbb7fae427468d82db9f2b3db124f9ac0b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.7 MB (37711361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f05ec0c73b4afc866c99864d86b1c66deb5d8bda84bf2cc78e1e763e0ed6a263`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:869c7d0747a17c53715581a2e862992eb8516c7f45f167821dfa80966a4870d1 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2c6d21737d8318aa15c4cc838475029a5efc36c0429e3d8da80d97d0b96d9aaf`  
		Last Modified: Tue, 21 Nov 2023 06:30:30 GMT  
		Size: 29.2 MB (29179277 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fa3a18531b093eb1a543ad01b2a54d4692f59bba8d49ea9793b3ff09e528cd93`  
		Last Modified: Wed, 22 Nov 2023 11:50:41 GMT  
		Size: 1.1 KB (1109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:395fd5be77a2adb2c1b863f9ba2c664074aacb120f379bbb0f45cda74cc09cf4`  
		Last Modified: Wed, 22 Nov 2023 11:50:41 GMT  
		Size: 2.3 MB (2345987 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1dbcb5e891e054cd85f29e62fff856117d8cb919630be0c7473b520168b8c261`  
		Last Modified: Wed, 22 Nov 2023 11:50:41 GMT  
		Size: 6.2 MB (6184583 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2654df736cfb30e0097cca6a637ae794285396f6e2b87031636c8056b66baed0`  
		Last Modified: Wed, 22 Nov 2023 11:50:41 GMT  
		Size: 283.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e54ea6c3f7f45d9ed3f003bcf9e0a717c342daae58d330fef355e712d15b732`  
		Last Modified: Wed, 22 Nov 2023 11:50:42 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:2b5053d245e0312a77b7827553fcf09a6b19a0bf825a7016a4125713ad0d814f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3053591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e04bc647daea7fbb746cd418f19740162bd910826c366cdcc3549c3888ad5e1b`

```dockerfile
```

-	Layers:
	-	`sha256:f04377bb8fcfc3a24c1a36aa0bdf9b2d9272b7a60e82a88b66e2bb0645703c07`  
		Last Modified: Wed, 22 Nov 2023 11:50:41 GMT  
		Size: 3.0 MB (3031971 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:601cddda9e5f7f3a82cfc305051ac3c1fc5f65a9722e4dbe06363cc8b6ea68be`  
		Last Modified: Wed, 22 Nov 2023 11:50:41 GMT  
		Size: 21.6 KB (21620 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6-bookworm` - linux; 386

```console
$ docker pull memcached@sha256:fa9dba8086765d68f2feecfc2ac08fb29c019597d09943bb480227e6cba87666
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.3 MB (39294993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93047050e75b6d4d64adb8a7c8f68cb118bad27ca9dc772120e251b174752cf9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:0c94521fdd9c0a4fdeeb9aad23e68cd053fba0dcd7c3af550aefa79377816e31 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:98bdfce9af831c2a0d0bfcca812d0039cd1666986550f552b4b4c625bd5aa31c`  
		Last Modified: Wed, 01 Nov 2023 00:43:26 GMT  
		Size: 30.2 MB (30164042 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1b647d4b10cf20ac5807101c7d0380701be684aa82f5c01ec41f674b5ef23d42`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 1.1 KB (1109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b61c058003459de4911c2901b2d799b03de754a1b9e64ffbe21a04992e962e62`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 2.5 MB (2492501 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:810b6db64df2fcc8f76941cdac75093cf35bd72ac3cd1fa5eb664e74c1f67cd8`  
		Last Modified: Wed, 01 Nov 2023 01:06:50 GMT  
		Size: 6.6 MB (6636937 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dbb899942df4149bd5fae8bac6e295285ec80f82d621f2b29c931ee348491cfb`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 282.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4a8530160ab232c37c0ddcbf5e3a731d835d378d1382843957f6c2a73b2b5be6`  
		Last Modified: Wed, 01 Nov 2023 01:06:50 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:dd7ce9519c31365127142232df2ed0b285e9acc03cd77c23c838bf932165def8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 KB (21498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eef82c92e07c11a92c337806d01cfb1c6cdc7a16608dcf304a38de34d2ef1dbb`

```dockerfile
```

-	Layers:
	-	`sha256:c0d9dd22513f8d3e791e1796d7ef1906e57c798c92dd35d0be9cf2eaecec5954`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 21.5 KB (21498 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6-bookworm` - linux; mips64le

```console
$ docker pull memcached@sha256:a7c198db1b0856aff4b1514137e473ea30bce2ef22f0192cfdce7e2e44f2a863
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.6 MB (37588022 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1654ec4454e597d7e7cb6a7d97e98208de241a3dfafc5e0532b9561eac91f013`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:e093749192323dc72b60a8440ddba26c415586f618b5e107fa264ba5eb2ca7ba in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:ebdff2138fee4a3ec27560ab1353dc51c12c2608ff721f5db3d24104872b702a`  
		Last Modified: Tue, 21 Nov 2023 04:20:35 GMT  
		Size: 29.1 MB (29141984 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:50b1ffce24cec457fe1757715d60bd669145e5babade7c57143c4b665a55389e`  
		Last Modified: Thu, 23 Nov 2023 01:10:58 GMT  
		Size: 1.1 KB (1112 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:893c712c491a058aada36756e9f176b6c6c2f3a2b3adf0cd94b896c8198ec3ee`  
		Last Modified: Thu, 23 Nov 2023 01:10:59 GMT  
		Size: 1.9 MB (1937483 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0b8443254952572331df084976853329b69a4348b3c620bb073b5c89fb943b2b`  
		Last Modified: Thu, 23 Nov 2023 01:10:59 GMT  
		Size: 6.5 MB (6507036 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:904bfc5c5c0923edd9be421332402b224bfcd49053bc9b3fae6173383f5cd395`  
		Last Modified: Thu, 23 Nov 2023 01:10:59 GMT  
		Size: 285.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c265216ad3407dbc99903d96423b3a2314bc48cc0118911d150a6bb087ff7d85`  
		Last Modified: Thu, 23 Nov 2023 01:11:00 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:e2fcd32899d09ff06793849927220bea14475e64f085972afbc1f3af74dc209b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.7 KB (21656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf1c2028769aa20a3e529d0f85c8144ba6b099f74cda0dfca2272b7831d2d7a5`

```dockerfile
```

-	Layers:
	-	`sha256:75bab713cb94cdececf4c3879050737e7cb4bbb6206daa071ea001692b53d659`  
		Last Modified: Thu, 23 Nov 2023 01:10:58 GMT  
		Size: 21.7 KB (21656 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6-bookworm` - linux; ppc64le

```console
$ docker pull memcached@sha256:d8d106a88d6a15fadf738e59a6dcfc3942f11c7a2d19b7473abce66af7f4d19c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.0 MB (43030916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85da4ca798d44fc951b843ec85c410207ecc3c56af6d1bf7c321c91266d54e1b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:8b22a531b6611a1e63dfc20e4e2931592e2d821bd4b64c4b2810bb9a36640c02 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c570d04e61d8e35a3c8f12179d048d701451f97f9cf2099ea3e3738512dbf062`  
		Last Modified: Tue, 21 Nov 2023 04:28:58 GMT  
		Size: 33.1 MB (33141607 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bcd0cf90a66e23cd3d72b99e7d36129b0e846407a07c30031b0c1e4ba115cd30`  
		Last Modified: Tue, 21 Nov 2023 23:46:47 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5e4166a0e033df4117b469f840c6f5527e87dbd13c582c0b50c182b4bb3ead79`  
		Last Modified: Tue, 21 Nov 2023 23:46:47 GMT  
		Size: 2.7 MB (2698215 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:947b7328e0db59b9870fe9c6d6b7fc4e8a8f1fef3d2a36064fe3d60f5314652d`  
		Last Modified: Tue, 21 Nov 2023 23:46:48 GMT  
		Size: 7.2 MB (7189577 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f011f72796530a711f1de9d543435299d02ed3636e4cd28aee1fa493fbc2bf4`  
		Last Modified: Tue, 21 Nov 2023 23:46:47 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9d27046f19e474530b87e1d0b429e9d85f403210dd3d91bf60d8303fef03af96`  
		Last Modified: Tue, 21 Nov 2023 23:46:48 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:4269af6aa39a29d6dca352659fbf04b7d1bb4e65151e63a3ffcf2749d853597e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3067036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6e9626f30d490d2014e9fbb19add0b6ac0f63c8f4af2082d04750fea7ec35ff`

```dockerfile
```

-	Layers:
	-	`sha256:70759e1722d82b89de5c0d71ba2050ecc9f29d95ee758369044a1fc79026a546`  
		Last Modified: Tue, 21 Nov 2023 23:46:47 GMT  
		Size: 3.0 MB (3045366 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:4f34d59241ff06b2bd0cb8239d96be938e1e13470264898863f307f84ab275b6`  
		Last Modified: Tue, 21 Nov 2023 23:46:47 GMT  
		Size: 21.7 KB (21670 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6-bookworm` - linux; s390x

```console
$ docker pull memcached@sha256:312625a69b30a0a0371060c62ec97a621d587675e55a8ced694303d8a7015d30
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.7 MB (35745726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13ebe1c7df28f24c49c7dc749c55574a0a51a84e31dcff380e6caa5441fca944`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:c33fa9fdde73983850798b6eb1cd062e0398109d1d773e6a937fead7475c8efc in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6daa625e5a040476e253e7acd0befa74254a4865ec836d6334a544d82a21d4be`  
		Last Modified: Tue, 21 Nov 2023 05:10:21 GMT  
		Size: 27.5 MB (27512885 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:410539cfd307a2626bf5520b21d1cff0d4c8a336ebea36ed08878d81eca92847`  
		Last Modified: Tue, 21 Nov 2023 15:56:02 GMT  
		Size: 1.1 KB (1109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1ba4cc4f8ba1aa1865931fde910e1ebac220aea9a207eff2f2556bc289a513d3`  
		Last Modified: Tue, 21 Nov 2023 15:56:03 GMT  
		Size: 2.2 MB (2152517 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a47325d5bddeb006ca8a01a6239f747f4ed2c21fd6a28226bdfe46d1981d8962`  
		Last Modified: Tue, 21 Nov 2023 15:56:03 GMT  
		Size: 6.1 MB (6078811 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:32f889bfd6f6b6b2d773abb9f72f86fe0c7469d2a271e5bd209a3eb9b1c61dea`  
		Last Modified: Tue, 21 Nov 2023 15:56:04 GMT  
		Size: 283.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:56ce84d34f650bc21b164be1bb375a2b43c761943b4d06497991ceca18be1009`  
		Last Modified: Tue, 21 Nov 2023 15:56:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:b070f08010996b181adf3fbb4b9004e0d125115bf1380df8c4ddb96a99827218
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3068089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:307228ea8d7a2ce5fee0e1c4c36745e1c0244aa6d316102bde5b655af1bedd24`

```dockerfile
```

-	Layers:
	-	`sha256:640994e8299bce5ed690d70d55a1bc2035868614a169e4cda3391dafb76e9469`  
		Last Modified: Tue, 21 Nov 2023 15:56:03 GMT  
		Size: 3.0 MB (3046321 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:1893b50125646067935dd81f10c259d7b0c3b7cf2f42c81abe2b0f93e45f4250`  
		Last Modified: Tue, 21 Nov 2023 15:56:03 GMT  
		Size: 21.8 KB (21768 bytes)  
		MIME: application/vnd.in-toto+json

## `memcached:1.6.22`

```console
$ docker pull memcached@sha256:9ed83da692bea50f7d0466186e0a2b527c047993805b98c99c1794bceb27d0e8
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 14
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v5
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

### `memcached:1.6.22` - linux; amd64

```console
$ docker pull memcached@sha256:7b0480ab945f960f703af2f286b02a7b620eb4f772e25a2a1374e0c7d32f46de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.8 MB (38815745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f65c7b1a196aa7dfe9520f598f699d5846d6ff0eed117a36ca216302174a1bb1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:d261a6f6921593f1e0b3f472ab1b1822e2c6deb0b369200f0b3370556bfad017 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1f7ce2fa46ab3942feabee654933948821303a5a821789dddab2d8c3df59e227`  
		Last Modified: Tue, 21 Nov 2023 05:25:58 GMT  
		Size: 29.1 MB (29149908 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3606f7d6f784848f3e26f4bc5fae3dde08d65681dbaba232236ac8855cddb881`  
		Last Modified: Tue, 21 Nov 2023 06:19:50 GMT  
		Size: 1.1 KB (1110 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d9e66f47c0a00f0a833454718ca9dc6504f38c45944b5ebf43ccac532dc520b6`  
		Last Modified: Tue, 21 Nov 2023 06:19:50 GMT  
		Size: 2.5 MB (2488339 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:26e0a53c88ab99ad6e23fbb12147cce82e922e4141af56338b4ec01c2ead2b07`  
		Last Modified: Tue, 21 Nov 2023 06:19:50 GMT  
		Size: 7.2 MB (7175988 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:afc0db62c179dab7a3fc4ff6848e150c3315896846d827282affab08909d6e23`  
		Last Modified: Tue, 21 Nov 2023 06:19:50 GMT  
		Size: 281.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7af609a76aa9ed2d446da8865870d0e2b3bff46785783284d956d755a714899b`  
		Last Modified: Tue, 21 Nov 2023 06:19:50 GMT  
		Size: 119.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.22` - unknown; unknown

```console
$ docker pull memcached@sha256:cb387d9a91a709e6a4193c58df1f36753dbc6c13b9788d741d6dd92ee262ea52
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3078549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3b5853b03b272d3ad2682a093fbc3b2ffd577e3c9fe01f926b5963b333208cd`

```dockerfile
```

-	Layers:
	-	`sha256:9630a5bf61090e535bcf3b7ad1349332584446ea948e10119e025a65fad57d26`  
		Last Modified: Tue, 21 Nov 2023 06:19:50 GMT  
		Size: 3.1 MB (3056780 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:a2ef4829ccc1863c60fdfcf41590326d17bfbdef204a7d37664c92bec494942b`  
		Last Modified: Tue, 21 Nov 2023 06:19:50 GMT  
		Size: 21.8 KB (21769 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6.22` - linux; arm variant v5

```console
$ docker pull memcached@sha256:c5fbea0a198cb4ae068e4761d5d1abab499e4ebc80275be6b7d797196cf3db54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34849973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b72ee44b42eca798309f6aa48ed2af9feca23c5eb64e5be38fa2536110b12ce`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:1ae8e5ac45b11d01083680b765e1fcfef9f7938f89d6f424572126fa946d8cdf in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f476aef5b6e1122850e68c81ef06fc2df17e968961b060483b4d2fb33018aae3`  
		Last Modified: Tue, 21 Nov 2023 05:03:55 GMT  
		Size: 26.9 MB (26922153 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:26dadbdb945a22546f6b2c171d0bededff72d7598719ab8f3877f67129e21730`  
		Last Modified: Tue, 21 Nov 2023 16:18:13 GMT  
		Size: 1.1 KB (1109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:44f46f0b8b7c11e6cd53e82541f819c66da246b152155fff8ce762f98c25219f`  
		Last Modified: Tue, 21 Nov 2023 16:18:14 GMT  
		Size: 2.1 MB (2089268 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:639e86d18160b654876d404a88b437cea26de29151122dfe8cbed9947f1b7b10`  
		Last Modified: Tue, 21 Nov 2023 16:18:14 GMT  
		Size: 5.8 MB (5837040 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7b963217677ca57533744aee2b331f059fbb6882f27abe2cc976462604e7b560`  
		Last Modified: Tue, 21 Nov 2023 16:18:15 GMT  
		Size: 283.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ac3a1fa5d4b6c48ea8ce4c375a197047f1480fbfb37c316b7d730d026d261219`  
		Last Modified: Tue, 21 Nov 2023 16:18:15 GMT  
		Size: 120.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.22` - unknown; unknown

```console
$ docker pull memcached@sha256:cd008d8c4d507d73b5f0153ed880e81e86a53741b480bbf6b1d318510e83a288
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.7 KB (21695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85e0f40569066724c087be3d901d5c5d984043271b56a33dec281e36032017f0`

```dockerfile
```

-	Layers:
	-	`sha256:2eff64dde44b4be85375aed8309f5d20476ca81876607d799b56c31addee0cb8`  
		Last Modified: Tue, 21 Nov 2023 16:18:13 GMT  
		Size: 21.7 KB (21695 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6.22` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:dd556de8d6e6b81c51ba9120fa924fbb7fae427468d82db9f2b3db124f9ac0b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.7 MB (37711361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f05ec0c73b4afc866c99864d86b1c66deb5d8bda84bf2cc78e1e763e0ed6a263`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:869c7d0747a17c53715581a2e862992eb8516c7f45f167821dfa80966a4870d1 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2c6d21737d8318aa15c4cc838475029a5efc36c0429e3d8da80d97d0b96d9aaf`  
		Last Modified: Tue, 21 Nov 2023 06:30:30 GMT  
		Size: 29.2 MB (29179277 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fa3a18531b093eb1a543ad01b2a54d4692f59bba8d49ea9793b3ff09e528cd93`  
		Last Modified: Wed, 22 Nov 2023 11:50:41 GMT  
		Size: 1.1 KB (1109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:395fd5be77a2adb2c1b863f9ba2c664074aacb120f379bbb0f45cda74cc09cf4`  
		Last Modified: Wed, 22 Nov 2023 11:50:41 GMT  
		Size: 2.3 MB (2345987 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1dbcb5e891e054cd85f29e62fff856117d8cb919630be0c7473b520168b8c261`  
		Last Modified: Wed, 22 Nov 2023 11:50:41 GMT  
		Size: 6.2 MB (6184583 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2654df736cfb30e0097cca6a637ae794285396f6e2b87031636c8056b66baed0`  
		Last Modified: Wed, 22 Nov 2023 11:50:41 GMT  
		Size: 283.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e54ea6c3f7f45d9ed3f003bcf9e0a717c342daae58d330fef355e712d15b732`  
		Last Modified: Wed, 22 Nov 2023 11:50:42 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.22` - unknown; unknown

```console
$ docker pull memcached@sha256:2b5053d245e0312a77b7827553fcf09a6b19a0bf825a7016a4125713ad0d814f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3053591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e04bc647daea7fbb746cd418f19740162bd910826c366cdcc3549c3888ad5e1b`

```dockerfile
```

-	Layers:
	-	`sha256:f04377bb8fcfc3a24c1a36aa0bdf9b2d9272b7a60e82a88b66e2bb0645703c07`  
		Last Modified: Wed, 22 Nov 2023 11:50:41 GMT  
		Size: 3.0 MB (3031971 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:601cddda9e5f7f3a82cfc305051ac3c1fc5f65a9722e4dbe06363cc8b6ea68be`  
		Last Modified: Wed, 22 Nov 2023 11:50:41 GMT  
		Size: 21.6 KB (21620 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6.22` - linux; 386

```console
$ docker pull memcached@sha256:fa9dba8086765d68f2feecfc2ac08fb29c019597d09943bb480227e6cba87666
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.3 MB (39294993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93047050e75b6d4d64adb8a7c8f68cb118bad27ca9dc772120e251b174752cf9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:0c94521fdd9c0a4fdeeb9aad23e68cd053fba0dcd7c3af550aefa79377816e31 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:98bdfce9af831c2a0d0bfcca812d0039cd1666986550f552b4b4c625bd5aa31c`  
		Last Modified: Wed, 01 Nov 2023 00:43:26 GMT  
		Size: 30.2 MB (30164042 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1b647d4b10cf20ac5807101c7d0380701be684aa82f5c01ec41f674b5ef23d42`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 1.1 KB (1109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b61c058003459de4911c2901b2d799b03de754a1b9e64ffbe21a04992e962e62`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 2.5 MB (2492501 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:810b6db64df2fcc8f76941cdac75093cf35bd72ac3cd1fa5eb664e74c1f67cd8`  
		Last Modified: Wed, 01 Nov 2023 01:06:50 GMT  
		Size: 6.6 MB (6636937 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dbb899942df4149bd5fae8bac6e295285ec80f82d621f2b29c931ee348491cfb`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 282.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4a8530160ab232c37c0ddcbf5e3a731d835d378d1382843957f6c2a73b2b5be6`  
		Last Modified: Wed, 01 Nov 2023 01:06:50 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.22` - unknown; unknown

```console
$ docker pull memcached@sha256:dd7ce9519c31365127142232df2ed0b285e9acc03cd77c23c838bf932165def8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 KB (21498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eef82c92e07c11a92c337806d01cfb1c6cdc7a16608dcf304a38de34d2ef1dbb`

```dockerfile
```

-	Layers:
	-	`sha256:c0d9dd22513f8d3e791e1796d7ef1906e57c798c92dd35d0be9cf2eaecec5954`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 21.5 KB (21498 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6.22` - linux; mips64le

```console
$ docker pull memcached@sha256:a7c198db1b0856aff4b1514137e473ea30bce2ef22f0192cfdce7e2e44f2a863
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.6 MB (37588022 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1654ec4454e597d7e7cb6a7d97e98208de241a3dfafc5e0532b9561eac91f013`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:e093749192323dc72b60a8440ddba26c415586f618b5e107fa264ba5eb2ca7ba in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:ebdff2138fee4a3ec27560ab1353dc51c12c2608ff721f5db3d24104872b702a`  
		Last Modified: Tue, 21 Nov 2023 04:20:35 GMT  
		Size: 29.1 MB (29141984 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:50b1ffce24cec457fe1757715d60bd669145e5babade7c57143c4b665a55389e`  
		Last Modified: Thu, 23 Nov 2023 01:10:58 GMT  
		Size: 1.1 KB (1112 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:893c712c491a058aada36756e9f176b6c6c2f3a2b3adf0cd94b896c8198ec3ee`  
		Last Modified: Thu, 23 Nov 2023 01:10:59 GMT  
		Size: 1.9 MB (1937483 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0b8443254952572331df084976853329b69a4348b3c620bb073b5c89fb943b2b`  
		Last Modified: Thu, 23 Nov 2023 01:10:59 GMT  
		Size: 6.5 MB (6507036 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:904bfc5c5c0923edd9be421332402b224bfcd49053bc9b3fae6173383f5cd395`  
		Last Modified: Thu, 23 Nov 2023 01:10:59 GMT  
		Size: 285.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c265216ad3407dbc99903d96423b3a2314bc48cc0118911d150a6bb087ff7d85`  
		Last Modified: Thu, 23 Nov 2023 01:11:00 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.22` - unknown; unknown

```console
$ docker pull memcached@sha256:e2fcd32899d09ff06793849927220bea14475e64f085972afbc1f3af74dc209b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.7 KB (21656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf1c2028769aa20a3e529d0f85c8144ba6b099f74cda0dfca2272b7831d2d7a5`

```dockerfile
```

-	Layers:
	-	`sha256:75bab713cb94cdececf4c3879050737e7cb4bbb6206daa071ea001692b53d659`  
		Last Modified: Thu, 23 Nov 2023 01:10:58 GMT  
		Size: 21.7 KB (21656 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6.22` - linux; ppc64le

```console
$ docker pull memcached@sha256:d8d106a88d6a15fadf738e59a6dcfc3942f11c7a2d19b7473abce66af7f4d19c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.0 MB (43030916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85da4ca798d44fc951b843ec85c410207ecc3c56af6d1bf7c321c91266d54e1b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:8b22a531b6611a1e63dfc20e4e2931592e2d821bd4b64c4b2810bb9a36640c02 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c570d04e61d8e35a3c8f12179d048d701451f97f9cf2099ea3e3738512dbf062`  
		Last Modified: Tue, 21 Nov 2023 04:28:58 GMT  
		Size: 33.1 MB (33141607 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bcd0cf90a66e23cd3d72b99e7d36129b0e846407a07c30031b0c1e4ba115cd30`  
		Last Modified: Tue, 21 Nov 2023 23:46:47 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5e4166a0e033df4117b469f840c6f5527e87dbd13c582c0b50c182b4bb3ead79`  
		Last Modified: Tue, 21 Nov 2023 23:46:47 GMT  
		Size: 2.7 MB (2698215 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:947b7328e0db59b9870fe9c6d6b7fc4e8a8f1fef3d2a36064fe3d60f5314652d`  
		Last Modified: Tue, 21 Nov 2023 23:46:48 GMT  
		Size: 7.2 MB (7189577 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f011f72796530a711f1de9d543435299d02ed3636e4cd28aee1fa493fbc2bf4`  
		Last Modified: Tue, 21 Nov 2023 23:46:47 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9d27046f19e474530b87e1d0b429e9d85f403210dd3d91bf60d8303fef03af96`  
		Last Modified: Tue, 21 Nov 2023 23:46:48 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.22` - unknown; unknown

```console
$ docker pull memcached@sha256:4269af6aa39a29d6dca352659fbf04b7d1bb4e65151e63a3ffcf2749d853597e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3067036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6e9626f30d490d2014e9fbb19add0b6ac0f63c8f4af2082d04750fea7ec35ff`

```dockerfile
```

-	Layers:
	-	`sha256:70759e1722d82b89de5c0d71ba2050ecc9f29d95ee758369044a1fc79026a546`  
		Last Modified: Tue, 21 Nov 2023 23:46:47 GMT  
		Size: 3.0 MB (3045366 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:4f34d59241ff06b2bd0cb8239d96be938e1e13470264898863f307f84ab275b6`  
		Last Modified: Tue, 21 Nov 2023 23:46:47 GMT  
		Size: 21.7 KB (21670 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6.22` - linux; s390x

```console
$ docker pull memcached@sha256:312625a69b30a0a0371060c62ec97a621d587675e55a8ced694303d8a7015d30
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.7 MB (35745726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13ebe1c7df28f24c49c7dc749c55574a0a51a84e31dcff380e6caa5441fca944`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:c33fa9fdde73983850798b6eb1cd062e0398109d1d773e6a937fead7475c8efc in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6daa625e5a040476e253e7acd0befa74254a4865ec836d6334a544d82a21d4be`  
		Last Modified: Tue, 21 Nov 2023 05:10:21 GMT  
		Size: 27.5 MB (27512885 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:410539cfd307a2626bf5520b21d1cff0d4c8a336ebea36ed08878d81eca92847`  
		Last Modified: Tue, 21 Nov 2023 15:56:02 GMT  
		Size: 1.1 KB (1109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1ba4cc4f8ba1aa1865931fde910e1ebac220aea9a207eff2f2556bc289a513d3`  
		Last Modified: Tue, 21 Nov 2023 15:56:03 GMT  
		Size: 2.2 MB (2152517 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a47325d5bddeb006ca8a01a6239f747f4ed2c21fd6a28226bdfe46d1981d8962`  
		Last Modified: Tue, 21 Nov 2023 15:56:03 GMT  
		Size: 6.1 MB (6078811 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:32f889bfd6f6b6b2d773abb9f72f86fe0c7469d2a271e5bd209a3eb9b1c61dea`  
		Last Modified: Tue, 21 Nov 2023 15:56:04 GMT  
		Size: 283.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:56ce84d34f650bc21b164be1bb375a2b43c761943b4d06497991ceca18be1009`  
		Last Modified: Tue, 21 Nov 2023 15:56:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.22` - unknown; unknown

```console
$ docker pull memcached@sha256:b070f08010996b181adf3fbb4b9004e0d125115bf1380df8c4ddb96a99827218
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3068089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:307228ea8d7a2ce5fee0e1c4c36745e1c0244aa6d316102bde5b655af1bedd24`

```dockerfile
```

-	Layers:
	-	`sha256:640994e8299bce5ed690d70d55a1bc2035868614a169e4cda3391dafb76e9469`  
		Last Modified: Tue, 21 Nov 2023 15:56:03 GMT  
		Size: 3.0 MB (3046321 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:1893b50125646067935dd81f10c259d7b0c3b7cf2f42c81abe2b0f93e45f4250`  
		Last Modified: Tue, 21 Nov 2023 15:56:03 GMT  
		Size: 21.8 KB (21768 bytes)  
		MIME: application/vnd.in-toto+json

## `memcached:1.6.22-alpine`

```console
$ docker pull memcached@sha256:93a9ff5ab97a213a027913f59bf902a118fa9750f88dbd4d513ebd920428820e
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 10
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `memcached:1.6.22-alpine` - linux; amd64

```console
$ docker pull memcached@sha256:f85dfa7d8ec9dc1b785c37ccf6dfa62bca5fec355c32ddf7957116376863284a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4471146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f687f33554b696db4e2422b52d11bd36b20649d152ca63d20848c83b0679237f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["/bin/sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN apk add --no-cache libsasl # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ce5e53c5eb3023b585266ac7ee39c0b268a83b4e16556b72f52bd67e39f596be`  
		Last Modified: Fri, 01 Dec 2023 00:14:01 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e958dac8143e41701702904f092ab10b8682434d3d88e5af758dafaeb3317428`  
		Last Modified: Fri, 01 Dec 2023 00:14:01 GMT  
		Size: 108.0 KB (107998 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:61dfbf83553658c4ab4a5ae4477150c88a3f30da8309b9cfefdc185b3764e501`  
		Last Modified: Fri, 01 Dec 2023 00:14:01 GMT  
		Size: 959.1 KB (959085 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8b397213e2806c5c7c6aca6c20bc2f69362c9f6204c5d3947eaaf870176d9a36`  
		Last Modified: Fri, 01 Dec 2023 00:14:01 GMT  
		Size: 277.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8c404d1dff37be469e83d35363176296e0129304273844e38a69edbd6861f08c`  
		Last Modified: Fri, 01 Dec 2023 00:14:02 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.22-alpine` - unknown; unknown

```console
$ docker pull memcached@sha256:6a508d9bd488a6e6f8bbaae93d8ff14548111b267a7440f64edec96b04f8a3cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 KB (97008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fdbf48b2b61dd467eec02ffd7b0e996989023a93d9ecbc7a655a0755362c38a`

```dockerfile
```

-	Layers:
	-	`sha256:5c3e16fb5448bac47fadf2a80df72f13e831b463525dc9823da6c85f1770bf69`  
		Last Modified: Fri, 01 Dec 2023 00:14:01 GMT  
		Size: 78.1 KB (78055 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:1d5f7cf7dffd0d16953251b75fd8b7224aae91e57357d5af853c41398d72a5f7`  
		Last Modified: Fri, 01 Dec 2023 00:14:01 GMT  
		Size: 19.0 KB (18953 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6.22-alpine` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:e9673caac3d318f89edf7ca6eaba8910416292f12f0f0abbf3d862a8b5af88ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4406434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a4e56736197b019e201b69449a358660e6806d076b61fd473dbcbb11caf5197`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["/bin/sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN apk add --no-cache libsasl # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4962e560ef629491acb51e64b06a5ee52545098f8403705778786a404e81434b`  
		Last Modified: Fri, 01 Dec 2023 15:25:24 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d4b10238ba82be69f174742e8ae9cd6e4484f32dce6eeb40dcbe3c5a4e0a1480`  
		Last Modified: Fri, 01 Dec 2023 15:25:24 GMT  
		Size: 124.1 KB (124087 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:276ae0cb4d4371459c3116e0453691ac59cdd9a6d649cb27bb3d3a090ef10fbf`  
		Last Modified: Fri, 01 Dec 2023 15:25:24 GMT  
		Size: 947.7 KB (947670 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:315ab34d41c816b04b8d07e4b7db199c17340b3b882b52819a0564f6be31a04c`  
		Last Modified: Fri, 01 Dec 2023 15:25:24 GMT  
		Size: 278.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:024d99cdc8f15c63cc478d1850db680f8c0dfae1ea2a5bca55e41fb0db12d020`  
		Last Modified: Fri, 01 Dec 2023 15:25:25 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.22-alpine` - unknown; unknown

```console
$ docker pull memcached@sha256:91dac18281e4a194ee9756cf2652c70b2fb0bd2ba9d26c5c86d44c762d111821
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.9 KB (96880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3590bb02748f6b9e8a22ef90e7b41976bcb90189d98a78beae80f5aab1cd1cf4`

```dockerfile
```

-	Layers:
	-	`sha256:605a9d206d49d790bef9ce82c45179355571f37a91c5730ca6f59a03e13c0c76`  
		Last Modified: Fri, 01 Dec 2023 15:25:24 GMT  
		Size: 78.1 KB (78074 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:95803ef4905954256ae922386b3196bdafabd328ecd648b88ed7d8c13ec3b640`  
		Last Modified: Fri, 01 Dec 2023 15:25:24 GMT  
		Size: 18.8 KB (18806 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6.22-alpine` - linux; 386

```console
$ docker pull memcached@sha256:c281c55fd61946d53161839c584fb2bab1e6701155ad4b32c816d6ab0dc21a08
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4692614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c2fd98aa81c35c4a5fa9401b2f61ac48a2632d3b4b4baacc4b7982b10310097`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 28 Sep 2023 20:38:19 GMT
ADD file:8402753f294e403e92353bd65c86a6428c960be5116c0a15484b663a84f66fcd in / 
# Thu, 28 Sep 2023 20:38:20 GMT
CMD ["/bin/sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN apk add --no-cache libsasl # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:dc95107ad2a031a015320bb397f73ec151d738127175b31ad643120697dc7e90`  
		Last Modified: Thu, 28 Sep 2023 20:39:32 GMT  
		Size: 3.2 MB (3235757 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4951068162aca253cfa98ba4876636d5f13870e8ae9df08734f097bb6291e163`  
		Last Modified: Wed, 18 Oct 2023 01:04:05 GMT  
		Size: 1.2 KB (1246 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:50e4c32dd77b7a60c60be859a9848c50b3da8b95360dea46acf070797f48ab2a`  
		Last Modified: Wed, 18 Oct 2023 01:04:05 GMT  
		Size: 109.5 KB (109458 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:77aecf5d85dda7360aa3010357b83f206e1873aa4df6de5692c0c39dbf083c2a`  
		Last Modified: Wed, 18 Oct 2023 01:04:06 GMT  
		Size: 1.3 MB (1345750 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:99e49c7a1306cd1125b7dbc332a0b1b47b2408c77e975df11b090c0ab5599be3`  
		Last Modified: Wed, 18 Oct 2023 01:04:06 GMT  
		Size: 281.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:68c5ecf5461e2d137f2c403e26fe6e0532a5ecf0eedcd77a5b18254c82b9a075`  
		Last Modified: Wed, 18 Oct 2023 01:04:07 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.22-alpine` - unknown; unknown

```console
$ docker pull memcached@sha256:f0efd827c59fd288434c24a501d257456e82560b34d98f97cfe8b132454e28b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 KB (18687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea78294aafd9f308a52d310f899433de63e91eaac550b4ace8c1b8647774c7b8`

```dockerfile
```

-	Layers:
	-	`sha256:8c15fbe468a3b1236cadb64627426b8e2cb8bb71fddd26e10cdc44abd3b3519c`  
		Last Modified: Wed, 18 Oct 2023 01:04:05 GMT  
		Size: 18.7 KB (18687 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6.22-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:bae49b5a412b4535ebab987425356a20af16fc1ce70c38e18f6aa6572cac522d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4460245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b845ad70056a07d2adbebdc425879a4eb74152c886dae5d8e5496c6114cd3cda`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:3450a1687b552498a987f87cb844b7f597c7181d7c3d31943d7b3036d5300d5e in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["/bin/sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN apk add --no-cache libsasl # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:4e13780adf2776477b14ef9c0f4f563f820a2fde166d472218037b979e84d31a`  
		Last Modified: Thu, 30 Nov 2023 23:20:01 GMT  
		Size: 3.3 MB (3348322 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a33c280bf18f1bba1782f90d468941796634b74c44d9aae4c406162114520e9a`  
		Last Modified: Fri, 01 Dec 2023 12:01:06 GMT  
		Size: 1.2 KB (1247 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a54d91525051bf65bd807cac3c6f1a685ac2fc6ec7f763df97c18a3ca4b6dde0`  
		Last Modified: Fri, 01 Dec 2023 12:01:07 GMT  
		Size: 123.9 KB (123864 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:73f73a883ca0c1147533ae5085475dee29244e8ef06b0455c52afa6ab50c3023`  
		Last Modified: Fri, 01 Dec 2023 12:01:07 GMT  
		Size: 986.4 KB (986410 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:183bb794a2f98d5b2192b311c4b597c47ee4ee0bb405558f67827c8afaf0b8d3`  
		Last Modified: Fri, 01 Dec 2023 12:01:07 GMT  
		Size: 280.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:556988ad767ddefdfb131bbf239cceba01e60b197c0893287ee0f6274e54a0c8`  
		Last Modified: Fri, 01 Dec 2023 12:01:08 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.22-alpine` - unknown; unknown

```console
$ docker pull memcached@sha256:df95592ada35b125fd73982e23f99a4fc3820ab083e12870f4edb179935ec44d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.3 KB (95332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67d44fe1dc00fdfaba957619ac6567e2ba40c2bad9a422ffb5287bb160b01fe7`

```dockerfile
```

-	Layers:
	-	`sha256:4a7a9ea74e3391f7a0e156b244eb474f674d42637b77983cfd9c92b23701d5ce`  
		Last Modified: Fri, 01 Dec 2023 12:01:06 GMT  
		Size: 76.5 KB (76477 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:671ec9ab176a20a138f0a3e238976e619a6f3011f598148b2cadd4c167721f81`  
		Last Modified: Fri, 01 Dec 2023 12:01:07 GMT  
		Size: 18.9 KB (18855 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6.22-alpine` - linux; s390x

```console
$ docker pull memcached@sha256:7af81a585082ce3ca180a3fac82a30bb37a43973123841b2dec30e5d096be8cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4285472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b785f0d9bb74e0e2b4f8772ce85a7b23cfc2e2f8dbb7ad428517b68cca17de38`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["/bin/sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN apk add --no-cache libsasl # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a7b34c58047c2f1ded65320321066565e57ddd2ed65156bde99267b8e575bf63`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:036bb49faad29b98ef9de81de4441efa5208c00e72ccea2b631c7b1c283f072d`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 112.8 KB (112781 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c1da6195feb453292bec9ae13a8968a7fbc7b611793ac2bc13df3614b514db3f`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 953.6 KB (953590 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a43896e685e7c2e1e51c75c1ed262d1c57940abdc2e68d74301201c9aa8ebdfe`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 281.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:928e080b9c3b24e2e655bd62e483670acb3c5508648e5a2784a6bebb4d252367`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.22-alpine` - unknown; unknown

```console
$ docker pull memcached@sha256:89eda6fd40656e7c2d5de572e4bdfbd821a333eb1067170caf9074dcbc141515
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.2 KB (95207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e34e69a75d4acd1221e6dd87a6f96bcf43e52e6ebaba333e1e4cc57d391f048`

```dockerfile
```

-	Layers:
	-	`sha256:c5dd02fe5ddfbc8ce715e0e666a98ae24e73371a2a8dee859d796538f4cf0618`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 76.4 KB (76419 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:13692e9f247d60b0cd5d0d4c0ccb23a86437ea348414e8548639ba89b5e4b65a`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 18.8 KB (18788 bytes)  
		MIME: application/vnd.in-toto+json

## `memcached:1.6.22-alpine3.18`

```console
$ docker pull memcached@sha256:93a9ff5ab97a213a027913f59bf902a118fa9750f88dbd4d513ebd920428820e
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 10
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `memcached:1.6.22-alpine3.18` - linux; amd64

```console
$ docker pull memcached@sha256:f85dfa7d8ec9dc1b785c37ccf6dfa62bca5fec355c32ddf7957116376863284a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4471146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f687f33554b696db4e2422b52d11bd36b20649d152ca63d20848c83b0679237f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["/bin/sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN apk add --no-cache libsasl # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ce5e53c5eb3023b585266ac7ee39c0b268a83b4e16556b72f52bd67e39f596be`  
		Last Modified: Fri, 01 Dec 2023 00:14:01 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e958dac8143e41701702904f092ab10b8682434d3d88e5af758dafaeb3317428`  
		Last Modified: Fri, 01 Dec 2023 00:14:01 GMT  
		Size: 108.0 KB (107998 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:61dfbf83553658c4ab4a5ae4477150c88a3f30da8309b9cfefdc185b3764e501`  
		Last Modified: Fri, 01 Dec 2023 00:14:01 GMT  
		Size: 959.1 KB (959085 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8b397213e2806c5c7c6aca6c20bc2f69362c9f6204c5d3947eaaf870176d9a36`  
		Last Modified: Fri, 01 Dec 2023 00:14:01 GMT  
		Size: 277.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8c404d1dff37be469e83d35363176296e0129304273844e38a69edbd6861f08c`  
		Last Modified: Fri, 01 Dec 2023 00:14:02 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.22-alpine3.18` - unknown; unknown

```console
$ docker pull memcached@sha256:6a508d9bd488a6e6f8bbaae93d8ff14548111b267a7440f64edec96b04f8a3cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 KB (97008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fdbf48b2b61dd467eec02ffd7b0e996989023a93d9ecbc7a655a0755362c38a`

```dockerfile
```

-	Layers:
	-	`sha256:5c3e16fb5448bac47fadf2a80df72f13e831b463525dc9823da6c85f1770bf69`  
		Last Modified: Fri, 01 Dec 2023 00:14:01 GMT  
		Size: 78.1 KB (78055 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:1d5f7cf7dffd0d16953251b75fd8b7224aae91e57357d5af853c41398d72a5f7`  
		Last Modified: Fri, 01 Dec 2023 00:14:01 GMT  
		Size: 19.0 KB (18953 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6.22-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:e9673caac3d318f89edf7ca6eaba8910416292f12f0f0abbf3d862a8b5af88ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4406434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a4e56736197b019e201b69449a358660e6806d076b61fd473dbcbb11caf5197`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["/bin/sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN apk add --no-cache libsasl # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4962e560ef629491acb51e64b06a5ee52545098f8403705778786a404e81434b`  
		Last Modified: Fri, 01 Dec 2023 15:25:24 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d4b10238ba82be69f174742e8ae9cd6e4484f32dce6eeb40dcbe3c5a4e0a1480`  
		Last Modified: Fri, 01 Dec 2023 15:25:24 GMT  
		Size: 124.1 KB (124087 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:276ae0cb4d4371459c3116e0453691ac59cdd9a6d649cb27bb3d3a090ef10fbf`  
		Last Modified: Fri, 01 Dec 2023 15:25:24 GMT  
		Size: 947.7 KB (947670 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:315ab34d41c816b04b8d07e4b7db199c17340b3b882b52819a0564f6be31a04c`  
		Last Modified: Fri, 01 Dec 2023 15:25:24 GMT  
		Size: 278.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:024d99cdc8f15c63cc478d1850db680f8c0dfae1ea2a5bca55e41fb0db12d020`  
		Last Modified: Fri, 01 Dec 2023 15:25:25 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.22-alpine3.18` - unknown; unknown

```console
$ docker pull memcached@sha256:91dac18281e4a194ee9756cf2652c70b2fb0bd2ba9d26c5c86d44c762d111821
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.9 KB (96880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3590bb02748f6b9e8a22ef90e7b41976bcb90189d98a78beae80f5aab1cd1cf4`

```dockerfile
```

-	Layers:
	-	`sha256:605a9d206d49d790bef9ce82c45179355571f37a91c5730ca6f59a03e13c0c76`  
		Last Modified: Fri, 01 Dec 2023 15:25:24 GMT  
		Size: 78.1 KB (78074 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:95803ef4905954256ae922386b3196bdafabd328ecd648b88ed7d8c13ec3b640`  
		Last Modified: Fri, 01 Dec 2023 15:25:24 GMT  
		Size: 18.8 KB (18806 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6.22-alpine3.18` - linux; 386

```console
$ docker pull memcached@sha256:c281c55fd61946d53161839c584fb2bab1e6701155ad4b32c816d6ab0dc21a08
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4692614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c2fd98aa81c35c4a5fa9401b2f61ac48a2632d3b4b4baacc4b7982b10310097`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 28 Sep 2023 20:38:19 GMT
ADD file:8402753f294e403e92353bd65c86a6428c960be5116c0a15484b663a84f66fcd in / 
# Thu, 28 Sep 2023 20:38:20 GMT
CMD ["/bin/sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN apk add --no-cache libsasl # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:dc95107ad2a031a015320bb397f73ec151d738127175b31ad643120697dc7e90`  
		Last Modified: Thu, 28 Sep 2023 20:39:32 GMT  
		Size: 3.2 MB (3235757 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4951068162aca253cfa98ba4876636d5f13870e8ae9df08734f097bb6291e163`  
		Last Modified: Wed, 18 Oct 2023 01:04:05 GMT  
		Size: 1.2 KB (1246 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:50e4c32dd77b7a60c60be859a9848c50b3da8b95360dea46acf070797f48ab2a`  
		Last Modified: Wed, 18 Oct 2023 01:04:05 GMT  
		Size: 109.5 KB (109458 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:77aecf5d85dda7360aa3010357b83f206e1873aa4df6de5692c0c39dbf083c2a`  
		Last Modified: Wed, 18 Oct 2023 01:04:06 GMT  
		Size: 1.3 MB (1345750 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:99e49c7a1306cd1125b7dbc332a0b1b47b2408c77e975df11b090c0ab5599be3`  
		Last Modified: Wed, 18 Oct 2023 01:04:06 GMT  
		Size: 281.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:68c5ecf5461e2d137f2c403e26fe6e0532a5ecf0eedcd77a5b18254c82b9a075`  
		Last Modified: Wed, 18 Oct 2023 01:04:07 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.22-alpine3.18` - unknown; unknown

```console
$ docker pull memcached@sha256:f0efd827c59fd288434c24a501d257456e82560b34d98f97cfe8b132454e28b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 KB (18687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea78294aafd9f308a52d310f899433de63e91eaac550b4ace8c1b8647774c7b8`

```dockerfile
```

-	Layers:
	-	`sha256:8c15fbe468a3b1236cadb64627426b8e2cb8bb71fddd26e10cdc44abd3b3519c`  
		Last Modified: Wed, 18 Oct 2023 01:04:05 GMT  
		Size: 18.7 KB (18687 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6.22-alpine3.18` - linux; ppc64le

```console
$ docker pull memcached@sha256:bae49b5a412b4535ebab987425356a20af16fc1ce70c38e18f6aa6572cac522d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4460245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b845ad70056a07d2adbebdc425879a4eb74152c886dae5d8e5496c6114cd3cda`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:3450a1687b552498a987f87cb844b7f597c7181d7c3d31943d7b3036d5300d5e in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["/bin/sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN apk add --no-cache libsasl # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:4e13780adf2776477b14ef9c0f4f563f820a2fde166d472218037b979e84d31a`  
		Last Modified: Thu, 30 Nov 2023 23:20:01 GMT  
		Size: 3.3 MB (3348322 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a33c280bf18f1bba1782f90d468941796634b74c44d9aae4c406162114520e9a`  
		Last Modified: Fri, 01 Dec 2023 12:01:06 GMT  
		Size: 1.2 KB (1247 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a54d91525051bf65bd807cac3c6f1a685ac2fc6ec7f763df97c18a3ca4b6dde0`  
		Last Modified: Fri, 01 Dec 2023 12:01:07 GMT  
		Size: 123.9 KB (123864 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:73f73a883ca0c1147533ae5085475dee29244e8ef06b0455c52afa6ab50c3023`  
		Last Modified: Fri, 01 Dec 2023 12:01:07 GMT  
		Size: 986.4 KB (986410 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:183bb794a2f98d5b2192b311c4b597c47ee4ee0bb405558f67827c8afaf0b8d3`  
		Last Modified: Fri, 01 Dec 2023 12:01:07 GMT  
		Size: 280.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:556988ad767ddefdfb131bbf239cceba01e60b197c0893287ee0f6274e54a0c8`  
		Last Modified: Fri, 01 Dec 2023 12:01:08 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.22-alpine3.18` - unknown; unknown

```console
$ docker pull memcached@sha256:df95592ada35b125fd73982e23f99a4fc3820ab083e12870f4edb179935ec44d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.3 KB (95332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67d44fe1dc00fdfaba957619ac6567e2ba40c2bad9a422ffb5287bb160b01fe7`

```dockerfile
```

-	Layers:
	-	`sha256:4a7a9ea74e3391f7a0e156b244eb474f674d42637b77983cfd9c92b23701d5ce`  
		Last Modified: Fri, 01 Dec 2023 12:01:06 GMT  
		Size: 76.5 KB (76477 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:671ec9ab176a20a138f0a3e238976e619a6f3011f598148b2cadd4c167721f81`  
		Last Modified: Fri, 01 Dec 2023 12:01:07 GMT  
		Size: 18.9 KB (18855 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6.22-alpine3.18` - linux; s390x

```console
$ docker pull memcached@sha256:7af81a585082ce3ca180a3fac82a30bb37a43973123841b2dec30e5d096be8cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4285472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b785f0d9bb74e0e2b4f8772ce85a7b23cfc2e2f8dbb7ad428517b68cca17de38`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["/bin/sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN apk add --no-cache libsasl # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a7b34c58047c2f1ded65320321066565e57ddd2ed65156bde99267b8e575bf63`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:036bb49faad29b98ef9de81de4441efa5208c00e72ccea2b631c7b1c283f072d`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 112.8 KB (112781 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c1da6195feb453292bec9ae13a8968a7fbc7b611793ac2bc13df3614b514db3f`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 953.6 KB (953590 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a43896e685e7c2e1e51c75c1ed262d1c57940abdc2e68d74301201c9aa8ebdfe`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 281.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:928e080b9c3b24e2e655bd62e483670acb3c5508648e5a2784a6bebb4d252367`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.22-alpine3.18` - unknown; unknown

```console
$ docker pull memcached@sha256:89eda6fd40656e7c2d5de572e4bdfbd821a333eb1067170caf9074dcbc141515
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.2 KB (95207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e34e69a75d4acd1221e6dd87a6f96bcf43e52e6ebaba333e1e4cc57d391f048`

```dockerfile
```

-	Layers:
	-	`sha256:c5dd02fe5ddfbc8ce715e0e666a98ae24e73371a2a8dee859d796538f4cf0618`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 76.4 KB (76419 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:13692e9f247d60b0cd5d0d4c0ccb23a86437ea348414e8548639ba89b5e4b65a`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 18.8 KB (18788 bytes)  
		MIME: application/vnd.in-toto+json

## `memcached:1.6.22-bookworm`

```console
$ docker pull memcached@sha256:9ed83da692bea50f7d0466186e0a2b527c047993805b98c99c1794bceb27d0e8
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 14
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v5
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

### `memcached:1.6.22-bookworm` - linux; amd64

```console
$ docker pull memcached@sha256:7b0480ab945f960f703af2f286b02a7b620eb4f772e25a2a1374e0c7d32f46de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.8 MB (38815745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f65c7b1a196aa7dfe9520f598f699d5846d6ff0eed117a36ca216302174a1bb1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:d261a6f6921593f1e0b3f472ab1b1822e2c6deb0b369200f0b3370556bfad017 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1f7ce2fa46ab3942feabee654933948821303a5a821789dddab2d8c3df59e227`  
		Last Modified: Tue, 21 Nov 2023 05:25:58 GMT  
		Size: 29.1 MB (29149908 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3606f7d6f784848f3e26f4bc5fae3dde08d65681dbaba232236ac8855cddb881`  
		Last Modified: Tue, 21 Nov 2023 06:19:50 GMT  
		Size: 1.1 KB (1110 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d9e66f47c0a00f0a833454718ca9dc6504f38c45944b5ebf43ccac532dc520b6`  
		Last Modified: Tue, 21 Nov 2023 06:19:50 GMT  
		Size: 2.5 MB (2488339 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:26e0a53c88ab99ad6e23fbb12147cce82e922e4141af56338b4ec01c2ead2b07`  
		Last Modified: Tue, 21 Nov 2023 06:19:50 GMT  
		Size: 7.2 MB (7175988 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:afc0db62c179dab7a3fc4ff6848e150c3315896846d827282affab08909d6e23`  
		Last Modified: Tue, 21 Nov 2023 06:19:50 GMT  
		Size: 281.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7af609a76aa9ed2d446da8865870d0e2b3bff46785783284d956d755a714899b`  
		Last Modified: Tue, 21 Nov 2023 06:19:50 GMT  
		Size: 119.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.22-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:cb387d9a91a709e6a4193c58df1f36753dbc6c13b9788d741d6dd92ee262ea52
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3078549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3b5853b03b272d3ad2682a093fbc3b2ffd577e3c9fe01f926b5963b333208cd`

```dockerfile
```

-	Layers:
	-	`sha256:9630a5bf61090e535bcf3b7ad1349332584446ea948e10119e025a65fad57d26`  
		Last Modified: Tue, 21 Nov 2023 06:19:50 GMT  
		Size: 3.1 MB (3056780 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:a2ef4829ccc1863c60fdfcf41590326d17bfbdef204a7d37664c92bec494942b`  
		Last Modified: Tue, 21 Nov 2023 06:19:50 GMT  
		Size: 21.8 KB (21769 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6.22-bookworm` - linux; arm variant v5

```console
$ docker pull memcached@sha256:c5fbea0a198cb4ae068e4761d5d1abab499e4ebc80275be6b7d797196cf3db54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34849973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b72ee44b42eca798309f6aa48ed2af9feca23c5eb64e5be38fa2536110b12ce`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:1ae8e5ac45b11d01083680b765e1fcfef9f7938f89d6f424572126fa946d8cdf in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f476aef5b6e1122850e68c81ef06fc2df17e968961b060483b4d2fb33018aae3`  
		Last Modified: Tue, 21 Nov 2023 05:03:55 GMT  
		Size: 26.9 MB (26922153 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:26dadbdb945a22546f6b2c171d0bededff72d7598719ab8f3877f67129e21730`  
		Last Modified: Tue, 21 Nov 2023 16:18:13 GMT  
		Size: 1.1 KB (1109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:44f46f0b8b7c11e6cd53e82541f819c66da246b152155fff8ce762f98c25219f`  
		Last Modified: Tue, 21 Nov 2023 16:18:14 GMT  
		Size: 2.1 MB (2089268 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:639e86d18160b654876d404a88b437cea26de29151122dfe8cbed9947f1b7b10`  
		Last Modified: Tue, 21 Nov 2023 16:18:14 GMT  
		Size: 5.8 MB (5837040 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7b963217677ca57533744aee2b331f059fbb6882f27abe2cc976462604e7b560`  
		Last Modified: Tue, 21 Nov 2023 16:18:15 GMT  
		Size: 283.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ac3a1fa5d4b6c48ea8ce4c375a197047f1480fbfb37c316b7d730d026d261219`  
		Last Modified: Tue, 21 Nov 2023 16:18:15 GMT  
		Size: 120.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.22-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:cd008d8c4d507d73b5f0153ed880e81e86a53741b480bbf6b1d318510e83a288
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.7 KB (21695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85e0f40569066724c087be3d901d5c5d984043271b56a33dec281e36032017f0`

```dockerfile
```

-	Layers:
	-	`sha256:2eff64dde44b4be85375aed8309f5d20476ca81876607d799b56c31addee0cb8`  
		Last Modified: Tue, 21 Nov 2023 16:18:13 GMT  
		Size: 21.7 KB (21695 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6.22-bookworm` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:dd556de8d6e6b81c51ba9120fa924fbb7fae427468d82db9f2b3db124f9ac0b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.7 MB (37711361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f05ec0c73b4afc866c99864d86b1c66deb5d8bda84bf2cc78e1e763e0ed6a263`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:869c7d0747a17c53715581a2e862992eb8516c7f45f167821dfa80966a4870d1 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2c6d21737d8318aa15c4cc838475029a5efc36c0429e3d8da80d97d0b96d9aaf`  
		Last Modified: Tue, 21 Nov 2023 06:30:30 GMT  
		Size: 29.2 MB (29179277 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fa3a18531b093eb1a543ad01b2a54d4692f59bba8d49ea9793b3ff09e528cd93`  
		Last Modified: Wed, 22 Nov 2023 11:50:41 GMT  
		Size: 1.1 KB (1109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:395fd5be77a2adb2c1b863f9ba2c664074aacb120f379bbb0f45cda74cc09cf4`  
		Last Modified: Wed, 22 Nov 2023 11:50:41 GMT  
		Size: 2.3 MB (2345987 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1dbcb5e891e054cd85f29e62fff856117d8cb919630be0c7473b520168b8c261`  
		Last Modified: Wed, 22 Nov 2023 11:50:41 GMT  
		Size: 6.2 MB (6184583 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2654df736cfb30e0097cca6a637ae794285396f6e2b87031636c8056b66baed0`  
		Last Modified: Wed, 22 Nov 2023 11:50:41 GMT  
		Size: 283.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e54ea6c3f7f45d9ed3f003bcf9e0a717c342daae58d330fef355e712d15b732`  
		Last Modified: Wed, 22 Nov 2023 11:50:42 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.22-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:2b5053d245e0312a77b7827553fcf09a6b19a0bf825a7016a4125713ad0d814f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3053591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e04bc647daea7fbb746cd418f19740162bd910826c366cdcc3549c3888ad5e1b`

```dockerfile
```

-	Layers:
	-	`sha256:f04377bb8fcfc3a24c1a36aa0bdf9b2d9272b7a60e82a88b66e2bb0645703c07`  
		Last Modified: Wed, 22 Nov 2023 11:50:41 GMT  
		Size: 3.0 MB (3031971 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:601cddda9e5f7f3a82cfc305051ac3c1fc5f65a9722e4dbe06363cc8b6ea68be`  
		Last Modified: Wed, 22 Nov 2023 11:50:41 GMT  
		Size: 21.6 KB (21620 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6.22-bookworm` - linux; 386

```console
$ docker pull memcached@sha256:fa9dba8086765d68f2feecfc2ac08fb29c019597d09943bb480227e6cba87666
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.3 MB (39294993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93047050e75b6d4d64adb8a7c8f68cb118bad27ca9dc772120e251b174752cf9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:0c94521fdd9c0a4fdeeb9aad23e68cd053fba0dcd7c3af550aefa79377816e31 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:98bdfce9af831c2a0d0bfcca812d0039cd1666986550f552b4b4c625bd5aa31c`  
		Last Modified: Wed, 01 Nov 2023 00:43:26 GMT  
		Size: 30.2 MB (30164042 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1b647d4b10cf20ac5807101c7d0380701be684aa82f5c01ec41f674b5ef23d42`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 1.1 KB (1109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b61c058003459de4911c2901b2d799b03de754a1b9e64ffbe21a04992e962e62`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 2.5 MB (2492501 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:810b6db64df2fcc8f76941cdac75093cf35bd72ac3cd1fa5eb664e74c1f67cd8`  
		Last Modified: Wed, 01 Nov 2023 01:06:50 GMT  
		Size: 6.6 MB (6636937 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dbb899942df4149bd5fae8bac6e295285ec80f82d621f2b29c931ee348491cfb`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 282.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4a8530160ab232c37c0ddcbf5e3a731d835d378d1382843957f6c2a73b2b5be6`  
		Last Modified: Wed, 01 Nov 2023 01:06:50 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.22-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:dd7ce9519c31365127142232df2ed0b285e9acc03cd77c23c838bf932165def8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 KB (21498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eef82c92e07c11a92c337806d01cfb1c6cdc7a16608dcf304a38de34d2ef1dbb`

```dockerfile
```

-	Layers:
	-	`sha256:c0d9dd22513f8d3e791e1796d7ef1906e57c798c92dd35d0be9cf2eaecec5954`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 21.5 KB (21498 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6.22-bookworm` - linux; mips64le

```console
$ docker pull memcached@sha256:a7c198db1b0856aff4b1514137e473ea30bce2ef22f0192cfdce7e2e44f2a863
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.6 MB (37588022 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1654ec4454e597d7e7cb6a7d97e98208de241a3dfafc5e0532b9561eac91f013`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:e093749192323dc72b60a8440ddba26c415586f618b5e107fa264ba5eb2ca7ba in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:ebdff2138fee4a3ec27560ab1353dc51c12c2608ff721f5db3d24104872b702a`  
		Last Modified: Tue, 21 Nov 2023 04:20:35 GMT  
		Size: 29.1 MB (29141984 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:50b1ffce24cec457fe1757715d60bd669145e5babade7c57143c4b665a55389e`  
		Last Modified: Thu, 23 Nov 2023 01:10:58 GMT  
		Size: 1.1 KB (1112 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:893c712c491a058aada36756e9f176b6c6c2f3a2b3adf0cd94b896c8198ec3ee`  
		Last Modified: Thu, 23 Nov 2023 01:10:59 GMT  
		Size: 1.9 MB (1937483 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0b8443254952572331df084976853329b69a4348b3c620bb073b5c89fb943b2b`  
		Last Modified: Thu, 23 Nov 2023 01:10:59 GMT  
		Size: 6.5 MB (6507036 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:904bfc5c5c0923edd9be421332402b224bfcd49053bc9b3fae6173383f5cd395`  
		Last Modified: Thu, 23 Nov 2023 01:10:59 GMT  
		Size: 285.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c265216ad3407dbc99903d96423b3a2314bc48cc0118911d150a6bb087ff7d85`  
		Last Modified: Thu, 23 Nov 2023 01:11:00 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.22-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:e2fcd32899d09ff06793849927220bea14475e64f085972afbc1f3af74dc209b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.7 KB (21656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf1c2028769aa20a3e529d0f85c8144ba6b099f74cda0dfca2272b7831d2d7a5`

```dockerfile
```

-	Layers:
	-	`sha256:75bab713cb94cdececf4c3879050737e7cb4bbb6206daa071ea001692b53d659`  
		Last Modified: Thu, 23 Nov 2023 01:10:58 GMT  
		Size: 21.7 KB (21656 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6.22-bookworm` - linux; ppc64le

```console
$ docker pull memcached@sha256:d8d106a88d6a15fadf738e59a6dcfc3942f11c7a2d19b7473abce66af7f4d19c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.0 MB (43030916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85da4ca798d44fc951b843ec85c410207ecc3c56af6d1bf7c321c91266d54e1b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:8b22a531b6611a1e63dfc20e4e2931592e2d821bd4b64c4b2810bb9a36640c02 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c570d04e61d8e35a3c8f12179d048d701451f97f9cf2099ea3e3738512dbf062`  
		Last Modified: Tue, 21 Nov 2023 04:28:58 GMT  
		Size: 33.1 MB (33141607 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bcd0cf90a66e23cd3d72b99e7d36129b0e846407a07c30031b0c1e4ba115cd30`  
		Last Modified: Tue, 21 Nov 2023 23:46:47 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5e4166a0e033df4117b469f840c6f5527e87dbd13c582c0b50c182b4bb3ead79`  
		Last Modified: Tue, 21 Nov 2023 23:46:47 GMT  
		Size: 2.7 MB (2698215 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:947b7328e0db59b9870fe9c6d6b7fc4e8a8f1fef3d2a36064fe3d60f5314652d`  
		Last Modified: Tue, 21 Nov 2023 23:46:48 GMT  
		Size: 7.2 MB (7189577 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f011f72796530a711f1de9d543435299d02ed3636e4cd28aee1fa493fbc2bf4`  
		Last Modified: Tue, 21 Nov 2023 23:46:47 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9d27046f19e474530b87e1d0b429e9d85f403210dd3d91bf60d8303fef03af96`  
		Last Modified: Tue, 21 Nov 2023 23:46:48 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.22-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:4269af6aa39a29d6dca352659fbf04b7d1bb4e65151e63a3ffcf2749d853597e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3067036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6e9626f30d490d2014e9fbb19add0b6ac0f63c8f4af2082d04750fea7ec35ff`

```dockerfile
```

-	Layers:
	-	`sha256:70759e1722d82b89de5c0d71ba2050ecc9f29d95ee758369044a1fc79026a546`  
		Last Modified: Tue, 21 Nov 2023 23:46:47 GMT  
		Size: 3.0 MB (3045366 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:4f34d59241ff06b2bd0cb8239d96be938e1e13470264898863f307f84ab275b6`  
		Last Modified: Tue, 21 Nov 2023 23:46:47 GMT  
		Size: 21.7 KB (21670 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6.22-bookworm` - linux; s390x

```console
$ docker pull memcached@sha256:312625a69b30a0a0371060c62ec97a621d587675e55a8ced694303d8a7015d30
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.7 MB (35745726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13ebe1c7df28f24c49c7dc749c55574a0a51a84e31dcff380e6caa5441fca944`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:c33fa9fdde73983850798b6eb1cd062e0398109d1d773e6a937fead7475c8efc in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6daa625e5a040476e253e7acd0befa74254a4865ec836d6334a544d82a21d4be`  
		Last Modified: Tue, 21 Nov 2023 05:10:21 GMT  
		Size: 27.5 MB (27512885 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:410539cfd307a2626bf5520b21d1cff0d4c8a336ebea36ed08878d81eca92847`  
		Last Modified: Tue, 21 Nov 2023 15:56:02 GMT  
		Size: 1.1 KB (1109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1ba4cc4f8ba1aa1865931fde910e1ebac220aea9a207eff2f2556bc289a513d3`  
		Last Modified: Tue, 21 Nov 2023 15:56:03 GMT  
		Size: 2.2 MB (2152517 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a47325d5bddeb006ca8a01a6239f747f4ed2c21fd6a28226bdfe46d1981d8962`  
		Last Modified: Tue, 21 Nov 2023 15:56:03 GMT  
		Size: 6.1 MB (6078811 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:32f889bfd6f6b6b2d773abb9f72f86fe0c7469d2a271e5bd209a3eb9b1c61dea`  
		Last Modified: Tue, 21 Nov 2023 15:56:04 GMT  
		Size: 283.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:56ce84d34f650bc21b164be1bb375a2b43c761943b4d06497991ceca18be1009`  
		Last Modified: Tue, 21 Nov 2023 15:56:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.22-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:b070f08010996b181adf3fbb4b9004e0d125115bf1380df8c4ddb96a99827218
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3068089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:307228ea8d7a2ce5fee0e1c4c36745e1c0244aa6d316102bde5b655af1bedd24`

```dockerfile
```

-	Layers:
	-	`sha256:640994e8299bce5ed690d70d55a1bc2035868614a169e4cda3391dafb76e9469`  
		Last Modified: Tue, 21 Nov 2023 15:56:03 GMT  
		Size: 3.0 MB (3046321 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:1893b50125646067935dd81f10c259d7b0c3b7cf2f42c81abe2b0f93e45f4250`  
		Last Modified: Tue, 21 Nov 2023 15:56:03 GMT  
		Size: 21.8 KB (21768 bytes)  
		MIME: application/vnd.in-toto+json

## `memcached:alpine`

```console
$ docker pull memcached@sha256:e8191559af396cda215a055e31a07bfc8178241854fa20f9e2cd32e4f1f5169e
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 11
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `memcached:alpine` - linux; amd64

```console
$ docker pull memcached@sha256:f85dfa7d8ec9dc1b785c37ccf6dfa62bca5fec355c32ddf7957116376863284a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4471146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f687f33554b696db4e2422b52d11bd36b20649d152ca63d20848c83b0679237f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["/bin/sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN apk add --no-cache libsasl # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ce5e53c5eb3023b585266ac7ee39c0b268a83b4e16556b72f52bd67e39f596be`  
		Last Modified: Fri, 01 Dec 2023 00:14:01 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e958dac8143e41701702904f092ab10b8682434d3d88e5af758dafaeb3317428`  
		Last Modified: Fri, 01 Dec 2023 00:14:01 GMT  
		Size: 108.0 KB (107998 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:61dfbf83553658c4ab4a5ae4477150c88a3f30da8309b9cfefdc185b3764e501`  
		Last Modified: Fri, 01 Dec 2023 00:14:01 GMT  
		Size: 959.1 KB (959085 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8b397213e2806c5c7c6aca6c20bc2f69362c9f6204c5d3947eaaf870176d9a36`  
		Last Modified: Fri, 01 Dec 2023 00:14:01 GMT  
		Size: 277.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8c404d1dff37be469e83d35363176296e0129304273844e38a69edbd6861f08c`  
		Last Modified: Fri, 01 Dec 2023 00:14:02 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:alpine` - unknown; unknown

```console
$ docker pull memcached@sha256:6a508d9bd488a6e6f8bbaae93d8ff14548111b267a7440f64edec96b04f8a3cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 KB (97008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fdbf48b2b61dd467eec02ffd7b0e996989023a93d9ecbc7a655a0755362c38a`

```dockerfile
```

-	Layers:
	-	`sha256:5c3e16fb5448bac47fadf2a80df72f13e831b463525dc9823da6c85f1770bf69`  
		Last Modified: Fri, 01 Dec 2023 00:14:01 GMT  
		Size: 78.1 KB (78055 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:1d5f7cf7dffd0d16953251b75fd8b7224aae91e57357d5af853c41398d72a5f7`  
		Last Modified: Fri, 01 Dec 2023 00:14:01 GMT  
		Size: 19.0 KB (18953 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:alpine` - linux; arm variant v7

```console
$ docker pull memcached@sha256:79a5646a0c845a791f36017fda3292281b48295b06c53f13d62c9f94237d4731
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3960292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2afac0e49af3ce3f1769abe11a29f8f5610c6a736d8c5b6c7b9770c8d8e94e91`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 06:43:29 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 17 Dec 2020 06:43:31 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Thu, 17 Dec 2020 06:43:33 GMT
ENV MEMCACHED_VERSION=1.6.9
# Thu, 17 Dec 2020 06:43:35 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Thu, 17 Dec 2020 06:46:32 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 17 Dec 2020 06:46:33 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 17 Dec 2020 06:46:35 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 17 Dec 2020 06:46:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 06:46:36 GMT
USER memcache
# Thu, 17 Dec 2020 06:46:38 GMT
EXPOSE 11211
# Thu, 17 Dec 2020 06:46:39 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68564bbfc09f153688e942bf54d5375d1e27f3507c0bed6b038c2ac8ce095aa5`  
		Last Modified: Thu, 17 Dec 2020 06:46:58 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cac3a91edee49d0b08a25706ae86059bed89941a08b496e72ef092e57c4ecb3`  
		Last Modified: Thu, 17 Dec 2020 06:46:58 GMT  
		Size: 13.8 KB (13825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf16e9bb942ec42a35a792beab65aea843209e7bdde7e856499b9fc85f93bc4e`  
		Last Modified: Thu, 17 Dec 2020 06:46:58 GMT  
		Size: 1.5 MB (1537248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc15394239bd0c083e1b6df806aa5ffeb8b9cc7e80113afc2959721de49f90d1`  
		Last Modified: Thu, 17 Dec 2020 06:46:58 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482f0eb571548eae5720c652ff7da13558e56a8722dc9932cf7eb1ef3eb33acb`  
		Last Modified: Thu, 17 Dec 2020 06:46:58 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:e9673caac3d318f89edf7ca6eaba8910416292f12f0f0abbf3d862a8b5af88ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4406434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a4e56736197b019e201b69449a358660e6806d076b61fd473dbcbb11caf5197`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["/bin/sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN apk add --no-cache libsasl # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4962e560ef629491acb51e64b06a5ee52545098f8403705778786a404e81434b`  
		Last Modified: Fri, 01 Dec 2023 15:25:24 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d4b10238ba82be69f174742e8ae9cd6e4484f32dce6eeb40dcbe3c5a4e0a1480`  
		Last Modified: Fri, 01 Dec 2023 15:25:24 GMT  
		Size: 124.1 KB (124087 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:276ae0cb4d4371459c3116e0453691ac59cdd9a6d649cb27bb3d3a090ef10fbf`  
		Last Modified: Fri, 01 Dec 2023 15:25:24 GMT  
		Size: 947.7 KB (947670 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:315ab34d41c816b04b8d07e4b7db199c17340b3b882b52819a0564f6be31a04c`  
		Last Modified: Fri, 01 Dec 2023 15:25:24 GMT  
		Size: 278.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:024d99cdc8f15c63cc478d1850db680f8c0dfae1ea2a5bca55e41fb0db12d020`  
		Last Modified: Fri, 01 Dec 2023 15:25:25 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:alpine` - unknown; unknown

```console
$ docker pull memcached@sha256:91dac18281e4a194ee9756cf2652c70b2fb0bd2ba9d26c5c86d44c762d111821
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.9 KB (96880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3590bb02748f6b9e8a22ef90e7b41976bcb90189d98a78beae80f5aab1cd1cf4`

```dockerfile
```

-	Layers:
	-	`sha256:605a9d206d49d790bef9ce82c45179355571f37a91c5730ca6f59a03e13c0c76`  
		Last Modified: Fri, 01 Dec 2023 15:25:24 GMT  
		Size: 78.1 KB (78074 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:95803ef4905954256ae922386b3196bdafabd328ecd648b88ed7d8c13ec3b640`  
		Last Modified: Fri, 01 Dec 2023 15:25:24 GMT  
		Size: 18.8 KB (18806 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:alpine` - linux; 386

```console
$ docker pull memcached@sha256:c281c55fd61946d53161839c584fb2bab1e6701155ad4b32c816d6ab0dc21a08
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4692614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c2fd98aa81c35c4a5fa9401b2f61ac48a2632d3b4b4baacc4b7982b10310097`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 28 Sep 2023 20:38:19 GMT
ADD file:8402753f294e403e92353bd65c86a6428c960be5116c0a15484b663a84f66fcd in / 
# Thu, 28 Sep 2023 20:38:20 GMT
CMD ["/bin/sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN apk add --no-cache libsasl # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:dc95107ad2a031a015320bb397f73ec151d738127175b31ad643120697dc7e90`  
		Last Modified: Thu, 28 Sep 2023 20:39:32 GMT  
		Size: 3.2 MB (3235757 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4951068162aca253cfa98ba4876636d5f13870e8ae9df08734f097bb6291e163`  
		Last Modified: Wed, 18 Oct 2023 01:04:05 GMT  
		Size: 1.2 KB (1246 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:50e4c32dd77b7a60c60be859a9848c50b3da8b95360dea46acf070797f48ab2a`  
		Last Modified: Wed, 18 Oct 2023 01:04:05 GMT  
		Size: 109.5 KB (109458 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:77aecf5d85dda7360aa3010357b83f206e1873aa4df6de5692c0c39dbf083c2a`  
		Last Modified: Wed, 18 Oct 2023 01:04:06 GMT  
		Size: 1.3 MB (1345750 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:99e49c7a1306cd1125b7dbc332a0b1b47b2408c77e975df11b090c0ab5599be3`  
		Last Modified: Wed, 18 Oct 2023 01:04:06 GMT  
		Size: 281.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:68c5ecf5461e2d137f2c403e26fe6e0532a5ecf0eedcd77a5b18254c82b9a075`  
		Last Modified: Wed, 18 Oct 2023 01:04:07 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:alpine` - unknown; unknown

```console
$ docker pull memcached@sha256:f0efd827c59fd288434c24a501d257456e82560b34d98f97cfe8b132454e28b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 KB (18687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea78294aafd9f308a52d310f899433de63e91eaac550b4ace8c1b8647774c7b8`

```dockerfile
```

-	Layers:
	-	`sha256:8c15fbe468a3b1236cadb64627426b8e2cb8bb71fddd26e10cdc44abd3b3519c`  
		Last Modified: Wed, 18 Oct 2023 01:04:05 GMT  
		Size: 18.7 KB (18687 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:bae49b5a412b4535ebab987425356a20af16fc1ce70c38e18f6aa6572cac522d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4460245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b845ad70056a07d2adbebdc425879a4eb74152c886dae5d8e5496c6114cd3cda`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:3450a1687b552498a987f87cb844b7f597c7181d7c3d31943d7b3036d5300d5e in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["/bin/sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN apk add --no-cache libsasl # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:4e13780adf2776477b14ef9c0f4f563f820a2fde166d472218037b979e84d31a`  
		Last Modified: Thu, 30 Nov 2023 23:20:01 GMT  
		Size: 3.3 MB (3348322 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a33c280bf18f1bba1782f90d468941796634b74c44d9aae4c406162114520e9a`  
		Last Modified: Fri, 01 Dec 2023 12:01:06 GMT  
		Size: 1.2 KB (1247 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a54d91525051bf65bd807cac3c6f1a685ac2fc6ec7f763df97c18a3ca4b6dde0`  
		Last Modified: Fri, 01 Dec 2023 12:01:07 GMT  
		Size: 123.9 KB (123864 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:73f73a883ca0c1147533ae5085475dee29244e8ef06b0455c52afa6ab50c3023`  
		Last Modified: Fri, 01 Dec 2023 12:01:07 GMT  
		Size: 986.4 KB (986410 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:183bb794a2f98d5b2192b311c4b597c47ee4ee0bb405558f67827c8afaf0b8d3`  
		Last Modified: Fri, 01 Dec 2023 12:01:07 GMT  
		Size: 280.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:556988ad767ddefdfb131bbf239cceba01e60b197c0893287ee0f6274e54a0c8`  
		Last Modified: Fri, 01 Dec 2023 12:01:08 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:alpine` - unknown; unknown

```console
$ docker pull memcached@sha256:df95592ada35b125fd73982e23f99a4fc3820ab083e12870f4edb179935ec44d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.3 KB (95332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67d44fe1dc00fdfaba957619ac6567e2ba40c2bad9a422ffb5287bb160b01fe7`

```dockerfile
```

-	Layers:
	-	`sha256:4a7a9ea74e3391f7a0e156b244eb474f674d42637b77983cfd9c92b23701d5ce`  
		Last Modified: Fri, 01 Dec 2023 12:01:06 GMT  
		Size: 76.5 KB (76477 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:671ec9ab176a20a138f0a3e238976e619a6f3011f598148b2cadd4c167721f81`  
		Last Modified: Fri, 01 Dec 2023 12:01:07 GMT  
		Size: 18.9 KB (18855 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:alpine` - linux; s390x

```console
$ docker pull memcached@sha256:7af81a585082ce3ca180a3fac82a30bb37a43973123841b2dec30e5d096be8cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4285472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b785f0d9bb74e0e2b4f8772ce85a7b23cfc2e2f8dbb7ad428517b68cca17de38`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["/bin/sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN apk add --no-cache libsasl # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a7b34c58047c2f1ded65320321066565e57ddd2ed65156bde99267b8e575bf63`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:036bb49faad29b98ef9de81de4441efa5208c00e72ccea2b631c7b1c283f072d`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 112.8 KB (112781 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c1da6195feb453292bec9ae13a8968a7fbc7b611793ac2bc13df3614b514db3f`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 953.6 KB (953590 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a43896e685e7c2e1e51c75c1ed262d1c57940abdc2e68d74301201c9aa8ebdfe`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 281.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:928e080b9c3b24e2e655bd62e483670acb3c5508648e5a2784a6bebb4d252367`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:alpine` - unknown; unknown

```console
$ docker pull memcached@sha256:89eda6fd40656e7c2d5de572e4bdfbd821a333eb1067170caf9074dcbc141515
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.2 KB (95207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e34e69a75d4acd1221e6dd87a6f96bcf43e52e6ebaba333e1e4cc57d391f048`

```dockerfile
```

-	Layers:
	-	`sha256:c5dd02fe5ddfbc8ce715e0e666a98ae24e73371a2a8dee859d796538f4cf0618`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 76.4 KB (76419 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:13692e9f247d60b0cd5d0d4c0ccb23a86437ea348414e8548639ba89b5e4b65a`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 18.8 KB (18788 bytes)  
		MIME: application/vnd.in-toto+json

## `memcached:alpine3.18`

```console
$ docker pull memcached@sha256:93a9ff5ab97a213a027913f59bf902a118fa9750f88dbd4d513ebd920428820e
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 10
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `memcached:alpine3.18` - linux; amd64

```console
$ docker pull memcached@sha256:f85dfa7d8ec9dc1b785c37ccf6dfa62bca5fec355c32ddf7957116376863284a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4471146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f687f33554b696db4e2422b52d11bd36b20649d152ca63d20848c83b0679237f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["/bin/sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN apk add --no-cache libsasl # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ce5e53c5eb3023b585266ac7ee39c0b268a83b4e16556b72f52bd67e39f596be`  
		Last Modified: Fri, 01 Dec 2023 00:14:01 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e958dac8143e41701702904f092ab10b8682434d3d88e5af758dafaeb3317428`  
		Last Modified: Fri, 01 Dec 2023 00:14:01 GMT  
		Size: 108.0 KB (107998 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:61dfbf83553658c4ab4a5ae4477150c88a3f30da8309b9cfefdc185b3764e501`  
		Last Modified: Fri, 01 Dec 2023 00:14:01 GMT  
		Size: 959.1 KB (959085 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8b397213e2806c5c7c6aca6c20bc2f69362c9f6204c5d3947eaaf870176d9a36`  
		Last Modified: Fri, 01 Dec 2023 00:14:01 GMT  
		Size: 277.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8c404d1dff37be469e83d35363176296e0129304273844e38a69edbd6861f08c`  
		Last Modified: Fri, 01 Dec 2023 00:14:02 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:alpine3.18` - unknown; unknown

```console
$ docker pull memcached@sha256:6a508d9bd488a6e6f8bbaae93d8ff14548111b267a7440f64edec96b04f8a3cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.0 KB (97008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fdbf48b2b61dd467eec02ffd7b0e996989023a93d9ecbc7a655a0755362c38a`

```dockerfile
```

-	Layers:
	-	`sha256:5c3e16fb5448bac47fadf2a80df72f13e831b463525dc9823da6c85f1770bf69`  
		Last Modified: Fri, 01 Dec 2023 00:14:01 GMT  
		Size: 78.1 KB (78055 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:1d5f7cf7dffd0d16953251b75fd8b7224aae91e57357d5af853c41398d72a5f7`  
		Last Modified: Fri, 01 Dec 2023 00:14:01 GMT  
		Size: 19.0 KB (18953 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:alpine3.18` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:e9673caac3d318f89edf7ca6eaba8910416292f12f0f0abbf3d862a8b5af88ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4406434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a4e56736197b019e201b69449a358660e6806d076b61fd473dbcbb11caf5197`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["/bin/sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN apk add --no-cache libsasl # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4962e560ef629491acb51e64b06a5ee52545098f8403705778786a404e81434b`  
		Last Modified: Fri, 01 Dec 2023 15:25:24 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d4b10238ba82be69f174742e8ae9cd6e4484f32dce6eeb40dcbe3c5a4e0a1480`  
		Last Modified: Fri, 01 Dec 2023 15:25:24 GMT  
		Size: 124.1 KB (124087 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:276ae0cb4d4371459c3116e0453691ac59cdd9a6d649cb27bb3d3a090ef10fbf`  
		Last Modified: Fri, 01 Dec 2023 15:25:24 GMT  
		Size: 947.7 KB (947670 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:315ab34d41c816b04b8d07e4b7db199c17340b3b882b52819a0564f6be31a04c`  
		Last Modified: Fri, 01 Dec 2023 15:25:24 GMT  
		Size: 278.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:024d99cdc8f15c63cc478d1850db680f8c0dfae1ea2a5bca55e41fb0db12d020`  
		Last Modified: Fri, 01 Dec 2023 15:25:25 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:alpine3.18` - unknown; unknown

```console
$ docker pull memcached@sha256:91dac18281e4a194ee9756cf2652c70b2fb0bd2ba9d26c5c86d44c762d111821
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.9 KB (96880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3590bb02748f6b9e8a22ef90e7b41976bcb90189d98a78beae80f5aab1cd1cf4`

```dockerfile
```

-	Layers:
	-	`sha256:605a9d206d49d790bef9ce82c45179355571f37a91c5730ca6f59a03e13c0c76`  
		Last Modified: Fri, 01 Dec 2023 15:25:24 GMT  
		Size: 78.1 KB (78074 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:95803ef4905954256ae922386b3196bdafabd328ecd648b88ed7d8c13ec3b640`  
		Last Modified: Fri, 01 Dec 2023 15:25:24 GMT  
		Size: 18.8 KB (18806 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:alpine3.18` - linux; 386

```console
$ docker pull memcached@sha256:c281c55fd61946d53161839c584fb2bab1e6701155ad4b32c816d6ab0dc21a08
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4692614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c2fd98aa81c35c4a5fa9401b2f61ac48a2632d3b4b4baacc4b7982b10310097`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 28 Sep 2023 20:38:19 GMT
ADD file:8402753f294e403e92353bd65c86a6428c960be5116c0a15484b663a84f66fcd in / 
# Thu, 28 Sep 2023 20:38:20 GMT
CMD ["/bin/sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN apk add --no-cache libsasl # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:dc95107ad2a031a015320bb397f73ec151d738127175b31ad643120697dc7e90`  
		Last Modified: Thu, 28 Sep 2023 20:39:32 GMT  
		Size: 3.2 MB (3235757 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4951068162aca253cfa98ba4876636d5f13870e8ae9df08734f097bb6291e163`  
		Last Modified: Wed, 18 Oct 2023 01:04:05 GMT  
		Size: 1.2 KB (1246 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:50e4c32dd77b7a60c60be859a9848c50b3da8b95360dea46acf070797f48ab2a`  
		Last Modified: Wed, 18 Oct 2023 01:04:05 GMT  
		Size: 109.5 KB (109458 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:77aecf5d85dda7360aa3010357b83f206e1873aa4df6de5692c0c39dbf083c2a`  
		Last Modified: Wed, 18 Oct 2023 01:04:06 GMT  
		Size: 1.3 MB (1345750 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:99e49c7a1306cd1125b7dbc332a0b1b47b2408c77e975df11b090c0ab5599be3`  
		Last Modified: Wed, 18 Oct 2023 01:04:06 GMT  
		Size: 281.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:68c5ecf5461e2d137f2c403e26fe6e0532a5ecf0eedcd77a5b18254c82b9a075`  
		Last Modified: Wed, 18 Oct 2023 01:04:07 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:alpine3.18` - unknown; unknown

```console
$ docker pull memcached@sha256:f0efd827c59fd288434c24a501d257456e82560b34d98f97cfe8b132454e28b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 KB (18687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea78294aafd9f308a52d310f899433de63e91eaac550b4ace8c1b8647774c7b8`

```dockerfile
```

-	Layers:
	-	`sha256:8c15fbe468a3b1236cadb64627426b8e2cb8bb71fddd26e10cdc44abd3b3519c`  
		Last Modified: Wed, 18 Oct 2023 01:04:05 GMT  
		Size: 18.7 KB (18687 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:alpine3.18` - linux; ppc64le

```console
$ docker pull memcached@sha256:bae49b5a412b4535ebab987425356a20af16fc1ce70c38e18f6aa6572cac522d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4460245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b845ad70056a07d2adbebdc425879a4eb74152c886dae5d8e5496c6114cd3cda`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:3450a1687b552498a987f87cb844b7f597c7181d7c3d31943d7b3036d5300d5e in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["/bin/sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN apk add --no-cache libsasl # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:4e13780adf2776477b14ef9c0f4f563f820a2fde166d472218037b979e84d31a`  
		Last Modified: Thu, 30 Nov 2023 23:20:01 GMT  
		Size: 3.3 MB (3348322 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a33c280bf18f1bba1782f90d468941796634b74c44d9aae4c406162114520e9a`  
		Last Modified: Fri, 01 Dec 2023 12:01:06 GMT  
		Size: 1.2 KB (1247 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a54d91525051bf65bd807cac3c6f1a685ac2fc6ec7f763df97c18a3ca4b6dde0`  
		Last Modified: Fri, 01 Dec 2023 12:01:07 GMT  
		Size: 123.9 KB (123864 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:73f73a883ca0c1147533ae5085475dee29244e8ef06b0455c52afa6ab50c3023`  
		Last Modified: Fri, 01 Dec 2023 12:01:07 GMT  
		Size: 986.4 KB (986410 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:183bb794a2f98d5b2192b311c4b597c47ee4ee0bb405558f67827c8afaf0b8d3`  
		Last Modified: Fri, 01 Dec 2023 12:01:07 GMT  
		Size: 280.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:556988ad767ddefdfb131bbf239cceba01e60b197c0893287ee0f6274e54a0c8`  
		Last Modified: Fri, 01 Dec 2023 12:01:08 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:alpine3.18` - unknown; unknown

```console
$ docker pull memcached@sha256:df95592ada35b125fd73982e23f99a4fc3820ab083e12870f4edb179935ec44d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.3 KB (95332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67d44fe1dc00fdfaba957619ac6567e2ba40c2bad9a422ffb5287bb160b01fe7`

```dockerfile
```

-	Layers:
	-	`sha256:4a7a9ea74e3391f7a0e156b244eb474f674d42637b77983cfd9c92b23701d5ce`  
		Last Modified: Fri, 01 Dec 2023 12:01:06 GMT  
		Size: 76.5 KB (76477 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:671ec9ab176a20a138f0a3e238976e619a6f3011f598148b2cadd4c167721f81`  
		Last Modified: Fri, 01 Dec 2023 12:01:07 GMT  
		Size: 18.9 KB (18855 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:alpine3.18` - linux; s390x

```console
$ docker pull memcached@sha256:7af81a585082ce3ca180a3fac82a30bb37a43973123841b2dec30e5d096be8cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4285472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b785f0d9bb74e0e2b4f8772ce85a7b23cfc2e2f8dbb7ad428517b68cca17de38`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["/bin/sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN apk add --no-cache libsasl # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a7b34c58047c2f1ded65320321066565e57ddd2ed65156bde99267b8e575bf63`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:036bb49faad29b98ef9de81de4441efa5208c00e72ccea2b631c7b1c283f072d`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 112.8 KB (112781 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c1da6195feb453292bec9ae13a8968a7fbc7b611793ac2bc13df3614b514db3f`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 953.6 KB (953590 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a43896e685e7c2e1e51c75c1ed262d1c57940abdc2e68d74301201c9aa8ebdfe`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 281.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:928e080b9c3b24e2e655bd62e483670acb3c5508648e5a2784a6bebb4d252367`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:alpine3.18` - unknown; unknown

```console
$ docker pull memcached@sha256:89eda6fd40656e7c2d5de572e4bdfbd821a333eb1067170caf9074dcbc141515
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.2 KB (95207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e34e69a75d4acd1221e6dd87a6f96bcf43e52e6ebaba333e1e4cc57d391f048`

```dockerfile
```

-	Layers:
	-	`sha256:c5dd02fe5ddfbc8ce715e0e666a98ae24e73371a2a8dee859d796538f4cf0618`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 76.4 KB (76419 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:13692e9f247d60b0cd5d0d4c0ccb23a86437ea348414e8548639ba89b5e4b65a`  
		Last Modified: Fri, 01 Dec 2023 11:03:57 GMT  
		Size: 18.8 KB (18788 bytes)  
		MIME: application/vnd.in-toto+json

## `memcached:bookworm`

```console
$ docker pull memcached@sha256:9ed83da692bea50f7d0466186e0a2b527c047993805b98c99c1794bceb27d0e8
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 14
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v5
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

### `memcached:bookworm` - linux; amd64

```console
$ docker pull memcached@sha256:7b0480ab945f960f703af2f286b02a7b620eb4f772e25a2a1374e0c7d32f46de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.8 MB (38815745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f65c7b1a196aa7dfe9520f598f699d5846d6ff0eed117a36ca216302174a1bb1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:d261a6f6921593f1e0b3f472ab1b1822e2c6deb0b369200f0b3370556bfad017 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1f7ce2fa46ab3942feabee654933948821303a5a821789dddab2d8c3df59e227`  
		Last Modified: Tue, 21 Nov 2023 05:25:58 GMT  
		Size: 29.1 MB (29149908 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3606f7d6f784848f3e26f4bc5fae3dde08d65681dbaba232236ac8855cddb881`  
		Last Modified: Tue, 21 Nov 2023 06:19:50 GMT  
		Size: 1.1 KB (1110 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d9e66f47c0a00f0a833454718ca9dc6504f38c45944b5ebf43ccac532dc520b6`  
		Last Modified: Tue, 21 Nov 2023 06:19:50 GMT  
		Size: 2.5 MB (2488339 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:26e0a53c88ab99ad6e23fbb12147cce82e922e4141af56338b4ec01c2ead2b07`  
		Last Modified: Tue, 21 Nov 2023 06:19:50 GMT  
		Size: 7.2 MB (7175988 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:afc0db62c179dab7a3fc4ff6848e150c3315896846d827282affab08909d6e23`  
		Last Modified: Tue, 21 Nov 2023 06:19:50 GMT  
		Size: 281.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7af609a76aa9ed2d446da8865870d0e2b3bff46785783284d956d755a714899b`  
		Last Modified: Tue, 21 Nov 2023 06:19:50 GMT  
		Size: 119.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:cb387d9a91a709e6a4193c58df1f36753dbc6c13b9788d741d6dd92ee262ea52
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3078549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3b5853b03b272d3ad2682a093fbc3b2ffd577e3c9fe01f926b5963b333208cd`

```dockerfile
```

-	Layers:
	-	`sha256:9630a5bf61090e535bcf3b7ad1349332584446ea948e10119e025a65fad57d26`  
		Last Modified: Tue, 21 Nov 2023 06:19:50 GMT  
		Size: 3.1 MB (3056780 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:a2ef4829ccc1863c60fdfcf41590326d17bfbdef204a7d37664c92bec494942b`  
		Last Modified: Tue, 21 Nov 2023 06:19:50 GMT  
		Size: 21.8 KB (21769 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:bookworm` - linux; arm variant v5

```console
$ docker pull memcached@sha256:c5fbea0a198cb4ae068e4761d5d1abab499e4ebc80275be6b7d797196cf3db54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34849973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b72ee44b42eca798309f6aa48ed2af9feca23c5eb64e5be38fa2536110b12ce`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:1ae8e5ac45b11d01083680b765e1fcfef9f7938f89d6f424572126fa946d8cdf in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f476aef5b6e1122850e68c81ef06fc2df17e968961b060483b4d2fb33018aae3`  
		Last Modified: Tue, 21 Nov 2023 05:03:55 GMT  
		Size: 26.9 MB (26922153 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:26dadbdb945a22546f6b2c171d0bededff72d7598719ab8f3877f67129e21730`  
		Last Modified: Tue, 21 Nov 2023 16:18:13 GMT  
		Size: 1.1 KB (1109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:44f46f0b8b7c11e6cd53e82541f819c66da246b152155fff8ce762f98c25219f`  
		Last Modified: Tue, 21 Nov 2023 16:18:14 GMT  
		Size: 2.1 MB (2089268 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:639e86d18160b654876d404a88b437cea26de29151122dfe8cbed9947f1b7b10`  
		Last Modified: Tue, 21 Nov 2023 16:18:14 GMT  
		Size: 5.8 MB (5837040 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7b963217677ca57533744aee2b331f059fbb6882f27abe2cc976462604e7b560`  
		Last Modified: Tue, 21 Nov 2023 16:18:15 GMT  
		Size: 283.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ac3a1fa5d4b6c48ea8ce4c375a197047f1480fbfb37c316b7d730d026d261219`  
		Last Modified: Tue, 21 Nov 2023 16:18:15 GMT  
		Size: 120.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:cd008d8c4d507d73b5f0153ed880e81e86a53741b480bbf6b1d318510e83a288
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.7 KB (21695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85e0f40569066724c087be3d901d5c5d984043271b56a33dec281e36032017f0`

```dockerfile
```

-	Layers:
	-	`sha256:2eff64dde44b4be85375aed8309f5d20476ca81876607d799b56c31addee0cb8`  
		Last Modified: Tue, 21 Nov 2023 16:18:13 GMT  
		Size: 21.7 KB (21695 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:bookworm` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:dd556de8d6e6b81c51ba9120fa924fbb7fae427468d82db9f2b3db124f9ac0b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.7 MB (37711361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f05ec0c73b4afc866c99864d86b1c66deb5d8bda84bf2cc78e1e763e0ed6a263`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:869c7d0747a17c53715581a2e862992eb8516c7f45f167821dfa80966a4870d1 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2c6d21737d8318aa15c4cc838475029a5efc36c0429e3d8da80d97d0b96d9aaf`  
		Last Modified: Tue, 21 Nov 2023 06:30:30 GMT  
		Size: 29.2 MB (29179277 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fa3a18531b093eb1a543ad01b2a54d4692f59bba8d49ea9793b3ff09e528cd93`  
		Last Modified: Wed, 22 Nov 2023 11:50:41 GMT  
		Size: 1.1 KB (1109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:395fd5be77a2adb2c1b863f9ba2c664074aacb120f379bbb0f45cda74cc09cf4`  
		Last Modified: Wed, 22 Nov 2023 11:50:41 GMT  
		Size: 2.3 MB (2345987 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1dbcb5e891e054cd85f29e62fff856117d8cb919630be0c7473b520168b8c261`  
		Last Modified: Wed, 22 Nov 2023 11:50:41 GMT  
		Size: 6.2 MB (6184583 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2654df736cfb30e0097cca6a637ae794285396f6e2b87031636c8056b66baed0`  
		Last Modified: Wed, 22 Nov 2023 11:50:41 GMT  
		Size: 283.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e54ea6c3f7f45d9ed3f003bcf9e0a717c342daae58d330fef355e712d15b732`  
		Last Modified: Wed, 22 Nov 2023 11:50:42 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:2b5053d245e0312a77b7827553fcf09a6b19a0bf825a7016a4125713ad0d814f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3053591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e04bc647daea7fbb746cd418f19740162bd910826c366cdcc3549c3888ad5e1b`

```dockerfile
```

-	Layers:
	-	`sha256:f04377bb8fcfc3a24c1a36aa0bdf9b2d9272b7a60e82a88b66e2bb0645703c07`  
		Last Modified: Wed, 22 Nov 2023 11:50:41 GMT  
		Size: 3.0 MB (3031971 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:601cddda9e5f7f3a82cfc305051ac3c1fc5f65a9722e4dbe06363cc8b6ea68be`  
		Last Modified: Wed, 22 Nov 2023 11:50:41 GMT  
		Size: 21.6 KB (21620 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:bookworm` - linux; 386

```console
$ docker pull memcached@sha256:fa9dba8086765d68f2feecfc2ac08fb29c019597d09943bb480227e6cba87666
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.3 MB (39294993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93047050e75b6d4d64adb8a7c8f68cb118bad27ca9dc772120e251b174752cf9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:0c94521fdd9c0a4fdeeb9aad23e68cd053fba0dcd7c3af550aefa79377816e31 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:98bdfce9af831c2a0d0bfcca812d0039cd1666986550f552b4b4c625bd5aa31c`  
		Last Modified: Wed, 01 Nov 2023 00:43:26 GMT  
		Size: 30.2 MB (30164042 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1b647d4b10cf20ac5807101c7d0380701be684aa82f5c01ec41f674b5ef23d42`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 1.1 KB (1109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b61c058003459de4911c2901b2d799b03de754a1b9e64ffbe21a04992e962e62`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 2.5 MB (2492501 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:810b6db64df2fcc8f76941cdac75093cf35bd72ac3cd1fa5eb664e74c1f67cd8`  
		Last Modified: Wed, 01 Nov 2023 01:06:50 GMT  
		Size: 6.6 MB (6636937 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dbb899942df4149bd5fae8bac6e295285ec80f82d621f2b29c931ee348491cfb`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 282.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4a8530160ab232c37c0ddcbf5e3a731d835d378d1382843957f6c2a73b2b5be6`  
		Last Modified: Wed, 01 Nov 2023 01:06:50 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:dd7ce9519c31365127142232df2ed0b285e9acc03cd77c23c838bf932165def8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 KB (21498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eef82c92e07c11a92c337806d01cfb1c6cdc7a16608dcf304a38de34d2ef1dbb`

```dockerfile
```

-	Layers:
	-	`sha256:c0d9dd22513f8d3e791e1796d7ef1906e57c798c92dd35d0be9cf2eaecec5954`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 21.5 KB (21498 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:bookworm` - linux; mips64le

```console
$ docker pull memcached@sha256:a7c198db1b0856aff4b1514137e473ea30bce2ef22f0192cfdce7e2e44f2a863
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.6 MB (37588022 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1654ec4454e597d7e7cb6a7d97e98208de241a3dfafc5e0532b9561eac91f013`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:e093749192323dc72b60a8440ddba26c415586f618b5e107fa264ba5eb2ca7ba in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:ebdff2138fee4a3ec27560ab1353dc51c12c2608ff721f5db3d24104872b702a`  
		Last Modified: Tue, 21 Nov 2023 04:20:35 GMT  
		Size: 29.1 MB (29141984 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:50b1ffce24cec457fe1757715d60bd669145e5babade7c57143c4b665a55389e`  
		Last Modified: Thu, 23 Nov 2023 01:10:58 GMT  
		Size: 1.1 KB (1112 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:893c712c491a058aada36756e9f176b6c6c2f3a2b3adf0cd94b896c8198ec3ee`  
		Last Modified: Thu, 23 Nov 2023 01:10:59 GMT  
		Size: 1.9 MB (1937483 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0b8443254952572331df084976853329b69a4348b3c620bb073b5c89fb943b2b`  
		Last Modified: Thu, 23 Nov 2023 01:10:59 GMT  
		Size: 6.5 MB (6507036 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:904bfc5c5c0923edd9be421332402b224bfcd49053bc9b3fae6173383f5cd395`  
		Last Modified: Thu, 23 Nov 2023 01:10:59 GMT  
		Size: 285.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c265216ad3407dbc99903d96423b3a2314bc48cc0118911d150a6bb087ff7d85`  
		Last Modified: Thu, 23 Nov 2023 01:11:00 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:e2fcd32899d09ff06793849927220bea14475e64f085972afbc1f3af74dc209b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.7 KB (21656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf1c2028769aa20a3e529d0f85c8144ba6b099f74cda0dfca2272b7831d2d7a5`

```dockerfile
```

-	Layers:
	-	`sha256:75bab713cb94cdececf4c3879050737e7cb4bbb6206daa071ea001692b53d659`  
		Last Modified: Thu, 23 Nov 2023 01:10:58 GMT  
		Size: 21.7 KB (21656 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:bookworm` - linux; ppc64le

```console
$ docker pull memcached@sha256:d8d106a88d6a15fadf738e59a6dcfc3942f11c7a2d19b7473abce66af7f4d19c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.0 MB (43030916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85da4ca798d44fc951b843ec85c410207ecc3c56af6d1bf7c321c91266d54e1b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:8b22a531b6611a1e63dfc20e4e2931592e2d821bd4b64c4b2810bb9a36640c02 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c570d04e61d8e35a3c8f12179d048d701451f97f9cf2099ea3e3738512dbf062`  
		Last Modified: Tue, 21 Nov 2023 04:28:58 GMT  
		Size: 33.1 MB (33141607 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bcd0cf90a66e23cd3d72b99e7d36129b0e846407a07c30031b0c1e4ba115cd30`  
		Last Modified: Tue, 21 Nov 2023 23:46:47 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5e4166a0e033df4117b469f840c6f5527e87dbd13c582c0b50c182b4bb3ead79`  
		Last Modified: Tue, 21 Nov 2023 23:46:47 GMT  
		Size: 2.7 MB (2698215 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:947b7328e0db59b9870fe9c6d6b7fc4e8a8f1fef3d2a36064fe3d60f5314652d`  
		Last Modified: Tue, 21 Nov 2023 23:46:48 GMT  
		Size: 7.2 MB (7189577 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f011f72796530a711f1de9d543435299d02ed3636e4cd28aee1fa493fbc2bf4`  
		Last Modified: Tue, 21 Nov 2023 23:46:47 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9d27046f19e474530b87e1d0b429e9d85f403210dd3d91bf60d8303fef03af96`  
		Last Modified: Tue, 21 Nov 2023 23:46:48 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:4269af6aa39a29d6dca352659fbf04b7d1bb4e65151e63a3ffcf2749d853597e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3067036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6e9626f30d490d2014e9fbb19add0b6ac0f63c8f4af2082d04750fea7ec35ff`

```dockerfile
```

-	Layers:
	-	`sha256:70759e1722d82b89de5c0d71ba2050ecc9f29d95ee758369044a1fc79026a546`  
		Last Modified: Tue, 21 Nov 2023 23:46:47 GMT  
		Size: 3.0 MB (3045366 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:4f34d59241ff06b2bd0cb8239d96be938e1e13470264898863f307f84ab275b6`  
		Last Modified: Tue, 21 Nov 2023 23:46:47 GMT  
		Size: 21.7 KB (21670 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:bookworm` - linux; s390x

```console
$ docker pull memcached@sha256:312625a69b30a0a0371060c62ec97a621d587675e55a8ced694303d8a7015d30
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.7 MB (35745726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13ebe1c7df28f24c49c7dc749c55574a0a51a84e31dcff380e6caa5441fca944`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:c33fa9fdde73983850798b6eb1cd062e0398109d1d773e6a937fead7475c8efc in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6daa625e5a040476e253e7acd0befa74254a4865ec836d6334a544d82a21d4be`  
		Last Modified: Tue, 21 Nov 2023 05:10:21 GMT  
		Size: 27.5 MB (27512885 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:410539cfd307a2626bf5520b21d1cff0d4c8a336ebea36ed08878d81eca92847`  
		Last Modified: Tue, 21 Nov 2023 15:56:02 GMT  
		Size: 1.1 KB (1109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1ba4cc4f8ba1aa1865931fde910e1ebac220aea9a207eff2f2556bc289a513d3`  
		Last Modified: Tue, 21 Nov 2023 15:56:03 GMT  
		Size: 2.2 MB (2152517 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a47325d5bddeb006ca8a01a6239f747f4ed2c21fd6a28226bdfe46d1981d8962`  
		Last Modified: Tue, 21 Nov 2023 15:56:03 GMT  
		Size: 6.1 MB (6078811 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:32f889bfd6f6b6b2d773abb9f72f86fe0c7469d2a271e5bd209a3eb9b1c61dea`  
		Last Modified: Tue, 21 Nov 2023 15:56:04 GMT  
		Size: 283.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:56ce84d34f650bc21b164be1bb375a2b43c761943b4d06497991ceca18be1009`  
		Last Modified: Tue, 21 Nov 2023 15:56:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:b070f08010996b181adf3fbb4b9004e0d125115bf1380df8c4ddb96a99827218
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3068089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:307228ea8d7a2ce5fee0e1c4c36745e1c0244aa6d316102bde5b655af1bedd24`

```dockerfile
```

-	Layers:
	-	`sha256:640994e8299bce5ed690d70d55a1bc2035868614a169e4cda3391dafb76e9469`  
		Last Modified: Tue, 21 Nov 2023 15:56:03 GMT  
		Size: 3.0 MB (3046321 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:1893b50125646067935dd81f10c259d7b0c3b7cf2f42c81abe2b0f93e45f4250`  
		Last Modified: Tue, 21 Nov 2023 15:56:03 GMT  
		Size: 21.8 KB (21768 bytes)  
		MIME: application/vnd.in-toto+json

## `memcached:latest`

```console
$ docker pull memcached@sha256:e86e92011ac296d084a8f12dc414c01952d86b7711dfc936fbd325f342581631
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 15
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v5
	-	unknown; unknown
	-	linux; arm variant v7
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

### `memcached:latest` - linux; amd64

```console
$ docker pull memcached@sha256:7b0480ab945f960f703af2f286b02a7b620eb4f772e25a2a1374e0c7d32f46de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.8 MB (38815745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f65c7b1a196aa7dfe9520f598f699d5846d6ff0eed117a36ca216302174a1bb1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:d261a6f6921593f1e0b3f472ab1b1822e2c6deb0b369200f0b3370556bfad017 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1f7ce2fa46ab3942feabee654933948821303a5a821789dddab2d8c3df59e227`  
		Last Modified: Tue, 21 Nov 2023 05:25:58 GMT  
		Size: 29.1 MB (29149908 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3606f7d6f784848f3e26f4bc5fae3dde08d65681dbaba232236ac8855cddb881`  
		Last Modified: Tue, 21 Nov 2023 06:19:50 GMT  
		Size: 1.1 KB (1110 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d9e66f47c0a00f0a833454718ca9dc6504f38c45944b5ebf43ccac532dc520b6`  
		Last Modified: Tue, 21 Nov 2023 06:19:50 GMT  
		Size: 2.5 MB (2488339 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:26e0a53c88ab99ad6e23fbb12147cce82e922e4141af56338b4ec01c2ead2b07`  
		Last Modified: Tue, 21 Nov 2023 06:19:50 GMT  
		Size: 7.2 MB (7175988 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:afc0db62c179dab7a3fc4ff6848e150c3315896846d827282affab08909d6e23`  
		Last Modified: Tue, 21 Nov 2023 06:19:50 GMT  
		Size: 281.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7af609a76aa9ed2d446da8865870d0e2b3bff46785783284d956d755a714899b`  
		Last Modified: Tue, 21 Nov 2023 06:19:50 GMT  
		Size: 119.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:latest` - unknown; unknown

```console
$ docker pull memcached@sha256:cb387d9a91a709e6a4193c58df1f36753dbc6c13b9788d741d6dd92ee262ea52
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3078549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3b5853b03b272d3ad2682a093fbc3b2ffd577e3c9fe01f926b5963b333208cd`

```dockerfile
```

-	Layers:
	-	`sha256:9630a5bf61090e535bcf3b7ad1349332584446ea948e10119e025a65fad57d26`  
		Last Modified: Tue, 21 Nov 2023 06:19:50 GMT  
		Size: 3.1 MB (3056780 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:a2ef4829ccc1863c60fdfcf41590326d17bfbdef204a7d37664c92bec494942b`  
		Last Modified: Tue, 21 Nov 2023 06:19:50 GMT  
		Size: 21.8 KB (21769 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:latest` - linux; arm variant v5

```console
$ docker pull memcached@sha256:c5fbea0a198cb4ae068e4761d5d1abab499e4ebc80275be6b7d797196cf3db54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34849973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b72ee44b42eca798309f6aa48ed2af9feca23c5eb64e5be38fa2536110b12ce`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:1ae8e5ac45b11d01083680b765e1fcfef9f7938f89d6f424572126fa946d8cdf in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f476aef5b6e1122850e68c81ef06fc2df17e968961b060483b4d2fb33018aae3`  
		Last Modified: Tue, 21 Nov 2023 05:03:55 GMT  
		Size: 26.9 MB (26922153 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:26dadbdb945a22546f6b2c171d0bededff72d7598719ab8f3877f67129e21730`  
		Last Modified: Tue, 21 Nov 2023 16:18:13 GMT  
		Size: 1.1 KB (1109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:44f46f0b8b7c11e6cd53e82541f819c66da246b152155fff8ce762f98c25219f`  
		Last Modified: Tue, 21 Nov 2023 16:18:14 GMT  
		Size: 2.1 MB (2089268 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:639e86d18160b654876d404a88b437cea26de29151122dfe8cbed9947f1b7b10`  
		Last Modified: Tue, 21 Nov 2023 16:18:14 GMT  
		Size: 5.8 MB (5837040 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7b963217677ca57533744aee2b331f059fbb6882f27abe2cc976462604e7b560`  
		Last Modified: Tue, 21 Nov 2023 16:18:15 GMT  
		Size: 283.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ac3a1fa5d4b6c48ea8ce4c375a197047f1480fbfb37c316b7d730d026d261219`  
		Last Modified: Tue, 21 Nov 2023 16:18:15 GMT  
		Size: 120.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:latest` - unknown; unknown

```console
$ docker pull memcached@sha256:cd008d8c4d507d73b5f0153ed880e81e86a53741b480bbf6b1d318510e83a288
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.7 KB (21695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85e0f40569066724c087be3d901d5c5d984043271b56a33dec281e36032017f0`

```dockerfile
```

-	Layers:
	-	`sha256:2eff64dde44b4be85375aed8309f5d20476ca81876607d799b56c31addee0cb8`  
		Last Modified: Tue, 21 Nov 2023 16:18:13 GMT  
		Size: 21.7 KB (21695 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:latest` - linux; arm variant v7

```console
$ docker pull memcached@sha256:2841be0a36134563966c09a6ed68b21053d20342ec8736cf92763c28077ead43
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28094215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cf74ffa940dd93988fc0beb6698c5796563c82a40b7dd668153969f64d2e6ca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 09 Feb 2023 06:12:09 GMT
ADD file:5f1a343224e8486690bd90dd1e50c8d84b3d770c51bb6829544e5cf650c0419c in / 
# Thu, 09 Feb 2023 06:12:10 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 07:52:31 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Thu, 09 Feb 2023 07:52:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:52:35 GMT
ENV MEMCACHED_VERSION=1.6.18
# Thu, 09 Feb 2023 07:52:35 GMT
ENV MEMCACHED_SHA1=be16909bb75ab972ee5fe438312501de01c4725a
# Thu, 09 Feb 2023 07:55:44 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Thu, 09 Feb 2023 07:55:44 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 09 Feb 2023 07:55:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 09 Feb 2023 07:55:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Feb 2023 07:55:44 GMT
USER memcache
# Thu, 09 Feb 2023 07:55:45 GMT
EXPOSE 11211
# Thu, 09 Feb 2023 07:55:45 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:e7318f6106ad75d7d482ae9dddf4d927b0872ef3ddb6e1330aa691fc8d17279e`  
		Last Modified: Thu, 09 Feb 2023 06:19:19 GMT  
		Size: 26.6 MB (26577666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de49d9d72daf1680b5f1b9532dd2eb0162829f36c8db9669935462636fbf99d9`  
		Last Modified: Thu, 09 Feb 2023 08:06:11 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0beac9d5bcac946f8c54c72b8a9c136914b1aa7a5fe2b8c3df4c7d8858ea6559`  
		Last Modified: Thu, 09 Feb 2023 08:06:11 GMT  
		Size: 312.1 KB (312088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4c9e5a265394e4c0f357779e6195a4e82d767a3691a0e77d427e56651c3e54a`  
		Last Modified: Thu, 09 Feb 2023 08:06:11 GMT  
		Size: 1.2 MB (1199163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ea82ad892fe1ae8623d84e32c8c027087cda8aa49e40d4546ed6942e471c60`  
		Last Modified: Thu, 09 Feb 2023 08:06:11 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2ae3bcdc0d114ba49a67df022b6f7215fc87f1f50e64939fcfbbec4eaadee5`  
		Last Modified: Thu, 09 Feb 2023 08:06:11 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:dd556de8d6e6b81c51ba9120fa924fbb7fae427468d82db9f2b3db124f9ac0b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.7 MB (37711361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f05ec0c73b4afc866c99864d86b1c66deb5d8bda84bf2cc78e1e763e0ed6a263`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:869c7d0747a17c53715581a2e862992eb8516c7f45f167821dfa80966a4870d1 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2c6d21737d8318aa15c4cc838475029a5efc36c0429e3d8da80d97d0b96d9aaf`  
		Last Modified: Tue, 21 Nov 2023 06:30:30 GMT  
		Size: 29.2 MB (29179277 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fa3a18531b093eb1a543ad01b2a54d4692f59bba8d49ea9793b3ff09e528cd93`  
		Last Modified: Wed, 22 Nov 2023 11:50:41 GMT  
		Size: 1.1 KB (1109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:395fd5be77a2adb2c1b863f9ba2c664074aacb120f379bbb0f45cda74cc09cf4`  
		Last Modified: Wed, 22 Nov 2023 11:50:41 GMT  
		Size: 2.3 MB (2345987 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1dbcb5e891e054cd85f29e62fff856117d8cb919630be0c7473b520168b8c261`  
		Last Modified: Wed, 22 Nov 2023 11:50:41 GMT  
		Size: 6.2 MB (6184583 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2654df736cfb30e0097cca6a637ae794285396f6e2b87031636c8056b66baed0`  
		Last Modified: Wed, 22 Nov 2023 11:50:41 GMT  
		Size: 283.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e54ea6c3f7f45d9ed3f003bcf9e0a717c342daae58d330fef355e712d15b732`  
		Last Modified: Wed, 22 Nov 2023 11:50:42 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:latest` - unknown; unknown

```console
$ docker pull memcached@sha256:2b5053d245e0312a77b7827553fcf09a6b19a0bf825a7016a4125713ad0d814f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3053591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e04bc647daea7fbb746cd418f19740162bd910826c366cdcc3549c3888ad5e1b`

```dockerfile
```

-	Layers:
	-	`sha256:f04377bb8fcfc3a24c1a36aa0bdf9b2d9272b7a60e82a88b66e2bb0645703c07`  
		Last Modified: Wed, 22 Nov 2023 11:50:41 GMT  
		Size: 3.0 MB (3031971 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:601cddda9e5f7f3a82cfc305051ac3c1fc5f65a9722e4dbe06363cc8b6ea68be`  
		Last Modified: Wed, 22 Nov 2023 11:50:41 GMT  
		Size: 21.6 KB (21620 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:latest` - linux; 386

```console
$ docker pull memcached@sha256:fa9dba8086765d68f2feecfc2ac08fb29c019597d09943bb480227e6cba87666
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.3 MB (39294993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93047050e75b6d4d64adb8a7c8f68cb118bad27ca9dc772120e251b174752cf9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:0c94521fdd9c0a4fdeeb9aad23e68cd053fba0dcd7c3af550aefa79377816e31 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:98bdfce9af831c2a0d0bfcca812d0039cd1666986550f552b4b4c625bd5aa31c`  
		Last Modified: Wed, 01 Nov 2023 00:43:26 GMT  
		Size: 30.2 MB (30164042 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1b647d4b10cf20ac5807101c7d0380701be684aa82f5c01ec41f674b5ef23d42`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 1.1 KB (1109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b61c058003459de4911c2901b2d799b03de754a1b9e64ffbe21a04992e962e62`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 2.5 MB (2492501 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:810b6db64df2fcc8f76941cdac75093cf35bd72ac3cd1fa5eb664e74c1f67cd8`  
		Last Modified: Wed, 01 Nov 2023 01:06:50 GMT  
		Size: 6.6 MB (6636937 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dbb899942df4149bd5fae8bac6e295285ec80f82d621f2b29c931ee348491cfb`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 282.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4a8530160ab232c37c0ddcbf5e3a731d835d378d1382843957f6c2a73b2b5be6`  
		Last Modified: Wed, 01 Nov 2023 01:06:50 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:latest` - unknown; unknown

```console
$ docker pull memcached@sha256:dd7ce9519c31365127142232df2ed0b285e9acc03cd77c23c838bf932165def8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 KB (21498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eef82c92e07c11a92c337806d01cfb1c6cdc7a16608dcf304a38de34d2ef1dbb`

```dockerfile
```

-	Layers:
	-	`sha256:c0d9dd22513f8d3e791e1796d7ef1906e57c798c92dd35d0be9cf2eaecec5954`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 21.5 KB (21498 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:latest` - linux; mips64le

```console
$ docker pull memcached@sha256:a7c198db1b0856aff4b1514137e473ea30bce2ef22f0192cfdce7e2e44f2a863
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.6 MB (37588022 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1654ec4454e597d7e7cb6a7d97e98208de241a3dfafc5e0532b9561eac91f013`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:e093749192323dc72b60a8440ddba26c415586f618b5e107fa264ba5eb2ca7ba in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:ebdff2138fee4a3ec27560ab1353dc51c12c2608ff721f5db3d24104872b702a`  
		Last Modified: Tue, 21 Nov 2023 04:20:35 GMT  
		Size: 29.1 MB (29141984 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:50b1ffce24cec457fe1757715d60bd669145e5babade7c57143c4b665a55389e`  
		Last Modified: Thu, 23 Nov 2023 01:10:58 GMT  
		Size: 1.1 KB (1112 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:893c712c491a058aada36756e9f176b6c6c2f3a2b3adf0cd94b896c8198ec3ee`  
		Last Modified: Thu, 23 Nov 2023 01:10:59 GMT  
		Size: 1.9 MB (1937483 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0b8443254952572331df084976853329b69a4348b3c620bb073b5c89fb943b2b`  
		Last Modified: Thu, 23 Nov 2023 01:10:59 GMT  
		Size: 6.5 MB (6507036 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:904bfc5c5c0923edd9be421332402b224bfcd49053bc9b3fae6173383f5cd395`  
		Last Modified: Thu, 23 Nov 2023 01:10:59 GMT  
		Size: 285.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c265216ad3407dbc99903d96423b3a2314bc48cc0118911d150a6bb087ff7d85`  
		Last Modified: Thu, 23 Nov 2023 01:11:00 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:latest` - unknown; unknown

```console
$ docker pull memcached@sha256:e2fcd32899d09ff06793849927220bea14475e64f085972afbc1f3af74dc209b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.7 KB (21656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf1c2028769aa20a3e529d0f85c8144ba6b099f74cda0dfca2272b7831d2d7a5`

```dockerfile
```

-	Layers:
	-	`sha256:75bab713cb94cdececf4c3879050737e7cb4bbb6206daa071ea001692b53d659`  
		Last Modified: Thu, 23 Nov 2023 01:10:58 GMT  
		Size: 21.7 KB (21656 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:latest` - linux; ppc64le

```console
$ docker pull memcached@sha256:d8d106a88d6a15fadf738e59a6dcfc3942f11c7a2d19b7473abce66af7f4d19c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.0 MB (43030916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85da4ca798d44fc951b843ec85c410207ecc3c56af6d1bf7c321c91266d54e1b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:8b22a531b6611a1e63dfc20e4e2931592e2d821bd4b64c4b2810bb9a36640c02 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c570d04e61d8e35a3c8f12179d048d701451f97f9cf2099ea3e3738512dbf062`  
		Last Modified: Tue, 21 Nov 2023 04:28:58 GMT  
		Size: 33.1 MB (33141607 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bcd0cf90a66e23cd3d72b99e7d36129b0e846407a07c30031b0c1e4ba115cd30`  
		Last Modified: Tue, 21 Nov 2023 23:46:47 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5e4166a0e033df4117b469f840c6f5527e87dbd13c582c0b50c182b4bb3ead79`  
		Last Modified: Tue, 21 Nov 2023 23:46:47 GMT  
		Size: 2.7 MB (2698215 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:947b7328e0db59b9870fe9c6d6b7fc4e8a8f1fef3d2a36064fe3d60f5314652d`  
		Last Modified: Tue, 21 Nov 2023 23:46:48 GMT  
		Size: 7.2 MB (7189577 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f011f72796530a711f1de9d543435299d02ed3636e4cd28aee1fa493fbc2bf4`  
		Last Modified: Tue, 21 Nov 2023 23:46:47 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9d27046f19e474530b87e1d0b429e9d85f403210dd3d91bf60d8303fef03af96`  
		Last Modified: Tue, 21 Nov 2023 23:46:48 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:latest` - unknown; unknown

```console
$ docker pull memcached@sha256:4269af6aa39a29d6dca352659fbf04b7d1bb4e65151e63a3ffcf2749d853597e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3067036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6e9626f30d490d2014e9fbb19add0b6ac0f63c8f4af2082d04750fea7ec35ff`

```dockerfile
```

-	Layers:
	-	`sha256:70759e1722d82b89de5c0d71ba2050ecc9f29d95ee758369044a1fc79026a546`  
		Last Modified: Tue, 21 Nov 2023 23:46:47 GMT  
		Size: 3.0 MB (3045366 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:4f34d59241ff06b2bd0cb8239d96be938e1e13470264898863f307f84ab275b6`  
		Last Modified: Tue, 21 Nov 2023 23:46:47 GMT  
		Size: 21.7 KB (21670 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:latest` - linux; s390x

```console
$ docker pull memcached@sha256:312625a69b30a0a0371060c62ec97a621d587675e55a8ced694303d8a7015d30
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.7 MB (35745726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13ebe1c7df28f24c49c7dc749c55574a0a51a84e31dcff380e6caa5441fca944`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:c33fa9fdde73983850798b6eb1cd062e0398109d1d773e6a937fead7475c8efc in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6daa625e5a040476e253e7acd0befa74254a4865ec836d6334a544d82a21d4be`  
		Last Modified: Tue, 21 Nov 2023 05:10:21 GMT  
		Size: 27.5 MB (27512885 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:410539cfd307a2626bf5520b21d1cff0d4c8a336ebea36ed08878d81eca92847`  
		Last Modified: Tue, 21 Nov 2023 15:56:02 GMT  
		Size: 1.1 KB (1109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1ba4cc4f8ba1aa1865931fde910e1ebac220aea9a207eff2f2556bc289a513d3`  
		Last Modified: Tue, 21 Nov 2023 15:56:03 GMT  
		Size: 2.2 MB (2152517 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a47325d5bddeb006ca8a01a6239f747f4ed2c21fd6a28226bdfe46d1981d8962`  
		Last Modified: Tue, 21 Nov 2023 15:56:03 GMT  
		Size: 6.1 MB (6078811 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:32f889bfd6f6b6b2d773abb9f72f86fe0c7469d2a271e5bd209a3eb9b1c61dea`  
		Last Modified: Tue, 21 Nov 2023 15:56:04 GMT  
		Size: 283.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:56ce84d34f650bc21b164be1bb375a2b43c761943b4d06497991ceca18be1009`  
		Last Modified: Tue, 21 Nov 2023 15:56:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:latest` - unknown; unknown

```console
$ docker pull memcached@sha256:b070f08010996b181adf3fbb4b9004e0d125115bf1380df8c4ddb96a99827218
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3068089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:307228ea8d7a2ce5fee0e1c4c36745e1c0244aa6d316102bde5b655af1bedd24`

```dockerfile
```

-	Layers:
	-	`sha256:640994e8299bce5ed690d70d55a1bc2035868614a169e4cda3391dafb76e9469`  
		Last Modified: Tue, 21 Nov 2023 15:56:03 GMT  
		Size: 3.0 MB (3046321 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:1893b50125646067935dd81f10c259d7b0c3b7cf2f42c81abe2b0f93e45f4250`  
		Last Modified: Tue, 21 Nov 2023 15:56:03 GMT  
		Size: 21.8 KB (21768 bytes)  
		MIME: application/vnd.in-toto+json
