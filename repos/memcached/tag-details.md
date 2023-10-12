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
-	[`memcached:1.6.21`](#memcached1621)
-	[`memcached:1.6.21-alpine`](#memcached1621-alpine)
-	[`memcached:1.6.21-alpine3.18`](#memcached1621-alpine318)
-	[`memcached:1.6.21-bookworm`](#memcached1621-bookworm)
-	[`memcached:alpine`](#memcachedalpine)
-	[`memcached:alpine3.18`](#memcachedalpine318)
-	[`memcached:bookworm`](#memcachedbookworm)
-	[`memcached:latest`](#memcachedlatest)

## `memcached:1`

```console
$ docker pull memcached@sha256:392f01c0e85fa9aeb0308a0c3b43b1ecde43203929c1d56d87ac469fd3d3e0a6
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
$ docker pull memcached@sha256:8af51889f0f774a00f36624e58faac309c258eafb8054c6abc6fbbb56c78d0a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.8 MB (38811465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fa23f6ace109fad9223ea2db53f79afa8b91b14051c61305f82bc2c781a788c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:55ad846fa191e603f48090eae0e4a7149c4066b94406593ec1898ad2c3347937 in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a378f10b321842c3042cdeff4f6997f34f4cb21f2eff27704b7f6193ab7b5fea`  
		Last Modified: Wed, 11 Oct 2023 18:39:34 GMT  
		Size: 29.1 MB (29149874 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e68aaf702a54364b3f216204ad2725f5b416fe496294086899b821bb5133552d`  
		Last Modified: Wed, 11 Oct 2023 20:07:27 GMT  
		Size: 1.1 KB (1110 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0fb853802e1447e9b1dbe3e8a86f27a5691286127397adf8d52f943d16b80042`  
		Last Modified: Wed, 11 Oct 2023 20:07:27 GMT  
		Size: 2.5 MB (2488274 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fcc9694d882f053fcf2e7bb33709dcb86eef6c29c3187c190ad93852af7a50f2`  
		Last Modified: Wed, 11 Oct 2023 20:07:28 GMT  
		Size: 7.2 MB (7171802 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fde136907f7040bd6126a5b2c0bca844fef33e2fc804c1f135e99393869cce4c`  
		Last Modified: Wed, 11 Oct 2023 20:07:27 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c121d0db5ccb2988b1fc0c76ce60a2e78309d77b264adf99e815e1ecf2c6a957`  
		Last Modified: Wed, 11 Oct 2023 20:07:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1` - unknown; unknown

```console
$ docker pull memcached@sha256:888d3aaaddc944acb247f0e42586c8c8a7f8c3262166ee89ceda0dbe3998cafa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2911211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06530a2f7a54ba7d86fc6cee0da9a46ea1aea89dc4beecbee6d54ed8eee82dd9`

```dockerfile
```

-	Layers:
	-	`sha256:7bbbdfb4ba86ed51b46d2fb83bf8cf4e095da6d5c9dd89697a3488dd392414d7`  
		Last Modified: Wed, 11 Oct 2023 20:07:27 GMT  
		Size: 2.9 MB (2889442 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:6fe7a995830937695f7110928df7e791673ab04015add73a1f2e9ec661bbc60f`  
		Last Modified: Wed, 11 Oct 2023 20:07:27 GMT  
		Size: 21.8 KB (21769 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1` - linux; arm variant v5

```console
$ docker pull memcached@sha256:a6919fc9976aa2c291f194860f40fcc9499d33cbd2592af9087e5d64b7930602
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34846023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5222dddac963b84d55ef902d40fa3f949ee73caac9614ca77c1f4a81ef009c6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:8c43adb3245fc6f2b10aa5a86c850db5dcf3515eaf7e46630922fe21f806bd2a in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:904e6393ef1ee28b37171369eb4f7cb04714631c711799819fccb83886bd212b`  
		Last Modified: Wed, 11 Oct 2023 17:40:47 GMT  
		Size: 26.9 MB (26922150 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f0569355cb85b70d6a614ea9604289ce8e724f0f9ff4d1d8a12afc24c4c9ad1f`  
		Last Modified: Thu, 12 Oct 2023 08:32:05 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6939032c8ff0687b012a85d3411c702266b934a677f96eb521658b44f5b4a8c0`  
		Last Modified: Thu, 12 Oct 2023 08:32:06 GMT  
		Size: 2.1 MB (2089182 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8e8a2a7338b5cacc7b6e4e3db2359eebb1936b0b14266d5bad0dfcc21c9becff`  
		Last Modified: Thu, 12 Oct 2023 08:32:06 GMT  
		Size: 5.8 MB (5833176 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:19f35a8116fe7e124bee612b2ac511694077a1f35f76ed056903987ab4921e34`  
		Last Modified: Thu, 12 Oct 2023 08:32:06 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a43775be6dfac6c255e35b164eacd7328df241f33f9245206a8eaf481062ccbc`  
		Last Modified: Thu, 12 Oct 2023 08:32:07 GMT  
		Size: 120.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1` - unknown; unknown

```console
$ docker pull memcached@sha256:f1276a05a4db6e8b7bb9d8374d480b85a79f1b92d4e7475c65e247bf1427200c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.7 KB (21695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe67b683a818ed7c22a49086ec4f22e53c6efa9040becea46adb07f550dae564`

```dockerfile
```

-	Layers:
	-	`sha256:12ecc330d2059d33dc7a7c518e7be06804f5fcadafdc8e2db030631f5c92b326`  
		Last Modified: Thu, 12 Oct 2023 08:32:05 GMT  
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
$ docker pull memcached@sha256:0c25b3c626a396c236dcf08792c850a178482c24e0c9dab0e784783178d10c13
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.4 MB (43442272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1595a8aa58bfc22ba6e995a58c63ea8b660aa8a9b10c57ab0cb8552d94080218`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:ec1a6e0aedd76c8fdc8544775f8b553f58950e9435f5cfe919f39374e222cfbb in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:e886f0f47ef56fcadb6ecaf2116056bbdb273e0afe07ed034498b198d386c04e`  
		Last Modified: Wed, 20 Sep 2023 02:47:36 GMT  
		Size: 29.2 MB (29157221 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7e25b15fcaee53caa22717c5b0b52fabf2480b0244a84530fca4c1edbb812044`  
		Last Modified: Tue, 03 Oct 2023 19:00:54 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:72fc5c44d6b752d2c2534f97f12ef44f915803ec4e564d7c9eb90d9d7bda2297`  
		Last Modified: Tue, 03 Oct 2023 19:00:54 GMT  
		Size: 2.3 MB (2343087 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7ba30437e42c2aebda3182e43b83b90012dd19e31adb9dc25bb3b714385cdefe`  
		Last Modified: Tue, 03 Oct 2023 19:00:55 GMT  
		Size: 11.9 MB (11940448 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:70abb5efa4268d01b1dfe9f6775f8f85a7fe395141dcc28909aa52ea6b741971`  
		Last Modified: Tue, 03 Oct 2023 19:00:54 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5a87a9f60806e352855b340f2c0c3610b8053006f0f542077c3add7e70782663`  
		Last Modified: Tue, 03 Oct 2023 19:00:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1` - unknown; unknown

```console
$ docker pull memcached@sha256:7a900749c7d177577d906a5d402b4a008b95ae3571e9de24b4f04060e8650d5d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2890735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:711e633b20942471e455d3210316a79109ffda2a13cb38f46bd9ab2d27c758ae`

```dockerfile
```

-	Layers:
	-	`sha256:6c4c4a32fc3b330e635796951e46bf9e6ed753212798e75baddd3a84e752de8c`  
		Last Modified: Tue, 03 Oct 2023 19:00:54 GMT  
		Size: 2.9 MB (2869112 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:d0ceb647ed388f03f95faf34bc93c1489afde267801855f46cfca84fca538c5a`  
		Last Modified: Tue, 03 Oct 2023 19:00:54 GMT  
		Size: 21.6 KB (21623 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1` - linux; 386

```console
$ docker pull memcached@sha256:dbf6fdd168abcb8b6fd831277bea0213784e54cdb824756684dd3b5337c42c65
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.6 MB (44649134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25680867a5df0eb88860f59d7855c9d7f3862a44283c1e59d608f9dbecff348b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:efe81f7066129aa6293627bfe4ea78b957897ba5ede951970156fccf1dbcde88 in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6ac07f93e07a1bad4555e13bd8efd06169988669fc88df95f4bf296a2b44523d`  
		Last Modified: Wed, 20 Sep 2023 00:46:48 GMT  
		Size: 30.1 MB (30141894 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:797b4215eddcf948eec0f19132f85ec1b0f3af264399e78d860bece37acc4888`  
		Last Modified: Tue, 03 Oct 2023 19:01:51 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3c78c0b20e6791912325d174e98f60d4f783c2f013f52ff3835892444d3a15d7`  
		Last Modified: Tue, 03 Oct 2023 19:01:51 GMT  
		Size: 2.5 MB (2490464 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c91bf1cea723f722413107daa57ab51060ab36a5f78fe8447568aa35be54fca5`  
		Last Modified: Tue, 03 Oct 2023 19:01:52 GMT  
		Size: 12.0 MB (12015261 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:07f7206e609641792c84dfac85e3e6df0602c4ca8d572353a8768ff0619fe328`  
		Last Modified: Tue, 03 Oct 2023 19:01:51 GMT  
		Size: 283.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7aac14495f4a088e0e208638d0b36b0b5ff0cf945aaf24c011ef08ca799279a9`  
		Last Modified: Tue, 03 Oct 2023 19:01:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1` - unknown; unknown

```console
$ docker pull memcached@sha256:16c8db3d95a2df8fae160a3942ff033ebb3bf6d9fe8df1643eb22c82e9402357
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 KB (21502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03bc49cf22d3ede52afc78d429b09999ba28174660a5e1b41fdb0f9d3a47067c`

```dockerfile
```

-	Layers:
	-	`sha256:890c3f7af1536aa0821f27c4ba142e022ba0c892f1310b4d82a9cc3a74717139`  
		Last Modified: Tue, 03 Oct 2023 19:01:51 GMT  
		Size: 21.5 KB (21502 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1` - linux; mips64le

```console
$ docker pull memcached@sha256:575825bdbf62fc255547394ef491710ba88f0be3ca735eaf246ece06f13363ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.4 MB (43398233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e3f951153522f4d9719c37a9862412f3e29e487d11322c5ff7a009cf8becca1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:850547a08e38ebc5a3659df86e70039a8d9828ae26ae485b077c98a959248dcb in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:0f581c6294fe7421dfee024e2c7dddd73ef3fbd7ff23b05bc3c1bf9f50885e85`  
		Last Modified: Wed, 20 Sep 2023 03:20:59 GMT  
		Size: 29.1 MB (29121674 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:15e25af5488ea4ad0df132fa2c22a282c1a17ad1460cdb25fe5939e03a753528`  
		Last Modified: Tue, 03 Oct 2023 19:04:40 GMT  
		Size: 1.1 KB (1113 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:19a5f416c9bf283212262e33fe8529d0ff3917fcee1e8ca9fb058170fd528211`  
		Last Modified: Tue, 03 Oct 2023 19:04:41 GMT  
		Size: 1.9 MB (1934931 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:05862af95003d85f9a1b5696dfb3588bdd8e34c74f067d845b722d70edfc679f`  
		Last Modified: Tue, 03 Oct 2023 19:04:41 GMT  
		Size: 12.3 MB (12340111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e8aae13855c46b73d2506b2d91036f6f0b4bc63b7d7ec12ecc63fd672c64c0f7`  
		Last Modified: Tue, 03 Oct 2023 19:04:40 GMT  
		Size: 282.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0709f88ce6a011ea45fd41c091ee6fcf4baa0610e0591a9fe0d10626eaf9475f`  
		Last Modified: Tue, 03 Oct 2023 19:04:41 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1` - unknown; unknown

```console
$ docker pull memcached@sha256:269b3e28059bf711ac45886388e91fa405b8a1e0ca1a114acefc997bbdad6d05
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 KB (21491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1059a2662b538952006866f53463fcea773b5e090eaead3a4ad49f4d0a656ae5`

```dockerfile
```

-	Layers:
	-	`sha256:e1052b07541ae6e041e59834c527075b62df62a33f7a9b9e96fda4b6237e83df`  
		Last Modified: Tue, 03 Oct 2023 19:04:40 GMT  
		Size: 21.5 KB (21491 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1` - linux; ppc64le

```console
$ docker pull memcached@sha256:532cf0a6053275c508a0503017b4f52ce356a64aba047eb2316bdcaca35bbc9a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49635445 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:111f6d9d894ab95e36b94efa3dad4a4c9d0def1fa3af71a4a0e57e907a2b4986`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:9a37b479e68a0d18babbef8dd04d09a0e6844a0080876d14144a34bfd9d0897a in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:696a66e961f2033dcf69b003ad7faf28ed2248da58efa1c08a9d496739a8eeeb`  
		Last Modified: Wed, 20 Sep 2023 08:49:51 GMT  
		Size: 33.1 MB (33119461 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ba4c0c64bfd7ea845d20c793ede5957878785e4bb16e2e81a3e1ed5cd0d7ca0e`  
		Last Modified: Tue, 03 Oct 2023 19:02:08 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8a7ae673337cbb772a0ccc237ce4009a7dd88e4fed23861c9ea6382e93a6685b`  
		Last Modified: Tue, 03 Oct 2023 19:02:09 GMT  
		Size: 2.7 MB (2694930 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:766c713a6dbc39908803d95aa7556e0a571349c941bddb8f694b3f36030e0c3c`  
		Last Modified: Tue, 03 Oct 2023 19:02:10 GMT  
		Size: 13.8 MB (13819538 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:75734e09fa81ca91f8bdd1481c8f88f95ea9ba7b0f24ab82d0aee2026a5d6474`  
		Last Modified: Tue, 03 Oct 2023 19:02:09 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f46fc74a04a0607353cbc3ace76b49b44029af75080fa56fec872060d38feed2`  
		Last Modified: Tue, 03 Oct 2023 19:02:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1` - unknown; unknown

```console
$ docker pull memcached@sha256:d73c6167b49dd216e6395e8720af5bd26884a25473d1eb80ee31d1e4b170a914
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2914816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48964548656eeecac440cb41e4f3f474f861d384c569653e582e3d508b04f6e5`

```dockerfile
```

-	Layers:
	-	`sha256:4e89c387c1399e94faaaf407614d23c90aa3104b5773f87d8cb4fe4b20312f8e`  
		Last Modified: Tue, 03 Oct 2023 19:02:09 GMT  
		Size: 2.9 MB (2893143 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:fb96286b26618de71f0df13dfc89225bc855d6802341b4032f0fb4161cb4a52e`  
		Last Modified: Tue, 03 Oct 2023 19:02:08 GMT  
		Size: 21.7 KB (21673 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1` - linux; s390x

```console
$ docker pull memcached@sha256:42a17150fd8b17aff6910890bbab808eab97e6f9d0f60003e75fac6ddd2b0bcf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40575835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:956090eeead5cd8ec7753b439eb43ddf3b2c5cd93edea3d7ce5bcdd168ec7588`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:6ed982ad3e8566d63315a27a81b33069910952aef4b2d3e0b607bd2caeac7ca4 in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:26dcff366e33abcf08b812052a4c12496aa406aa267655e984aa7a84ca254cd8`  
		Last Modified: Wed, 20 Sep 2023 02:59:47 GMT  
		Size: 27.5 MB (27489966 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:04795616cce62da1faee69d189f2f4863a3818651e9f54e7552be41e35752766`  
		Last Modified: Tue, 03 Oct 2023 19:01:27 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cbacb720efba986e695a3270bc384924abb78c413d1c4793cd388fbab1da828b`  
		Last Modified: Tue, 03 Oct 2023 19:01:27 GMT  
		Size: 2.2 MB (2150908 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:07a927de051febdc6284e8ec146cbc267ffdd1049fadf2bc35639f53b72b7862`  
		Last Modified: Tue, 03 Oct 2023 19:01:28 GMT  
		Size: 10.9 MB (10933444 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5a2703a37bdc4f133106c52c5a040d30708c01a79aa0d1714bcba3b42105692e`  
		Last Modified: Tue, 03 Oct 2023 19:01:28 GMT  
		Size: 285.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c0a860b98e7d941cd44043f66c4cc9d2a540ab3b8cb9aa15123102865599e0c7`  
		Last Modified: Tue, 03 Oct 2023 19:01:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1` - unknown; unknown

```console
$ docker pull memcached@sha256:029d2884ff06e1b3673d9a7998c7299cc3da7ed18f46b344e13c14867574bae4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2897027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e57e1f9eb901fd307d1e2dd72b5606ba1f6f0ef82c31c01041513ed98e33b55`

```dockerfile
```

-	Layers:
	-	`sha256:13af4843cce0c7df5b25984623ef20fe08955ca99bbc64f5056c4d1bb2062f13`  
		Last Modified: Tue, 03 Oct 2023 19:01:27 GMT  
		Size: 2.9 MB (2875422 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:2e615a884e0baa9f5e54063b8983b99c841ac4fd854bf56780c1184d51637b1d`  
		Last Modified: Tue, 03 Oct 2023 19:01:27 GMT  
		Size: 21.6 KB (21605 bytes)  
		MIME: application/vnd.in-toto+json

## `memcached:1-alpine`

```console
$ docker pull memcached@sha256:535282ea08869aedc9bd20cbd714f07a27019c8b1e3aa64aa7321c96fb747844
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
$ docker pull memcached@sha256:27fe55ab0ecba9a8d3ddd67b823da4f1727d10eb46d36ab5af7e693421ebdb4f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4466251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3e0c0ff5c009f0e410e2fc6d29099b24315b4246c64cebae8068e86c22ba8a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["/bin/sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN apk add --no-cache libsasl # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3f9365fb2eebc56ba7006618c6ee8cde403af71bb4777c9b2b1c6ddcc107ee55`  
		Last Modified: Tue, 03 Oct 2023 19:01:12 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ec2c14990e92682477b554b5ccec603b864340a582d8ac4ab7becf52c09e9459`  
		Last Modified: Tue, 03 Oct 2023 19:01:12 GMT  
		Size: 108.0 KB (108015 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a0e994f33a8fb2b64e76f431cb35d0f0f92f0830352e44c589d8770bedfe96c3`  
		Last Modified: Tue, 03 Oct 2023 19:01:13 GMT  
		Size: 954.6 KB (954626 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:69c0dd1ede28d4dfdee1e54dc519270184463fa8812e781a930c0301b851c327`  
		Last Modified: Tue, 03 Oct 2023 19:01:12 GMT  
		Size: 277.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c9a4377466b783eeeab01987a823353e5cfbc2a5f02d632db14c654decf3ec5e`  
		Last Modified: Tue, 03 Oct 2023 19:01:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-alpine` - unknown; unknown

```console
$ docker pull memcached@sha256:6ebfa6199008800194514397c12c233ea35c27ee5d22bea93fc978228a9f98f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.2 KB (95222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc3627763f4a9bb22db274ce8453a9d0146e88c0f4e0624f69059e5a9a69ec31`

```dockerfile
```

-	Layers:
	-	`sha256:7e739eda7910762ab0244ff165c2ff431bf4f10a39730614a8fca28a9a91b97d`  
		Last Modified: Tue, 03 Oct 2023 19:01:12 GMT  
		Size: 76.3 KB (76268 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:a04f216271188784dc836fa4905c7d5fbcfb49537cf5cfb5fe5b0229694cf12c`  
		Last Modified: Tue, 03 Oct 2023 19:01:12 GMT  
		Size: 19.0 KB (18954 bytes)  
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
$ docker pull memcached@sha256:1152b588a2cd7e90f0d7ae86fe3ce262e47c50c62642b5714b0019cef7779a00
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4401705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31bcc2b506321f6395c1d68cfc40f7391530051e5862186db1d5875e2c2803be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["/bin/sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN apk add --no-cache libsasl # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a8a999d5f4398538233c73f556a07cf646c7600543368cbc84b997cd76545de1`  
		Last Modified: Tue, 03 Oct 2023 19:03:35 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e035f8f759de7f5b35527c5cc46cd4132a10e0a501e022fbde2fedcf47fdd684`  
		Last Modified: Tue, 03 Oct 2023 19:03:35 GMT  
		Size: 124.1 KB (124080 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:585097acb28da9160246ad53fa72c119ac6e97a2852f420712485b66d6ed808a`  
		Last Modified: Tue, 03 Oct 2023 19:03:36 GMT  
		Size: 944.1 KB (944147 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:802f5f839e31fd8f8dd89ec2421af9fa8227dd43d5ca883f44d9ff2962cd0848`  
		Last Modified: Tue, 03 Oct 2023 19:03:35 GMT  
		Size: 281.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:65fc6300aa54fcd82f813153e3a5a880a2dca2a26edc3f7f907fe395a01a5474`  
		Last Modified: Tue, 03 Oct 2023 19:03:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-alpine` - unknown; unknown

```console
$ docker pull memcached@sha256:5b2e4db4700ecd5765dd85cbc125a24968150122eb9f8181949dc39310085671
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.1 KB (95095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e78ca75a52728eb7207c54b73b899cb6919fd230b814373dc1612765d95bcc0c`

```dockerfile
```

-	Layers:
	-	`sha256:36799473bd1d28916d0df4c2af578542c27261dcc2dbba98964d2d7e956bd73f`  
		Last Modified: Tue, 03 Oct 2023 19:03:35 GMT  
		Size: 76.3 KB (76289 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:c088a7e985146394427f4d604d17a54445f5934b07e790774b7472540d932737`  
		Last Modified: Tue, 03 Oct 2023 19:03:35 GMT  
		Size: 18.8 KB (18806 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1-alpine` - linux; 386

```console
$ docker pull memcached@sha256:8b880914dfffd537639b55f5f49cf6c6e9f0773891eb922685e0ce94ccde66b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4283801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f38744e29d4692d1345bf5101db090800c52e9ae211735a610dd8e848ca426d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:8402753f294e403e92353bd65c86a6428c960be5116c0a15484b663a84f66fcd in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["/bin/sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN apk add --no-cache libsasl # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:dc95107ad2a031a015320bb397f73ec151d738127175b31ad643120697dc7e90`  
		Last Modified: Thu, 28 Sep 2023 20:39:32 GMT  
		Size: 3.2 MB (3235757 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f36c14bb55ad2eb4c208a601b1c61872c3725ed95c0c2893c27a822ed5c33a58`  
		Last Modified: Tue, 03 Oct 2023 19:01:33 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1298cb8dafd972511af84e02d7b883a21241c52cf40b58d6979490001961f21c`  
		Last Modified: Tue, 03 Oct 2023 19:01:33 GMT  
		Size: 109.5 KB (109459 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:df4a91e2b048d49e66ddd9893c09f30f39a1d597e80105c7f8962e7f5f7139d9`  
		Last Modified: Tue, 03 Oct 2023 19:01:33 GMT  
		Size: 936.9 KB (936943 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9907fafebdae96d5487b7fb8157a823f61825ffefba79657a80bce23a2545448`  
		Last Modified: Tue, 03 Oct 2023 19:01:34 GMT  
		Size: 276.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ee6a4d82ccc808127f6aaa710b646e700271ad4eff9c41b9965accad5d5d3788`  
		Last Modified: Tue, 03 Oct 2023 19:01:34 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-alpine` - unknown; unknown

```console
$ docker pull memcached@sha256:fb404e06827e8d747912612afcca348dc58c4e9ee3ce83c4831cb09f12ab48fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 KB (18684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a050cea12e0cdebacb3a5a2ffc5ab6955496025789c041df169c407640f44bc8`

```dockerfile
```

-	Layers:
	-	`sha256:a3947c8d08a3d57e33242e44fb32c1cbd0106df35f9e5f83cb91293591da71c9`  
		Last Modified: Tue, 03 Oct 2023 19:01:33 GMT  
		Size: 18.7 KB (18684 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:32095d8b4daa6df8ff99e36c278c2cb210287066783a65050834bb28667fb2a2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4454721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26527e4ce577d5d1e1fdb3716fde4350e5a3ce0c3b3fd8dd527c6672f8eddcdf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["/bin/sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN apk add --no-cache libsasl # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9a6a9d9fc3b5def98513c33801853ba827c0c7bed9f2b4af3150b75fd4146d74`  
		Last Modified: Tue, 03 Oct 2023 19:06:17 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5dc7c33273d553c8b716261a6aee873fe5544c9200c9061bcc05b037a7c03ab5`  
		Last Modified: Tue, 03 Oct 2023 19:06:17 GMT  
		Size: 123.9 KB (123855 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0873dc2389c5bf83f2b2741fd0639e7dc70b2aa758884d63a794abe95622269b`  
		Last Modified: Tue, 03 Oct 2023 19:06:17 GMT  
		Size: 982.7 KB (982715 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:923b81392db2de0355d0715a2abf7bd7d715b4fac9d0bf39d5c08d7aeeed5270`  
		Last Modified: Tue, 03 Oct 2023 19:06:17 GMT  
		Size: 277.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dd619103d38407e95e05dd7d7f228e66bb5a61f3b561beb35198e92f9cdd0b99`  
		Last Modified: Tue, 03 Oct 2023 19:06:18 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-alpine` - unknown; unknown

```console
$ docker pull memcached@sha256:aaa2281dd27a5acbf1364325e1d6ff0a576cfd236847437e2382c07b7199c2ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.3 KB (93262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f9ccd98630f55e4cdd33076a1d3e7f9c11399077a20d0aa9f5af15fcb40bd81`

```dockerfile
```

-	Layers:
	-	`sha256:9c3b535b067358c4894b956bcbf5380d163ce977d0c30028d799f467af8f87d6`  
		Last Modified: Tue, 03 Oct 2023 19:06:17 GMT  
		Size: 74.4 KB (74406 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:9d03d340727841dba89e688d83cd797f9808417dd8d04970fd76395482b117ff`  
		Last Modified: Tue, 03 Oct 2023 19:06:17 GMT  
		Size: 18.9 KB (18856 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1-alpine` - linux; s390x

```console
$ docker pull memcached@sha256:0ff7f30ca924f54a50160e70bd590b2ef357c97b6e8bbfcb81fdde97dd5cfbb0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4279633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad89852ec7f35640342fc548839c205af73d8c0f60e54c113b34e9dc519e71c3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["/bin/sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN apk add --no-cache libsasl # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1a648ad7883b3087dfacc17e14f4e6158d881dd1e09b9c5bd27bdd0d89ee44fd`  
		Last Modified: Tue, 03 Oct 2023 20:00:49 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a950f9727c19a31b79f709cdf984608d7788a9ed00dacbce4b14535b7589886f`  
		Last Modified: Tue, 03 Oct 2023 20:00:49 GMT  
		Size: 112.8 KB (112780 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b42424189685c7b481e859243008fea5d1967c6bbc3ccaaf13bf601c56926ebb`  
		Last Modified: Tue, 03 Oct 2023 20:00:49 GMT  
		Size: 950.1 KB (950102 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bf2263fe42a85daea831aafa6f50aeeef49d0ce1aa5841ddde0951667f85b684`  
		Last Modified: Tue, 03 Oct 2023 20:00:49 GMT  
		Size: 281.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:75eaf7af52231f2a4943c93eafc5d565b71c6079a1fee0fdc2605ad3eb81cd58`  
		Last Modified: Tue, 03 Oct 2023 20:00:49 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-alpine` - unknown; unknown

```console
$ docker pull memcached@sha256:d2b9bd3538d99a100b4ebf104d9d5029917eecd3eec97d7086f7e4244b373d10
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.1 KB (93124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ade4e328bfbe610c689ab718878e6d07c31e5b67895795550a21d77730847d83`

```dockerfile
```

-	Layers:
	-	`sha256:7350d7c047abc3727f9639268d2cc1a5d7e53cbc81ae534da5e93272b5a48b59`  
		Last Modified: Tue, 03 Oct 2023 20:00:49 GMT  
		Size: 74.3 KB (74336 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:39706e52b9159fe158fe5027b73cb21482efb8781e1ab8853bcb19fc8125bbc8`  
		Last Modified: Tue, 03 Oct 2023 20:00:49 GMT  
		Size: 18.8 KB (18788 bytes)  
		MIME: application/vnd.in-toto+json

## `memcached:1-alpine3.18`

```console
$ docker pull memcached@sha256:eaba3015e1bf3a26f3d14ed455ef867e00d395963d0523c4275258f4890af5e1
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
$ docker pull memcached@sha256:27fe55ab0ecba9a8d3ddd67b823da4f1727d10eb46d36ab5af7e693421ebdb4f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4466251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3e0c0ff5c009f0e410e2fc6d29099b24315b4246c64cebae8068e86c22ba8a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["/bin/sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN apk add --no-cache libsasl # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3f9365fb2eebc56ba7006618c6ee8cde403af71bb4777c9b2b1c6ddcc107ee55`  
		Last Modified: Tue, 03 Oct 2023 19:01:12 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ec2c14990e92682477b554b5ccec603b864340a582d8ac4ab7becf52c09e9459`  
		Last Modified: Tue, 03 Oct 2023 19:01:12 GMT  
		Size: 108.0 KB (108015 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a0e994f33a8fb2b64e76f431cb35d0f0f92f0830352e44c589d8770bedfe96c3`  
		Last Modified: Tue, 03 Oct 2023 19:01:13 GMT  
		Size: 954.6 KB (954626 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:69c0dd1ede28d4dfdee1e54dc519270184463fa8812e781a930c0301b851c327`  
		Last Modified: Tue, 03 Oct 2023 19:01:12 GMT  
		Size: 277.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c9a4377466b783eeeab01987a823353e5cfbc2a5f02d632db14c654decf3ec5e`  
		Last Modified: Tue, 03 Oct 2023 19:01:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-alpine3.18` - unknown; unknown

```console
$ docker pull memcached@sha256:6ebfa6199008800194514397c12c233ea35c27ee5d22bea93fc978228a9f98f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.2 KB (95222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc3627763f4a9bb22db274ce8453a9d0146e88c0f4e0624f69059e5a9a69ec31`

```dockerfile
```

-	Layers:
	-	`sha256:7e739eda7910762ab0244ff165c2ff431bf4f10a39730614a8fca28a9a91b97d`  
		Last Modified: Tue, 03 Oct 2023 19:01:12 GMT  
		Size: 76.3 KB (76268 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:a04f216271188784dc836fa4905c7d5fbcfb49537cf5cfb5fe5b0229694cf12c`  
		Last Modified: Tue, 03 Oct 2023 19:01:12 GMT  
		Size: 19.0 KB (18954 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:1152b588a2cd7e90f0d7ae86fe3ce262e47c50c62642b5714b0019cef7779a00
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4401705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31bcc2b506321f6395c1d68cfc40f7391530051e5862186db1d5875e2c2803be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["/bin/sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN apk add --no-cache libsasl # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a8a999d5f4398538233c73f556a07cf646c7600543368cbc84b997cd76545de1`  
		Last Modified: Tue, 03 Oct 2023 19:03:35 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e035f8f759de7f5b35527c5cc46cd4132a10e0a501e022fbde2fedcf47fdd684`  
		Last Modified: Tue, 03 Oct 2023 19:03:35 GMT  
		Size: 124.1 KB (124080 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:585097acb28da9160246ad53fa72c119ac6e97a2852f420712485b66d6ed808a`  
		Last Modified: Tue, 03 Oct 2023 19:03:36 GMT  
		Size: 944.1 KB (944147 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:802f5f839e31fd8f8dd89ec2421af9fa8227dd43d5ca883f44d9ff2962cd0848`  
		Last Modified: Tue, 03 Oct 2023 19:03:35 GMT  
		Size: 281.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:65fc6300aa54fcd82f813153e3a5a880a2dca2a26edc3f7f907fe395a01a5474`  
		Last Modified: Tue, 03 Oct 2023 19:03:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-alpine3.18` - unknown; unknown

```console
$ docker pull memcached@sha256:5b2e4db4700ecd5765dd85cbc125a24968150122eb9f8181949dc39310085671
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.1 KB (95095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e78ca75a52728eb7207c54b73b899cb6919fd230b814373dc1612765d95bcc0c`

```dockerfile
```

-	Layers:
	-	`sha256:36799473bd1d28916d0df4c2af578542c27261dcc2dbba98964d2d7e956bd73f`  
		Last Modified: Tue, 03 Oct 2023 19:03:35 GMT  
		Size: 76.3 KB (76289 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:c088a7e985146394427f4d604d17a54445f5934b07e790774b7472540d932737`  
		Last Modified: Tue, 03 Oct 2023 19:03:35 GMT  
		Size: 18.8 KB (18806 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1-alpine3.18` - linux; 386

```console
$ docker pull memcached@sha256:8b880914dfffd537639b55f5f49cf6c6e9f0773891eb922685e0ce94ccde66b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4283801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f38744e29d4692d1345bf5101db090800c52e9ae211735a610dd8e848ca426d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:8402753f294e403e92353bd65c86a6428c960be5116c0a15484b663a84f66fcd in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["/bin/sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN apk add --no-cache libsasl # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:dc95107ad2a031a015320bb397f73ec151d738127175b31ad643120697dc7e90`  
		Last Modified: Thu, 28 Sep 2023 20:39:32 GMT  
		Size: 3.2 MB (3235757 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f36c14bb55ad2eb4c208a601b1c61872c3725ed95c0c2893c27a822ed5c33a58`  
		Last Modified: Tue, 03 Oct 2023 19:01:33 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1298cb8dafd972511af84e02d7b883a21241c52cf40b58d6979490001961f21c`  
		Last Modified: Tue, 03 Oct 2023 19:01:33 GMT  
		Size: 109.5 KB (109459 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:df4a91e2b048d49e66ddd9893c09f30f39a1d597e80105c7f8962e7f5f7139d9`  
		Last Modified: Tue, 03 Oct 2023 19:01:33 GMT  
		Size: 936.9 KB (936943 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9907fafebdae96d5487b7fb8157a823f61825ffefba79657a80bce23a2545448`  
		Last Modified: Tue, 03 Oct 2023 19:01:34 GMT  
		Size: 276.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ee6a4d82ccc808127f6aaa710b646e700271ad4eff9c41b9965accad5d5d3788`  
		Last Modified: Tue, 03 Oct 2023 19:01:34 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-alpine3.18` - unknown; unknown

```console
$ docker pull memcached@sha256:fb404e06827e8d747912612afcca348dc58c4e9ee3ce83c4831cb09f12ab48fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 KB (18684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a050cea12e0cdebacb3a5a2ffc5ab6955496025789c041df169c407640f44bc8`

```dockerfile
```

-	Layers:
	-	`sha256:a3947c8d08a3d57e33242e44fb32c1cbd0106df35f9e5f83cb91293591da71c9`  
		Last Modified: Tue, 03 Oct 2023 19:01:33 GMT  
		Size: 18.7 KB (18684 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1-alpine3.18` - linux; ppc64le

```console
$ docker pull memcached@sha256:32095d8b4daa6df8ff99e36c278c2cb210287066783a65050834bb28667fb2a2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4454721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26527e4ce577d5d1e1fdb3716fde4350e5a3ce0c3b3fd8dd527c6672f8eddcdf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["/bin/sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN apk add --no-cache libsasl # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9a6a9d9fc3b5def98513c33801853ba827c0c7bed9f2b4af3150b75fd4146d74`  
		Last Modified: Tue, 03 Oct 2023 19:06:17 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5dc7c33273d553c8b716261a6aee873fe5544c9200c9061bcc05b037a7c03ab5`  
		Last Modified: Tue, 03 Oct 2023 19:06:17 GMT  
		Size: 123.9 KB (123855 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0873dc2389c5bf83f2b2741fd0639e7dc70b2aa758884d63a794abe95622269b`  
		Last Modified: Tue, 03 Oct 2023 19:06:17 GMT  
		Size: 982.7 KB (982715 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:923b81392db2de0355d0715a2abf7bd7d715b4fac9d0bf39d5c08d7aeeed5270`  
		Last Modified: Tue, 03 Oct 2023 19:06:17 GMT  
		Size: 277.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dd619103d38407e95e05dd7d7f228e66bb5a61f3b561beb35198e92f9cdd0b99`  
		Last Modified: Tue, 03 Oct 2023 19:06:18 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-alpine3.18` - unknown; unknown

```console
$ docker pull memcached@sha256:aaa2281dd27a5acbf1364325e1d6ff0a576cfd236847437e2382c07b7199c2ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.3 KB (93262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f9ccd98630f55e4cdd33076a1d3e7f9c11399077a20d0aa9f5af15fcb40bd81`

```dockerfile
```

-	Layers:
	-	`sha256:9c3b535b067358c4894b956bcbf5380d163ce977d0c30028d799f467af8f87d6`  
		Last Modified: Tue, 03 Oct 2023 19:06:17 GMT  
		Size: 74.4 KB (74406 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:9d03d340727841dba89e688d83cd797f9808417dd8d04970fd76395482b117ff`  
		Last Modified: Tue, 03 Oct 2023 19:06:17 GMT  
		Size: 18.9 KB (18856 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1-alpine3.18` - linux; s390x

```console
$ docker pull memcached@sha256:0ff7f30ca924f54a50160e70bd590b2ef357c97b6e8bbfcb81fdde97dd5cfbb0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4279633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad89852ec7f35640342fc548839c205af73d8c0f60e54c113b34e9dc519e71c3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["/bin/sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN apk add --no-cache libsasl # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1a648ad7883b3087dfacc17e14f4e6158d881dd1e09b9c5bd27bdd0d89ee44fd`  
		Last Modified: Tue, 03 Oct 2023 20:00:49 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a950f9727c19a31b79f709cdf984608d7788a9ed00dacbce4b14535b7589886f`  
		Last Modified: Tue, 03 Oct 2023 20:00:49 GMT  
		Size: 112.8 KB (112780 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b42424189685c7b481e859243008fea5d1967c6bbc3ccaaf13bf601c56926ebb`  
		Last Modified: Tue, 03 Oct 2023 20:00:49 GMT  
		Size: 950.1 KB (950102 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bf2263fe42a85daea831aafa6f50aeeef49d0ce1aa5841ddde0951667f85b684`  
		Last Modified: Tue, 03 Oct 2023 20:00:49 GMT  
		Size: 281.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:75eaf7af52231f2a4943c93eafc5d565b71c6079a1fee0fdc2605ad3eb81cd58`  
		Last Modified: Tue, 03 Oct 2023 20:00:49 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-alpine3.18` - unknown; unknown

```console
$ docker pull memcached@sha256:d2b9bd3538d99a100b4ebf104d9d5029917eecd3eec97d7086f7e4244b373d10
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.1 KB (93124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ade4e328bfbe610c689ab718878e6d07c31e5b67895795550a21d77730847d83`

```dockerfile
```

-	Layers:
	-	`sha256:7350d7c047abc3727f9639268d2cc1a5d7e53cbc81ae534da5e93272b5a48b59`  
		Last Modified: Tue, 03 Oct 2023 20:00:49 GMT  
		Size: 74.3 KB (74336 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:39706e52b9159fe158fe5027b73cb21482efb8781e1ab8853bcb19fc8125bbc8`  
		Last Modified: Tue, 03 Oct 2023 20:00:49 GMT  
		Size: 18.8 KB (18788 bytes)  
		MIME: application/vnd.in-toto+json

## `memcached:1-bookworm`

```console
$ docker pull memcached@sha256:eef4a056175ad8203df2a1835ae16307e5a70aec3222b409d1114486b2a4bb65
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
$ docker pull memcached@sha256:8af51889f0f774a00f36624e58faac309c258eafb8054c6abc6fbbb56c78d0a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.8 MB (38811465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fa23f6ace109fad9223ea2db53f79afa8b91b14051c61305f82bc2c781a788c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:55ad846fa191e603f48090eae0e4a7149c4066b94406593ec1898ad2c3347937 in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a378f10b321842c3042cdeff4f6997f34f4cb21f2eff27704b7f6193ab7b5fea`  
		Last Modified: Wed, 11 Oct 2023 18:39:34 GMT  
		Size: 29.1 MB (29149874 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e68aaf702a54364b3f216204ad2725f5b416fe496294086899b821bb5133552d`  
		Last Modified: Wed, 11 Oct 2023 20:07:27 GMT  
		Size: 1.1 KB (1110 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0fb853802e1447e9b1dbe3e8a86f27a5691286127397adf8d52f943d16b80042`  
		Last Modified: Wed, 11 Oct 2023 20:07:27 GMT  
		Size: 2.5 MB (2488274 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fcc9694d882f053fcf2e7bb33709dcb86eef6c29c3187c190ad93852af7a50f2`  
		Last Modified: Wed, 11 Oct 2023 20:07:28 GMT  
		Size: 7.2 MB (7171802 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fde136907f7040bd6126a5b2c0bca844fef33e2fc804c1f135e99393869cce4c`  
		Last Modified: Wed, 11 Oct 2023 20:07:27 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c121d0db5ccb2988b1fc0c76ce60a2e78309d77b264adf99e815e1ecf2c6a957`  
		Last Modified: Wed, 11 Oct 2023 20:07:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:888d3aaaddc944acb247f0e42586c8c8a7f8c3262166ee89ceda0dbe3998cafa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2911211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06530a2f7a54ba7d86fc6cee0da9a46ea1aea89dc4beecbee6d54ed8eee82dd9`

```dockerfile
```

-	Layers:
	-	`sha256:7bbbdfb4ba86ed51b46d2fb83bf8cf4e095da6d5c9dd89697a3488dd392414d7`  
		Last Modified: Wed, 11 Oct 2023 20:07:27 GMT  
		Size: 2.9 MB (2889442 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:6fe7a995830937695f7110928df7e791673ab04015add73a1f2e9ec661bbc60f`  
		Last Modified: Wed, 11 Oct 2023 20:07:27 GMT  
		Size: 21.8 KB (21769 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1-bookworm` - linux; arm variant v5

```console
$ docker pull memcached@sha256:a6919fc9976aa2c291f194860f40fcc9499d33cbd2592af9087e5d64b7930602
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34846023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5222dddac963b84d55ef902d40fa3f949ee73caac9614ca77c1f4a81ef009c6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:8c43adb3245fc6f2b10aa5a86c850db5dcf3515eaf7e46630922fe21f806bd2a in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:904e6393ef1ee28b37171369eb4f7cb04714631c711799819fccb83886bd212b`  
		Last Modified: Wed, 11 Oct 2023 17:40:47 GMT  
		Size: 26.9 MB (26922150 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f0569355cb85b70d6a614ea9604289ce8e724f0f9ff4d1d8a12afc24c4c9ad1f`  
		Last Modified: Thu, 12 Oct 2023 08:32:05 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6939032c8ff0687b012a85d3411c702266b934a677f96eb521658b44f5b4a8c0`  
		Last Modified: Thu, 12 Oct 2023 08:32:06 GMT  
		Size: 2.1 MB (2089182 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8e8a2a7338b5cacc7b6e4e3db2359eebb1936b0b14266d5bad0dfcc21c9becff`  
		Last Modified: Thu, 12 Oct 2023 08:32:06 GMT  
		Size: 5.8 MB (5833176 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:19f35a8116fe7e124bee612b2ac511694077a1f35f76ed056903987ab4921e34`  
		Last Modified: Thu, 12 Oct 2023 08:32:06 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a43775be6dfac6c255e35b164eacd7328df241f33f9245206a8eaf481062ccbc`  
		Last Modified: Thu, 12 Oct 2023 08:32:07 GMT  
		Size: 120.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:f1276a05a4db6e8b7bb9d8374d480b85a79f1b92d4e7475c65e247bf1427200c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.7 KB (21695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe67b683a818ed7c22a49086ec4f22e53c6efa9040becea46adb07f550dae564`

```dockerfile
```

-	Layers:
	-	`sha256:12ecc330d2059d33dc7a7c518e7be06804f5fcadafdc8e2db030631f5c92b326`  
		Last Modified: Thu, 12 Oct 2023 08:32:05 GMT  
		Size: 21.7 KB (21695 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1-bookworm` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:0c25b3c626a396c236dcf08792c850a178482c24e0c9dab0e784783178d10c13
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.4 MB (43442272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1595a8aa58bfc22ba6e995a58c63ea8b660aa8a9b10c57ab0cb8552d94080218`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:ec1a6e0aedd76c8fdc8544775f8b553f58950e9435f5cfe919f39374e222cfbb in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:e886f0f47ef56fcadb6ecaf2116056bbdb273e0afe07ed034498b198d386c04e`  
		Last Modified: Wed, 20 Sep 2023 02:47:36 GMT  
		Size: 29.2 MB (29157221 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7e25b15fcaee53caa22717c5b0b52fabf2480b0244a84530fca4c1edbb812044`  
		Last Modified: Tue, 03 Oct 2023 19:00:54 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:72fc5c44d6b752d2c2534f97f12ef44f915803ec4e564d7c9eb90d9d7bda2297`  
		Last Modified: Tue, 03 Oct 2023 19:00:54 GMT  
		Size: 2.3 MB (2343087 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7ba30437e42c2aebda3182e43b83b90012dd19e31adb9dc25bb3b714385cdefe`  
		Last Modified: Tue, 03 Oct 2023 19:00:55 GMT  
		Size: 11.9 MB (11940448 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:70abb5efa4268d01b1dfe9f6775f8f85a7fe395141dcc28909aa52ea6b741971`  
		Last Modified: Tue, 03 Oct 2023 19:00:54 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5a87a9f60806e352855b340f2c0c3610b8053006f0f542077c3add7e70782663`  
		Last Modified: Tue, 03 Oct 2023 19:00:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:7a900749c7d177577d906a5d402b4a008b95ae3571e9de24b4f04060e8650d5d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2890735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:711e633b20942471e455d3210316a79109ffda2a13cb38f46bd9ab2d27c758ae`

```dockerfile
```

-	Layers:
	-	`sha256:6c4c4a32fc3b330e635796951e46bf9e6ed753212798e75baddd3a84e752de8c`  
		Last Modified: Tue, 03 Oct 2023 19:00:54 GMT  
		Size: 2.9 MB (2869112 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:d0ceb647ed388f03f95faf34bc93c1489afde267801855f46cfca84fca538c5a`  
		Last Modified: Tue, 03 Oct 2023 19:00:54 GMT  
		Size: 21.6 KB (21623 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1-bookworm` - linux; 386

```console
$ docker pull memcached@sha256:dbf6fdd168abcb8b6fd831277bea0213784e54cdb824756684dd3b5337c42c65
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.6 MB (44649134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25680867a5df0eb88860f59d7855c9d7f3862a44283c1e59d608f9dbecff348b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:efe81f7066129aa6293627bfe4ea78b957897ba5ede951970156fccf1dbcde88 in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6ac07f93e07a1bad4555e13bd8efd06169988669fc88df95f4bf296a2b44523d`  
		Last Modified: Wed, 20 Sep 2023 00:46:48 GMT  
		Size: 30.1 MB (30141894 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:797b4215eddcf948eec0f19132f85ec1b0f3af264399e78d860bece37acc4888`  
		Last Modified: Tue, 03 Oct 2023 19:01:51 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3c78c0b20e6791912325d174e98f60d4f783c2f013f52ff3835892444d3a15d7`  
		Last Modified: Tue, 03 Oct 2023 19:01:51 GMT  
		Size: 2.5 MB (2490464 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c91bf1cea723f722413107daa57ab51060ab36a5f78fe8447568aa35be54fca5`  
		Last Modified: Tue, 03 Oct 2023 19:01:52 GMT  
		Size: 12.0 MB (12015261 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:07f7206e609641792c84dfac85e3e6df0602c4ca8d572353a8768ff0619fe328`  
		Last Modified: Tue, 03 Oct 2023 19:01:51 GMT  
		Size: 283.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7aac14495f4a088e0e208638d0b36b0b5ff0cf945aaf24c011ef08ca799279a9`  
		Last Modified: Tue, 03 Oct 2023 19:01:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:16c8db3d95a2df8fae160a3942ff033ebb3bf6d9fe8df1643eb22c82e9402357
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 KB (21502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03bc49cf22d3ede52afc78d429b09999ba28174660a5e1b41fdb0f9d3a47067c`

```dockerfile
```

-	Layers:
	-	`sha256:890c3f7af1536aa0821f27c4ba142e022ba0c892f1310b4d82a9cc3a74717139`  
		Last Modified: Tue, 03 Oct 2023 19:01:51 GMT  
		Size: 21.5 KB (21502 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1-bookworm` - linux; mips64le

```console
$ docker pull memcached@sha256:575825bdbf62fc255547394ef491710ba88f0be3ca735eaf246ece06f13363ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.4 MB (43398233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e3f951153522f4d9719c37a9862412f3e29e487d11322c5ff7a009cf8becca1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:850547a08e38ebc5a3659df86e70039a8d9828ae26ae485b077c98a959248dcb in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:0f581c6294fe7421dfee024e2c7dddd73ef3fbd7ff23b05bc3c1bf9f50885e85`  
		Last Modified: Wed, 20 Sep 2023 03:20:59 GMT  
		Size: 29.1 MB (29121674 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:15e25af5488ea4ad0df132fa2c22a282c1a17ad1460cdb25fe5939e03a753528`  
		Last Modified: Tue, 03 Oct 2023 19:04:40 GMT  
		Size: 1.1 KB (1113 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:19a5f416c9bf283212262e33fe8529d0ff3917fcee1e8ca9fb058170fd528211`  
		Last Modified: Tue, 03 Oct 2023 19:04:41 GMT  
		Size: 1.9 MB (1934931 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:05862af95003d85f9a1b5696dfb3588bdd8e34c74f067d845b722d70edfc679f`  
		Last Modified: Tue, 03 Oct 2023 19:04:41 GMT  
		Size: 12.3 MB (12340111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e8aae13855c46b73d2506b2d91036f6f0b4bc63b7d7ec12ecc63fd672c64c0f7`  
		Last Modified: Tue, 03 Oct 2023 19:04:40 GMT  
		Size: 282.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0709f88ce6a011ea45fd41c091ee6fcf4baa0610e0591a9fe0d10626eaf9475f`  
		Last Modified: Tue, 03 Oct 2023 19:04:41 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:269b3e28059bf711ac45886388e91fa405b8a1e0ca1a114acefc997bbdad6d05
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 KB (21491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1059a2662b538952006866f53463fcea773b5e090eaead3a4ad49f4d0a656ae5`

```dockerfile
```

-	Layers:
	-	`sha256:e1052b07541ae6e041e59834c527075b62df62a33f7a9b9e96fda4b6237e83df`  
		Last Modified: Tue, 03 Oct 2023 19:04:40 GMT  
		Size: 21.5 KB (21491 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1-bookworm` - linux; ppc64le

```console
$ docker pull memcached@sha256:532cf0a6053275c508a0503017b4f52ce356a64aba047eb2316bdcaca35bbc9a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49635445 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:111f6d9d894ab95e36b94efa3dad4a4c9d0def1fa3af71a4a0e57e907a2b4986`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:9a37b479e68a0d18babbef8dd04d09a0e6844a0080876d14144a34bfd9d0897a in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:696a66e961f2033dcf69b003ad7faf28ed2248da58efa1c08a9d496739a8eeeb`  
		Last Modified: Wed, 20 Sep 2023 08:49:51 GMT  
		Size: 33.1 MB (33119461 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ba4c0c64bfd7ea845d20c793ede5957878785e4bb16e2e81a3e1ed5cd0d7ca0e`  
		Last Modified: Tue, 03 Oct 2023 19:02:08 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8a7ae673337cbb772a0ccc237ce4009a7dd88e4fed23861c9ea6382e93a6685b`  
		Last Modified: Tue, 03 Oct 2023 19:02:09 GMT  
		Size: 2.7 MB (2694930 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:766c713a6dbc39908803d95aa7556e0a571349c941bddb8f694b3f36030e0c3c`  
		Last Modified: Tue, 03 Oct 2023 19:02:10 GMT  
		Size: 13.8 MB (13819538 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:75734e09fa81ca91f8bdd1481c8f88f95ea9ba7b0f24ab82d0aee2026a5d6474`  
		Last Modified: Tue, 03 Oct 2023 19:02:09 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f46fc74a04a0607353cbc3ace76b49b44029af75080fa56fec872060d38feed2`  
		Last Modified: Tue, 03 Oct 2023 19:02:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:d73c6167b49dd216e6395e8720af5bd26884a25473d1eb80ee31d1e4b170a914
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2914816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48964548656eeecac440cb41e4f3f474f861d384c569653e582e3d508b04f6e5`

```dockerfile
```

-	Layers:
	-	`sha256:4e89c387c1399e94faaaf407614d23c90aa3104b5773f87d8cb4fe4b20312f8e`  
		Last Modified: Tue, 03 Oct 2023 19:02:09 GMT  
		Size: 2.9 MB (2893143 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:fb96286b26618de71f0df13dfc89225bc855d6802341b4032f0fb4161cb4a52e`  
		Last Modified: Tue, 03 Oct 2023 19:02:08 GMT  
		Size: 21.7 KB (21673 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1-bookworm` - linux; s390x

```console
$ docker pull memcached@sha256:42a17150fd8b17aff6910890bbab808eab97e6f9d0f60003e75fac6ddd2b0bcf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40575835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:956090eeead5cd8ec7753b439eb43ddf3b2c5cd93edea3d7ce5bcdd168ec7588`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:6ed982ad3e8566d63315a27a81b33069910952aef4b2d3e0b607bd2caeac7ca4 in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:26dcff366e33abcf08b812052a4c12496aa406aa267655e984aa7a84ca254cd8`  
		Last Modified: Wed, 20 Sep 2023 02:59:47 GMT  
		Size: 27.5 MB (27489966 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:04795616cce62da1faee69d189f2f4863a3818651e9f54e7552be41e35752766`  
		Last Modified: Tue, 03 Oct 2023 19:01:27 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cbacb720efba986e695a3270bc384924abb78c413d1c4793cd388fbab1da828b`  
		Last Modified: Tue, 03 Oct 2023 19:01:27 GMT  
		Size: 2.2 MB (2150908 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:07a927de051febdc6284e8ec146cbc267ffdd1049fadf2bc35639f53b72b7862`  
		Last Modified: Tue, 03 Oct 2023 19:01:28 GMT  
		Size: 10.9 MB (10933444 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5a2703a37bdc4f133106c52c5a040d30708c01a79aa0d1714bcba3b42105692e`  
		Last Modified: Tue, 03 Oct 2023 19:01:28 GMT  
		Size: 285.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c0a860b98e7d941cd44043f66c4cc9d2a540ab3b8cb9aa15123102865599e0c7`  
		Last Modified: Tue, 03 Oct 2023 19:01:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:029d2884ff06e1b3673d9a7998c7299cc3da7ed18f46b344e13c14867574bae4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2897027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e57e1f9eb901fd307d1e2dd72b5606ba1f6f0ef82c31c01041513ed98e33b55`

```dockerfile
```

-	Layers:
	-	`sha256:13af4843cce0c7df5b25984623ef20fe08955ca99bbc64f5056c4d1bb2062f13`  
		Last Modified: Tue, 03 Oct 2023 19:01:27 GMT  
		Size: 2.9 MB (2875422 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:2e615a884e0baa9f5e54063b8983b99c841ac4fd854bf56780c1184d51637b1d`  
		Last Modified: Tue, 03 Oct 2023 19:01:27 GMT  
		Size: 21.6 KB (21605 bytes)  
		MIME: application/vnd.in-toto+json

## `memcached:1.6`

```console
$ docker pull memcached@sha256:392f01c0e85fa9aeb0308a0c3b43b1ecde43203929c1d56d87ac469fd3d3e0a6
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
$ docker pull memcached@sha256:8af51889f0f774a00f36624e58faac309c258eafb8054c6abc6fbbb56c78d0a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.8 MB (38811465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fa23f6ace109fad9223ea2db53f79afa8b91b14051c61305f82bc2c781a788c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:55ad846fa191e603f48090eae0e4a7149c4066b94406593ec1898ad2c3347937 in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a378f10b321842c3042cdeff4f6997f34f4cb21f2eff27704b7f6193ab7b5fea`  
		Last Modified: Wed, 11 Oct 2023 18:39:34 GMT  
		Size: 29.1 MB (29149874 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e68aaf702a54364b3f216204ad2725f5b416fe496294086899b821bb5133552d`  
		Last Modified: Wed, 11 Oct 2023 20:07:27 GMT  
		Size: 1.1 KB (1110 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0fb853802e1447e9b1dbe3e8a86f27a5691286127397adf8d52f943d16b80042`  
		Last Modified: Wed, 11 Oct 2023 20:07:27 GMT  
		Size: 2.5 MB (2488274 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fcc9694d882f053fcf2e7bb33709dcb86eef6c29c3187c190ad93852af7a50f2`  
		Last Modified: Wed, 11 Oct 2023 20:07:28 GMT  
		Size: 7.2 MB (7171802 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fde136907f7040bd6126a5b2c0bca844fef33e2fc804c1f135e99393869cce4c`  
		Last Modified: Wed, 11 Oct 2023 20:07:27 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c121d0db5ccb2988b1fc0c76ce60a2e78309d77b264adf99e815e1ecf2c6a957`  
		Last Modified: Wed, 11 Oct 2023 20:07:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6` - unknown; unknown

```console
$ docker pull memcached@sha256:888d3aaaddc944acb247f0e42586c8c8a7f8c3262166ee89ceda0dbe3998cafa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2911211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06530a2f7a54ba7d86fc6cee0da9a46ea1aea89dc4beecbee6d54ed8eee82dd9`

```dockerfile
```

-	Layers:
	-	`sha256:7bbbdfb4ba86ed51b46d2fb83bf8cf4e095da6d5c9dd89697a3488dd392414d7`  
		Last Modified: Wed, 11 Oct 2023 20:07:27 GMT  
		Size: 2.9 MB (2889442 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:6fe7a995830937695f7110928df7e791673ab04015add73a1f2e9ec661bbc60f`  
		Last Modified: Wed, 11 Oct 2023 20:07:27 GMT  
		Size: 21.8 KB (21769 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6` - linux; arm variant v5

```console
$ docker pull memcached@sha256:a6919fc9976aa2c291f194860f40fcc9499d33cbd2592af9087e5d64b7930602
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34846023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5222dddac963b84d55ef902d40fa3f949ee73caac9614ca77c1f4a81ef009c6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:8c43adb3245fc6f2b10aa5a86c850db5dcf3515eaf7e46630922fe21f806bd2a in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:904e6393ef1ee28b37171369eb4f7cb04714631c711799819fccb83886bd212b`  
		Last Modified: Wed, 11 Oct 2023 17:40:47 GMT  
		Size: 26.9 MB (26922150 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f0569355cb85b70d6a614ea9604289ce8e724f0f9ff4d1d8a12afc24c4c9ad1f`  
		Last Modified: Thu, 12 Oct 2023 08:32:05 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6939032c8ff0687b012a85d3411c702266b934a677f96eb521658b44f5b4a8c0`  
		Last Modified: Thu, 12 Oct 2023 08:32:06 GMT  
		Size: 2.1 MB (2089182 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8e8a2a7338b5cacc7b6e4e3db2359eebb1936b0b14266d5bad0dfcc21c9becff`  
		Last Modified: Thu, 12 Oct 2023 08:32:06 GMT  
		Size: 5.8 MB (5833176 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:19f35a8116fe7e124bee612b2ac511694077a1f35f76ed056903987ab4921e34`  
		Last Modified: Thu, 12 Oct 2023 08:32:06 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a43775be6dfac6c255e35b164eacd7328df241f33f9245206a8eaf481062ccbc`  
		Last Modified: Thu, 12 Oct 2023 08:32:07 GMT  
		Size: 120.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6` - unknown; unknown

```console
$ docker pull memcached@sha256:f1276a05a4db6e8b7bb9d8374d480b85a79f1b92d4e7475c65e247bf1427200c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.7 KB (21695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe67b683a818ed7c22a49086ec4f22e53c6efa9040becea46adb07f550dae564`

```dockerfile
```

-	Layers:
	-	`sha256:12ecc330d2059d33dc7a7c518e7be06804f5fcadafdc8e2db030631f5c92b326`  
		Last Modified: Thu, 12 Oct 2023 08:32:05 GMT  
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
$ docker pull memcached@sha256:0c25b3c626a396c236dcf08792c850a178482c24e0c9dab0e784783178d10c13
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.4 MB (43442272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1595a8aa58bfc22ba6e995a58c63ea8b660aa8a9b10c57ab0cb8552d94080218`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:ec1a6e0aedd76c8fdc8544775f8b553f58950e9435f5cfe919f39374e222cfbb in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:e886f0f47ef56fcadb6ecaf2116056bbdb273e0afe07ed034498b198d386c04e`  
		Last Modified: Wed, 20 Sep 2023 02:47:36 GMT  
		Size: 29.2 MB (29157221 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7e25b15fcaee53caa22717c5b0b52fabf2480b0244a84530fca4c1edbb812044`  
		Last Modified: Tue, 03 Oct 2023 19:00:54 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:72fc5c44d6b752d2c2534f97f12ef44f915803ec4e564d7c9eb90d9d7bda2297`  
		Last Modified: Tue, 03 Oct 2023 19:00:54 GMT  
		Size: 2.3 MB (2343087 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7ba30437e42c2aebda3182e43b83b90012dd19e31adb9dc25bb3b714385cdefe`  
		Last Modified: Tue, 03 Oct 2023 19:00:55 GMT  
		Size: 11.9 MB (11940448 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:70abb5efa4268d01b1dfe9f6775f8f85a7fe395141dcc28909aa52ea6b741971`  
		Last Modified: Tue, 03 Oct 2023 19:00:54 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5a87a9f60806e352855b340f2c0c3610b8053006f0f542077c3add7e70782663`  
		Last Modified: Tue, 03 Oct 2023 19:00:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6` - unknown; unknown

```console
$ docker pull memcached@sha256:7a900749c7d177577d906a5d402b4a008b95ae3571e9de24b4f04060e8650d5d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2890735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:711e633b20942471e455d3210316a79109ffda2a13cb38f46bd9ab2d27c758ae`

```dockerfile
```

-	Layers:
	-	`sha256:6c4c4a32fc3b330e635796951e46bf9e6ed753212798e75baddd3a84e752de8c`  
		Last Modified: Tue, 03 Oct 2023 19:00:54 GMT  
		Size: 2.9 MB (2869112 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:d0ceb647ed388f03f95faf34bc93c1489afde267801855f46cfca84fca538c5a`  
		Last Modified: Tue, 03 Oct 2023 19:00:54 GMT  
		Size: 21.6 KB (21623 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6` - linux; 386

```console
$ docker pull memcached@sha256:dbf6fdd168abcb8b6fd831277bea0213784e54cdb824756684dd3b5337c42c65
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.6 MB (44649134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25680867a5df0eb88860f59d7855c9d7f3862a44283c1e59d608f9dbecff348b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:efe81f7066129aa6293627bfe4ea78b957897ba5ede951970156fccf1dbcde88 in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6ac07f93e07a1bad4555e13bd8efd06169988669fc88df95f4bf296a2b44523d`  
		Last Modified: Wed, 20 Sep 2023 00:46:48 GMT  
		Size: 30.1 MB (30141894 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:797b4215eddcf948eec0f19132f85ec1b0f3af264399e78d860bece37acc4888`  
		Last Modified: Tue, 03 Oct 2023 19:01:51 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3c78c0b20e6791912325d174e98f60d4f783c2f013f52ff3835892444d3a15d7`  
		Last Modified: Tue, 03 Oct 2023 19:01:51 GMT  
		Size: 2.5 MB (2490464 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c91bf1cea723f722413107daa57ab51060ab36a5f78fe8447568aa35be54fca5`  
		Last Modified: Tue, 03 Oct 2023 19:01:52 GMT  
		Size: 12.0 MB (12015261 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:07f7206e609641792c84dfac85e3e6df0602c4ca8d572353a8768ff0619fe328`  
		Last Modified: Tue, 03 Oct 2023 19:01:51 GMT  
		Size: 283.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7aac14495f4a088e0e208638d0b36b0b5ff0cf945aaf24c011ef08ca799279a9`  
		Last Modified: Tue, 03 Oct 2023 19:01:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6` - unknown; unknown

```console
$ docker pull memcached@sha256:16c8db3d95a2df8fae160a3942ff033ebb3bf6d9fe8df1643eb22c82e9402357
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 KB (21502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03bc49cf22d3ede52afc78d429b09999ba28174660a5e1b41fdb0f9d3a47067c`

```dockerfile
```

-	Layers:
	-	`sha256:890c3f7af1536aa0821f27c4ba142e022ba0c892f1310b4d82a9cc3a74717139`  
		Last Modified: Tue, 03 Oct 2023 19:01:51 GMT  
		Size: 21.5 KB (21502 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6` - linux; mips64le

```console
$ docker pull memcached@sha256:575825bdbf62fc255547394ef491710ba88f0be3ca735eaf246ece06f13363ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.4 MB (43398233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e3f951153522f4d9719c37a9862412f3e29e487d11322c5ff7a009cf8becca1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:850547a08e38ebc5a3659df86e70039a8d9828ae26ae485b077c98a959248dcb in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:0f581c6294fe7421dfee024e2c7dddd73ef3fbd7ff23b05bc3c1bf9f50885e85`  
		Last Modified: Wed, 20 Sep 2023 03:20:59 GMT  
		Size: 29.1 MB (29121674 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:15e25af5488ea4ad0df132fa2c22a282c1a17ad1460cdb25fe5939e03a753528`  
		Last Modified: Tue, 03 Oct 2023 19:04:40 GMT  
		Size: 1.1 KB (1113 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:19a5f416c9bf283212262e33fe8529d0ff3917fcee1e8ca9fb058170fd528211`  
		Last Modified: Tue, 03 Oct 2023 19:04:41 GMT  
		Size: 1.9 MB (1934931 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:05862af95003d85f9a1b5696dfb3588bdd8e34c74f067d845b722d70edfc679f`  
		Last Modified: Tue, 03 Oct 2023 19:04:41 GMT  
		Size: 12.3 MB (12340111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e8aae13855c46b73d2506b2d91036f6f0b4bc63b7d7ec12ecc63fd672c64c0f7`  
		Last Modified: Tue, 03 Oct 2023 19:04:40 GMT  
		Size: 282.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0709f88ce6a011ea45fd41c091ee6fcf4baa0610e0591a9fe0d10626eaf9475f`  
		Last Modified: Tue, 03 Oct 2023 19:04:41 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6` - unknown; unknown

```console
$ docker pull memcached@sha256:269b3e28059bf711ac45886388e91fa405b8a1e0ca1a114acefc997bbdad6d05
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 KB (21491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1059a2662b538952006866f53463fcea773b5e090eaead3a4ad49f4d0a656ae5`

```dockerfile
```

-	Layers:
	-	`sha256:e1052b07541ae6e041e59834c527075b62df62a33f7a9b9e96fda4b6237e83df`  
		Last Modified: Tue, 03 Oct 2023 19:04:40 GMT  
		Size: 21.5 KB (21491 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6` - linux; ppc64le

```console
$ docker pull memcached@sha256:532cf0a6053275c508a0503017b4f52ce356a64aba047eb2316bdcaca35bbc9a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49635445 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:111f6d9d894ab95e36b94efa3dad4a4c9d0def1fa3af71a4a0e57e907a2b4986`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:9a37b479e68a0d18babbef8dd04d09a0e6844a0080876d14144a34bfd9d0897a in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:696a66e961f2033dcf69b003ad7faf28ed2248da58efa1c08a9d496739a8eeeb`  
		Last Modified: Wed, 20 Sep 2023 08:49:51 GMT  
		Size: 33.1 MB (33119461 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ba4c0c64bfd7ea845d20c793ede5957878785e4bb16e2e81a3e1ed5cd0d7ca0e`  
		Last Modified: Tue, 03 Oct 2023 19:02:08 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8a7ae673337cbb772a0ccc237ce4009a7dd88e4fed23861c9ea6382e93a6685b`  
		Last Modified: Tue, 03 Oct 2023 19:02:09 GMT  
		Size: 2.7 MB (2694930 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:766c713a6dbc39908803d95aa7556e0a571349c941bddb8f694b3f36030e0c3c`  
		Last Modified: Tue, 03 Oct 2023 19:02:10 GMT  
		Size: 13.8 MB (13819538 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:75734e09fa81ca91f8bdd1481c8f88f95ea9ba7b0f24ab82d0aee2026a5d6474`  
		Last Modified: Tue, 03 Oct 2023 19:02:09 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f46fc74a04a0607353cbc3ace76b49b44029af75080fa56fec872060d38feed2`  
		Last Modified: Tue, 03 Oct 2023 19:02:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6` - unknown; unknown

```console
$ docker pull memcached@sha256:d73c6167b49dd216e6395e8720af5bd26884a25473d1eb80ee31d1e4b170a914
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2914816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48964548656eeecac440cb41e4f3f474f861d384c569653e582e3d508b04f6e5`

```dockerfile
```

-	Layers:
	-	`sha256:4e89c387c1399e94faaaf407614d23c90aa3104b5773f87d8cb4fe4b20312f8e`  
		Last Modified: Tue, 03 Oct 2023 19:02:09 GMT  
		Size: 2.9 MB (2893143 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:fb96286b26618de71f0df13dfc89225bc855d6802341b4032f0fb4161cb4a52e`  
		Last Modified: Tue, 03 Oct 2023 19:02:08 GMT  
		Size: 21.7 KB (21673 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6` - linux; s390x

```console
$ docker pull memcached@sha256:42a17150fd8b17aff6910890bbab808eab97e6f9d0f60003e75fac6ddd2b0bcf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40575835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:956090eeead5cd8ec7753b439eb43ddf3b2c5cd93edea3d7ce5bcdd168ec7588`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:6ed982ad3e8566d63315a27a81b33069910952aef4b2d3e0b607bd2caeac7ca4 in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:26dcff366e33abcf08b812052a4c12496aa406aa267655e984aa7a84ca254cd8`  
		Last Modified: Wed, 20 Sep 2023 02:59:47 GMT  
		Size: 27.5 MB (27489966 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:04795616cce62da1faee69d189f2f4863a3818651e9f54e7552be41e35752766`  
		Last Modified: Tue, 03 Oct 2023 19:01:27 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cbacb720efba986e695a3270bc384924abb78c413d1c4793cd388fbab1da828b`  
		Last Modified: Tue, 03 Oct 2023 19:01:27 GMT  
		Size: 2.2 MB (2150908 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:07a927de051febdc6284e8ec146cbc267ffdd1049fadf2bc35639f53b72b7862`  
		Last Modified: Tue, 03 Oct 2023 19:01:28 GMT  
		Size: 10.9 MB (10933444 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5a2703a37bdc4f133106c52c5a040d30708c01a79aa0d1714bcba3b42105692e`  
		Last Modified: Tue, 03 Oct 2023 19:01:28 GMT  
		Size: 285.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c0a860b98e7d941cd44043f66c4cc9d2a540ab3b8cb9aa15123102865599e0c7`  
		Last Modified: Tue, 03 Oct 2023 19:01:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6` - unknown; unknown

```console
$ docker pull memcached@sha256:029d2884ff06e1b3673d9a7998c7299cc3da7ed18f46b344e13c14867574bae4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2897027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e57e1f9eb901fd307d1e2dd72b5606ba1f6f0ef82c31c01041513ed98e33b55`

```dockerfile
```

-	Layers:
	-	`sha256:13af4843cce0c7df5b25984623ef20fe08955ca99bbc64f5056c4d1bb2062f13`  
		Last Modified: Tue, 03 Oct 2023 19:01:27 GMT  
		Size: 2.9 MB (2875422 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:2e615a884e0baa9f5e54063b8983b99c841ac4fd854bf56780c1184d51637b1d`  
		Last Modified: Tue, 03 Oct 2023 19:01:27 GMT  
		Size: 21.6 KB (21605 bytes)  
		MIME: application/vnd.in-toto+json

## `memcached:1.6-alpine`

```console
$ docker pull memcached@sha256:535282ea08869aedc9bd20cbd714f07a27019c8b1e3aa64aa7321c96fb747844
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
$ docker pull memcached@sha256:27fe55ab0ecba9a8d3ddd67b823da4f1727d10eb46d36ab5af7e693421ebdb4f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4466251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3e0c0ff5c009f0e410e2fc6d29099b24315b4246c64cebae8068e86c22ba8a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["/bin/sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN apk add --no-cache libsasl # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3f9365fb2eebc56ba7006618c6ee8cde403af71bb4777c9b2b1c6ddcc107ee55`  
		Last Modified: Tue, 03 Oct 2023 19:01:12 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ec2c14990e92682477b554b5ccec603b864340a582d8ac4ab7becf52c09e9459`  
		Last Modified: Tue, 03 Oct 2023 19:01:12 GMT  
		Size: 108.0 KB (108015 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a0e994f33a8fb2b64e76f431cb35d0f0f92f0830352e44c589d8770bedfe96c3`  
		Last Modified: Tue, 03 Oct 2023 19:01:13 GMT  
		Size: 954.6 KB (954626 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:69c0dd1ede28d4dfdee1e54dc519270184463fa8812e781a930c0301b851c327`  
		Last Modified: Tue, 03 Oct 2023 19:01:12 GMT  
		Size: 277.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c9a4377466b783eeeab01987a823353e5cfbc2a5f02d632db14c654decf3ec5e`  
		Last Modified: Tue, 03 Oct 2023 19:01:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6-alpine` - unknown; unknown

```console
$ docker pull memcached@sha256:6ebfa6199008800194514397c12c233ea35c27ee5d22bea93fc978228a9f98f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.2 KB (95222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc3627763f4a9bb22db274ce8453a9d0146e88c0f4e0624f69059e5a9a69ec31`

```dockerfile
```

-	Layers:
	-	`sha256:7e739eda7910762ab0244ff165c2ff431bf4f10a39730614a8fca28a9a91b97d`  
		Last Modified: Tue, 03 Oct 2023 19:01:12 GMT  
		Size: 76.3 KB (76268 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:a04f216271188784dc836fa4905c7d5fbcfb49537cf5cfb5fe5b0229694cf12c`  
		Last Modified: Tue, 03 Oct 2023 19:01:12 GMT  
		Size: 19.0 KB (18954 bytes)  
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
$ docker pull memcached@sha256:1152b588a2cd7e90f0d7ae86fe3ce262e47c50c62642b5714b0019cef7779a00
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4401705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31bcc2b506321f6395c1d68cfc40f7391530051e5862186db1d5875e2c2803be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["/bin/sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN apk add --no-cache libsasl # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a8a999d5f4398538233c73f556a07cf646c7600543368cbc84b997cd76545de1`  
		Last Modified: Tue, 03 Oct 2023 19:03:35 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e035f8f759de7f5b35527c5cc46cd4132a10e0a501e022fbde2fedcf47fdd684`  
		Last Modified: Tue, 03 Oct 2023 19:03:35 GMT  
		Size: 124.1 KB (124080 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:585097acb28da9160246ad53fa72c119ac6e97a2852f420712485b66d6ed808a`  
		Last Modified: Tue, 03 Oct 2023 19:03:36 GMT  
		Size: 944.1 KB (944147 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:802f5f839e31fd8f8dd89ec2421af9fa8227dd43d5ca883f44d9ff2962cd0848`  
		Last Modified: Tue, 03 Oct 2023 19:03:35 GMT  
		Size: 281.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:65fc6300aa54fcd82f813153e3a5a880a2dca2a26edc3f7f907fe395a01a5474`  
		Last Modified: Tue, 03 Oct 2023 19:03:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6-alpine` - unknown; unknown

```console
$ docker pull memcached@sha256:5b2e4db4700ecd5765dd85cbc125a24968150122eb9f8181949dc39310085671
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.1 KB (95095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e78ca75a52728eb7207c54b73b899cb6919fd230b814373dc1612765d95bcc0c`

```dockerfile
```

-	Layers:
	-	`sha256:36799473bd1d28916d0df4c2af578542c27261dcc2dbba98964d2d7e956bd73f`  
		Last Modified: Tue, 03 Oct 2023 19:03:35 GMT  
		Size: 76.3 KB (76289 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:c088a7e985146394427f4d604d17a54445f5934b07e790774b7472540d932737`  
		Last Modified: Tue, 03 Oct 2023 19:03:35 GMT  
		Size: 18.8 KB (18806 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6-alpine` - linux; 386

```console
$ docker pull memcached@sha256:8b880914dfffd537639b55f5f49cf6c6e9f0773891eb922685e0ce94ccde66b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4283801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f38744e29d4692d1345bf5101db090800c52e9ae211735a610dd8e848ca426d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:8402753f294e403e92353bd65c86a6428c960be5116c0a15484b663a84f66fcd in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["/bin/sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN apk add --no-cache libsasl # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:dc95107ad2a031a015320bb397f73ec151d738127175b31ad643120697dc7e90`  
		Last Modified: Thu, 28 Sep 2023 20:39:32 GMT  
		Size: 3.2 MB (3235757 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f36c14bb55ad2eb4c208a601b1c61872c3725ed95c0c2893c27a822ed5c33a58`  
		Last Modified: Tue, 03 Oct 2023 19:01:33 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1298cb8dafd972511af84e02d7b883a21241c52cf40b58d6979490001961f21c`  
		Last Modified: Tue, 03 Oct 2023 19:01:33 GMT  
		Size: 109.5 KB (109459 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:df4a91e2b048d49e66ddd9893c09f30f39a1d597e80105c7f8962e7f5f7139d9`  
		Last Modified: Tue, 03 Oct 2023 19:01:33 GMT  
		Size: 936.9 KB (936943 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9907fafebdae96d5487b7fb8157a823f61825ffefba79657a80bce23a2545448`  
		Last Modified: Tue, 03 Oct 2023 19:01:34 GMT  
		Size: 276.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ee6a4d82ccc808127f6aaa710b646e700271ad4eff9c41b9965accad5d5d3788`  
		Last Modified: Tue, 03 Oct 2023 19:01:34 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6-alpine` - unknown; unknown

```console
$ docker pull memcached@sha256:fb404e06827e8d747912612afcca348dc58c4e9ee3ce83c4831cb09f12ab48fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 KB (18684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a050cea12e0cdebacb3a5a2ffc5ab6955496025789c041df169c407640f44bc8`

```dockerfile
```

-	Layers:
	-	`sha256:a3947c8d08a3d57e33242e44fb32c1cbd0106df35f9e5f83cb91293591da71c9`  
		Last Modified: Tue, 03 Oct 2023 19:01:33 GMT  
		Size: 18.7 KB (18684 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:32095d8b4daa6df8ff99e36c278c2cb210287066783a65050834bb28667fb2a2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4454721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26527e4ce577d5d1e1fdb3716fde4350e5a3ce0c3b3fd8dd527c6672f8eddcdf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["/bin/sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN apk add --no-cache libsasl # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9a6a9d9fc3b5def98513c33801853ba827c0c7bed9f2b4af3150b75fd4146d74`  
		Last Modified: Tue, 03 Oct 2023 19:06:17 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5dc7c33273d553c8b716261a6aee873fe5544c9200c9061bcc05b037a7c03ab5`  
		Last Modified: Tue, 03 Oct 2023 19:06:17 GMT  
		Size: 123.9 KB (123855 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0873dc2389c5bf83f2b2741fd0639e7dc70b2aa758884d63a794abe95622269b`  
		Last Modified: Tue, 03 Oct 2023 19:06:17 GMT  
		Size: 982.7 KB (982715 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:923b81392db2de0355d0715a2abf7bd7d715b4fac9d0bf39d5c08d7aeeed5270`  
		Last Modified: Tue, 03 Oct 2023 19:06:17 GMT  
		Size: 277.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dd619103d38407e95e05dd7d7f228e66bb5a61f3b561beb35198e92f9cdd0b99`  
		Last Modified: Tue, 03 Oct 2023 19:06:18 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6-alpine` - unknown; unknown

```console
$ docker pull memcached@sha256:aaa2281dd27a5acbf1364325e1d6ff0a576cfd236847437e2382c07b7199c2ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.3 KB (93262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f9ccd98630f55e4cdd33076a1d3e7f9c11399077a20d0aa9f5af15fcb40bd81`

```dockerfile
```

-	Layers:
	-	`sha256:9c3b535b067358c4894b956bcbf5380d163ce977d0c30028d799f467af8f87d6`  
		Last Modified: Tue, 03 Oct 2023 19:06:17 GMT  
		Size: 74.4 KB (74406 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:9d03d340727841dba89e688d83cd797f9808417dd8d04970fd76395482b117ff`  
		Last Modified: Tue, 03 Oct 2023 19:06:17 GMT  
		Size: 18.9 KB (18856 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6-alpine` - linux; s390x

```console
$ docker pull memcached@sha256:0ff7f30ca924f54a50160e70bd590b2ef357c97b6e8bbfcb81fdde97dd5cfbb0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4279633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad89852ec7f35640342fc548839c205af73d8c0f60e54c113b34e9dc519e71c3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["/bin/sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN apk add --no-cache libsasl # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1a648ad7883b3087dfacc17e14f4e6158d881dd1e09b9c5bd27bdd0d89ee44fd`  
		Last Modified: Tue, 03 Oct 2023 20:00:49 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a950f9727c19a31b79f709cdf984608d7788a9ed00dacbce4b14535b7589886f`  
		Last Modified: Tue, 03 Oct 2023 20:00:49 GMT  
		Size: 112.8 KB (112780 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b42424189685c7b481e859243008fea5d1967c6bbc3ccaaf13bf601c56926ebb`  
		Last Modified: Tue, 03 Oct 2023 20:00:49 GMT  
		Size: 950.1 KB (950102 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bf2263fe42a85daea831aafa6f50aeeef49d0ce1aa5841ddde0951667f85b684`  
		Last Modified: Tue, 03 Oct 2023 20:00:49 GMT  
		Size: 281.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:75eaf7af52231f2a4943c93eafc5d565b71c6079a1fee0fdc2605ad3eb81cd58`  
		Last Modified: Tue, 03 Oct 2023 20:00:49 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6-alpine` - unknown; unknown

```console
$ docker pull memcached@sha256:d2b9bd3538d99a100b4ebf104d9d5029917eecd3eec97d7086f7e4244b373d10
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.1 KB (93124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ade4e328bfbe610c689ab718878e6d07c31e5b67895795550a21d77730847d83`

```dockerfile
```

-	Layers:
	-	`sha256:7350d7c047abc3727f9639268d2cc1a5d7e53cbc81ae534da5e93272b5a48b59`  
		Last Modified: Tue, 03 Oct 2023 20:00:49 GMT  
		Size: 74.3 KB (74336 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:39706e52b9159fe158fe5027b73cb21482efb8781e1ab8853bcb19fc8125bbc8`  
		Last Modified: Tue, 03 Oct 2023 20:00:49 GMT  
		Size: 18.8 KB (18788 bytes)  
		MIME: application/vnd.in-toto+json

## `memcached:1.6-alpine3.18`

```console
$ docker pull memcached@sha256:eaba3015e1bf3a26f3d14ed455ef867e00d395963d0523c4275258f4890af5e1
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
$ docker pull memcached@sha256:27fe55ab0ecba9a8d3ddd67b823da4f1727d10eb46d36ab5af7e693421ebdb4f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4466251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3e0c0ff5c009f0e410e2fc6d29099b24315b4246c64cebae8068e86c22ba8a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["/bin/sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN apk add --no-cache libsasl # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3f9365fb2eebc56ba7006618c6ee8cde403af71bb4777c9b2b1c6ddcc107ee55`  
		Last Modified: Tue, 03 Oct 2023 19:01:12 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ec2c14990e92682477b554b5ccec603b864340a582d8ac4ab7becf52c09e9459`  
		Last Modified: Tue, 03 Oct 2023 19:01:12 GMT  
		Size: 108.0 KB (108015 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a0e994f33a8fb2b64e76f431cb35d0f0f92f0830352e44c589d8770bedfe96c3`  
		Last Modified: Tue, 03 Oct 2023 19:01:13 GMT  
		Size: 954.6 KB (954626 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:69c0dd1ede28d4dfdee1e54dc519270184463fa8812e781a930c0301b851c327`  
		Last Modified: Tue, 03 Oct 2023 19:01:12 GMT  
		Size: 277.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c9a4377466b783eeeab01987a823353e5cfbc2a5f02d632db14c654decf3ec5e`  
		Last Modified: Tue, 03 Oct 2023 19:01:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6-alpine3.18` - unknown; unknown

```console
$ docker pull memcached@sha256:6ebfa6199008800194514397c12c233ea35c27ee5d22bea93fc978228a9f98f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.2 KB (95222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc3627763f4a9bb22db274ce8453a9d0146e88c0f4e0624f69059e5a9a69ec31`

```dockerfile
```

-	Layers:
	-	`sha256:7e739eda7910762ab0244ff165c2ff431bf4f10a39730614a8fca28a9a91b97d`  
		Last Modified: Tue, 03 Oct 2023 19:01:12 GMT  
		Size: 76.3 KB (76268 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:a04f216271188784dc836fa4905c7d5fbcfb49537cf5cfb5fe5b0229694cf12c`  
		Last Modified: Tue, 03 Oct 2023 19:01:12 GMT  
		Size: 19.0 KB (18954 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:1152b588a2cd7e90f0d7ae86fe3ce262e47c50c62642b5714b0019cef7779a00
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4401705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31bcc2b506321f6395c1d68cfc40f7391530051e5862186db1d5875e2c2803be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["/bin/sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN apk add --no-cache libsasl # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a8a999d5f4398538233c73f556a07cf646c7600543368cbc84b997cd76545de1`  
		Last Modified: Tue, 03 Oct 2023 19:03:35 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e035f8f759de7f5b35527c5cc46cd4132a10e0a501e022fbde2fedcf47fdd684`  
		Last Modified: Tue, 03 Oct 2023 19:03:35 GMT  
		Size: 124.1 KB (124080 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:585097acb28da9160246ad53fa72c119ac6e97a2852f420712485b66d6ed808a`  
		Last Modified: Tue, 03 Oct 2023 19:03:36 GMT  
		Size: 944.1 KB (944147 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:802f5f839e31fd8f8dd89ec2421af9fa8227dd43d5ca883f44d9ff2962cd0848`  
		Last Modified: Tue, 03 Oct 2023 19:03:35 GMT  
		Size: 281.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:65fc6300aa54fcd82f813153e3a5a880a2dca2a26edc3f7f907fe395a01a5474`  
		Last Modified: Tue, 03 Oct 2023 19:03:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6-alpine3.18` - unknown; unknown

```console
$ docker pull memcached@sha256:5b2e4db4700ecd5765dd85cbc125a24968150122eb9f8181949dc39310085671
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.1 KB (95095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e78ca75a52728eb7207c54b73b899cb6919fd230b814373dc1612765d95bcc0c`

```dockerfile
```

-	Layers:
	-	`sha256:36799473bd1d28916d0df4c2af578542c27261dcc2dbba98964d2d7e956bd73f`  
		Last Modified: Tue, 03 Oct 2023 19:03:35 GMT  
		Size: 76.3 KB (76289 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:c088a7e985146394427f4d604d17a54445f5934b07e790774b7472540d932737`  
		Last Modified: Tue, 03 Oct 2023 19:03:35 GMT  
		Size: 18.8 KB (18806 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6-alpine3.18` - linux; 386

```console
$ docker pull memcached@sha256:8b880914dfffd537639b55f5f49cf6c6e9f0773891eb922685e0ce94ccde66b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4283801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f38744e29d4692d1345bf5101db090800c52e9ae211735a610dd8e848ca426d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:8402753f294e403e92353bd65c86a6428c960be5116c0a15484b663a84f66fcd in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["/bin/sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN apk add --no-cache libsasl # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:dc95107ad2a031a015320bb397f73ec151d738127175b31ad643120697dc7e90`  
		Last Modified: Thu, 28 Sep 2023 20:39:32 GMT  
		Size: 3.2 MB (3235757 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f36c14bb55ad2eb4c208a601b1c61872c3725ed95c0c2893c27a822ed5c33a58`  
		Last Modified: Tue, 03 Oct 2023 19:01:33 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1298cb8dafd972511af84e02d7b883a21241c52cf40b58d6979490001961f21c`  
		Last Modified: Tue, 03 Oct 2023 19:01:33 GMT  
		Size: 109.5 KB (109459 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:df4a91e2b048d49e66ddd9893c09f30f39a1d597e80105c7f8962e7f5f7139d9`  
		Last Modified: Tue, 03 Oct 2023 19:01:33 GMT  
		Size: 936.9 KB (936943 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9907fafebdae96d5487b7fb8157a823f61825ffefba79657a80bce23a2545448`  
		Last Modified: Tue, 03 Oct 2023 19:01:34 GMT  
		Size: 276.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ee6a4d82ccc808127f6aaa710b646e700271ad4eff9c41b9965accad5d5d3788`  
		Last Modified: Tue, 03 Oct 2023 19:01:34 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6-alpine3.18` - unknown; unknown

```console
$ docker pull memcached@sha256:fb404e06827e8d747912612afcca348dc58c4e9ee3ce83c4831cb09f12ab48fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 KB (18684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a050cea12e0cdebacb3a5a2ffc5ab6955496025789c041df169c407640f44bc8`

```dockerfile
```

-	Layers:
	-	`sha256:a3947c8d08a3d57e33242e44fb32c1cbd0106df35f9e5f83cb91293591da71c9`  
		Last Modified: Tue, 03 Oct 2023 19:01:33 GMT  
		Size: 18.7 KB (18684 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6-alpine3.18` - linux; ppc64le

```console
$ docker pull memcached@sha256:32095d8b4daa6df8ff99e36c278c2cb210287066783a65050834bb28667fb2a2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4454721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26527e4ce577d5d1e1fdb3716fde4350e5a3ce0c3b3fd8dd527c6672f8eddcdf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["/bin/sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN apk add --no-cache libsasl # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9a6a9d9fc3b5def98513c33801853ba827c0c7bed9f2b4af3150b75fd4146d74`  
		Last Modified: Tue, 03 Oct 2023 19:06:17 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5dc7c33273d553c8b716261a6aee873fe5544c9200c9061bcc05b037a7c03ab5`  
		Last Modified: Tue, 03 Oct 2023 19:06:17 GMT  
		Size: 123.9 KB (123855 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0873dc2389c5bf83f2b2741fd0639e7dc70b2aa758884d63a794abe95622269b`  
		Last Modified: Tue, 03 Oct 2023 19:06:17 GMT  
		Size: 982.7 KB (982715 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:923b81392db2de0355d0715a2abf7bd7d715b4fac9d0bf39d5c08d7aeeed5270`  
		Last Modified: Tue, 03 Oct 2023 19:06:17 GMT  
		Size: 277.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dd619103d38407e95e05dd7d7f228e66bb5a61f3b561beb35198e92f9cdd0b99`  
		Last Modified: Tue, 03 Oct 2023 19:06:18 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6-alpine3.18` - unknown; unknown

```console
$ docker pull memcached@sha256:aaa2281dd27a5acbf1364325e1d6ff0a576cfd236847437e2382c07b7199c2ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.3 KB (93262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f9ccd98630f55e4cdd33076a1d3e7f9c11399077a20d0aa9f5af15fcb40bd81`

```dockerfile
```

-	Layers:
	-	`sha256:9c3b535b067358c4894b956bcbf5380d163ce977d0c30028d799f467af8f87d6`  
		Last Modified: Tue, 03 Oct 2023 19:06:17 GMT  
		Size: 74.4 KB (74406 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:9d03d340727841dba89e688d83cd797f9808417dd8d04970fd76395482b117ff`  
		Last Modified: Tue, 03 Oct 2023 19:06:17 GMT  
		Size: 18.9 KB (18856 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6-alpine3.18` - linux; s390x

```console
$ docker pull memcached@sha256:0ff7f30ca924f54a50160e70bd590b2ef357c97b6e8bbfcb81fdde97dd5cfbb0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4279633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad89852ec7f35640342fc548839c205af73d8c0f60e54c113b34e9dc519e71c3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["/bin/sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN apk add --no-cache libsasl # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1a648ad7883b3087dfacc17e14f4e6158d881dd1e09b9c5bd27bdd0d89ee44fd`  
		Last Modified: Tue, 03 Oct 2023 20:00:49 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a950f9727c19a31b79f709cdf984608d7788a9ed00dacbce4b14535b7589886f`  
		Last Modified: Tue, 03 Oct 2023 20:00:49 GMT  
		Size: 112.8 KB (112780 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b42424189685c7b481e859243008fea5d1967c6bbc3ccaaf13bf601c56926ebb`  
		Last Modified: Tue, 03 Oct 2023 20:00:49 GMT  
		Size: 950.1 KB (950102 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bf2263fe42a85daea831aafa6f50aeeef49d0ce1aa5841ddde0951667f85b684`  
		Last Modified: Tue, 03 Oct 2023 20:00:49 GMT  
		Size: 281.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:75eaf7af52231f2a4943c93eafc5d565b71c6079a1fee0fdc2605ad3eb81cd58`  
		Last Modified: Tue, 03 Oct 2023 20:00:49 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6-alpine3.18` - unknown; unknown

```console
$ docker pull memcached@sha256:d2b9bd3538d99a100b4ebf104d9d5029917eecd3eec97d7086f7e4244b373d10
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.1 KB (93124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ade4e328bfbe610c689ab718878e6d07c31e5b67895795550a21d77730847d83`

```dockerfile
```

-	Layers:
	-	`sha256:7350d7c047abc3727f9639268d2cc1a5d7e53cbc81ae534da5e93272b5a48b59`  
		Last Modified: Tue, 03 Oct 2023 20:00:49 GMT  
		Size: 74.3 KB (74336 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:39706e52b9159fe158fe5027b73cb21482efb8781e1ab8853bcb19fc8125bbc8`  
		Last Modified: Tue, 03 Oct 2023 20:00:49 GMT  
		Size: 18.8 KB (18788 bytes)  
		MIME: application/vnd.in-toto+json

## `memcached:1.6-bookworm`

```console
$ docker pull memcached@sha256:eef4a056175ad8203df2a1835ae16307e5a70aec3222b409d1114486b2a4bb65
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
$ docker pull memcached@sha256:8af51889f0f774a00f36624e58faac309c258eafb8054c6abc6fbbb56c78d0a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.8 MB (38811465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fa23f6ace109fad9223ea2db53f79afa8b91b14051c61305f82bc2c781a788c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:55ad846fa191e603f48090eae0e4a7149c4066b94406593ec1898ad2c3347937 in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a378f10b321842c3042cdeff4f6997f34f4cb21f2eff27704b7f6193ab7b5fea`  
		Last Modified: Wed, 11 Oct 2023 18:39:34 GMT  
		Size: 29.1 MB (29149874 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e68aaf702a54364b3f216204ad2725f5b416fe496294086899b821bb5133552d`  
		Last Modified: Wed, 11 Oct 2023 20:07:27 GMT  
		Size: 1.1 KB (1110 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0fb853802e1447e9b1dbe3e8a86f27a5691286127397adf8d52f943d16b80042`  
		Last Modified: Wed, 11 Oct 2023 20:07:27 GMT  
		Size: 2.5 MB (2488274 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fcc9694d882f053fcf2e7bb33709dcb86eef6c29c3187c190ad93852af7a50f2`  
		Last Modified: Wed, 11 Oct 2023 20:07:28 GMT  
		Size: 7.2 MB (7171802 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fde136907f7040bd6126a5b2c0bca844fef33e2fc804c1f135e99393869cce4c`  
		Last Modified: Wed, 11 Oct 2023 20:07:27 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c121d0db5ccb2988b1fc0c76ce60a2e78309d77b264adf99e815e1ecf2c6a957`  
		Last Modified: Wed, 11 Oct 2023 20:07:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:888d3aaaddc944acb247f0e42586c8c8a7f8c3262166ee89ceda0dbe3998cafa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2911211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06530a2f7a54ba7d86fc6cee0da9a46ea1aea89dc4beecbee6d54ed8eee82dd9`

```dockerfile
```

-	Layers:
	-	`sha256:7bbbdfb4ba86ed51b46d2fb83bf8cf4e095da6d5c9dd89697a3488dd392414d7`  
		Last Modified: Wed, 11 Oct 2023 20:07:27 GMT  
		Size: 2.9 MB (2889442 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:6fe7a995830937695f7110928df7e791673ab04015add73a1f2e9ec661bbc60f`  
		Last Modified: Wed, 11 Oct 2023 20:07:27 GMT  
		Size: 21.8 KB (21769 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6-bookworm` - linux; arm variant v5

```console
$ docker pull memcached@sha256:a6919fc9976aa2c291f194860f40fcc9499d33cbd2592af9087e5d64b7930602
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34846023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5222dddac963b84d55ef902d40fa3f949ee73caac9614ca77c1f4a81ef009c6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:8c43adb3245fc6f2b10aa5a86c850db5dcf3515eaf7e46630922fe21f806bd2a in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:904e6393ef1ee28b37171369eb4f7cb04714631c711799819fccb83886bd212b`  
		Last Modified: Wed, 11 Oct 2023 17:40:47 GMT  
		Size: 26.9 MB (26922150 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f0569355cb85b70d6a614ea9604289ce8e724f0f9ff4d1d8a12afc24c4c9ad1f`  
		Last Modified: Thu, 12 Oct 2023 08:32:05 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6939032c8ff0687b012a85d3411c702266b934a677f96eb521658b44f5b4a8c0`  
		Last Modified: Thu, 12 Oct 2023 08:32:06 GMT  
		Size: 2.1 MB (2089182 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8e8a2a7338b5cacc7b6e4e3db2359eebb1936b0b14266d5bad0dfcc21c9becff`  
		Last Modified: Thu, 12 Oct 2023 08:32:06 GMT  
		Size: 5.8 MB (5833176 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:19f35a8116fe7e124bee612b2ac511694077a1f35f76ed056903987ab4921e34`  
		Last Modified: Thu, 12 Oct 2023 08:32:06 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a43775be6dfac6c255e35b164eacd7328df241f33f9245206a8eaf481062ccbc`  
		Last Modified: Thu, 12 Oct 2023 08:32:07 GMT  
		Size: 120.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:f1276a05a4db6e8b7bb9d8374d480b85a79f1b92d4e7475c65e247bf1427200c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.7 KB (21695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe67b683a818ed7c22a49086ec4f22e53c6efa9040becea46adb07f550dae564`

```dockerfile
```

-	Layers:
	-	`sha256:12ecc330d2059d33dc7a7c518e7be06804f5fcadafdc8e2db030631f5c92b326`  
		Last Modified: Thu, 12 Oct 2023 08:32:05 GMT  
		Size: 21.7 KB (21695 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6-bookworm` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:0c25b3c626a396c236dcf08792c850a178482c24e0c9dab0e784783178d10c13
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.4 MB (43442272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1595a8aa58bfc22ba6e995a58c63ea8b660aa8a9b10c57ab0cb8552d94080218`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:ec1a6e0aedd76c8fdc8544775f8b553f58950e9435f5cfe919f39374e222cfbb in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:e886f0f47ef56fcadb6ecaf2116056bbdb273e0afe07ed034498b198d386c04e`  
		Last Modified: Wed, 20 Sep 2023 02:47:36 GMT  
		Size: 29.2 MB (29157221 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7e25b15fcaee53caa22717c5b0b52fabf2480b0244a84530fca4c1edbb812044`  
		Last Modified: Tue, 03 Oct 2023 19:00:54 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:72fc5c44d6b752d2c2534f97f12ef44f915803ec4e564d7c9eb90d9d7bda2297`  
		Last Modified: Tue, 03 Oct 2023 19:00:54 GMT  
		Size: 2.3 MB (2343087 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7ba30437e42c2aebda3182e43b83b90012dd19e31adb9dc25bb3b714385cdefe`  
		Last Modified: Tue, 03 Oct 2023 19:00:55 GMT  
		Size: 11.9 MB (11940448 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:70abb5efa4268d01b1dfe9f6775f8f85a7fe395141dcc28909aa52ea6b741971`  
		Last Modified: Tue, 03 Oct 2023 19:00:54 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5a87a9f60806e352855b340f2c0c3610b8053006f0f542077c3add7e70782663`  
		Last Modified: Tue, 03 Oct 2023 19:00:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:7a900749c7d177577d906a5d402b4a008b95ae3571e9de24b4f04060e8650d5d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2890735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:711e633b20942471e455d3210316a79109ffda2a13cb38f46bd9ab2d27c758ae`

```dockerfile
```

-	Layers:
	-	`sha256:6c4c4a32fc3b330e635796951e46bf9e6ed753212798e75baddd3a84e752de8c`  
		Last Modified: Tue, 03 Oct 2023 19:00:54 GMT  
		Size: 2.9 MB (2869112 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:d0ceb647ed388f03f95faf34bc93c1489afde267801855f46cfca84fca538c5a`  
		Last Modified: Tue, 03 Oct 2023 19:00:54 GMT  
		Size: 21.6 KB (21623 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6-bookworm` - linux; 386

```console
$ docker pull memcached@sha256:dbf6fdd168abcb8b6fd831277bea0213784e54cdb824756684dd3b5337c42c65
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.6 MB (44649134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25680867a5df0eb88860f59d7855c9d7f3862a44283c1e59d608f9dbecff348b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:efe81f7066129aa6293627bfe4ea78b957897ba5ede951970156fccf1dbcde88 in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6ac07f93e07a1bad4555e13bd8efd06169988669fc88df95f4bf296a2b44523d`  
		Last Modified: Wed, 20 Sep 2023 00:46:48 GMT  
		Size: 30.1 MB (30141894 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:797b4215eddcf948eec0f19132f85ec1b0f3af264399e78d860bece37acc4888`  
		Last Modified: Tue, 03 Oct 2023 19:01:51 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3c78c0b20e6791912325d174e98f60d4f783c2f013f52ff3835892444d3a15d7`  
		Last Modified: Tue, 03 Oct 2023 19:01:51 GMT  
		Size: 2.5 MB (2490464 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c91bf1cea723f722413107daa57ab51060ab36a5f78fe8447568aa35be54fca5`  
		Last Modified: Tue, 03 Oct 2023 19:01:52 GMT  
		Size: 12.0 MB (12015261 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:07f7206e609641792c84dfac85e3e6df0602c4ca8d572353a8768ff0619fe328`  
		Last Modified: Tue, 03 Oct 2023 19:01:51 GMT  
		Size: 283.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7aac14495f4a088e0e208638d0b36b0b5ff0cf945aaf24c011ef08ca799279a9`  
		Last Modified: Tue, 03 Oct 2023 19:01:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:16c8db3d95a2df8fae160a3942ff033ebb3bf6d9fe8df1643eb22c82e9402357
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 KB (21502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03bc49cf22d3ede52afc78d429b09999ba28174660a5e1b41fdb0f9d3a47067c`

```dockerfile
```

-	Layers:
	-	`sha256:890c3f7af1536aa0821f27c4ba142e022ba0c892f1310b4d82a9cc3a74717139`  
		Last Modified: Tue, 03 Oct 2023 19:01:51 GMT  
		Size: 21.5 KB (21502 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6-bookworm` - linux; mips64le

```console
$ docker pull memcached@sha256:575825bdbf62fc255547394ef491710ba88f0be3ca735eaf246ece06f13363ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.4 MB (43398233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e3f951153522f4d9719c37a9862412f3e29e487d11322c5ff7a009cf8becca1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:850547a08e38ebc5a3659df86e70039a8d9828ae26ae485b077c98a959248dcb in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:0f581c6294fe7421dfee024e2c7dddd73ef3fbd7ff23b05bc3c1bf9f50885e85`  
		Last Modified: Wed, 20 Sep 2023 03:20:59 GMT  
		Size: 29.1 MB (29121674 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:15e25af5488ea4ad0df132fa2c22a282c1a17ad1460cdb25fe5939e03a753528`  
		Last Modified: Tue, 03 Oct 2023 19:04:40 GMT  
		Size: 1.1 KB (1113 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:19a5f416c9bf283212262e33fe8529d0ff3917fcee1e8ca9fb058170fd528211`  
		Last Modified: Tue, 03 Oct 2023 19:04:41 GMT  
		Size: 1.9 MB (1934931 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:05862af95003d85f9a1b5696dfb3588bdd8e34c74f067d845b722d70edfc679f`  
		Last Modified: Tue, 03 Oct 2023 19:04:41 GMT  
		Size: 12.3 MB (12340111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e8aae13855c46b73d2506b2d91036f6f0b4bc63b7d7ec12ecc63fd672c64c0f7`  
		Last Modified: Tue, 03 Oct 2023 19:04:40 GMT  
		Size: 282.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0709f88ce6a011ea45fd41c091ee6fcf4baa0610e0591a9fe0d10626eaf9475f`  
		Last Modified: Tue, 03 Oct 2023 19:04:41 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:269b3e28059bf711ac45886388e91fa405b8a1e0ca1a114acefc997bbdad6d05
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 KB (21491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1059a2662b538952006866f53463fcea773b5e090eaead3a4ad49f4d0a656ae5`

```dockerfile
```

-	Layers:
	-	`sha256:e1052b07541ae6e041e59834c527075b62df62a33f7a9b9e96fda4b6237e83df`  
		Last Modified: Tue, 03 Oct 2023 19:04:40 GMT  
		Size: 21.5 KB (21491 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6-bookworm` - linux; ppc64le

```console
$ docker pull memcached@sha256:532cf0a6053275c508a0503017b4f52ce356a64aba047eb2316bdcaca35bbc9a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49635445 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:111f6d9d894ab95e36b94efa3dad4a4c9d0def1fa3af71a4a0e57e907a2b4986`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:9a37b479e68a0d18babbef8dd04d09a0e6844a0080876d14144a34bfd9d0897a in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:696a66e961f2033dcf69b003ad7faf28ed2248da58efa1c08a9d496739a8eeeb`  
		Last Modified: Wed, 20 Sep 2023 08:49:51 GMT  
		Size: 33.1 MB (33119461 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ba4c0c64bfd7ea845d20c793ede5957878785e4bb16e2e81a3e1ed5cd0d7ca0e`  
		Last Modified: Tue, 03 Oct 2023 19:02:08 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8a7ae673337cbb772a0ccc237ce4009a7dd88e4fed23861c9ea6382e93a6685b`  
		Last Modified: Tue, 03 Oct 2023 19:02:09 GMT  
		Size: 2.7 MB (2694930 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:766c713a6dbc39908803d95aa7556e0a571349c941bddb8f694b3f36030e0c3c`  
		Last Modified: Tue, 03 Oct 2023 19:02:10 GMT  
		Size: 13.8 MB (13819538 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:75734e09fa81ca91f8bdd1481c8f88f95ea9ba7b0f24ab82d0aee2026a5d6474`  
		Last Modified: Tue, 03 Oct 2023 19:02:09 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f46fc74a04a0607353cbc3ace76b49b44029af75080fa56fec872060d38feed2`  
		Last Modified: Tue, 03 Oct 2023 19:02:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:d73c6167b49dd216e6395e8720af5bd26884a25473d1eb80ee31d1e4b170a914
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2914816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48964548656eeecac440cb41e4f3f474f861d384c569653e582e3d508b04f6e5`

```dockerfile
```

-	Layers:
	-	`sha256:4e89c387c1399e94faaaf407614d23c90aa3104b5773f87d8cb4fe4b20312f8e`  
		Last Modified: Tue, 03 Oct 2023 19:02:09 GMT  
		Size: 2.9 MB (2893143 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:fb96286b26618de71f0df13dfc89225bc855d6802341b4032f0fb4161cb4a52e`  
		Last Modified: Tue, 03 Oct 2023 19:02:08 GMT  
		Size: 21.7 KB (21673 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6-bookworm` - linux; s390x

```console
$ docker pull memcached@sha256:42a17150fd8b17aff6910890bbab808eab97e6f9d0f60003e75fac6ddd2b0bcf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40575835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:956090eeead5cd8ec7753b439eb43ddf3b2c5cd93edea3d7ce5bcdd168ec7588`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:6ed982ad3e8566d63315a27a81b33069910952aef4b2d3e0b607bd2caeac7ca4 in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:26dcff366e33abcf08b812052a4c12496aa406aa267655e984aa7a84ca254cd8`  
		Last Modified: Wed, 20 Sep 2023 02:59:47 GMT  
		Size: 27.5 MB (27489966 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:04795616cce62da1faee69d189f2f4863a3818651e9f54e7552be41e35752766`  
		Last Modified: Tue, 03 Oct 2023 19:01:27 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cbacb720efba986e695a3270bc384924abb78c413d1c4793cd388fbab1da828b`  
		Last Modified: Tue, 03 Oct 2023 19:01:27 GMT  
		Size: 2.2 MB (2150908 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:07a927de051febdc6284e8ec146cbc267ffdd1049fadf2bc35639f53b72b7862`  
		Last Modified: Tue, 03 Oct 2023 19:01:28 GMT  
		Size: 10.9 MB (10933444 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5a2703a37bdc4f133106c52c5a040d30708c01a79aa0d1714bcba3b42105692e`  
		Last Modified: Tue, 03 Oct 2023 19:01:28 GMT  
		Size: 285.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c0a860b98e7d941cd44043f66c4cc9d2a540ab3b8cb9aa15123102865599e0c7`  
		Last Modified: Tue, 03 Oct 2023 19:01:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:029d2884ff06e1b3673d9a7998c7299cc3da7ed18f46b344e13c14867574bae4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2897027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e57e1f9eb901fd307d1e2dd72b5606ba1f6f0ef82c31c01041513ed98e33b55`

```dockerfile
```

-	Layers:
	-	`sha256:13af4843cce0c7df5b25984623ef20fe08955ca99bbc64f5056c4d1bb2062f13`  
		Last Modified: Tue, 03 Oct 2023 19:01:27 GMT  
		Size: 2.9 MB (2875422 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:2e615a884e0baa9f5e54063b8983b99c841ac4fd854bf56780c1184d51637b1d`  
		Last Modified: Tue, 03 Oct 2023 19:01:27 GMT  
		Size: 21.6 KB (21605 bytes)  
		MIME: application/vnd.in-toto+json

## `memcached:1.6.21`

```console
$ docker pull memcached@sha256:eef4a056175ad8203df2a1835ae16307e5a70aec3222b409d1114486b2a4bb65
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

### `memcached:1.6.21` - linux; amd64

```console
$ docker pull memcached@sha256:8af51889f0f774a00f36624e58faac309c258eafb8054c6abc6fbbb56c78d0a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.8 MB (38811465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fa23f6ace109fad9223ea2db53f79afa8b91b14051c61305f82bc2c781a788c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:55ad846fa191e603f48090eae0e4a7149c4066b94406593ec1898ad2c3347937 in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a378f10b321842c3042cdeff4f6997f34f4cb21f2eff27704b7f6193ab7b5fea`  
		Last Modified: Wed, 11 Oct 2023 18:39:34 GMT  
		Size: 29.1 MB (29149874 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e68aaf702a54364b3f216204ad2725f5b416fe496294086899b821bb5133552d`  
		Last Modified: Wed, 11 Oct 2023 20:07:27 GMT  
		Size: 1.1 KB (1110 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0fb853802e1447e9b1dbe3e8a86f27a5691286127397adf8d52f943d16b80042`  
		Last Modified: Wed, 11 Oct 2023 20:07:27 GMT  
		Size: 2.5 MB (2488274 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fcc9694d882f053fcf2e7bb33709dcb86eef6c29c3187c190ad93852af7a50f2`  
		Last Modified: Wed, 11 Oct 2023 20:07:28 GMT  
		Size: 7.2 MB (7171802 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fde136907f7040bd6126a5b2c0bca844fef33e2fc804c1f135e99393869cce4c`  
		Last Modified: Wed, 11 Oct 2023 20:07:27 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c121d0db5ccb2988b1fc0c76ce60a2e78309d77b264adf99e815e1ecf2c6a957`  
		Last Modified: Wed, 11 Oct 2023 20:07:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.21` - unknown; unknown

```console
$ docker pull memcached@sha256:888d3aaaddc944acb247f0e42586c8c8a7f8c3262166ee89ceda0dbe3998cafa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2911211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06530a2f7a54ba7d86fc6cee0da9a46ea1aea89dc4beecbee6d54ed8eee82dd9`

```dockerfile
```

-	Layers:
	-	`sha256:7bbbdfb4ba86ed51b46d2fb83bf8cf4e095da6d5c9dd89697a3488dd392414d7`  
		Last Modified: Wed, 11 Oct 2023 20:07:27 GMT  
		Size: 2.9 MB (2889442 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:6fe7a995830937695f7110928df7e791673ab04015add73a1f2e9ec661bbc60f`  
		Last Modified: Wed, 11 Oct 2023 20:07:27 GMT  
		Size: 21.8 KB (21769 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6.21` - linux; arm variant v5

```console
$ docker pull memcached@sha256:a6919fc9976aa2c291f194860f40fcc9499d33cbd2592af9087e5d64b7930602
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34846023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5222dddac963b84d55ef902d40fa3f949ee73caac9614ca77c1f4a81ef009c6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:8c43adb3245fc6f2b10aa5a86c850db5dcf3515eaf7e46630922fe21f806bd2a in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:904e6393ef1ee28b37171369eb4f7cb04714631c711799819fccb83886bd212b`  
		Last Modified: Wed, 11 Oct 2023 17:40:47 GMT  
		Size: 26.9 MB (26922150 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f0569355cb85b70d6a614ea9604289ce8e724f0f9ff4d1d8a12afc24c4c9ad1f`  
		Last Modified: Thu, 12 Oct 2023 08:32:05 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6939032c8ff0687b012a85d3411c702266b934a677f96eb521658b44f5b4a8c0`  
		Last Modified: Thu, 12 Oct 2023 08:32:06 GMT  
		Size: 2.1 MB (2089182 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8e8a2a7338b5cacc7b6e4e3db2359eebb1936b0b14266d5bad0dfcc21c9becff`  
		Last Modified: Thu, 12 Oct 2023 08:32:06 GMT  
		Size: 5.8 MB (5833176 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:19f35a8116fe7e124bee612b2ac511694077a1f35f76ed056903987ab4921e34`  
		Last Modified: Thu, 12 Oct 2023 08:32:06 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a43775be6dfac6c255e35b164eacd7328df241f33f9245206a8eaf481062ccbc`  
		Last Modified: Thu, 12 Oct 2023 08:32:07 GMT  
		Size: 120.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.21` - unknown; unknown

```console
$ docker pull memcached@sha256:f1276a05a4db6e8b7bb9d8374d480b85a79f1b92d4e7475c65e247bf1427200c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.7 KB (21695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe67b683a818ed7c22a49086ec4f22e53c6efa9040becea46adb07f550dae564`

```dockerfile
```

-	Layers:
	-	`sha256:12ecc330d2059d33dc7a7c518e7be06804f5fcadafdc8e2db030631f5c92b326`  
		Last Modified: Thu, 12 Oct 2023 08:32:05 GMT  
		Size: 21.7 KB (21695 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6.21` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:0c25b3c626a396c236dcf08792c850a178482c24e0c9dab0e784783178d10c13
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.4 MB (43442272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1595a8aa58bfc22ba6e995a58c63ea8b660aa8a9b10c57ab0cb8552d94080218`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:ec1a6e0aedd76c8fdc8544775f8b553f58950e9435f5cfe919f39374e222cfbb in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:e886f0f47ef56fcadb6ecaf2116056bbdb273e0afe07ed034498b198d386c04e`  
		Last Modified: Wed, 20 Sep 2023 02:47:36 GMT  
		Size: 29.2 MB (29157221 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7e25b15fcaee53caa22717c5b0b52fabf2480b0244a84530fca4c1edbb812044`  
		Last Modified: Tue, 03 Oct 2023 19:00:54 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:72fc5c44d6b752d2c2534f97f12ef44f915803ec4e564d7c9eb90d9d7bda2297`  
		Last Modified: Tue, 03 Oct 2023 19:00:54 GMT  
		Size: 2.3 MB (2343087 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7ba30437e42c2aebda3182e43b83b90012dd19e31adb9dc25bb3b714385cdefe`  
		Last Modified: Tue, 03 Oct 2023 19:00:55 GMT  
		Size: 11.9 MB (11940448 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:70abb5efa4268d01b1dfe9f6775f8f85a7fe395141dcc28909aa52ea6b741971`  
		Last Modified: Tue, 03 Oct 2023 19:00:54 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5a87a9f60806e352855b340f2c0c3610b8053006f0f542077c3add7e70782663`  
		Last Modified: Tue, 03 Oct 2023 19:00:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.21` - unknown; unknown

```console
$ docker pull memcached@sha256:7a900749c7d177577d906a5d402b4a008b95ae3571e9de24b4f04060e8650d5d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2890735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:711e633b20942471e455d3210316a79109ffda2a13cb38f46bd9ab2d27c758ae`

```dockerfile
```

-	Layers:
	-	`sha256:6c4c4a32fc3b330e635796951e46bf9e6ed753212798e75baddd3a84e752de8c`  
		Last Modified: Tue, 03 Oct 2023 19:00:54 GMT  
		Size: 2.9 MB (2869112 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:d0ceb647ed388f03f95faf34bc93c1489afde267801855f46cfca84fca538c5a`  
		Last Modified: Tue, 03 Oct 2023 19:00:54 GMT  
		Size: 21.6 KB (21623 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6.21` - linux; 386

```console
$ docker pull memcached@sha256:dbf6fdd168abcb8b6fd831277bea0213784e54cdb824756684dd3b5337c42c65
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.6 MB (44649134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25680867a5df0eb88860f59d7855c9d7f3862a44283c1e59d608f9dbecff348b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:efe81f7066129aa6293627bfe4ea78b957897ba5ede951970156fccf1dbcde88 in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6ac07f93e07a1bad4555e13bd8efd06169988669fc88df95f4bf296a2b44523d`  
		Last Modified: Wed, 20 Sep 2023 00:46:48 GMT  
		Size: 30.1 MB (30141894 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:797b4215eddcf948eec0f19132f85ec1b0f3af264399e78d860bece37acc4888`  
		Last Modified: Tue, 03 Oct 2023 19:01:51 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3c78c0b20e6791912325d174e98f60d4f783c2f013f52ff3835892444d3a15d7`  
		Last Modified: Tue, 03 Oct 2023 19:01:51 GMT  
		Size: 2.5 MB (2490464 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c91bf1cea723f722413107daa57ab51060ab36a5f78fe8447568aa35be54fca5`  
		Last Modified: Tue, 03 Oct 2023 19:01:52 GMT  
		Size: 12.0 MB (12015261 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:07f7206e609641792c84dfac85e3e6df0602c4ca8d572353a8768ff0619fe328`  
		Last Modified: Tue, 03 Oct 2023 19:01:51 GMT  
		Size: 283.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7aac14495f4a088e0e208638d0b36b0b5ff0cf945aaf24c011ef08ca799279a9`  
		Last Modified: Tue, 03 Oct 2023 19:01:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.21` - unknown; unknown

```console
$ docker pull memcached@sha256:16c8db3d95a2df8fae160a3942ff033ebb3bf6d9fe8df1643eb22c82e9402357
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 KB (21502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03bc49cf22d3ede52afc78d429b09999ba28174660a5e1b41fdb0f9d3a47067c`

```dockerfile
```

-	Layers:
	-	`sha256:890c3f7af1536aa0821f27c4ba142e022ba0c892f1310b4d82a9cc3a74717139`  
		Last Modified: Tue, 03 Oct 2023 19:01:51 GMT  
		Size: 21.5 KB (21502 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6.21` - linux; mips64le

```console
$ docker pull memcached@sha256:575825bdbf62fc255547394ef491710ba88f0be3ca735eaf246ece06f13363ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.4 MB (43398233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e3f951153522f4d9719c37a9862412f3e29e487d11322c5ff7a009cf8becca1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:850547a08e38ebc5a3659df86e70039a8d9828ae26ae485b077c98a959248dcb in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:0f581c6294fe7421dfee024e2c7dddd73ef3fbd7ff23b05bc3c1bf9f50885e85`  
		Last Modified: Wed, 20 Sep 2023 03:20:59 GMT  
		Size: 29.1 MB (29121674 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:15e25af5488ea4ad0df132fa2c22a282c1a17ad1460cdb25fe5939e03a753528`  
		Last Modified: Tue, 03 Oct 2023 19:04:40 GMT  
		Size: 1.1 KB (1113 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:19a5f416c9bf283212262e33fe8529d0ff3917fcee1e8ca9fb058170fd528211`  
		Last Modified: Tue, 03 Oct 2023 19:04:41 GMT  
		Size: 1.9 MB (1934931 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:05862af95003d85f9a1b5696dfb3588bdd8e34c74f067d845b722d70edfc679f`  
		Last Modified: Tue, 03 Oct 2023 19:04:41 GMT  
		Size: 12.3 MB (12340111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e8aae13855c46b73d2506b2d91036f6f0b4bc63b7d7ec12ecc63fd672c64c0f7`  
		Last Modified: Tue, 03 Oct 2023 19:04:40 GMT  
		Size: 282.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0709f88ce6a011ea45fd41c091ee6fcf4baa0610e0591a9fe0d10626eaf9475f`  
		Last Modified: Tue, 03 Oct 2023 19:04:41 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.21` - unknown; unknown

```console
$ docker pull memcached@sha256:269b3e28059bf711ac45886388e91fa405b8a1e0ca1a114acefc997bbdad6d05
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 KB (21491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1059a2662b538952006866f53463fcea773b5e090eaead3a4ad49f4d0a656ae5`

```dockerfile
```

-	Layers:
	-	`sha256:e1052b07541ae6e041e59834c527075b62df62a33f7a9b9e96fda4b6237e83df`  
		Last Modified: Tue, 03 Oct 2023 19:04:40 GMT  
		Size: 21.5 KB (21491 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6.21` - linux; ppc64le

```console
$ docker pull memcached@sha256:532cf0a6053275c508a0503017b4f52ce356a64aba047eb2316bdcaca35bbc9a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49635445 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:111f6d9d894ab95e36b94efa3dad4a4c9d0def1fa3af71a4a0e57e907a2b4986`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:9a37b479e68a0d18babbef8dd04d09a0e6844a0080876d14144a34bfd9d0897a in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:696a66e961f2033dcf69b003ad7faf28ed2248da58efa1c08a9d496739a8eeeb`  
		Last Modified: Wed, 20 Sep 2023 08:49:51 GMT  
		Size: 33.1 MB (33119461 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ba4c0c64bfd7ea845d20c793ede5957878785e4bb16e2e81a3e1ed5cd0d7ca0e`  
		Last Modified: Tue, 03 Oct 2023 19:02:08 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8a7ae673337cbb772a0ccc237ce4009a7dd88e4fed23861c9ea6382e93a6685b`  
		Last Modified: Tue, 03 Oct 2023 19:02:09 GMT  
		Size: 2.7 MB (2694930 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:766c713a6dbc39908803d95aa7556e0a571349c941bddb8f694b3f36030e0c3c`  
		Last Modified: Tue, 03 Oct 2023 19:02:10 GMT  
		Size: 13.8 MB (13819538 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:75734e09fa81ca91f8bdd1481c8f88f95ea9ba7b0f24ab82d0aee2026a5d6474`  
		Last Modified: Tue, 03 Oct 2023 19:02:09 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f46fc74a04a0607353cbc3ace76b49b44029af75080fa56fec872060d38feed2`  
		Last Modified: Tue, 03 Oct 2023 19:02:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.21` - unknown; unknown

```console
$ docker pull memcached@sha256:d73c6167b49dd216e6395e8720af5bd26884a25473d1eb80ee31d1e4b170a914
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2914816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48964548656eeecac440cb41e4f3f474f861d384c569653e582e3d508b04f6e5`

```dockerfile
```

-	Layers:
	-	`sha256:4e89c387c1399e94faaaf407614d23c90aa3104b5773f87d8cb4fe4b20312f8e`  
		Last Modified: Tue, 03 Oct 2023 19:02:09 GMT  
		Size: 2.9 MB (2893143 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:fb96286b26618de71f0df13dfc89225bc855d6802341b4032f0fb4161cb4a52e`  
		Last Modified: Tue, 03 Oct 2023 19:02:08 GMT  
		Size: 21.7 KB (21673 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6.21` - linux; s390x

```console
$ docker pull memcached@sha256:42a17150fd8b17aff6910890bbab808eab97e6f9d0f60003e75fac6ddd2b0bcf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40575835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:956090eeead5cd8ec7753b439eb43ddf3b2c5cd93edea3d7ce5bcdd168ec7588`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:6ed982ad3e8566d63315a27a81b33069910952aef4b2d3e0b607bd2caeac7ca4 in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:26dcff366e33abcf08b812052a4c12496aa406aa267655e984aa7a84ca254cd8`  
		Last Modified: Wed, 20 Sep 2023 02:59:47 GMT  
		Size: 27.5 MB (27489966 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:04795616cce62da1faee69d189f2f4863a3818651e9f54e7552be41e35752766`  
		Last Modified: Tue, 03 Oct 2023 19:01:27 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cbacb720efba986e695a3270bc384924abb78c413d1c4793cd388fbab1da828b`  
		Last Modified: Tue, 03 Oct 2023 19:01:27 GMT  
		Size: 2.2 MB (2150908 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:07a927de051febdc6284e8ec146cbc267ffdd1049fadf2bc35639f53b72b7862`  
		Last Modified: Tue, 03 Oct 2023 19:01:28 GMT  
		Size: 10.9 MB (10933444 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5a2703a37bdc4f133106c52c5a040d30708c01a79aa0d1714bcba3b42105692e`  
		Last Modified: Tue, 03 Oct 2023 19:01:28 GMT  
		Size: 285.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c0a860b98e7d941cd44043f66c4cc9d2a540ab3b8cb9aa15123102865599e0c7`  
		Last Modified: Tue, 03 Oct 2023 19:01:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.21` - unknown; unknown

```console
$ docker pull memcached@sha256:029d2884ff06e1b3673d9a7998c7299cc3da7ed18f46b344e13c14867574bae4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2897027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e57e1f9eb901fd307d1e2dd72b5606ba1f6f0ef82c31c01041513ed98e33b55`

```dockerfile
```

-	Layers:
	-	`sha256:13af4843cce0c7df5b25984623ef20fe08955ca99bbc64f5056c4d1bb2062f13`  
		Last Modified: Tue, 03 Oct 2023 19:01:27 GMT  
		Size: 2.9 MB (2875422 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:2e615a884e0baa9f5e54063b8983b99c841ac4fd854bf56780c1184d51637b1d`  
		Last Modified: Tue, 03 Oct 2023 19:01:27 GMT  
		Size: 21.6 KB (21605 bytes)  
		MIME: application/vnd.in-toto+json

## `memcached:1.6.21-alpine`

```console
$ docker pull memcached@sha256:eaba3015e1bf3a26f3d14ed455ef867e00d395963d0523c4275258f4890af5e1
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

### `memcached:1.6.21-alpine` - linux; amd64

```console
$ docker pull memcached@sha256:27fe55ab0ecba9a8d3ddd67b823da4f1727d10eb46d36ab5af7e693421ebdb4f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4466251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3e0c0ff5c009f0e410e2fc6d29099b24315b4246c64cebae8068e86c22ba8a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["/bin/sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN apk add --no-cache libsasl # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3f9365fb2eebc56ba7006618c6ee8cde403af71bb4777c9b2b1c6ddcc107ee55`  
		Last Modified: Tue, 03 Oct 2023 19:01:12 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ec2c14990e92682477b554b5ccec603b864340a582d8ac4ab7becf52c09e9459`  
		Last Modified: Tue, 03 Oct 2023 19:01:12 GMT  
		Size: 108.0 KB (108015 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a0e994f33a8fb2b64e76f431cb35d0f0f92f0830352e44c589d8770bedfe96c3`  
		Last Modified: Tue, 03 Oct 2023 19:01:13 GMT  
		Size: 954.6 KB (954626 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:69c0dd1ede28d4dfdee1e54dc519270184463fa8812e781a930c0301b851c327`  
		Last Modified: Tue, 03 Oct 2023 19:01:12 GMT  
		Size: 277.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c9a4377466b783eeeab01987a823353e5cfbc2a5f02d632db14c654decf3ec5e`  
		Last Modified: Tue, 03 Oct 2023 19:01:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.21-alpine` - unknown; unknown

```console
$ docker pull memcached@sha256:6ebfa6199008800194514397c12c233ea35c27ee5d22bea93fc978228a9f98f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.2 KB (95222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc3627763f4a9bb22db274ce8453a9d0146e88c0f4e0624f69059e5a9a69ec31`

```dockerfile
```

-	Layers:
	-	`sha256:7e739eda7910762ab0244ff165c2ff431bf4f10a39730614a8fca28a9a91b97d`  
		Last Modified: Tue, 03 Oct 2023 19:01:12 GMT  
		Size: 76.3 KB (76268 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:a04f216271188784dc836fa4905c7d5fbcfb49537cf5cfb5fe5b0229694cf12c`  
		Last Modified: Tue, 03 Oct 2023 19:01:12 GMT  
		Size: 19.0 KB (18954 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6.21-alpine` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:1152b588a2cd7e90f0d7ae86fe3ce262e47c50c62642b5714b0019cef7779a00
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4401705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31bcc2b506321f6395c1d68cfc40f7391530051e5862186db1d5875e2c2803be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["/bin/sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN apk add --no-cache libsasl # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a8a999d5f4398538233c73f556a07cf646c7600543368cbc84b997cd76545de1`  
		Last Modified: Tue, 03 Oct 2023 19:03:35 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e035f8f759de7f5b35527c5cc46cd4132a10e0a501e022fbde2fedcf47fdd684`  
		Last Modified: Tue, 03 Oct 2023 19:03:35 GMT  
		Size: 124.1 KB (124080 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:585097acb28da9160246ad53fa72c119ac6e97a2852f420712485b66d6ed808a`  
		Last Modified: Tue, 03 Oct 2023 19:03:36 GMT  
		Size: 944.1 KB (944147 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:802f5f839e31fd8f8dd89ec2421af9fa8227dd43d5ca883f44d9ff2962cd0848`  
		Last Modified: Tue, 03 Oct 2023 19:03:35 GMT  
		Size: 281.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:65fc6300aa54fcd82f813153e3a5a880a2dca2a26edc3f7f907fe395a01a5474`  
		Last Modified: Tue, 03 Oct 2023 19:03:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.21-alpine` - unknown; unknown

```console
$ docker pull memcached@sha256:5b2e4db4700ecd5765dd85cbc125a24968150122eb9f8181949dc39310085671
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.1 KB (95095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e78ca75a52728eb7207c54b73b899cb6919fd230b814373dc1612765d95bcc0c`

```dockerfile
```

-	Layers:
	-	`sha256:36799473bd1d28916d0df4c2af578542c27261dcc2dbba98964d2d7e956bd73f`  
		Last Modified: Tue, 03 Oct 2023 19:03:35 GMT  
		Size: 76.3 KB (76289 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:c088a7e985146394427f4d604d17a54445f5934b07e790774b7472540d932737`  
		Last Modified: Tue, 03 Oct 2023 19:03:35 GMT  
		Size: 18.8 KB (18806 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6.21-alpine` - linux; 386

```console
$ docker pull memcached@sha256:8b880914dfffd537639b55f5f49cf6c6e9f0773891eb922685e0ce94ccde66b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4283801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f38744e29d4692d1345bf5101db090800c52e9ae211735a610dd8e848ca426d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:8402753f294e403e92353bd65c86a6428c960be5116c0a15484b663a84f66fcd in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["/bin/sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN apk add --no-cache libsasl # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:dc95107ad2a031a015320bb397f73ec151d738127175b31ad643120697dc7e90`  
		Last Modified: Thu, 28 Sep 2023 20:39:32 GMT  
		Size: 3.2 MB (3235757 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f36c14bb55ad2eb4c208a601b1c61872c3725ed95c0c2893c27a822ed5c33a58`  
		Last Modified: Tue, 03 Oct 2023 19:01:33 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1298cb8dafd972511af84e02d7b883a21241c52cf40b58d6979490001961f21c`  
		Last Modified: Tue, 03 Oct 2023 19:01:33 GMT  
		Size: 109.5 KB (109459 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:df4a91e2b048d49e66ddd9893c09f30f39a1d597e80105c7f8962e7f5f7139d9`  
		Last Modified: Tue, 03 Oct 2023 19:01:33 GMT  
		Size: 936.9 KB (936943 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9907fafebdae96d5487b7fb8157a823f61825ffefba79657a80bce23a2545448`  
		Last Modified: Tue, 03 Oct 2023 19:01:34 GMT  
		Size: 276.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ee6a4d82ccc808127f6aaa710b646e700271ad4eff9c41b9965accad5d5d3788`  
		Last Modified: Tue, 03 Oct 2023 19:01:34 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.21-alpine` - unknown; unknown

```console
$ docker pull memcached@sha256:fb404e06827e8d747912612afcca348dc58c4e9ee3ce83c4831cb09f12ab48fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 KB (18684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a050cea12e0cdebacb3a5a2ffc5ab6955496025789c041df169c407640f44bc8`

```dockerfile
```

-	Layers:
	-	`sha256:a3947c8d08a3d57e33242e44fb32c1cbd0106df35f9e5f83cb91293591da71c9`  
		Last Modified: Tue, 03 Oct 2023 19:01:33 GMT  
		Size: 18.7 KB (18684 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6.21-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:32095d8b4daa6df8ff99e36c278c2cb210287066783a65050834bb28667fb2a2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4454721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26527e4ce577d5d1e1fdb3716fde4350e5a3ce0c3b3fd8dd527c6672f8eddcdf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["/bin/sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN apk add --no-cache libsasl # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9a6a9d9fc3b5def98513c33801853ba827c0c7bed9f2b4af3150b75fd4146d74`  
		Last Modified: Tue, 03 Oct 2023 19:06:17 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5dc7c33273d553c8b716261a6aee873fe5544c9200c9061bcc05b037a7c03ab5`  
		Last Modified: Tue, 03 Oct 2023 19:06:17 GMT  
		Size: 123.9 KB (123855 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0873dc2389c5bf83f2b2741fd0639e7dc70b2aa758884d63a794abe95622269b`  
		Last Modified: Tue, 03 Oct 2023 19:06:17 GMT  
		Size: 982.7 KB (982715 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:923b81392db2de0355d0715a2abf7bd7d715b4fac9d0bf39d5c08d7aeeed5270`  
		Last Modified: Tue, 03 Oct 2023 19:06:17 GMT  
		Size: 277.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dd619103d38407e95e05dd7d7f228e66bb5a61f3b561beb35198e92f9cdd0b99`  
		Last Modified: Tue, 03 Oct 2023 19:06:18 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.21-alpine` - unknown; unknown

```console
$ docker pull memcached@sha256:aaa2281dd27a5acbf1364325e1d6ff0a576cfd236847437e2382c07b7199c2ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.3 KB (93262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f9ccd98630f55e4cdd33076a1d3e7f9c11399077a20d0aa9f5af15fcb40bd81`

```dockerfile
```

-	Layers:
	-	`sha256:9c3b535b067358c4894b956bcbf5380d163ce977d0c30028d799f467af8f87d6`  
		Last Modified: Tue, 03 Oct 2023 19:06:17 GMT  
		Size: 74.4 KB (74406 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:9d03d340727841dba89e688d83cd797f9808417dd8d04970fd76395482b117ff`  
		Last Modified: Tue, 03 Oct 2023 19:06:17 GMT  
		Size: 18.9 KB (18856 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6.21-alpine` - linux; s390x

```console
$ docker pull memcached@sha256:0ff7f30ca924f54a50160e70bd590b2ef357c97b6e8bbfcb81fdde97dd5cfbb0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4279633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad89852ec7f35640342fc548839c205af73d8c0f60e54c113b34e9dc519e71c3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["/bin/sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN apk add --no-cache libsasl # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1a648ad7883b3087dfacc17e14f4e6158d881dd1e09b9c5bd27bdd0d89ee44fd`  
		Last Modified: Tue, 03 Oct 2023 20:00:49 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a950f9727c19a31b79f709cdf984608d7788a9ed00dacbce4b14535b7589886f`  
		Last Modified: Tue, 03 Oct 2023 20:00:49 GMT  
		Size: 112.8 KB (112780 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b42424189685c7b481e859243008fea5d1967c6bbc3ccaaf13bf601c56926ebb`  
		Last Modified: Tue, 03 Oct 2023 20:00:49 GMT  
		Size: 950.1 KB (950102 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bf2263fe42a85daea831aafa6f50aeeef49d0ce1aa5841ddde0951667f85b684`  
		Last Modified: Tue, 03 Oct 2023 20:00:49 GMT  
		Size: 281.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:75eaf7af52231f2a4943c93eafc5d565b71c6079a1fee0fdc2605ad3eb81cd58`  
		Last Modified: Tue, 03 Oct 2023 20:00:49 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.21-alpine` - unknown; unknown

```console
$ docker pull memcached@sha256:d2b9bd3538d99a100b4ebf104d9d5029917eecd3eec97d7086f7e4244b373d10
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.1 KB (93124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ade4e328bfbe610c689ab718878e6d07c31e5b67895795550a21d77730847d83`

```dockerfile
```

-	Layers:
	-	`sha256:7350d7c047abc3727f9639268d2cc1a5d7e53cbc81ae534da5e93272b5a48b59`  
		Last Modified: Tue, 03 Oct 2023 20:00:49 GMT  
		Size: 74.3 KB (74336 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:39706e52b9159fe158fe5027b73cb21482efb8781e1ab8853bcb19fc8125bbc8`  
		Last Modified: Tue, 03 Oct 2023 20:00:49 GMT  
		Size: 18.8 KB (18788 bytes)  
		MIME: application/vnd.in-toto+json

## `memcached:1.6.21-alpine3.18`

```console
$ docker pull memcached@sha256:eaba3015e1bf3a26f3d14ed455ef867e00d395963d0523c4275258f4890af5e1
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

### `memcached:1.6.21-alpine3.18` - linux; amd64

```console
$ docker pull memcached@sha256:27fe55ab0ecba9a8d3ddd67b823da4f1727d10eb46d36ab5af7e693421ebdb4f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4466251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3e0c0ff5c009f0e410e2fc6d29099b24315b4246c64cebae8068e86c22ba8a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["/bin/sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN apk add --no-cache libsasl # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3f9365fb2eebc56ba7006618c6ee8cde403af71bb4777c9b2b1c6ddcc107ee55`  
		Last Modified: Tue, 03 Oct 2023 19:01:12 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ec2c14990e92682477b554b5ccec603b864340a582d8ac4ab7becf52c09e9459`  
		Last Modified: Tue, 03 Oct 2023 19:01:12 GMT  
		Size: 108.0 KB (108015 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a0e994f33a8fb2b64e76f431cb35d0f0f92f0830352e44c589d8770bedfe96c3`  
		Last Modified: Tue, 03 Oct 2023 19:01:13 GMT  
		Size: 954.6 KB (954626 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:69c0dd1ede28d4dfdee1e54dc519270184463fa8812e781a930c0301b851c327`  
		Last Modified: Tue, 03 Oct 2023 19:01:12 GMT  
		Size: 277.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c9a4377466b783eeeab01987a823353e5cfbc2a5f02d632db14c654decf3ec5e`  
		Last Modified: Tue, 03 Oct 2023 19:01:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.21-alpine3.18` - unknown; unknown

```console
$ docker pull memcached@sha256:6ebfa6199008800194514397c12c233ea35c27ee5d22bea93fc978228a9f98f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.2 KB (95222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc3627763f4a9bb22db274ce8453a9d0146e88c0f4e0624f69059e5a9a69ec31`

```dockerfile
```

-	Layers:
	-	`sha256:7e739eda7910762ab0244ff165c2ff431bf4f10a39730614a8fca28a9a91b97d`  
		Last Modified: Tue, 03 Oct 2023 19:01:12 GMT  
		Size: 76.3 KB (76268 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:a04f216271188784dc836fa4905c7d5fbcfb49537cf5cfb5fe5b0229694cf12c`  
		Last Modified: Tue, 03 Oct 2023 19:01:12 GMT  
		Size: 19.0 KB (18954 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6.21-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:1152b588a2cd7e90f0d7ae86fe3ce262e47c50c62642b5714b0019cef7779a00
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4401705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31bcc2b506321f6395c1d68cfc40f7391530051e5862186db1d5875e2c2803be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["/bin/sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN apk add --no-cache libsasl # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a8a999d5f4398538233c73f556a07cf646c7600543368cbc84b997cd76545de1`  
		Last Modified: Tue, 03 Oct 2023 19:03:35 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e035f8f759de7f5b35527c5cc46cd4132a10e0a501e022fbde2fedcf47fdd684`  
		Last Modified: Tue, 03 Oct 2023 19:03:35 GMT  
		Size: 124.1 KB (124080 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:585097acb28da9160246ad53fa72c119ac6e97a2852f420712485b66d6ed808a`  
		Last Modified: Tue, 03 Oct 2023 19:03:36 GMT  
		Size: 944.1 KB (944147 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:802f5f839e31fd8f8dd89ec2421af9fa8227dd43d5ca883f44d9ff2962cd0848`  
		Last Modified: Tue, 03 Oct 2023 19:03:35 GMT  
		Size: 281.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:65fc6300aa54fcd82f813153e3a5a880a2dca2a26edc3f7f907fe395a01a5474`  
		Last Modified: Tue, 03 Oct 2023 19:03:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.21-alpine3.18` - unknown; unknown

```console
$ docker pull memcached@sha256:5b2e4db4700ecd5765dd85cbc125a24968150122eb9f8181949dc39310085671
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.1 KB (95095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e78ca75a52728eb7207c54b73b899cb6919fd230b814373dc1612765d95bcc0c`

```dockerfile
```

-	Layers:
	-	`sha256:36799473bd1d28916d0df4c2af578542c27261dcc2dbba98964d2d7e956bd73f`  
		Last Modified: Tue, 03 Oct 2023 19:03:35 GMT  
		Size: 76.3 KB (76289 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:c088a7e985146394427f4d604d17a54445f5934b07e790774b7472540d932737`  
		Last Modified: Tue, 03 Oct 2023 19:03:35 GMT  
		Size: 18.8 KB (18806 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6.21-alpine3.18` - linux; 386

```console
$ docker pull memcached@sha256:8b880914dfffd537639b55f5f49cf6c6e9f0773891eb922685e0ce94ccde66b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4283801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f38744e29d4692d1345bf5101db090800c52e9ae211735a610dd8e848ca426d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:8402753f294e403e92353bd65c86a6428c960be5116c0a15484b663a84f66fcd in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["/bin/sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN apk add --no-cache libsasl # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:dc95107ad2a031a015320bb397f73ec151d738127175b31ad643120697dc7e90`  
		Last Modified: Thu, 28 Sep 2023 20:39:32 GMT  
		Size: 3.2 MB (3235757 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f36c14bb55ad2eb4c208a601b1c61872c3725ed95c0c2893c27a822ed5c33a58`  
		Last Modified: Tue, 03 Oct 2023 19:01:33 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1298cb8dafd972511af84e02d7b883a21241c52cf40b58d6979490001961f21c`  
		Last Modified: Tue, 03 Oct 2023 19:01:33 GMT  
		Size: 109.5 KB (109459 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:df4a91e2b048d49e66ddd9893c09f30f39a1d597e80105c7f8962e7f5f7139d9`  
		Last Modified: Tue, 03 Oct 2023 19:01:33 GMT  
		Size: 936.9 KB (936943 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9907fafebdae96d5487b7fb8157a823f61825ffefba79657a80bce23a2545448`  
		Last Modified: Tue, 03 Oct 2023 19:01:34 GMT  
		Size: 276.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ee6a4d82ccc808127f6aaa710b646e700271ad4eff9c41b9965accad5d5d3788`  
		Last Modified: Tue, 03 Oct 2023 19:01:34 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.21-alpine3.18` - unknown; unknown

```console
$ docker pull memcached@sha256:fb404e06827e8d747912612afcca348dc58c4e9ee3ce83c4831cb09f12ab48fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 KB (18684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a050cea12e0cdebacb3a5a2ffc5ab6955496025789c041df169c407640f44bc8`

```dockerfile
```

-	Layers:
	-	`sha256:a3947c8d08a3d57e33242e44fb32c1cbd0106df35f9e5f83cb91293591da71c9`  
		Last Modified: Tue, 03 Oct 2023 19:01:33 GMT  
		Size: 18.7 KB (18684 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6.21-alpine3.18` - linux; ppc64le

```console
$ docker pull memcached@sha256:32095d8b4daa6df8ff99e36c278c2cb210287066783a65050834bb28667fb2a2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4454721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26527e4ce577d5d1e1fdb3716fde4350e5a3ce0c3b3fd8dd527c6672f8eddcdf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["/bin/sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN apk add --no-cache libsasl # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9a6a9d9fc3b5def98513c33801853ba827c0c7bed9f2b4af3150b75fd4146d74`  
		Last Modified: Tue, 03 Oct 2023 19:06:17 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5dc7c33273d553c8b716261a6aee873fe5544c9200c9061bcc05b037a7c03ab5`  
		Last Modified: Tue, 03 Oct 2023 19:06:17 GMT  
		Size: 123.9 KB (123855 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0873dc2389c5bf83f2b2741fd0639e7dc70b2aa758884d63a794abe95622269b`  
		Last Modified: Tue, 03 Oct 2023 19:06:17 GMT  
		Size: 982.7 KB (982715 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:923b81392db2de0355d0715a2abf7bd7d715b4fac9d0bf39d5c08d7aeeed5270`  
		Last Modified: Tue, 03 Oct 2023 19:06:17 GMT  
		Size: 277.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dd619103d38407e95e05dd7d7f228e66bb5a61f3b561beb35198e92f9cdd0b99`  
		Last Modified: Tue, 03 Oct 2023 19:06:18 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.21-alpine3.18` - unknown; unknown

```console
$ docker pull memcached@sha256:aaa2281dd27a5acbf1364325e1d6ff0a576cfd236847437e2382c07b7199c2ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.3 KB (93262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f9ccd98630f55e4cdd33076a1d3e7f9c11399077a20d0aa9f5af15fcb40bd81`

```dockerfile
```

-	Layers:
	-	`sha256:9c3b535b067358c4894b956bcbf5380d163ce977d0c30028d799f467af8f87d6`  
		Last Modified: Tue, 03 Oct 2023 19:06:17 GMT  
		Size: 74.4 KB (74406 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:9d03d340727841dba89e688d83cd797f9808417dd8d04970fd76395482b117ff`  
		Last Modified: Tue, 03 Oct 2023 19:06:17 GMT  
		Size: 18.9 KB (18856 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6.21-alpine3.18` - linux; s390x

```console
$ docker pull memcached@sha256:0ff7f30ca924f54a50160e70bd590b2ef357c97b6e8bbfcb81fdde97dd5cfbb0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4279633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad89852ec7f35640342fc548839c205af73d8c0f60e54c113b34e9dc519e71c3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["/bin/sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN apk add --no-cache libsasl # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1a648ad7883b3087dfacc17e14f4e6158d881dd1e09b9c5bd27bdd0d89ee44fd`  
		Last Modified: Tue, 03 Oct 2023 20:00:49 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a950f9727c19a31b79f709cdf984608d7788a9ed00dacbce4b14535b7589886f`  
		Last Modified: Tue, 03 Oct 2023 20:00:49 GMT  
		Size: 112.8 KB (112780 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b42424189685c7b481e859243008fea5d1967c6bbc3ccaaf13bf601c56926ebb`  
		Last Modified: Tue, 03 Oct 2023 20:00:49 GMT  
		Size: 950.1 KB (950102 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bf2263fe42a85daea831aafa6f50aeeef49d0ce1aa5841ddde0951667f85b684`  
		Last Modified: Tue, 03 Oct 2023 20:00:49 GMT  
		Size: 281.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:75eaf7af52231f2a4943c93eafc5d565b71c6079a1fee0fdc2605ad3eb81cd58`  
		Last Modified: Tue, 03 Oct 2023 20:00:49 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.21-alpine3.18` - unknown; unknown

```console
$ docker pull memcached@sha256:d2b9bd3538d99a100b4ebf104d9d5029917eecd3eec97d7086f7e4244b373d10
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.1 KB (93124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ade4e328bfbe610c689ab718878e6d07c31e5b67895795550a21d77730847d83`

```dockerfile
```

-	Layers:
	-	`sha256:7350d7c047abc3727f9639268d2cc1a5d7e53cbc81ae534da5e93272b5a48b59`  
		Last Modified: Tue, 03 Oct 2023 20:00:49 GMT  
		Size: 74.3 KB (74336 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:39706e52b9159fe158fe5027b73cb21482efb8781e1ab8853bcb19fc8125bbc8`  
		Last Modified: Tue, 03 Oct 2023 20:00:49 GMT  
		Size: 18.8 KB (18788 bytes)  
		MIME: application/vnd.in-toto+json

## `memcached:1.6.21-bookworm`

```console
$ docker pull memcached@sha256:eef4a056175ad8203df2a1835ae16307e5a70aec3222b409d1114486b2a4bb65
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

### `memcached:1.6.21-bookworm` - linux; amd64

```console
$ docker pull memcached@sha256:8af51889f0f774a00f36624e58faac309c258eafb8054c6abc6fbbb56c78d0a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.8 MB (38811465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fa23f6ace109fad9223ea2db53f79afa8b91b14051c61305f82bc2c781a788c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:55ad846fa191e603f48090eae0e4a7149c4066b94406593ec1898ad2c3347937 in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a378f10b321842c3042cdeff4f6997f34f4cb21f2eff27704b7f6193ab7b5fea`  
		Last Modified: Wed, 11 Oct 2023 18:39:34 GMT  
		Size: 29.1 MB (29149874 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e68aaf702a54364b3f216204ad2725f5b416fe496294086899b821bb5133552d`  
		Last Modified: Wed, 11 Oct 2023 20:07:27 GMT  
		Size: 1.1 KB (1110 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0fb853802e1447e9b1dbe3e8a86f27a5691286127397adf8d52f943d16b80042`  
		Last Modified: Wed, 11 Oct 2023 20:07:27 GMT  
		Size: 2.5 MB (2488274 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fcc9694d882f053fcf2e7bb33709dcb86eef6c29c3187c190ad93852af7a50f2`  
		Last Modified: Wed, 11 Oct 2023 20:07:28 GMT  
		Size: 7.2 MB (7171802 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fde136907f7040bd6126a5b2c0bca844fef33e2fc804c1f135e99393869cce4c`  
		Last Modified: Wed, 11 Oct 2023 20:07:27 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c121d0db5ccb2988b1fc0c76ce60a2e78309d77b264adf99e815e1ecf2c6a957`  
		Last Modified: Wed, 11 Oct 2023 20:07:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.21-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:888d3aaaddc944acb247f0e42586c8c8a7f8c3262166ee89ceda0dbe3998cafa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2911211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06530a2f7a54ba7d86fc6cee0da9a46ea1aea89dc4beecbee6d54ed8eee82dd9`

```dockerfile
```

-	Layers:
	-	`sha256:7bbbdfb4ba86ed51b46d2fb83bf8cf4e095da6d5c9dd89697a3488dd392414d7`  
		Last Modified: Wed, 11 Oct 2023 20:07:27 GMT  
		Size: 2.9 MB (2889442 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:6fe7a995830937695f7110928df7e791673ab04015add73a1f2e9ec661bbc60f`  
		Last Modified: Wed, 11 Oct 2023 20:07:27 GMT  
		Size: 21.8 KB (21769 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6.21-bookworm` - linux; arm variant v5

```console
$ docker pull memcached@sha256:a6919fc9976aa2c291f194860f40fcc9499d33cbd2592af9087e5d64b7930602
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34846023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5222dddac963b84d55ef902d40fa3f949ee73caac9614ca77c1f4a81ef009c6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:8c43adb3245fc6f2b10aa5a86c850db5dcf3515eaf7e46630922fe21f806bd2a in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:904e6393ef1ee28b37171369eb4f7cb04714631c711799819fccb83886bd212b`  
		Last Modified: Wed, 11 Oct 2023 17:40:47 GMT  
		Size: 26.9 MB (26922150 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f0569355cb85b70d6a614ea9604289ce8e724f0f9ff4d1d8a12afc24c4c9ad1f`  
		Last Modified: Thu, 12 Oct 2023 08:32:05 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6939032c8ff0687b012a85d3411c702266b934a677f96eb521658b44f5b4a8c0`  
		Last Modified: Thu, 12 Oct 2023 08:32:06 GMT  
		Size: 2.1 MB (2089182 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8e8a2a7338b5cacc7b6e4e3db2359eebb1936b0b14266d5bad0dfcc21c9becff`  
		Last Modified: Thu, 12 Oct 2023 08:32:06 GMT  
		Size: 5.8 MB (5833176 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:19f35a8116fe7e124bee612b2ac511694077a1f35f76ed056903987ab4921e34`  
		Last Modified: Thu, 12 Oct 2023 08:32:06 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a43775be6dfac6c255e35b164eacd7328df241f33f9245206a8eaf481062ccbc`  
		Last Modified: Thu, 12 Oct 2023 08:32:07 GMT  
		Size: 120.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.21-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:f1276a05a4db6e8b7bb9d8374d480b85a79f1b92d4e7475c65e247bf1427200c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.7 KB (21695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe67b683a818ed7c22a49086ec4f22e53c6efa9040becea46adb07f550dae564`

```dockerfile
```

-	Layers:
	-	`sha256:12ecc330d2059d33dc7a7c518e7be06804f5fcadafdc8e2db030631f5c92b326`  
		Last Modified: Thu, 12 Oct 2023 08:32:05 GMT  
		Size: 21.7 KB (21695 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6.21-bookworm` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:0c25b3c626a396c236dcf08792c850a178482c24e0c9dab0e784783178d10c13
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.4 MB (43442272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1595a8aa58bfc22ba6e995a58c63ea8b660aa8a9b10c57ab0cb8552d94080218`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:ec1a6e0aedd76c8fdc8544775f8b553f58950e9435f5cfe919f39374e222cfbb in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:e886f0f47ef56fcadb6ecaf2116056bbdb273e0afe07ed034498b198d386c04e`  
		Last Modified: Wed, 20 Sep 2023 02:47:36 GMT  
		Size: 29.2 MB (29157221 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7e25b15fcaee53caa22717c5b0b52fabf2480b0244a84530fca4c1edbb812044`  
		Last Modified: Tue, 03 Oct 2023 19:00:54 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:72fc5c44d6b752d2c2534f97f12ef44f915803ec4e564d7c9eb90d9d7bda2297`  
		Last Modified: Tue, 03 Oct 2023 19:00:54 GMT  
		Size: 2.3 MB (2343087 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7ba30437e42c2aebda3182e43b83b90012dd19e31adb9dc25bb3b714385cdefe`  
		Last Modified: Tue, 03 Oct 2023 19:00:55 GMT  
		Size: 11.9 MB (11940448 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:70abb5efa4268d01b1dfe9f6775f8f85a7fe395141dcc28909aa52ea6b741971`  
		Last Modified: Tue, 03 Oct 2023 19:00:54 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5a87a9f60806e352855b340f2c0c3610b8053006f0f542077c3add7e70782663`  
		Last Modified: Tue, 03 Oct 2023 19:00:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.21-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:7a900749c7d177577d906a5d402b4a008b95ae3571e9de24b4f04060e8650d5d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2890735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:711e633b20942471e455d3210316a79109ffda2a13cb38f46bd9ab2d27c758ae`

```dockerfile
```

-	Layers:
	-	`sha256:6c4c4a32fc3b330e635796951e46bf9e6ed753212798e75baddd3a84e752de8c`  
		Last Modified: Tue, 03 Oct 2023 19:00:54 GMT  
		Size: 2.9 MB (2869112 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:d0ceb647ed388f03f95faf34bc93c1489afde267801855f46cfca84fca538c5a`  
		Last Modified: Tue, 03 Oct 2023 19:00:54 GMT  
		Size: 21.6 KB (21623 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6.21-bookworm` - linux; 386

```console
$ docker pull memcached@sha256:dbf6fdd168abcb8b6fd831277bea0213784e54cdb824756684dd3b5337c42c65
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.6 MB (44649134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25680867a5df0eb88860f59d7855c9d7f3862a44283c1e59d608f9dbecff348b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:efe81f7066129aa6293627bfe4ea78b957897ba5ede951970156fccf1dbcde88 in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6ac07f93e07a1bad4555e13bd8efd06169988669fc88df95f4bf296a2b44523d`  
		Last Modified: Wed, 20 Sep 2023 00:46:48 GMT  
		Size: 30.1 MB (30141894 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:797b4215eddcf948eec0f19132f85ec1b0f3af264399e78d860bece37acc4888`  
		Last Modified: Tue, 03 Oct 2023 19:01:51 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3c78c0b20e6791912325d174e98f60d4f783c2f013f52ff3835892444d3a15d7`  
		Last Modified: Tue, 03 Oct 2023 19:01:51 GMT  
		Size: 2.5 MB (2490464 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c91bf1cea723f722413107daa57ab51060ab36a5f78fe8447568aa35be54fca5`  
		Last Modified: Tue, 03 Oct 2023 19:01:52 GMT  
		Size: 12.0 MB (12015261 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:07f7206e609641792c84dfac85e3e6df0602c4ca8d572353a8768ff0619fe328`  
		Last Modified: Tue, 03 Oct 2023 19:01:51 GMT  
		Size: 283.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7aac14495f4a088e0e208638d0b36b0b5ff0cf945aaf24c011ef08ca799279a9`  
		Last Modified: Tue, 03 Oct 2023 19:01:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.21-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:16c8db3d95a2df8fae160a3942ff033ebb3bf6d9fe8df1643eb22c82e9402357
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 KB (21502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03bc49cf22d3ede52afc78d429b09999ba28174660a5e1b41fdb0f9d3a47067c`

```dockerfile
```

-	Layers:
	-	`sha256:890c3f7af1536aa0821f27c4ba142e022ba0c892f1310b4d82a9cc3a74717139`  
		Last Modified: Tue, 03 Oct 2023 19:01:51 GMT  
		Size: 21.5 KB (21502 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6.21-bookworm` - linux; mips64le

```console
$ docker pull memcached@sha256:575825bdbf62fc255547394ef491710ba88f0be3ca735eaf246ece06f13363ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.4 MB (43398233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e3f951153522f4d9719c37a9862412f3e29e487d11322c5ff7a009cf8becca1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:850547a08e38ebc5a3659df86e70039a8d9828ae26ae485b077c98a959248dcb in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:0f581c6294fe7421dfee024e2c7dddd73ef3fbd7ff23b05bc3c1bf9f50885e85`  
		Last Modified: Wed, 20 Sep 2023 03:20:59 GMT  
		Size: 29.1 MB (29121674 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:15e25af5488ea4ad0df132fa2c22a282c1a17ad1460cdb25fe5939e03a753528`  
		Last Modified: Tue, 03 Oct 2023 19:04:40 GMT  
		Size: 1.1 KB (1113 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:19a5f416c9bf283212262e33fe8529d0ff3917fcee1e8ca9fb058170fd528211`  
		Last Modified: Tue, 03 Oct 2023 19:04:41 GMT  
		Size: 1.9 MB (1934931 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:05862af95003d85f9a1b5696dfb3588bdd8e34c74f067d845b722d70edfc679f`  
		Last Modified: Tue, 03 Oct 2023 19:04:41 GMT  
		Size: 12.3 MB (12340111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e8aae13855c46b73d2506b2d91036f6f0b4bc63b7d7ec12ecc63fd672c64c0f7`  
		Last Modified: Tue, 03 Oct 2023 19:04:40 GMT  
		Size: 282.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0709f88ce6a011ea45fd41c091ee6fcf4baa0610e0591a9fe0d10626eaf9475f`  
		Last Modified: Tue, 03 Oct 2023 19:04:41 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.21-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:269b3e28059bf711ac45886388e91fa405b8a1e0ca1a114acefc997bbdad6d05
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 KB (21491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1059a2662b538952006866f53463fcea773b5e090eaead3a4ad49f4d0a656ae5`

```dockerfile
```

-	Layers:
	-	`sha256:e1052b07541ae6e041e59834c527075b62df62a33f7a9b9e96fda4b6237e83df`  
		Last Modified: Tue, 03 Oct 2023 19:04:40 GMT  
		Size: 21.5 KB (21491 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6.21-bookworm` - linux; ppc64le

```console
$ docker pull memcached@sha256:532cf0a6053275c508a0503017b4f52ce356a64aba047eb2316bdcaca35bbc9a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49635445 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:111f6d9d894ab95e36b94efa3dad4a4c9d0def1fa3af71a4a0e57e907a2b4986`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:9a37b479e68a0d18babbef8dd04d09a0e6844a0080876d14144a34bfd9d0897a in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:696a66e961f2033dcf69b003ad7faf28ed2248da58efa1c08a9d496739a8eeeb`  
		Last Modified: Wed, 20 Sep 2023 08:49:51 GMT  
		Size: 33.1 MB (33119461 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ba4c0c64bfd7ea845d20c793ede5957878785e4bb16e2e81a3e1ed5cd0d7ca0e`  
		Last Modified: Tue, 03 Oct 2023 19:02:08 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8a7ae673337cbb772a0ccc237ce4009a7dd88e4fed23861c9ea6382e93a6685b`  
		Last Modified: Tue, 03 Oct 2023 19:02:09 GMT  
		Size: 2.7 MB (2694930 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:766c713a6dbc39908803d95aa7556e0a571349c941bddb8f694b3f36030e0c3c`  
		Last Modified: Tue, 03 Oct 2023 19:02:10 GMT  
		Size: 13.8 MB (13819538 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:75734e09fa81ca91f8bdd1481c8f88f95ea9ba7b0f24ab82d0aee2026a5d6474`  
		Last Modified: Tue, 03 Oct 2023 19:02:09 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f46fc74a04a0607353cbc3ace76b49b44029af75080fa56fec872060d38feed2`  
		Last Modified: Tue, 03 Oct 2023 19:02:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.21-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:d73c6167b49dd216e6395e8720af5bd26884a25473d1eb80ee31d1e4b170a914
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2914816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48964548656eeecac440cb41e4f3f474f861d384c569653e582e3d508b04f6e5`

```dockerfile
```

-	Layers:
	-	`sha256:4e89c387c1399e94faaaf407614d23c90aa3104b5773f87d8cb4fe4b20312f8e`  
		Last Modified: Tue, 03 Oct 2023 19:02:09 GMT  
		Size: 2.9 MB (2893143 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:fb96286b26618de71f0df13dfc89225bc855d6802341b4032f0fb4161cb4a52e`  
		Last Modified: Tue, 03 Oct 2023 19:02:08 GMT  
		Size: 21.7 KB (21673 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1.6.21-bookworm` - linux; s390x

```console
$ docker pull memcached@sha256:42a17150fd8b17aff6910890bbab808eab97e6f9d0f60003e75fac6ddd2b0bcf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40575835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:956090eeead5cd8ec7753b439eb43ddf3b2c5cd93edea3d7ce5bcdd168ec7588`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:6ed982ad3e8566d63315a27a81b33069910952aef4b2d3e0b607bd2caeac7ca4 in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:26dcff366e33abcf08b812052a4c12496aa406aa267655e984aa7a84ca254cd8`  
		Last Modified: Wed, 20 Sep 2023 02:59:47 GMT  
		Size: 27.5 MB (27489966 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:04795616cce62da1faee69d189f2f4863a3818651e9f54e7552be41e35752766`  
		Last Modified: Tue, 03 Oct 2023 19:01:27 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cbacb720efba986e695a3270bc384924abb78c413d1c4793cd388fbab1da828b`  
		Last Modified: Tue, 03 Oct 2023 19:01:27 GMT  
		Size: 2.2 MB (2150908 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:07a927de051febdc6284e8ec146cbc267ffdd1049fadf2bc35639f53b72b7862`  
		Last Modified: Tue, 03 Oct 2023 19:01:28 GMT  
		Size: 10.9 MB (10933444 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5a2703a37bdc4f133106c52c5a040d30708c01a79aa0d1714bcba3b42105692e`  
		Last Modified: Tue, 03 Oct 2023 19:01:28 GMT  
		Size: 285.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c0a860b98e7d941cd44043f66c4cc9d2a540ab3b8cb9aa15123102865599e0c7`  
		Last Modified: Tue, 03 Oct 2023 19:01:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1.6.21-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:029d2884ff06e1b3673d9a7998c7299cc3da7ed18f46b344e13c14867574bae4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2897027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e57e1f9eb901fd307d1e2dd72b5606ba1f6f0ef82c31c01041513ed98e33b55`

```dockerfile
```

-	Layers:
	-	`sha256:13af4843cce0c7df5b25984623ef20fe08955ca99bbc64f5056c4d1bb2062f13`  
		Last Modified: Tue, 03 Oct 2023 19:01:27 GMT  
		Size: 2.9 MB (2875422 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:2e615a884e0baa9f5e54063b8983b99c841ac4fd854bf56780c1184d51637b1d`  
		Last Modified: Tue, 03 Oct 2023 19:01:27 GMT  
		Size: 21.6 KB (21605 bytes)  
		MIME: application/vnd.in-toto+json

## `memcached:alpine`

```console
$ docker pull memcached@sha256:535282ea08869aedc9bd20cbd714f07a27019c8b1e3aa64aa7321c96fb747844
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
$ docker pull memcached@sha256:27fe55ab0ecba9a8d3ddd67b823da4f1727d10eb46d36ab5af7e693421ebdb4f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4466251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3e0c0ff5c009f0e410e2fc6d29099b24315b4246c64cebae8068e86c22ba8a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["/bin/sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN apk add --no-cache libsasl # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3f9365fb2eebc56ba7006618c6ee8cde403af71bb4777c9b2b1c6ddcc107ee55`  
		Last Modified: Tue, 03 Oct 2023 19:01:12 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ec2c14990e92682477b554b5ccec603b864340a582d8ac4ab7becf52c09e9459`  
		Last Modified: Tue, 03 Oct 2023 19:01:12 GMT  
		Size: 108.0 KB (108015 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a0e994f33a8fb2b64e76f431cb35d0f0f92f0830352e44c589d8770bedfe96c3`  
		Last Modified: Tue, 03 Oct 2023 19:01:13 GMT  
		Size: 954.6 KB (954626 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:69c0dd1ede28d4dfdee1e54dc519270184463fa8812e781a930c0301b851c327`  
		Last Modified: Tue, 03 Oct 2023 19:01:12 GMT  
		Size: 277.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c9a4377466b783eeeab01987a823353e5cfbc2a5f02d632db14c654decf3ec5e`  
		Last Modified: Tue, 03 Oct 2023 19:01:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:alpine` - unknown; unknown

```console
$ docker pull memcached@sha256:6ebfa6199008800194514397c12c233ea35c27ee5d22bea93fc978228a9f98f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.2 KB (95222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc3627763f4a9bb22db274ce8453a9d0146e88c0f4e0624f69059e5a9a69ec31`

```dockerfile
```

-	Layers:
	-	`sha256:7e739eda7910762ab0244ff165c2ff431bf4f10a39730614a8fca28a9a91b97d`  
		Last Modified: Tue, 03 Oct 2023 19:01:12 GMT  
		Size: 76.3 KB (76268 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:a04f216271188784dc836fa4905c7d5fbcfb49537cf5cfb5fe5b0229694cf12c`  
		Last Modified: Tue, 03 Oct 2023 19:01:12 GMT  
		Size: 19.0 KB (18954 bytes)  
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
$ docker pull memcached@sha256:1152b588a2cd7e90f0d7ae86fe3ce262e47c50c62642b5714b0019cef7779a00
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4401705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31bcc2b506321f6395c1d68cfc40f7391530051e5862186db1d5875e2c2803be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["/bin/sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN apk add --no-cache libsasl # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a8a999d5f4398538233c73f556a07cf646c7600543368cbc84b997cd76545de1`  
		Last Modified: Tue, 03 Oct 2023 19:03:35 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e035f8f759de7f5b35527c5cc46cd4132a10e0a501e022fbde2fedcf47fdd684`  
		Last Modified: Tue, 03 Oct 2023 19:03:35 GMT  
		Size: 124.1 KB (124080 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:585097acb28da9160246ad53fa72c119ac6e97a2852f420712485b66d6ed808a`  
		Last Modified: Tue, 03 Oct 2023 19:03:36 GMT  
		Size: 944.1 KB (944147 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:802f5f839e31fd8f8dd89ec2421af9fa8227dd43d5ca883f44d9ff2962cd0848`  
		Last Modified: Tue, 03 Oct 2023 19:03:35 GMT  
		Size: 281.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:65fc6300aa54fcd82f813153e3a5a880a2dca2a26edc3f7f907fe395a01a5474`  
		Last Modified: Tue, 03 Oct 2023 19:03:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:alpine` - unknown; unknown

```console
$ docker pull memcached@sha256:5b2e4db4700ecd5765dd85cbc125a24968150122eb9f8181949dc39310085671
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.1 KB (95095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e78ca75a52728eb7207c54b73b899cb6919fd230b814373dc1612765d95bcc0c`

```dockerfile
```

-	Layers:
	-	`sha256:36799473bd1d28916d0df4c2af578542c27261dcc2dbba98964d2d7e956bd73f`  
		Last Modified: Tue, 03 Oct 2023 19:03:35 GMT  
		Size: 76.3 KB (76289 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:c088a7e985146394427f4d604d17a54445f5934b07e790774b7472540d932737`  
		Last Modified: Tue, 03 Oct 2023 19:03:35 GMT  
		Size: 18.8 KB (18806 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:alpine` - linux; 386

```console
$ docker pull memcached@sha256:8b880914dfffd537639b55f5f49cf6c6e9f0773891eb922685e0ce94ccde66b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4283801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f38744e29d4692d1345bf5101db090800c52e9ae211735a610dd8e848ca426d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:8402753f294e403e92353bd65c86a6428c960be5116c0a15484b663a84f66fcd in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["/bin/sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN apk add --no-cache libsasl # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:dc95107ad2a031a015320bb397f73ec151d738127175b31ad643120697dc7e90`  
		Last Modified: Thu, 28 Sep 2023 20:39:32 GMT  
		Size: 3.2 MB (3235757 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f36c14bb55ad2eb4c208a601b1c61872c3725ed95c0c2893c27a822ed5c33a58`  
		Last Modified: Tue, 03 Oct 2023 19:01:33 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1298cb8dafd972511af84e02d7b883a21241c52cf40b58d6979490001961f21c`  
		Last Modified: Tue, 03 Oct 2023 19:01:33 GMT  
		Size: 109.5 KB (109459 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:df4a91e2b048d49e66ddd9893c09f30f39a1d597e80105c7f8962e7f5f7139d9`  
		Last Modified: Tue, 03 Oct 2023 19:01:33 GMT  
		Size: 936.9 KB (936943 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9907fafebdae96d5487b7fb8157a823f61825ffefba79657a80bce23a2545448`  
		Last Modified: Tue, 03 Oct 2023 19:01:34 GMT  
		Size: 276.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ee6a4d82ccc808127f6aaa710b646e700271ad4eff9c41b9965accad5d5d3788`  
		Last Modified: Tue, 03 Oct 2023 19:01:34 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:alpine` - unknown; unknown

```console
$ docker pull memcached@sha256:fb404e06827e8d747912612afcca348dc58c4e9ee3ce83c4831cb09f12ab48fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 KB (18684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a050cea12e0cdebacb3a5a2ffc5ab6955496025789c041df169c407640f44bc8`

```dockerfile
```

-	Layers:
	-	`sha256:a3947c8d08a3d57e33242e44fb32c1cbd0106df35f9e5f83cb91293591da71c9`  
		Last Modified: Tue, 03 Oct 2023 19:01:33 GMT  
		Size: 18.7 KB (18684 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:32095d8b4daa6df8ff99e36c278c2cb210287066783a65050834bb28667fb2a2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4454721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26527e4ce577d5d1e1fdb3716fde4350e5a3ce0c3b3fd8dd527c6672f8eddcdf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["/bin/sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN apk add --no-cache libsasl # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9a6a9d9fc3b5def98513c33801853ba827c0c7bed9f2b4af3150b75fd4146d74`  
		Last Modified: Tue, 03 Oct 2023 19:06:17 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5dc7c33273d553c8b716261a6aee873fe5544c9200c9061bcc05b037a7c03ab5`  
		Last Modified: Tue, 03 Oct 2023 19:06:17 GMT  
		Size: 123.9 KB (123855 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0873dc2389c5bf83f2b2741fd0639e7dc70b2aa758884d63a794abe95622269b`  
		Last Modified: Tue, 03 Oct 2023 19:06:17 GMT  
		Size: 982.7 KB (982715 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:923b81392db2de0355d0715a2abf7bd7d715b4fac9d0bf39d5c08d7aeeed5270`  
		Last Modified: Tue, 03 Oct 2023 19:06:17 GMT  
		Size: 277.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dd619103d38407e95e05dd7d7f228e66bb5a61f3b561beb35198e92f9cdd0b99`  
		Last Modified: Tue, 03 Oct 2023 19:06:18 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:alpine` - unknown; unknown

```console
$ docker pull memcached@sha256:aaa2281dd27a5acbf1364325e1d6ff0a576cfd236847437e2382c07b7199c2ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.3 KB (93262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f9ccd98630f55e4cdd33076a1d3e7f9c11399077a20d0aa9f5af15fcb40bd81`

```dockerfile
```

-	Layers:
	-	`sha256:9c3b535b067358c4894b956bcbf5380d163ce977d0c30028d799f467af8f87d6`  
		Last Modified: Tue, 03 Oct 2023 19:06:17 GMT  
		Size: 74.4 KB (74406 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:9d03d340727841dba89e688d83cd797f9808417dd8d04970fd76395482b117ff`  
		Last Modified: Tue, 03 Oct 2023 19:06:17 GMT  
		Size: 18.9 KB (18856 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:alpine` - linux; s390x

```console
$ docker pull memcached@sha256:0ff7f30ca924f54a50160e70bd590b2ef357c97b6e8bbfcb81fdde97dd5cfbb0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4279633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad89852ec7f35640342fc548839c205af73d8c0f60e54c113b34e9dc519e71c3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["/bin/sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN apk add --no-cache libsasl # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1a648ad7883b3087dfacc17e14f4e6158d881dd1e09b9c5bd27bdd0d89ee44fd`  
		Last Modified: Tue, 03 Oct 2023 20:00:49 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a950f9727c19a31b79f709cdf984608d7788a9ed00dacbce4b14535b7589886f`  
		Last Modified: Tue, 03 Oct 2023 20:00:49 GMT  
		Size: 112.8 KB (112780 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b42424189685c7b481e859243008fea5d1967c6bbc3ccaaf13bf601c56926ebb`  
		Last Modified: Tue, 03 Oct 2023 20:00:49 GMT  
		Size: 950.1 KB (950102 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bf2263fe42a85daea831aafa6f50aeeef49d0ce1aa5841ddde0951667f85b684`  
		Last Modified: Tue, 03 Oct 2023 20:00:49 GMT  
		Size: 281.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:75eaf7af52231f2a4943c93eafc5d565b71c6079a1fee0fdc2605ad3eb81cd58`  
		Last Modified: Tue, 03 Oct 2023 20:00:49 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:alpine` - unknown; unknown

```console
$ docker pull memcached@sha256:d2b9bd3538d99a100b4ebf104d9d5029917eecd3eec97d7086f7e4244b373d10
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.1 KB (93124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ade4e328bfbe610c689ab718878e6d07c31e5b67895795550a21d77730847d83`

```dockerfile
```

-	Layers:
	-	`sha256:7350d7c047abc3727f9639268d2cc1a5d7e53cbc81ae534da5e93272b5a48b59`  
		Last Modified: Tue, 03 Oct 2023 20:00:49 GMT  
		Size: 74.3 KB (74336 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:39706e52b9159fe158fe5027b73cb21482efb8781e1ab8853bcb19fc8125bbc8`  
		Last Modified: Tue, 03 Oct 2023 20:00:49 GMT  
		Size: 18.8 KB (18788 bytes)  
		MIME: application/vnd.in-toto+json

## `memcached:alpine3.18`

```console
$ docker pull memcached@sha256:eaba3015e1bf3a26f3d14ed455ef867e00d395963d0523c4275258f4890af5e1
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
$ docker pull memcached@sha256:27fe55ab0ecba9a8d3ddd67b823da4f1727d10eb46d36ab5af7e693421ebdb4f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4466251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3e0c0ff5c009f0e410e2fc6d29099b24315b4246c64cebae8068e86c22ba8a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["/bin/sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN apk add --no-cache libsasl # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3f9365fb2eebc56ba7006618c6ee8cde403af71bb4777c9b2b1c6ddcc107ee55`  
		Last Modified: Tue, 03 Oct 2023 19:01:12 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ec2c14990e92682477b554b5ccec603b864340a582d8ac4ab7becf52c09e9459`  
		Last Modified: Tue, 03 Oct 2023 19:01:12 GMT  
		Size: 108.0 KB (108015 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a0e994f33a8fb2b64e76f431cb35d0f0f92f0830352e44c589d8770bedfe96c3`  
		Last Modified: Tue, 03 Oct 2023 19:01:13 GMT  
		Size: 954.6 KB (954626 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:69c0dd1ede28d4dfdee1e54dc519270184463fa8812e781a930c0301b851c327`  
		Last Modified: Tue, 03 Oct 2023 19:01:12 GMT  
		Size: 277.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c9a4377466b783eeeab01987a823353e5cfbc2a5f02d632db14c654decf3ec5e`  
		Last Modified: Tue, 03 Oct 2023 19:01:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:alpine3.18` - unknown; unknown

```console
$ docker pull memcached@sha256:6ebfa6199008800194514397c12c233ea35c27ee5d22bea93fc978228a9f98f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.2 KB (95222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc3627763f4a9bb22db274ce8453a9d0146e88c0f4e0624f69059e5a9a69ec31`

```dockerfile
```

-	Layers:
	-	`sha256:7e739eda7910762ab0244ff165c2ff431bf4f10a39730614a8fca28a9a91b97d`  
		Last Modified: Tue, 03 Oct 2023 19:01:12 GMT  
		Size: 76.3 KB (76268 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:a04f216271188784dc836fa4905c7d5fbcfb49537cf5cfb5fe5b0229694cf12c`  
		Last Modified: Tue, 03 Oct 2023 19:01:12 GMT  
		Size: 19.0 KB (18954 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:alpine3.18` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:1152b588a2cd7e90f0d7ae86fe3ce262e47c50c62642b5714b0019cef7779a00
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4401705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31bcc2b506321f6395c1d68cfc40f7391530051e5862186db1d5875e2c2803be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["/bin/sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN apk add --no-cache libsasl # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a8a999d5f4398538233c73f556a07cf646c7600543368cbc84b997cd76545de1`  
		Last Modified: Tue, 03 Oct 2023 19:03:35 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e035f8f759de7f5b35527c5cc46cd4132a10e0a501e022fbde2fedcf47fdd684`  
		Last Modified: Tue, 03 Oct 2023 19:03:35 GMT  
		Size: 124.1 KB (124080 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:585097acb28da9160246ad53fa72c119ac6e97a2852f420712485b66d6ed808a`  
		Last Modified: Tue, 03 Oct 2023 19:03:36 GMT  
		Size: 944.1 KB (944147 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:802f5f839e31fd8f8dd89ec2421af9fa8227dd43d5ca883f44d9ff2962cd0848`  
		Last Modified: Tue, 03 Oct 2023 19:03:35 GMT  
		Size: 281.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:65fc6300aa54fcd82f813153e3a5a880a2dca2a26edc3f7f907fe395a01a5474`  
		Last Modified: Tue, 03 Oct 2023 19:03:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:alpine3.18` - unknown; unknown

```console
$ docker pull memcached@sha256:5b2e4db4700ecd5765dd85cbc125a24968150122eb9f8181949dc39310085671
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.1 KB (95095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e78ca75a52728eb7207c54b73b899cb6919fd230b814373dc1612765d95bcc0c`

```dockerfile
```

-	Layers:
	-	`sha256:36799473bd1d28916d0df4c2af578542c27261dcc2dbba98964d2d7e956bd73f`  
		Last Modified: Tue, 03 Oct 2023 19:03:35 GMT  
		Size: 76.3 KB (76289 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:c088a7e985146394427f4d604d17a54445f5934b07e790774b7472540d932737`  
		Last Modified: Tue, 03 Oct 2023 19:03:35 GMT  
		Size: 18.8 KB (18806 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:alpine3.18` - linux; 386

```console
$ docker pull memcached@sha256:8b880914dfffd537639b55f5f49cf6c6e9f0773891eb922685e0ce94ccde66b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4283801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f38744e29d4692d1345bf5101db090800c52e9ae211735a610dd8e848ca426d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:8402753f294e403e92353bd65c86a6428c960be5116c0a15484b663a84f66fcd in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["/bin/sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN apk add --no-cache libsasl # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:dc95107ad2a031a015320bb397f73ec151d738127175b31ad643120697dc7e90`  
		Last Modified: Thu, 28 Sep 2023 20:39:32 GMT  
		Size: 3.2 MB (3235757 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f36c14bb55ad2eb4c208a601b1c61872c3725ed95c0c2893c27a822ed5c33a58`  
		Last Modified: Tue, 03 Oct 2023 19:01:33 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1298cb8dafd972511af84e02d7b883a21241c52cf40b58d6979490001961f21c`  
		Last Modified: Tue, 03 Oct 2023 19:01:33 GMT  
		Size: 109.5 KB (109459 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:df4a91e2b048d49e66ddd9893c09f30f39a1d597e80105c7f8962e7f5f7139d9`  
		Last Modified: Tue, 03 Oct 2023 19:01:33 GMT  
		Size: 936.9 KB (936943 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9907fafebdae96d5487b7fb8157a823f61825ffefba79657a80bce23a2545448`  
		Last Modified: Tue, 03 Oct 2023 19:01:34 GMT  
		Size: 276.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ee6a4d82ccc808127f6aaa710b646e700271ad4eff9c41b9965accad5d5d3788`  
		Last Modified: Tue, 03 Oct 2023 19:01:34 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:alpine3.18` - unknown; unknown

```console
$ docker pull memcached@sha256:fb404e06827e8d747912612afcca348dc58c4e9ee3ce83c4831cb09f12ab48fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.7 KB (18684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a050cea12e0cdebacb3a5a2ffc5ab6955496025789c041df169c407640f44bc8`

```dockerfile
```

-	Layers:
	-	`sha256:a3947c8d08a3d57e33242e44fb32c1cbd0106df35f9e5f83cb91293591da71c9`  
		Last Modified: Tue, 03 Oct 2023 19:01:33 GMT  
		Size: 18.7 KB (18684 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:alpine3.18` - linux; ppc64le

```console
$ docker pull memcached@sha256:32095d8b4daa6df8ff99e36c278c2cb210287066783a65050834bb28667fb2a2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4454721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26527e4ce577d5d1e1fdb3716fde4350e5a3ce0c3b3fd8dd527c6672f8eddcdf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["/bin/sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN apk add --no-cache libsasl # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9a6a9d9fc3b5def98513c33801853ba827c0c7bed9f2b4af3150b75fd4146d74`  
		Last Modified: Tue, 03 Oct 2023 19:06:17 GMT  
		Size: 1.2 KB (1244 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5dc7c33273d553c8b716261a6aee873fe5544c9200c9061bcc05b037a7c03ab5`  
		Last Modified: Tue, 03 Oct 2023 19:06:17 GMT  
		Size: 123.9 KB (123855 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0873dc2389c5bf83f2b2741fd0639e7dc70b2aa758884d63a794abe95622269b`  
		Last Modified: Tue, 03 Oct 2023 19:06:17 GMT  
		Size: 982.7 KB (982715 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:923b81392db2de0355d0715a2abf7bd7d715b4fac9d0bf39d5c08d7aeeed5270`  
		Last Modified: Tue, 03 Oct 2023 19:06:17 GMT  
		Size: 277.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dd619103d38407e95e05dd7d7f228e66bb5a61f3b561beb35198e92f9cdd0b99`  
		Last Modified: Tue, 03 Oct 2023 19:06:18 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:alpine3.18` - unknown; unknown

```console
$ docker pull memcached@sha256:aaa2281dd27a5acbf1364325e1d6ff0a576cfd236847437e2382c07b7199c2ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.3 KB (93262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f9ccd98630f55e4cdd33076a1d3e7f9c11399077a20d0aa9f5af15fcb40bd81`

```dockerfile
```

-	Layers:
	-	`sha256:9c3b535b067358c4894b956bcbf5380d163ce977d0c30028d799f467af8f87d6`  
		Last Modified: Tue, 03 Oct 2023 19:06:17 GMT  
		Size: 74.4 KB (74406 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:9d03d340727841dba89e688d83cd797f9808417dd8d04970fd76395482b117ff`  
		Last Modified: Tue, 03 Oct 2023 19:06:17 GMT  
		Size: 18.9 KB (18856 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:alpine3.18` - linux; s390x

```console
$ docker pull memcached@sha256:0ff7f30ca924f54a50160e70bd590b2ef357c97b6e8bbfcb81fdde97dd5cfbb0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4279633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad89852ec7f35640342fc548839c205af73d8c0f60e54c113b34e9dc519e71c3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["/bin/sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN apk add --no-cache libsasl # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1a648ad7883b3087dfacc17e14f4e6158d881dd1e09b9c5bd27bdd0d89ee44fd`  
		Last Modified: Tue, 03 Oct 2023 20:00:49 GMT  
		Size: 1.2 KB (1245 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a950f9727c19a31b79f709cdf984608d7788a9ed00dacbce4b14535b7589886f`  
		Last Modified: Tue, 03 Oct 2023 20:00:49 GMT  
		Size: 112.8 KB (112780 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b42424189685c7b481e859243008fea5d1967c6bbc3ccaaf13bf601c56926ebb`  
		Last Modified: Tue, 03 Oct 2023 20:00:49 GMT  
		Size: 950.1 KB (950102 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bf2263fe42a85daea831aafa6f50aeeef49d0ce1aa5841ddde0951667f85b684`  
		Last Modified: Tue, 03 Oct 2023 20:00:49 GMT  
		Size: 281.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:75eaf7af52231f2a4943c93eafc5d565b71c6079a1fee0fdc2605ad3eb81cd58`  
		Last Modified: Tue, 03 Oct 2023 20:00:49 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:alpine3.18` - unknown; unknown

```console
$ docker pull memcached@sha256:d2b9bd3538d99a100b4ebf104d9d5029917eecd3eec97d7086f7e4244b373d10
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.1 KB (93124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ade4e328bfbe610c689ab718878e6d07c31e5b67895795550a21d77730847d83`

```dockerfile
```

-	Layers:
	-	`sha256:7350d7c047abc3727f9639268d2cc1a5d7e53cbc81ae534da5e93272b5a48b59`  
		Last Modified: Tue, 03 Oct 2023 20:00:49 GMT  
		Size: 74.3 KB (74336 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:39706e52b9159fe158fe5027b73cb21482efb8781e1ab8853bcb19fc8125bbc8`  
		Last Modified: Tue, 03 Oct 2023 20:00:49 GMT  
		Size: 18.8 KB (18788 bytes)  
		MIME: application/vnd.in-toto+json

## `memcached:bookworm`

```console
$ docker pull memcached@sha256:eef4a056175ad8203df2a1835ae16307e5a70aec3222b409d1114486b2a4bb65
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
$ docker pull memcached@sha256:8af51889f0f774a00f36624e58faac309c258eafb8054c6abc6fbbb56c78d0a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.8 MB (38811465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fa23f6ace109fad9223ea2db53f79afa8b91b14051c61305f82bc2c781a788c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:55ad846fa191e603f48090eae0e4a7149c4066b94406593ec1898ad2c3347937 in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a378f10b321842c3042cdeff4f6997f34f4cb21f2eff27704b7f6193ab7b5fea`  
		Last Modified: Wed, 11 Oct 2023 18:39:34 GMT  
		Size: 29.1 MB (29149874 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e68aaf702a54364b3f216204ad2725f5b416fe496294086899b821bb5133552d`  
		Last Modified: Wed, 11 Oct 2023 20:07:27 GMT  
		Size: 1.1 KB (1110 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0fb853802e1447e9b1dbe3e8a86f27a5691286127397adf8d52f943d16b80042`  
		Last Modified: Wed, 11 Oct 2023 20:07:27 GMT  
		Size: 2.5 MB (2488274 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fcc9694d882f053fcf2e7bb33709dcb86eef6c29c3187c190ad93852af7a50f2`  
		Last Modified: Wed, 11 Oct 2023 20:07:28 GMT  
		Size: 7.2 MB (7171802 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fde136907f7040bd6126a5b2c0bca844fef33e2fc804c1f135e99393869cce4c`  
		Last Modified: Wed, 11 Oct 2023 20:07:27 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c121d0db5ccb2988b1fc0c76ce60a2e78309d77b264adf99e815e1ecf2c6a957`  
		Last Modified: Wed, 11 Oct 2023 20:07:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:888d3aaaddc944acb247f0e42586c8c8a7f8c3262166ee89ceda0dbe3998cafa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2911211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06530a2f7a54ba7d86fc6cee0da9a46ea1aea89dc4beecbee6d54ed8eee82dd9`

```dockerfile
```

-	Layers:
	-	`sha256:7bbbdfb4ba86ed51b46d2fb83bf8cf4e095da6d5c9dd89697a3488dd392414d7`  
		Last Modified: Wed, 11 Oct 2023 20:07:27 GMT  
		Size: 2.9 MB (2889442 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:6fe7a995830937695f7110928df7e791673ab04015add73a1f2e9ec661bbc60f`  
		Last Modified: Wed, 11 Oct 2023 20:07:27 GMT  
		Size: 21.8 KB (21769 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:bookworm` - linux; arm variant v5

```console
$ docker pull memcached@sha256:a6919fc9976aa2c291f194860f40fcc9499d33cbd2592af9087e5d64b7930602
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34846023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5222dddac963b84d55ef902d40fa3f949ee73caac9614ca77c1f4a81ef009c6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:8c43adb3245fc6f2b10aa5a86c850db5dcf3515eaf7e46630922fe21f806bd2a in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:904e6393ef1ee28b37171369eb4f7cb04714631c711799819fccb83886bd212b`  
		Last Modified: Wed, 11 Oct 2023 17:40:47 GMT  
		Size: 26.9 MB (26922150 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f0569355cb85b70d6a614ea9604289ce8e724f0f9ff4d1d8a12afc24c4c9ad1f`  
		Last Modified: Thu, 12 Oct 2023 08:32:05 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6939032c8ff0687b012a85d3411c702266b934a677f96eb521658b44f5b4a8c0`  
		Last Modified: Thu, 12 Oct 2023 08:32:06 GMT  
		Size: 2.1 MB (2089182 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8e8a2a7338b5cacc7b6e4e3db2359eebb1936b0b14266d5bad0dfcc21c9becff`  
		Last Modified: Thu, 12 Oct 2023 08:32:06 GMT  
		Size: 5.8 MB (5833176 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:19f35a8116fe7e124bee612b2ac511694077a1f35f76ed056903987ab4921e34`  
		Last Modified: Thu, 12 Oct 2023 08:32:06 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a43775be6dfac6c255e35b164eacd7328df241f33f9245206a8eaf481062ccbc`  
		Last Modified: Thu, 12 Oct 2023 08:32:07 GMT  
		Size: 120.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:f1276a05a4db6e8b7bb9d8374d480b85a79f1b92d4e7475c65e247bf1427200c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.7 KB (21695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe67b683a818ed7c22a49086ec4f22e53c6efa9040becea46adb07f550dae564`

```dockerfile
```

-	Layers:
	-	`sha256:12ecc330d2059d33dc7a7c518e7be06804f5fcadafdc8e2db030631f5c92b326`  
		Last Modified: Thu, 12 Oct 2023 08:32:05 GMT  
		Size: 21.7 KB (21695 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:bookworm` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:0c25b3c626a396c236dcf08792c850a178482c24e0c9dab0e784783178d10c13
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.4 MB (43442272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1595a8aa58bfc22ba6e995a58c63ea8b660aa8a9b10c57ab0cb8552d94080218`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:ec1a6e0aedd76c8fdc8544775f8b553f58950e9435f5cfe919f39374e222cfbb in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:e886f0f47ef56fcadb6ecaf2116056bbdb273e0afe07ed034498b198d386c04e`  
		Last Modified: Wed, 20 Sep 2023 02:47:36 GMT  
		Size: 29.2 MB (29157221 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7e25b15fcaee53caa22717c5b0b52fabf2480b0244a84530fca4c1edbb812044`  
		Last Modified: Tue, 03 Oct 2023 19:00:54 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:72fc5c44d6b752d2c2534f97f12ef44f915803ec4e564d7c9eb90d9d7bda2297`  
		Last Modified: Tue, 03 Oct 2023 19:00:54 GMT  
		Size: 2.3 MB (2343087 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7ba30437e42c2aebda3182e43b83b90012dd19e31adb9dc25bb3b714385cdefe`  
		Last Modified: Tue, 03 Oct 2023 19:00:55 GMT  
		Size: 11.9 MB (11940448 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:70abb5efa4268d01b1dfe9f6775f8f85a7fe395141dcc28909aa52ea6b741971`  
		Last Modified: Tue, 03 Oct 2023 19:00:54 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5a87a9f60806e352855b340f2c0c3610b8053006f0f542077c3add7e70782663`  
		Last Modified: Tue, 03 Oct 2023 19:00:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:7a900749c7d177577d906a5d402b4a008b95ae3571e9de24b4f04060e8650d5d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2890735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:711e633b20942471e455d3210316a79109ffda2a13cb38f46bd9ab2d27c758ae`

```dockerfile
```

-	Layers:
	-	`sha256:6c4c4a32fc3b330e635796951e46bf9e6ed753212798e75baddd3a84e752de8c`  
		Last Modified: Tue, 03 Oct 2023 19:00:54 GMT  
		Size: 2.9 MB (2869112 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:d0ceb647ed388f03f95faf34bc93c1489afde267801855f46cfca84fca538c5a`  
		Last Modified: Tue, 03 Oct 2023 19:00:54 GMT  
		Size: 21.6 KB (21623 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:bookworm` - linux; 386

```console
$ docker pull memcached@sha256:dbf6fdd168abcb8b6fd831277bea0213784e54cdb824756684dd3b5337c42c65
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.6 MB (44649134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25680867a5df0eb88860f59d7855c9d7f3862a44283c1e59d608f9dbecff348b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:efe81f7066129aa6293627bfe4ea78b957897ba5ede951970156fccf1dbcde88 in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6ac07f93e07a1bad4555e13bd8efd06169988669fc88df95f4bf296a2b44523d`  
		Last Modified: Wed, 20 Sep 2023 00:46:48 GMT  
		Size: 30.1 MB (30141894 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:797b4215eddcf948eec0f19132f85ec1b0f3af264399e78d860bece37acc4888`  
		Last Modified: Tue, 03 Oct 2023 19:01:51 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3c78c0b20e6791912325d174e98f60d4f783c2f013f52ff3835892444d3a15d7`  
		Last Modified: Tue, 03 Oct 2023 19:01:51 GMT  
		Size: 2.5 MB (2490464 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c91bf1cea723f722413107daa57ab51060ab36a5f78fe8447568aa35be54fca5`  
		Last Modified: Tue, 03 Oct 2023 19:01:52 GMT  
		Size: 12.0 MB (12015261 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:07f7206e609641792c84dfac85e3e6df0602c4ca8d572353a8768ff0619fe328`  
		Last Modified: Tue, 03 Oct 2023 19:01:51 GMT  
		Size: 283.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7aac14495f4a088e0e208638d0b36b0b5ff0cf945aaf24c011ef08ca799279a9`  
		Last Modified: Tue, 03 Oct 2023 19:01:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:16c8db3d95a2df8fae160a3942ff033ebb3bf6d9fe8df1643eb22c82e9402357
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 KB (21502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03bc49cf22d3ede52afc78d429b09999ba28174660a5e1b41fdb0f9d3a47067c`

```dockerfile
```

-	Layers:
	-	`sha256:890c3f7af1536aa0821f27c4ba142e022ba0c892f1310b4d82a9cc3a74717139`  
		Last Modified: Tue, 03 Oct 2023 19:01:51 GMT  
		Size: 21.5 KB (21502 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:bookworm` - linux; mips64le

```console
$ docker pull memcached@sha256:575825bdbf62fc255547394ef491710ba88f0be3ca735eaf246ece06f13363ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.4 MB (43398233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e3f951153522f4d9719c37a9862412f3e29e487d11322c5ff7a009cf8becca1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:850547a08e38ebc5a3659df86e70039a8d9828ae26ae485b077c98a959248dcb in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:0f581c6294fe7421dfee024e2c7dddd73ef3fbd7ff23b05bc3c1bf9f50885e85`  
		Last Modified: Wed, 20 Sep 2023 03:20:59 GMT  
		Size: 29.1 MB (29121674 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:15e25af5488ea4ad0df132fa2c22a282c1a17ad1460cdb25fe5939e03a753528`  
		Last Modified: Tue, 03 Oct 2023 19:04:40 GMT  
		Size: 1.1 KB (1113 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:19a5f416c9bf283212262e33fe8529d0ff3917fcee1e8ca9fb058170fd528211`  
		Last Modified: Tue, 03 Oct 2023 19:04:41 GMT  
		Size: 1.9 MB (1934931 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:05862af95003d85f9a1b5696dfb3588bdd8e34c74f067d845b722d70edfc679f`  
		Last Modified: Tue, 03 Oct 2023 19:04:41 GMT  
		Size: 12.3 MB (12340111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e8aae13855c46b73d2506b2d91036f6f0b4bc63b7d7ec12ecc63fd672c64c0f7`  
		Last Modified: Tue, 03 Oct 2023 19:04:40 GMT  
		Size: 282.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0709f88ce6a011ea45fd41c091ee6fcf4baa0610e0591a9fe0d10626eaf9475f`  
		Last Modified: Tue, 03 Oct 2023 19:04:41 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:269b3e28059bf711ac45886388e91fa405b8a1e0ca1a114acefc997bbdad6d05
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 KB (21491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1059a2662b538952006866f53463fcea773b5e090eaead3a4ad49f4d0a656ae5`

```dockerfile
```

-	Layers:
	-	`sha256:e1052b07541ae6e041e59834c527075b62df62a33f7a9b9e96fda4b6237e83df`  
		Last Modified: Tue, 03 Oct 2023 19:04:40 GMT  
		Size: 21.5 KB (21491 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:bookworm` - linux; ppc64le

```console
$ docker pull memcached@sha256:532cf0a6053275c508a0503017b4f52ce356a64aba047eb2316bdcaca35bbc9a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49635445 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:111f6d9d894ab95e36b94efa3dad4a4c9d0def1fa3af71a4a0e57e907a2b4986`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:9a37b479e68a0d18babbef8dd04d09a0e6844a0080876d14144a34bfd9d0897a in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:696a66e961f2033dcf69b003ad7faf28ed2248da58efa1c08a9d496739a8eeeb`  
		Last Modified: Wed, 20 Sep 2023 08:49:51 GMT  
		Size: 33.1 MB (33119461 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ba4c0c64bfd7ea845d20c793ede5957878785e4bb16e2e81a3e1ed5cd0d7ca0e`  
		Last Modified: Tue, 03 Oct 2023 19:02:08 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8a7ae673337cbb772a0ccc237ce4009a7dd88e4fed23861c9ea6382e93a6685b`  
		Last Modified: Tue, 03 Oct 2023 19:02:09 GMT  
		Size: 2.7 MB (2694930 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:766c713a6dbc39908803d95aa7556e0a571349c941bddb8f694b3f36030e0c3c`  
		Last Modified: Tue, 03 Oct 2023 19:02:10 GMT  
		Size: 13.8 MB (13819538 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:75734e09fa81ca91f8bdd1481c8f88f95ea9ba7b0f24ab82d0aee2026a5d6474`  
		Last Modified: Tue, 03 Oct 2023 19:02:09 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f46fc74a04a0607353cbc3ace76b49b44029af75080fa56fec872060d38feed2`  
		Last Modified: Tue, 03 Oct 2023 19:02:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:d73c6167b49dd216e6395e8720af5bd26884a25473d1eb80ee31d1e4b170a914
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2914816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48964548656eeecac440cb41e4f3f474f861d384c569653e582e3d508b04f6e5`

```dockerfile
```

-	Layers:
	-	`sha256:4e89c387c1399e94faaaf407614d23c90aa3104b5773f87d8cb4fe4b20312f8e`  
		Last Modified: Tue, 03 Oct 2023 19:02:09 GMT  
		Size: 2.9 MB (2893143 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:fb96286b26618de71f0df13dfc89225bc855d6802341b4032f0fb4161cb4a52e`  
		Last Modified: Tue, 03 Oct 2023 19:02:08 GMT  
		Size: 21.7 KB (21673 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:bookworm` - linux; s390x

```console
$ docker pull memcached@sha256:42a17150fd8b17aff6910890bbab808eab97e6f9d0f60003e75fac6ddd2b0bcf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40575835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:956090eeead5cd8ec7753b439eb43ddf3b2c5cd93edea3d7ce5bcdd168ec7588`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:6ed982ad3e8566d63315a27a81b33069910952aef4b2d3e0b607bd2caeac7ca4 in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:26dcff366e33abcf08b812052a4c12496aa406aa267655e984aa7a84ca254cd8`  
		Last Modified: Wed, 20 Sep 2023 02:59:47 GMT  
		Size: 27.5 MB (27489966 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:04795616cce62da1faee69d189f2f4863a3818651e9f54e7552be41e35752766`  
		Last Modified: Tue, 03 Oct 2023 19:01:27 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cbacb720efba986e695a3270bc384924abb78c413d1c4793cd388fbab1da828b`  
		Last Modified: Tue, 03 Oct 2023 19:01:27 GMT  
		Size: 2.2 MB (2150908 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:07a927de051febdc6284e8ec146cbc267ffdd1049fadf2bc35639f53b72b7862`  
		Last Modified: Tue, 03 Oct 2023 19:01:28 GMT  
		Size: 10.9 MB (10933444 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5a2703a37bdc4f133106c52c5a040d30708c01a79aa0d1714bcba3b42105692e`  
		Last Modified: Tue, 03 Oct 2023 19:01:28 GMT  
		Size: 285.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c0a860b98e7d941cd44043f66c4cc9d2a540ab3b8cb9aa15123102865599e0c7`  
		Last Modified: Tue, 03 Oct 2023 19:01:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:029d2884ff06e1b3673d9a7998c7299cc3da7ed18f46b344e13c14867574bae4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2897027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e57e1f9eb901fd307d1e2dd72b5606ba1f6f0ef82c31c01041513ed98e33b55`

```dockerfile
```

-	Layers:
	-	`sha256:13af4843cce0c7df5b25984623ef20fe08955ca99bbc64f5056c4d1bb2062f13`  
		Last Modified: Tue, 03 Oct 2023 19:01:27 GMT  
		Size: 2.9 MB (2875422 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:2e615a884e0baa9f5e54063b8983b99c841ac4fd854bf56780c1184d51637b1d`  
		Last Modified: Tue, 03 Oct 2023 19:01:27 GMT  
		Size: 21.6 KB (21605 bytes)  
		MIME: application/vnd.in-toto+json

## `memcached:latest`

```console
$ docker pull memcached@sha256:392f01c0e85fa9aeb0308a0c3b43b1ecde43203929c1d56d87ac469fd3d3e0a6
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
$ docker pull memcached@sha256:8af51889f0f774a00f36624e58faac309c258eafb8054c6abc6fbbb56c78d0a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.8 MB (38811465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fa23f6ace109fad9223ea2db53f79afa8b91b14051c61305f82bc2c781a788c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:55ad846fa191e603f48090eae0e4a7149c4066b94406593ec1898ad2c3347937 in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a378f10b321842c3042cdeff4f6997f34f4cb21f2eff27704b7f6193ab7b5fea`  
		Last Modified: Wed, 11 Oct 2023 18:39:34 GMT  
		Size: 29.1 MB (29149874 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e68aaf702a54364b3f216204ad2725f5b416fe496294086899b821bb5133552d`  
		Last Modified: Wed, 11 Oct 2023 20:07:27 GMT  
		Size: 1.1 KB (1110 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0fb853802e1447e9b1dbe3e8a86f27a5691286127397adf8d52f943d16b80042`  
		Last Modified: Wed, 11 Oct 2023 20:07:27 GMT  
		Size: 2.5 MB (2488274 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fcc9694d882f053fcf2e7bb33709dcb86eef6c29c3187c190ad93852af7a50f2`  
		Last Modified: Wed, 11 Oct 2023 20:07:28 GMT  
		Size: 7.2 MB (7171802 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fde136907f7040bd6126a5b2c0bca844fef33e2fc804c1f135e99393869cce4c`  
		Last Modified: Wed, 11 Oct 2023 20:07:27 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c121d0db5ccb2988b1fc0c76ce60a2e78309d77b264adf99e815e1ecf2c6a957`  
		Last Modified: Wed, 11 Oct 2023 20:07:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:latest` - unknown; unknown

```console
$ docker pull memcached@sha256:888d3aaaddc944acb247f0e42586c8c8a7f8c3262166ee89ceda0dbe3998cafa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2911211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06530a2f7a54ba7d86fc6cee0da9a46ea1aea89dc4beecbee6d54ed8eee82dd9`

```dockerfile
```

-	Layers:
	-	`sha256:7bbbdfb4ba86ed51b46d2fb83bf8cf4e095da6d5c9dd89697a3488dd392414d7`  
		Last Modified: Wed, 11 Oct 2023 20:07:27 GMT  
		Size: 2.9 MB (2889442 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:6fe7a995830937695f7110928df7e791673ab04015add73a1f2e9ec661bbc60f`  
		Last Modified: Wed, 11 Oct 2023 20:07:27 GMT  
		Size: 21.8 KB (21769 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:latest` - linux; arm variant v5

```console
$ docker pull memcached@sha256:a6919fc9976aa2c291f194860f40fcc9499d33cbd2592af9087e5d64b7930602
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34846023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5222dddac963b84d55ef902d40fa3f949ee73caac9614ca77c1f4a81ef009c6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:8c43adb3245fc6f2b10aa5a86c850db5dcf3515eaf7e46630922fe21f806bd2a in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:904e6393ef1ee28b37171369eb4f7cb04714631c711799819fccb83886bd212b`  
		Last Modified: Wed, 11 Oct 2023 17:40:47 GMT  
		Size: 26.9 MB (26922150 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f0569355cb85b70d6a614ea9604289ce8e724f0f9ff4d1d8a12afc24c4c9ad1f`  
		Last Modified: Thu, 12 Oct 2023 08:32:05 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6939032c8ff0687b012a85d3411c702266b934a677f96eb521658b44f5b4a8c0`  
		Last Modified: Thu, 12 Oct 2023 08:32:06 GMT  
		Size: 2.1 MB (2089182 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8e8a2a7338b5cacc7b6e4e3db2359eebb1936b0b14266d5bad0dfcc21c9becff`  
		Last Modified: Thu, 12 Oct 2023 08:32:06 GMT  
		Size: 5.8 MB (5833176 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:19f35a8116fe7e124bee612b2ac511694077a1f35f76ed056903987ab4921e34`  
		Last Modified: Thu, 12 Oct 2023 08:32:06 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a43775be6dfac6c255e35b164eacd7328df241f33f9245206a8eaf481062ccbc`  
		Last Modified: Thu, 12 Oct 2023 08:32:07 GMT  
		Size: 120.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:latest` - unknown; unknown

```console
$ docker pull memcached@sha256:f1276a05a4db6e8b7bb9d8374d480b85a79f1b92d4e7475c65e247bf1427200c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.7 KB (21695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe67b683a818ed7c22a49086ec4f22e53c6efa9040becea46adb07f550dae564`

```dockerfile
```

-	Layers:
	-	`sha256:12ecc330d2059d33dc7a7c518e7be06804f5fcadafdc8e2db030631f5c92b326`  
		Last Modified: Thu, 12 Oct 2023 08:32:05 GMT  
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
$ docker pull memcached@sha256:0c25b3c626a396c236dcf08792c850a178482c24e0c9dab0e784783178d10c13
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.4 MB (43442272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1595a8aa58bfc22ba6e995a58c63ea8b660aa8a9b10c57ab0cb8552d94080218`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:ec1a6e0aedd76c8fdc8544775f8b553f58950e9435f5cfe919f39374e222cfbb in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:e886f0f47ef56fcadb6ecaf2116056bbdb273e0afe07ed034498b198d386c04e`  
		Last Modified: Wed, 20 Sep 2023 02:47:36 GMT  
		Size: 29.2 MB (29157221 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7e25b15fcaee53caa22717c5b0b52fabf2480b0244a84530fca4c1edbb812044`  
		Last Modified: Tue, 03 Oct 2023 19:00:54 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:72fc5c44d6b752d2c2534f97f12ef44f915803ec4e564d7c9eb90d9d7bda2297`  
		Last Modified: Tue, 03 Oct 2023 19:00:54 GMT  
		Size: 2.3 MB (2343087 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7ba30437e42c2aebda3182e43b83b90012dd19e31adb9dc25bb3b714385cdefe`  
		Last Modified: Tue, 03 Oct 2023 19:00:55 GMT  
		Size: 11.9 MB (11940448 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:70abb5efa4268d01b1dfe9f6775f8f85a7fe395141dcc28909aa52ea6b741971`  
		Last Modified: Tue, 03 Oct 2023 19:00:54 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5a87a9f60806e352855b340f2c0c3610b8053006f0f542077c3add7e70782663`  
		Last Modified: Tue, 03 Oct 2023 19:00:55 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:latest` - unknown; unknown

```console
$ docker pull memcached@sha256:7a900749c7d177577d906a5d402b4a008b95ae3571e9de24b4f04060e8650d5d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2890735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:711e633b20942471e455d3210316a79109ffda2a13cb38f46bd9ab2d27c758ae`

```dockerfile
```

-	Layers:
	-	`sha256:6c4c4a32fc3b330e635796951e46bf9e6ed753212798e75baddd3a84e752de8c`  
		Last Modified: Tue, 03 Oct 2023 19:00:54 GMT  
		Size: 2.9 MB (2869112 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:d0ceb647ed388f03f95faf34bc93c1489afde267801855f46cfca84fca538c5a`  
		Last Modified: Tue, 03 Oct 2023 19:00:54 GMT  
		Size: 21.6 KB (21623 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:latest` - linux; 386

```console
$ docker pull memcached@sha256:dbf6fdd168abcb8b6fd831277bea0213784e54cdb824756684dd3b5337c42c65
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.6 MB (44649134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25680867a5df0eb88860f59d7855c9d7f3862a44283c1e59d608f9dbecff348b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:efe81f7066129aa6293627bfe4ea78b957897ba5ede951970156fccf1dbcde88 in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6ac07f93e07a1bad4555e13bd8efd06169988669fc88df95f4bf296a2b44523d`  
		Last Modified: Wed, 20 Sep 2023 00:46:48 GMT  
		Size: 30.1 MB (30141894 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:797b4215eddcf948eec0f19132f85ec1b0f3af264399e78d860bece37acc4888`  
		Last Modified: Tue, 03 Oct 2023 19:01:51 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3c78c0b20e6791912325d174e98f60d4f783c2f013f52ff3835892444d3a15d7`  
		Last Modified: Tue, 03 Oct 2023 19:01:51 GMT  
		Size: 2.5 MB (2490464 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c91bf1cea723f722413107daa57ab51060ab36a5f78fe8447568aa35be54fca5`  
		Last Modified: Tue, 03 Oct 2023 19:01:52 GMT  
		Size: 12.0 MB (12015261 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:07f7206e609641792c84dfac85e3e6df0602c4ca8d572353a8768ff0619fe328`  
		Last Modified: Tue, 03 Oct 2023 19:01:51 GMT  
		Size: 283.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7aac14495f4a088e0e208638d0b36b0b5ff0cf945aaf24c011ef08ca799279a9`  
		Last Modified: Tue, 03 Oct 2023 19:01:53 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:latest` - unknown; unknown

```console
$ docker pull memcached@sha256:16c8db3d95a2df8fae160a3942ff033ebb3bf6d9fe8df1643eb22c82e9402357
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 KB (21502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03bc49cf22d3ede52afc78d429b09999ba28174660a5e1b41fdb0f9d3a47067c`

```dockerfile
```

-	Layers:
	-	`sha256:890c3f7af1536aa0821f27c4ba142e022ba0c892f1310b4d82a9cc3a74717139`  
		Last Modified: Tue, 03 Oct 2023 19:01:51 GMT  
		Size: 21.5 KB (21502 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:latest` - linux; mips64le

```console
$ docker pull memcached@sha256:575825bdbf62fc255547394ef491710ba88f0be3ca735eaf246ece06f13363ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.4 MB (43398233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e3f951153522f4d9719c37a9862412f3e29e487d11322c5ff7a009cf8becca1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:850547a08e38ebc5a3659df86e70039a8d9828ae26ae485b077c98a959248dcb in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:0f581c6294fe7421dfee024e2c7dddd73ef3fbd7ff23b05bc3c1bf9f50885e85`  
		Last Modified: Wed, 20 Sep 2023 03:20:59 GMT  
		Size: 29.1 MB (29121674 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:15e25af5488ea4ad0df132fa2c22a282c1a17ad1460cdb25fe5939e03a753528`  
		Last Modified: Tue, 03 Oct 2023 19:04:40 GMT  
		Size: 1.1 KB (1113 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:19a5f416c9bf283212262e33fe8529d0ff3917fcee1e8ca9fb058170fd528211`  
		Last Modified: Tue, 03 Oct 2023 19:04:41 GMT  
		Size: 1.9 MB (1934931 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:05862af95003d85f9a1b5696dfb3588bdd8e34c74f067d845b722d70edfc679f`  
		Last Modified: Tue, 03 Oct 2023 19:04:41 GMT  
		Size: 12.3 MB (12340111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e8aae13855c46b73d2506b2d91036f6f0b4bc63b7d7ec12ecc63fd672c64c0f7`  
		Last Modified: Tue, 03 Oct 2023 19:04:40 GMT  
		Size: 282.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0709f88ce6a011ea45fd41c091ee6fcf4baa0610e0591a9fe0d10626eaf9475f`  
		Last Modified: Tue, 03 Oct 2023 19:04:41 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:latest` - unknown; unknown

```console
$ docker pull memcached@sha256:269b3e28059bf711ac45886388e91fa405b8a1e0ca1a114acefc997bbdad6d05
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 KB (21491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1059a2662b538952006866f53463fcea773b5e090eaead3a4ad49f4d0a656ae5`

```dockerfile
```

-	Layers:
	-	`sha256:e1052b07541ae6e041e59834c527075b62df62a33f7a9b9e96fda4b6237e83df`  
		Last Modified: Tue, 03 Oct 2023 19:04:40 GMT  
		Size: 21.5 KB (21491 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:latest` - linux; ppc64le

```console
$ docker pull memcached@sha256:532cf0a6053275c508a0503017b4f52ce356a64aba047eb2316bdcaca35bbc9a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49635445 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:111f6d9d894ab95e36b94efa3dad4a4c9d0def1fa3af71a4a0e57e907a2b4986`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:9a37b479e68a0d18babbef8dd04d09a0e6844a0080876d14144a34bfd9d0897a in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:696a66e961f2033dcf69b003ad7faf28ed2248da58efa1c08a9d496739a8eeeb`  
		Last Modified: Wed, 20 Sep 2023 08:49:51 GMT  
		Size: 33.1 MB (33119461 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ba4c0c64bfd7ea845d20c793ede5957878785e4bb16e2e81a3e1ed5cd0d7ca0e`  
		Last Modified: Tue, 03 Oct 2023 19:02:08 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8a7ae673337cbb772a0ccc237ce4009a7dd88e4fed23861c9ea6382e93a6685b`  
		Last Modified: Tue, 03 Oct 2023 19:02:09 GMT  
		Size: 2.7 MB (2694930 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:766c713a6dbc39908803d95aa7556e0a571349c941bddb8f694b3f36030e0c3c`  
		Last Modified: Tue, 03 Oct 2023 19:02:10 GMT  
		Size: 13.8 MB (13819538 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:75734e09fa81ca91f8bdd1481c8f88f95ea9ba7b0f24ab82d0aee2026a5d6474`  
		Last Modified: Tue, 03 Oct 2023 19:02:09 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f46fc74a04a0607353cbc3ace76b49b44029af75080fa56fec872060d38feed2`  
		Last Modified: Tue, 03 Oct 2023 19:02:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:latest` - unknown; unknown

```console
$ docker pull memcached@sha256:d73c6167b49dd216e6395e8720af5bd26884a25473d1eb80ee31d1e4b170a914
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2914816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48964548656eeecac440cb41e4f3f474f861d384c569653e582e3d508b04f6e5`

```dockerfile
```

-	Layers:
	-	`sha256:4e89c387c1399e94faaaf407614d23c90aa3104b5773f87d8cb4fe4b20312f8e`  
		Last Modified: Tue, 03 Oct 2023 19:02:09 GMT  
		Size: 2.9 MB (2893143 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:fb96286b26618de71f0df13dfc89225bc855d6802341b4032f0fb4161cb4a52e`  
		Last Modified: Tue, 03 Oct 2023 19:02:08 GMT  
		Size: 21.7 KB (21673 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:latest` - linux; s390x

```console
$ docker pull memcached@sha256:42a17150fd8b17aff6910890bbab808eab97e6f9d0f60003e75fac6ddd2b0bcf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40575835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:956090eeead5cd8ec7753b439eb43ddf3b2c5cd93edea3d7ce5bcdd168ec7588`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:6ed982ad3e8566d63315a27a81b33069910952aef4b2d3e0b607bd2caeac7ca4 in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:26dcff366e33abcf08b812052a4c12496aa406aa267655e984aa7a84ca254cd8`  
		Last Modified: Wed, 20 Sep 2023 02:59:47 GMT  
		Size: 27.5 MB (27489966 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:04795616cce62da1faee69d189f2f4863a3818651e9f54e7552be41e35752766`  
		Last Modified: Tue, 03 Oct 2023 19:01:27 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cbacb720efba986e695a3270bc384924abb78c413d1c4793cd388fbab1da828b`  
		Last Modified: Tue, 03 Oct 2023 19:01:27 GMT  
		Size: 2.2 MB (2150908 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:07a927de051febdc6284e8ec146cbc267ffdd1049fadf2bc35639f53b72b7862`  
		Last Modified: Tue, 03 Oct 2023 19:01:28 GMT  
		Size: 10.9 MB (10933444 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5a2703a37bdc4f133106c52c5a040d30708c01a79aa0d1714bcba3b42105692e`  
		Last Modified: Tue, 03 Oct 2023 19:01:28 GMT  
		Size: 285.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c0a860b98e7d941cd44043f66c4cc9d2a540ab3b8cb9aa15123102865599e0c7`  
		Last Modified: Tue, 03 Oct 2023 19:01:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:latest` - unknown; unknown

```console
$ docker pull memcached@sha256:029d2884ff06e1b3673d9a7998c7299cc3da7ed18f46b344e13c14867574bae4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2897027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e57e1f9eb901fd307d1e2dd72b5606ba1f6f0ef82c31c01041513ed98e33b55`

```dockerfile
```

-	Layers:
	-	`sha256:13af4843cce0c7df5b25984623ef20fe08955ca99bbc64f5056c4d1bb2062f13`  
		Last Modified: Tue, 03 Oct 2023 19:01:27 GMT  
		Size: 2.9 MB (2875422 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:2e615a884e0baa9f5e54063b8983b99c841ac4fd854bf56780c1184d51637b1d`  
		Last Modified: Tue, 03 Oct 2023 19:01:27 GMT  
		Size: 21.6 KB (21605 bytes)  
		MIME: application/vnd.in-toto+json
