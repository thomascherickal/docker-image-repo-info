<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `memcached`

-	[`memcached:1`](#memcached1)
-	[`memcached:1-alpine`](#memcached1-alpine)
-	[`memcached:1-alpine3.15`](#memcached1-alpine315)
-	[`memcached:1-bullseye`](#memcached1-bullseye)
-	[`memcached:1.6`](#memcached16)
-	[`memcached:1.6-alpine`](#memcached16-alpine)
-	[`memcached:1.6-alpine3.15`](#memcached16-alpine315)
-	[`memcached:1.6-bullseye`](#memcached16-bullseye)
-	[`memcached:1.6.15`](#memcached1615)
-	[`memcached:1.6.15-alpine`](#memcached1615-alpine)
-	[`memcached:1.6.15-alpine3.15`](#memcached1615-alpine315)
-	[`memcached:1.6.15-bullseye`](#memcached1615-bullseye)
-	[`memcached:alpine`](#memcachedalpine)
-	[`memcached:alpine3.15`](#memcachedalpine315)
-	[`memcached:bullseye`](#memcachedbullseye)
-	[`memcached:latest`](#memcachedlatest)

## `memcached:1`

```console
$ docker pull memcached@sha256:05917d8f91b97eff3ffb98497dd139c65f61c2107649cf73db6cced7e7667b94
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

### `memcached:1` - linux; amd64

```console
$ docker pull memcached@sha256:58a41bfdd7492d7d9be5ea8ab1abeffa106a2193e98e6646be91d06ad37d0675
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32968652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:065555a745051537085b4135608198e45686d4574eda4d7093537d1107a1feff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 11 May 2022 01:20:16 GMT
ADD file:4a0bb88956083aa56032fdd9601d9b66c39b18c896ba35ea33594cd75621640a in / 
# Wed, 11 May 2022 01:20:16 GMT
CMD ["bash"]
# Wed, 11 May 2022 04:44:00 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 11 May 2022 04:44:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 04:44:03 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 11 May 2022 04:44:03 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 11 May 2022 04:46:42 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 May 2022 04:46:42 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 May 2022 04:46:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 04:46:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 04:46:43 GMT
USER memcache
# Wed, 11 May 2022 04:46:43 GMT
EXPOSE 11211
# Wed, 11 May 2022 04:46:43 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:214ca5fb90323fe769c63a12af092f2572bf1c6b300263e09883909fc865d260`  
		Last Modified: Wed, 11 May 2022 01:25:13 GMT  
		Size: 31.4 MB (31379476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae8d4b1feabc5879929064e635eb9f14ef5b8a15bac772048359ca7ff051d1c`  
		Last Modified: Wed, 11 May 2022 04:47:13 GMT  
		Size: 5.0 KB (4975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dc491b9af677c0a71fa36fcbf2faea8087acafa69e2d760fcaea4f26fb5eb2a`  
		Last Modified: Wed, 11 May 2022 04:47:14 GMT  
		Size: 328.1 KB (328091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c355a147dff081cfbbf9d104870e2195eb0213138ae88d87a585b466fc521d4a`  
		Last Modified: Wed, 11 May 2022 04:47:14 GMT  
		Size: 1.3 MB (1255702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0cc0d566fb2a731f9d4dd270354fe902ec4b175b95e3552e17d53a76601b28d`  
		Last Modified: Wed, 11 May 2022 04:47:13 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d5c91075c8421465ad8ef2fe32f6daab4ff01b837e03aee3568d39c64cb2d3`  
		Last Modified: Wed, 11 May 2022 04:47:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm variant v5

```console
$ docker pull memcached@sha256:7114dc5aaa1603875d79f65e4d27cf83fd5c6ff279092e5019313c2e676e8563
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30469996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:711c043049190c6786a1fe335232c7bee5a0c58134e9481f385ae99e18cff3a2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 11 May 2022 00:50:34 GMT
ADD file:72357b75d7e4546f06abf4648ab600980e742a3017f36da3c7a6c086f2f5fb56 in / 
# Wed, 11 May 2022 00:50:35 GMT
CMD ["bash"]
# Wed, 11 May 2022 19:59:38 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 11 May 2022 19:59:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 19:59:48 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 11 May 2022 19:59:49 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 11 May 2022 20:04:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 May 2022 20:04:12 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 May 2022 20:04:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 20:04:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 20:04:14 GMT
USER memcache
# Wed, 11 May 2022 20:04:15 GMT
EXPOSE 11211
# Wed, 11 May 2022 20:04:15 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f7b69be15db1cb94a249f74b27edd4f5e5923a8701b026179a593f6888e897aa`  
		Last Modified: Wed, 11 May 2022 01:05:51 GMT  
		Size: 28.9 MB (28921122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e23defdefe7366c4546b3284b11bdbedcf73c55c4cad0c49a2e12b6bc971f653`  
		Last Modified: Wed, 11 May 2022 20:05:07 GMT  
		Size: 4.9 KB (4893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aed101d7cb94db52f647e3cf585d3a7702b5a01cb3f7c3fc86aedcd94fb5b01`  
		Last Modified: Wed, 11 May 2022 20:05:07 GMT  
		Size: 316.6 KB (316610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80e354b9ae9a23ca02681ddaca03fe3a6fa45069b80a683e38123aa3a0174fab`  
		Last Modified: Wed, 11 May 2022 20:05:08 GMT  
		Size: 1.2 MB (1226962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d82b2d2d5ab7db68fddbbf26596ed21c9c4506e0355be942188f9a81557bdd`  
		Last Modified: Wed, 11 May 2022 20:05:07 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd35d60f098711fce5b4a2d107b57cfe22a70cbb6bf47476c42ea4d975b6c3f7`  
		Last Modified: Wed, 11 May 2022 20:05:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm variant v7

```console
$ docker pull memcached@sha256:34dee5b2772158236707bc1811db77d4adc27d86ca6b1b096fb444a8cfef133e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28091607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad29267829b7cd5d6051ca12869e51112bded24fc2e06656b673942a215f1c84`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 20 Apr 2022 13:27:18 GMT
ADD file:1a0e290eb32b3533f9d1684c683ad866b5003579790b25ad61b2044dc6c20bbb in / 
# Wed, 20 Apr 2022 13:27:18 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 21:47:36 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 20 Apr 2022 21:47:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 21:47:45 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 20 Apr 2022 21:47:45 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 20 Apr 2022 21:51:42 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 20 Apr 2022 21:51:42 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 20 Apr 2022 21:51:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 20 Apr 2022 21:51:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Apr 2022 21:51:45 GMT
USER memcache
# Wed, 20 Apr 2022 21:51:45 GMT
EXPOSE 11211
# Wed, 20 Apr 2022 21:51:46 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a6b2963233cd14b47391f0e25f2a485bbeabb87e771a71b73e5cde7c013963da`  
		Last Modified: Wed, 20 Apr 2022 13:43:41 GMT  
		Size: 26.6 MB (26575758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4b149950ca557655b7e9b7229a81d7d772f2aad316a5ce7de452664795a377`  
		Last Modified: Wed, 20 Apr 2022 22:04:23 GMT  
		Size: 4.9 KB (4893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d14f3b12cc24aac4e3614237409e18959637d8420b534524bc1fe63e7456a660`  
		Last Modified: Wed, 20 Apr 2022 22:04:23 GMT  
		Size: 312.1 KB (312059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca5c1518bd4380c5c22f884d402b699c75cb53de72de7d5b2a53e99d8ba56d9e`  
		Last Modified: Wed, 20 Apr 2022 22:04:24 GMT  
		Size: 1.2 MB (1198488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd1a54f20b40e9c7302a4ab0c46cc590140bde81aba4ab1d149dd8b2b3edade`  
		Last Modified: Wed, 20 Apr 2022 22:04:23 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6e66d52d7551a05a10e5a70971eef4ad0803f499c934fd1ec734a144e5bc64`  
		Last Modified: Wed, 20 Apr 2022 22:04:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:6c452eece1271128806922efd79c0ef0f809e6705d855d6a271f5208d2a2117d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31444857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d45eed3b8e469acc08e97e874bb1e8b4f004720606f20212dad652f79ca29db4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 11 May 2022 00:46:59 GMT
ADD file:158a0e401328bd7c0d49b9e8539186098967218f1b1a8c811f4398d29b74397f in / 
# Wed, 11 May 2022 00:47:00 GMT
CMD ["bash"]
# Wed, 11 May 2022 02:27:34 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 11 May 2022 02:27:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:27:38 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 11 May 2022 02:27:39 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 11 May 2022 02:30:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 May 2022 02:30:13 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 May 2022 02:30:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 02:30:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 02:30:15 GMT
USER memcache
# Wed, 11 May 2022 02:30:16 GMT
EXPOSE 11211
# Wed, 11 May 2022 02:30:17 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:dfdd5ffb257742b891ccad9400a77dad2a6260b2451e0f5e48a9ade1d17a87ec`  
		Last Modified: Wed, 11 May 2022 00:53:46 GMT  
		Size: 30.1 MB (30065693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:921e9eec57430f29a509862965b1bc0f909703c8c5e73b2345205cbd6b715910`  
		Last Modified: Wed, 11 May 2022 02:31:07 GMT  
		Size: 4.9 KB (4900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:984aa2c2269106d51c47bed797929d496825d1dee8883d84918fd98cd809ba76`  
		Last Modified: Wed, 11 May 2022 02:31:07 GMT  
		Size: 119.2 KB (119215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b52324e4c1cc245d2131fae3776a0359730099f17e8039fa1db0d0b6310a195`  
		Last Modified: Wed, 11 May 2022 02:31:08 GMT  
		Size: 1.3 MB (1254642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70bc38e444a829155cb5ad8ca3f2b8cc68a6065e19b795707656cec98edadbfc`  
		Last Modified: Wed, 11 May 2022 02:31:07 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b29514622ffb8a37130cc9662034040cbc8ff1d5c7b8ce620f49c0d26b24b73`  
		Last Modified: Wed, 11 May 2022 02:31:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; 386

```console
$ docker pull memcached@sha256:faedc990d98e8f3b6058c1e3f9ace6816b59338aaf906a8099a0b1141713d345
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33778000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74fb9295e5de207e5aade7877e8b45371b49a320bf3eafbfe65ea15c6f70dd59`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 11 May 2022 01:39:14 GMT
ADD file:9eecb0fd311177f9d226e914c411aef49b5de1930e73019d2ee24afed515b5a2 in / 
# Wed, 11 May 2022 01:39:14 GMT
CMD ["bash"]
# Wed, 11 May 2022 04:32:45 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 11 May 2022 04:32:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 04:32:49 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 11 May 2022 04:32:50 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 11 May 2022 04:35:41 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 May 2022 04:35:43 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 May 2022 04:35:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 04:35:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 04:35:45 GMT
USER memcache
# Wed, 11 May 2022 04:35:46 GMT
EXPOSE 11211
# Wed, 11 May 2022 04:35:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:91c5bdbe4bf9f1970dd54ba71e2523649adce4e5240c2ff8a87711bf389ecba3`  
		Last Modified: Wed, 11 May 2022 01:46:25 GMT  
		Size: 32.4 MB (32389776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cbc080a4e6972a45023b1c0d8d9f74e9df257677ec7503a9f8756eabb61b5e0`  
		Last Modified: Wed, 11 May 2022 04:36:36 GMT  
		Size: 4.8 KB (4771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdfcc6e2f39957ee91e94aa2f1264a35ccef2b3aed8ae29d859144d763ed06ab`  
		Last Modified: Wed, 11 May 2022 04:36:36 GMT  
		Size: 130.1 KB (130140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a68472399b32a22e31b1b551482a4fec929210d4db3da6b3010fdb3a97bf0944`  
		Last Modified: Wed, 11 May 2022 04:36:37 GMT  
		Size: 1.3 MB (1252905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a1040db24a5a1a06568a3d81752b73f002172ebec23d3ace2181c365e6216c9`  
		Last Modified: Wed, 11 May 2022 04:36:36 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496cfb26b818ba873c9dbd7203c2551d9c1503db7a8281c82b03ecd7987dfe44`  
		Last Modified: Wed, 11 May 2022 04:36:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; mips64le

```console
$ docker pull memcached@sha256:d4d70ee02bd6a268e51e7cb45ae2ab6028a3f5546e3566abea4839b7bc0b2795
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31014729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5edfa57d6aec6089194206346467a5708554650f75a703542020f03dda6cfb13`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 11 May 2022 02:23:35 GMT
ADD file:d47dce2adbc9352ef1d437730bab3b579dd8d2bf29dd60cd8a8b65396b39e36e in / 
# Wed, 11 May 2022 02:23:40 GMT
CMD ["bash"]
# Wed, 11 May 2022 04:26:13 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 11 May 2022 04:26:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 04:26:33 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 11 May 2022 04:26:36 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 11 May 2022 04:33:31 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 May 2022 04:33:33 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 May 2022 04:33:38 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 04:33:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 04:33:43 GMT
USER memcache
# Wed, 11 May 2022 04:33:45 GMT
EXPOSE 11211
# Wed, 11 May 2022 04:33:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:438a36bf0b6e75ff6f0fbb2b7669dfb86361416f4d808912d30cf5b91ad2eea9`  
		Last Modified: Wed, 11 May 2022 02:33:43 GMT  
		Size: 29.6 MB (29641051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2947248cd8e754e130fecb9083b0ad0025e50361a44987eadfb6edfeb2e3908c`  
		Last Modified: Wed, 11 May 2022 04:34:05 GMT  
		Size: 4.9 KB (4861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3849c71c1ab16dd8196e74fd37ae70b3a0b89a3b07a9cb7f76535725af27a86a`  
		Last Modified: Wed, 11 May 2022 04:34:05 GMT  
		Size: 117.2 KB (117156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f24b722d80efb82b9982c69a407116125ad8a340447344e252517f9798849b9`  
		Last Modified: Wed, 11 May 2022 04:34:06 GMT  
		Size: 1.3 MB (1251254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f4827b1598450f78ff6da5317e269d8fdc544d21ff25409586a2db03053022`  
		Last Modified: Wed, 11 May 2022 04:34:05 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:090d97f72bbcf506ab0dc4d8e19c3a1522513237327ced2e711f0613fb262865`  
		Last Modified: Wed, 11 May 2022 04:34:05 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; ppc64le

```console
$ docker pull memcached@sha256:673643121e94f08dd12197b69994ec2cad834c15326b37ba83861eb00aa22134
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36971800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:821c76dba347fd635474ef0126da0d404cc404e989635b028d0da3c2dfb273b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 11 May 2022 01:32:29 GMT
ADD file:1e94716789ec21981460f74be38a668bc212bd804c1d41cecf90036a5bccac5a in / 
# Wed, 11 May 2022 01:32:34 GMT
CMD ["bash"]
# Wed, 11 May 2022 07:51:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 11 May 2022 07:51:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 07:51:40 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 11 May 2022 07:51:48 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 11 May 2022 07:57:31 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 May 2022 07:57:33 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 May 2022 07:57:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 07:57:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 07:57:49 GMT
USER memcache
# Wed, 11 May 2022 07:57:55 GMT
EXPOSE 11211
# Wed, 11 May 2022 07:58:00 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2533109ed11eefd6415e0370d6d7a3ea879b582b1887c98b819a598ad18fca24`  
		Last Modified: Wed, 11 May 2022 01:43:03 GMT  
		Size: 35.3 MB (35286467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:103a6713e9bf2853760692eb30b886453378b61e3fb83321c0ce1fec39bdf2f2`  
		Last Modified: Wed, 11 May 2022 07:59:13 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9173dced38a5c576a66100ed6df59833b82ee6847ed29531d690b7377a72e02d`  
		Last Modified: Wed, 11 May 2022 07:59:13 GMT  
		Size: 356.9 KB (356938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e15378aab9e7b0eefd835da5eeee5fe567c111dcf6df814b34f6755cf27c45`  
		Last Modified: Wed, 11 May 2022 07:59:13 GMT  
		Size: 1.3 MB (1323008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523888230dfa0221ad182120061be4802ac72d7a19047277ffc452c5003537b5`  
		Last Modified: Wed, 11 May 2022 07:59:13 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12893f041469d0edbc3132e6af823296c231a18db48dc29c665658f6ba859c9f`  
		Last Modified: Wed, 11 May 2022 07:59:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; s390x

```console
$ docker pull memcached@sha256:d0221a850100573af43f6113f62398369ddaa506aef1fd1e114da8fdd4403330
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31225739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37e72a40047bd848bbedd03871f17d8132f625301f2203038b265841fa1a660f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 11 May 2022 00:44:17 GMT
ADD file:d93a1cf64a813d01774cd628dfd683c006e20159e2ab3464c2159c8d9897c725 in / 
# Wed, 11 May 2022 00:44:19 GMT
CMD ["bash"]
# Wed, 11 May 2022 02:35:31 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 11 May 2022 02:35:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:35:34 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 11 May 2022 02:35:34 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 11 May 2022 02:39:02 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 May 2022 02:39:03 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 May 2022 02:39:03 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 02:39:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 02:39:03 GMT
USER memcache
# Wed, 11 May 2022 02:39:03 GMT
EXPOSE 11211
# Wed, 11 May 2022 02:39:04 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9f3750f6094217808e26d471752341db88153c8d5b5f9bb11577b74671303bbc`  
		Last Modified: Wed, 11 May 2022 00:50:03 GMT  
		Size: 29.7 MB (29654739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29541285df59f95a596b1911b49171e64e2361189a163533e77dbf2961b8f685`  
		Last Modified: Wed, 11 May 2022 02:40:04 GMT  
		Size: 5.0 KB (5026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c94a32e11bca5f817bc7015ceff49279fcd263d523198a38cc02607b7899e261`  
		Last Modified: Wed, 11 May 2022 02:40:04 GMT  
		Size: 324.2 KB (324197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57395e3cd66c2852ddaac636856f0245c1cfdca358d6bb75128950b9d9042481`  
		Last Modified: Wed, 11 May 2022 02:40:04 GMT  
		Size: 1.2 MB (1241369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ed03e37cb4ad7ab6dfc00b4938e9e5ec27777eb89fe1918ffc45a5a8de10c0`  
		Last Modified: Wed, 11 May 2022 02:40:04 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79cc46e5a2551dd05d1dcb476692b2a5d1c7e5181f253ad3938c179835018b95`  
		Last Modified: Wed, 11 May 2022 02:40:03 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1-alpine`

```console
$ docker pull memcached@sha256:0374a1e43929f2da9d7acf6887903eb3337ea92f0b8fd080aec28d2b902065aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1-alpine` - linux; amd64

```console
$ docker pull memcached@sha256:fbb3eda59b2f6851b1335f6fd43fa5a371ac197b06f84c0363341b7cd1c066f1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3864898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bcea36e93e267587df645dc2c39d08513419e129eb5b28db4a204207d64a9ea6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 09:54:14 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 05 Apr 2022 09:54:15 GMT
RUN apk add --no-cache libsasl
# Tue, 05 Apr 2022 09:54:15 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 05 Apr 2022 09:54:15 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 05 Apr 2022 09:57:57 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 05 Apr 2022 09:57:57 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 05 Apr 2022 09:57:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 05 Apr 2022 09:57:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 09:57:58 GMT
USER memcache
# Tue, 05 Apr 2022 09:57:58 GMT
EXPOSE 11211
# Tue, 05 Apr 2022 09:57:58 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c437462196847904d5021a85f817fecbb0b84eca04e4677f3a907f95125ebd3`  
		Last Modified: Tue, 05 Apr 2022 09:58:27 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37749f62d258e02c4f026b7ed0cb874d23b47abaa2c5860e41b3c099fdeb1d15`  
		Last Modified: Tue, 05 Apr 2022 09:58:27 GMT  
		Size: 109.2 KB (109172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf6c1e9f5167a143f222aea98c5b9c1d58ad0f9eed19d753fa1c4ffdfdd0269`  
		Last Modified: Tue, 05 Apr 2022 09:58:27 GMT  
		Size: 939.5 KB (939497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550e19164877083e509bb0c014a831674a7b77ddcf111d980a4f2b1bd1a78171`  
		Last Modified: Tue, 05 Apr 2022 09:58:27 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:515f37e9ad844fe3fdd82c3504b1c092e11e2c8f5f8395bc8944c96c768f3d3c`  
		Last Modified: Tue, 05 Apr 2022 09:58:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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
$ docker pull memcached@sha256:d38012edd86b9a7abab01b390d4bbce8c39201ebedfd0066fcff6b6fb20cf178
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3757025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e0f3d4ef24801f58b76d5d0e24224de96c6e02fba4eccb3fa2e037e94403f0a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:15:56 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 05 Apr 2022 04:15:57 GMT
RUN apk add --no-cache libsasl
# Tue, 05 Apr 2022 04:15:58 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 05 Apr 2022 04:15:59 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 05 Apr 2022 04:18:36 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 05 Apr 2022 04:18:37 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 05 Apr 2022 04:18:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 05 Apr 2022 04:18:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 04:18:39 GMT
USER memcache
# Tue, 05 Apr 2022 04:18:40 GMT
EXPOSE 11211
# Tue, 05 Apr 2022 04:18:41 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa012cdcd391bd8cd78796fe53eb96b7585962832b802667f44cedd88405d0cc`  
		Last Modified: Tue, 05 Apr 2022 04:19:28 GMT  
		Size: 1.2 KB (1238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca8ad568702372595d83e4a4b906e000230b00315e1fd6ef6d219697badb387`  
		Last Modified: Tue, 05 Apr 2022 04:19:28 GMT  
		Size: 110.5 KB (110499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:265ae8d237ddc109ffe7e544e93a0dc1cea5bfe3fa5685fca792afda6d67ed0f`  
		Last Modified: Tue, 05 Apr 2022 04:19:29 GMT  
		Size: 928.4 KB (928406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce17e42e65242140f2a8f7c6d0a16bf4f1b64b0ba276ed8341905ed6f63e4a7b`  
		Last Modified: Tue, 05 Apr 2022 04:19:28 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30070b7f5a7be9b35fb6b8c7f1b6cb0de4508d927cc49caf12b3f6e220b0cc60`  
		Last Modified: Tue, 05 Apr 2022 04:19:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; 386

```console
$ docker pull memcached@sha256:5378334a3366058f6987024a1963dceafda46b182d6236b4685f816238f99992
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3888728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be3d8aa97e2099f400479214a98c34c3a23c21939afde5c6611961b33539a8bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:25 GMT
ADD file:7d51a0f8691eb78c9062fd31984423a93d276a67b4ed5d1a706e1c2cd9fea23a in / 
# Mon, 04 Apr 2022 23:38:25 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:52:17 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 05 Apr 2022 03:52:18 GMT
RUN apk add --no-cache libsasl
# Tue, 05 Apr 2022 03:52:19 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 05 Apr 2022 03:52:20 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 05 Apr 2022 03:55:15 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 05 Apr 2022 03:55:17 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 05 Apr 2022 03:55:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 05 Apr 2022 03:55:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 03:55:19 GMT
USER memcache
# Tue, 05 Apr 2022 03:55:20 GMT
EXPOSE 11211
# Tue, 05 Apr 2022 03:55:21 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:73b28a5955ec7fb46f2cf0434e4901a889f7dda3f8c9ec496300feb256c7eda8`  
		Last Modified: Mon, 04 Apr 2022 19:10:03 GMT  
		Size: 2.8 MB (2818974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06cddc8f8c3aabebd92d18ccbc0c9181ed94cc4b15b5adbda9e2bfdf4b8f38e9`  
		Last Modified: Tue, 05 Apr 2022 03:56:08 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad8594347186db0e9366f74b1e03bd14ed234378b2d1238a6b56504a86608fa6`  
		Last Modified: Tue, 05 Apr 2022 03:56:08 GMT  
		Size: 120.9 KB (120869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d7907ab18015191139b22c9b7b25c6a23d1c569470a49f2eb3e1ef985c4450`  
		Last Modified: Tue, 05 Apr 2022 03:56:08 GMT  
		Size: 947.2 KB (947242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3d6dff2eb04a8a959a2e8d101ca3da2646db4b2125b02fd6505c61ce53215b`  
		Last Modified: Tue, 05 Apr 2022 03:56:08 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:845b50269336006037a46780211bf0b2b95df971864d348d10c893aa2bf3afe3`  
		Last Modified: Tue, 05 Apr 2022 03:56:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:d1110704ee41f1dce802400ce09904c39aff25c66c1e1b87c64781b0bd9527d4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3905105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1827e9495120e553b560bd77e162a97bfdb923a96c36b2dea8afd967fdc57bd1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:30 GMT
ADD file:960cf6f9d3d1cfcb36c2d67dd4c3eaba7db1d0c7afe97968512248d7f234ad47 in / 
# Tue, 05 Apr 2022 00:23:32 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 10:09:23 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 05 Apr 2022 10:09:31 GMT
RUN apk add --no-cache libsasl
# Tue, 05 Apr 2022 10:09:35 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 05 Apr 2022 10:09:41 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 05 Apr 2022 10:12:56 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 05 Apr 2022 10:12:58 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 05 Apr 2022 10:13:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 05 Apr 2022 10:13:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 10:13:10 GMT
USER memcache
# Tue, 05 Apr 2022 10:13:12 GMT
EXPOSE 11211
# Tue, 05 Apr 2022 10:13:14 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1877acf2d48ed8bcb5bd9756a95aca0c077457be7cf4fcef25807f4e9be88db1`  
		Last Modified: Mon, 04 Apr 2022 19:09:49 GMT  
		Size: 2.8 MB (2811186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8124818eb8eba84f8929c5e21fa177a0224a632a260382b31fd9ea53de0cb63`  
		Last Modified: Tue, 05 Apr 2022 10:14:09 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65727b8884a0072f667d76a190572aecbef43ea2013aa1fab131f8ad94cf6027`  
		Last Modified: Tue, 05 Apr 2022 10:14:09 GMT  
		Size: 126.2 KB (126153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fdd85c6abf5a16922e7e67ae0f58814880550c8e561aa25fe98f824c65e283f`  
		Last Modified: Tue, 05 Apr 2022 10:14:09 GMT  
		Size: 966.1 KB (966088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72641c2cb945038b7f950ba927f9377d909670cd2c8a2f99f0027cfe6f34d41f`  
		Last Modified: Tue, 05 Apr 2022 10:14:09 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27047ea6a5173f1f7f40a46c10833cfbf360f9ac71f5595dd2b745afc3f9f3bb`  
		Last Modified: Tue, 05 Apr 2022 10:14:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; s390x

```console
$ docker pull memcached@sha256:f4d6b61f33632664a2176b827e6f04dc9b43bece1e1225f1c27d3f218fcaf90c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3650153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d81b27c0ae4d75825efc6c14a9b31769a43cebc314ab07e25b9024fe3b7d6bf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:18:54 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 05 Apr 2022 11:18:55 GMT
RUN apk add --no-cache libsasl
# Tue, 05 Apr 2022 11:18:55 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 05 Apr 2022 11:18:55 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 05 Apr 2022 11:22:16 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 05 Apr 2022 11:22:16 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 05 Apr 2022 11:22:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 05 Apr 2022 11:22:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 11:22:17 GMT
USER memcache
# Tue, 05 Apr 2022 11:22:17 GMT
EXPOSE 11211
# Tue, 05 Apr 2022 11:22:17 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d92848f08937ad9e3c8df84e91a6ae677af747e7ae736062bf8303e6f98a5a`  
		Last Modified: Tue, 05 Apr 2022 11:23:08 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee4699d5d9185c820000eb9490520b6c45f7c7df9e07c67d79ec6efac05ff170`  
		Last Modified: Tue, 05 Apr 2022 11:23:08 GMT  
		Size: 113.5 KB (113464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c834b41bef6837d1312846d4839e66a0070dd934cb4388ff09a93112f6cdc0`  
		Last Modified: Tue, 05 Apr 2022 11:23:09 GMT  
		Size: 934.6 KB (934639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd760c99b09ff84bd3f703d93a143abd83f2ecfc7c941856bdd4222a4da2b7a`  
		Last Modified: Tue, 05 Apr 2022 11:23:08 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b4795384f4f0fbaa99dd9e3683dfd3639ccbcd001144f0b8d1f050c3a765283`  
		Last Modified: Tue, 05 Apr 2022 11:23:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1-alpine3.15`

```console
$ docker pull memcached@sha256:06bc630f006be575ae4e8a55e515a66daba0ed432f0e46ecfacf654daf4f07e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1-alpine3.15` - linux; amd64

```console
$ docker pull memcached@sha256:fbb3eda59b2f6851b1335f6fd43fa5a371ac197b06f84c0363341b7cd1c066f1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3864898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bcea36e93e267587df645dc2c39d08513419e129eb5b28db4a204207d64a9ea6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 09:54:14 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 05 Apr 2022 09:54:15 GMT
RUN apk add --no-cache libsasl
# Tue, 05 Apr 2022 09:54:15 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 05 Apr 2022 09:54:15 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 05 Apr 2022 09:57:57 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 05 Apr 2022 09:57:57 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 05 Apr 2022 09:57:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 05 Apr 2022 09:57:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 09:57:58 GMT
USER memcache
# Tue, 05 Apr 2022 09:57:58 GMT
EXPOSE 11211
# Tue, 05 Apr 2022 09:57:58 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c437462196847904d5021a85f817fecbb0b84eca04e4677f3a907f95125ebd3`  
		Last Modified: Tue, 05 Apr 2022 09:58:27 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37749f62d258e02c4f026b7ed0cb874d23b47abaa2c5860e41b3c099fdeb1d15`  
		Last Modified: Tue, 05 Apr 2022 09:58:27 GMT  
		Size: 109.2 KB (109172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf6c1e9f5167a143f222aea98c5b9c1d58ad0f9eed19d753fa1c4ffdfdd0269`  
		Last Modified: Tue, 05 Apr 2022 09:58:27 GMT  
		Size: 939.5 KB (939497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550e19164877083e509bb0c014a831674a7b77ddcf111d980a4f2b1bd1a78171`  
		Last Modified: Tue, 05 Apr 2022 09:58:27 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:515f37e9ad844fe3fdd82c3504b1c092e11e2c8f5f8395bc8944c96c768f3d3c`  
		Last Modified: Tue, 05 Apr 2022 09:58:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:d38012edd86b9a7abab01b390d4bbce8c39201ebedfd0066fcff6b6fb20cf178
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3757025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e0f3d4ef24801f58b76d5d0e24224de96c6e02fba4eccb3fa2e037e94403f0a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:15:56 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 05 Apr 2022 04:15:57 GMT
RUN apk add --no-cache libsasl
# Tue, 05 Apr 2022 04:15:58 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 05 Apr 2022 04:15:59 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 05 Apr 2022 04:18:36 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 05 Apr 2022 04:18:37 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 05 Apr 2022 04:18:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 05 Apr 2022 04:18:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 04:18:39 GMT
USER memcache
# Tue, 05 Apr 2022 04:18:40 GMT
EXPOSE 11211
# Tue, 05 Apr 2022 04:18:41 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa012cdcd391bd8cd78796fe53eb96b7585962832b802667f44cedd88405d0cc`  
		Last Modified: Tue, 05 Apr 2022 04:19:28 GMT  
		Size: 1.2 KB (1238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca8ad568702372595d83e4a4b906e000230b00315e1fd6ef6d219697badb387`  
		Last Modified: Tue, 05 Apr 2022 04:19:28 GMT  
		Size: 110.5 KB (110499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:265ae8d237ddc109ffe7e544e93a0dc1cea5bfe3fa5685fca792afda6d67ed0f`  
		Last Modified: Tue, 05 Apr 2022 04:19:29 GMT  
		Size: 928.4 KB (928406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce17e42e65242140f2a8f7c6d0a16bf4f1b64b0ba276ed8341905ed6f63e4a7b`  
		Last Modified: Tue, 05 Apr 2022 04:19:28 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30070b7f5a7be9b35fb6b8c7f1b6cb0de4508d927cc49caf12b3f6e220b0cc60`  
		Last Modified: Tue, 05 Apr 2022 04:19:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.15` - linux; 386

```console
$ docker pull memcached@sha256:5378334a3366058f6987024a1963dceafda46b182d6236b4685f816238f99992
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3888728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be3d8aa97e2099f400479214a98c34c3a23c21939afde5c6611961b33539a8bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:25 GMT
ADD file:7d51a0f8691eb78c9062fd31984423a93d276a67b4ed5d1a706e1c2cd9fea23a in / 
# Mon, 04 Apr 2022 23:38:25 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:52:17 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 05 Apr 2022 03:52:18 GMT
RUN apk add --no-cache libsasl
# Tue, 05 Apr 2022 03:52:19 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 05 Apr 2022 03:52:20 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 05 Apr 2022 03:55:15 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 05 Apr 2022 03:55:17 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 05 Apr 2022 03:55:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 05 Apr 2022 03:55:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 03:55:19 GMT
USER memcache
# Tue, 05 Apr 2022 03:55:20 GMT
EXPOSE 11211
# Tue, 05 Apr 2022 03:55:21 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:73b28a5955ec7fb46f2cf0434e4901a889f7dda3f8c9ec496300feb256c7eda8`  
		Last Modified: Mon, 04 Apr 2022 19:10:03 GMT  
		Size: 2.8 MB (2818974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06cddc8f8c3aabebd92d18ccbc0c9181ed94cc4b15b5adbda9e2bfdf4b8f38e9`  
		Last Modified: Tue, 05 Apr 2022 03:56:08 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad8594347186db0e9366f74b1e03bd14ed234378b2d1238a6b56504a86608fa6`  
		Last Modified: Tue, 05 Apr 2022 03:56:08 GMT  
		Size: 120.9 KB (120869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d7907ab18015191139b22c9b7b25c6a23d1c569470a49f2eb3e1ef985c4450`  
		Last Modified: Tue, 05 Apr 2022 03:56:08 GMT  
		Size: 947.2 KB (947242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3d6dff2eb04a8a959a2e8d101ca3da2646db4b2125b02fd6505c61ce53215b`  
		Last Modified: Tue, 05 Apr 2022 03:56:08 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:845b50269336006037a46780211bf0b2b95df971864d348d10c893aa2bf3afe3`  
		Last Modified: Tue, 05 Apr 2022 03:56:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.15` - linux; ppc64le

```console
$ docker pull memcached@sha256:d1110704ee41f1dce802400ce09904c39aff25c66c1e1b87c64781b0bd9527d4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3905105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1827e9495120e553b560bd77e162a97bfdb923a96c36b2dea8afd967fdc57bd1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:30 GMT
ADD file:960cf6f9d3d1cfcb36c2d67dd4c3eaba7db1d0c7afe97968512248d7f234ad47 in / 
# Tue, 05 Apr 2022 00:23:32 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 10:09:23 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 05 Apr 2022 10:09:31 GMT
RUN apk add --no-cache libsasl
# Tue, 05 Apr 2022 10:09:35 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 05 Apr 2022 10:09:41 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 05 Apr 2022 10:12:56 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 05 Apr 2022 10:12:58 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 05 Apr 2022 10:13:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 05 Apr 2022 10:13:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 10:13:10 GMT
USER memcache
# Tue, 05 Apr 2022 10:13:12 GMT
EXPOSE 11211
# Tue, 05 Apr 2022 10:13:14 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1877acf2d48ed8bcb5bd9756a95aca0c077457be7cf4fcef25807f4e9be88db1`  
		Last Modified: Mon, 04 Apr 2022 19:09:49 GMT  
		Size: 2.8 MB (2811186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8124818eb8eba84f8929c5e21fa177a0224a632a260382b31fd9ea53de0cb63`  
		Last Modified: Tue, 05 Apr 2022 10:14:09 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65727b8884a0072f667d76a190572aecbef43ea2013aa1fab131f8ad94cf6027`  
		Last Modified: Tue, 05 Apr 2022 10:14:09 GMT  
		Size: 126.2 KB (126153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fdd85c6abf5a16922e7e67ae0f58814880550c8e561aa25fe98f824c65e283f`  
		Last Modified: Tue, 05 Apr 2022 10:14:09 GMT  
		Size: 966.1 KB (966088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72641c2cb945038b7f950ba927f9377d909670cd2c8a2f99f0027cfe6f34d41f`  
		Last Modified: Tue, 05 Apr 2022 10:14:09 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27047ea6a5173f1f7f40a46c10833cfbf360f9ac71f5595dd2b745afc3f9f3bb`  
		Last Modified: Tue, 05 Apr 2022 10:14:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.15` - linux; s390x

```console
$ docker pull memcached@sha256:f4d6b61f33632664a2176b827e6f04dc9b43bece1e1225f1c27d3f218fcaf90c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3650153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d81b27c0ae4d75825efc6c14a9b31769a43cebc314ab07e25b9024fe3b7d6bf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:18:54 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 05 Apr 2022 11:18:55 GMT
RUN apk add --no-cache libsasl
# Tue, 05 Apr 2022 11:18:55 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 05 Apr 2022 11:18:55 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 05 Apr 2022 11:22:16 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 05 Apr 2022 11:22:16 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 05 Apr 2022 11:22:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 05 Apr 2022 11:22:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 11:22:17 GMT
USER memcache
# Tue, 05 Apr 2022 11:22:17 GMT
EXPOSE 11211
# Tue, 05 Apr 2022 11:22:17 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d92848f08937ad9e3c8df84e91a6ae677af747e7ae736062bf8303e6f98a5a`  
		Last Modified: Tue, 05 Apr 2022 11:23:08 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee4699d5d9185c820000eb9490520b6c45f7c7df9e07c67d79ec6efac05ff170`  
		Last Modified: Tue, 05 Apr 2022 11:23:08 GMT  
		Size: 113.5 KB (113464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c834b41bef6837d1312846d4839e66a0070dd934cb4388ff09a93112f6cdc0`  
		Last Modified: Tue, 05 Apr 2022 11:23:09 GMT  
		Size: 934.6 KB (934639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd760c99b09ff84bd3f703d93a143abd83f2ecfc7c941856bdd4222a4da2b7a`  
		Last Modified: Tue, 05 Apr 2022 11:23:08 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b4795384f4f0fbaa99dd9e3683dfd3639ccbcd001144f0b8d1f050c3a765283`  
		Last Modified: Tue, 05 Apr 2022 11:23:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1-bullseye`

```console
$ docker pull memcached@sha256:05917d8f91b97eff3ffb98497dd139c65f61c2107649cf73db6cced7e7667b94
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

### `memcached:1-bullseye` - linux; amd64

```console
$ docker pull memcached@sha256:58a41bfdd7492d7d9be5ea8ab1abeffa106a2193e98e6646be91d06ad37d0675
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32968652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:065555a745051537085b4135608198e45686d4574eda4d7093537d1107a1feff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 11 May 2022 01:20:16 GMT
ADD file:4a0bb88956083aa56032fdd9601d9b66c39b18c896ba35ea33594cd75621640a in / 
# Wed, 11 May 2022 01:20:16 GMT
CMD ["bash"]
# Wed, 11 May 2022 04:44:00 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 11 May 2022 04:44:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 04:44:03 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 11 May 2022 04:44:03 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 11 May 2022 04:46:42 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 May 2022 04:46:42 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 May 2022 04:46:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 04:46:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 04:46:43 GMT
USER memcache
# Wed, 11 May 2022 04:46:43 GMT
EXPOSE 11211
# Wed, 11 May 2022 04:46:43 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:214ca5fb90323fe769c63a12af092f2572bf1c6b300263e09883909fc865d260`  
		Last Modified: Wed, 11 May 2022 01:25:13 GMT  
		Size: 31.4 MB (31379476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae8d4b1feabc5879929064e635eb9f14ef5b8a15bac772048359ca7ff051d1c`  
		Last Modified: Wed, 11 May 2022 04:47:13 GMT  
		Size: 5.0 KB (4975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dc491b9af677c0a71fa36fcbf2faea8087acafa69e2d760fcaea4f26fb5eb2a`  
		Last Modified: Wed, 11 May 2022 04:47:14 GMT  
		Size: 328.1 KB (328091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c355a147dff081cfbbf9d104870e2195eb0213138ae88d87a585b466fc521d4a`  
		Last Modified: Wed, 11 May 2022 04:47:14 GMT  
		Size: 1.3 MB (1255702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0cc0d566fb2a731f9d4dd270354fe902ec4b175b95e3552e17d53a76601b28d`  
		Last Modified: Wed, 11 May 2022 04:47:13 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d5c91075c8421465ad8ef2fe32f6daab4ff01b837e03aee3568d39c64cb2d3`  
		Last Modified: Wed, 11 May 2022 04:47:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; arm variant v5

```console
$ docker pull memcached@sha256:7114dc5aaa1603875d79f65e4d27cf83fd5c6ff279092e5019313c2e676e8563
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30469996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:711c043049190c6786a1fe335232c7bee5a0c58134e9481f385ae99e18cff3a2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 11 May 2022 00:50:34 GMT
ADD file:72357b75d7e4546f06abf4648ab600980e742a3017f36da3c7a6c086f2f5fb56 in / 
# Wed, 11 May 2022 00:50:35 GMT
CMD ["bash"]
# Wed, 11 May 2022 19:59:38 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 11 May 2022 19:59:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 19:59:48 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 11 May 2022 19:59:49 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 11 May 2022 20:04:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 May 2022 20:04:12 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 May 2022 20:04:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 20:04:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 20:04:14 GMT
USER memcache
# Wed, 11 May 2022 20:04:15 GMT
EXPOSE 11211
# Wed, 11 May 2022 20:04:15 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f7b69be15db1cb94a249f74b27edd4f5e5923a8701b026179a593f6888e897aa`  
		Last Modified: Wed, 11 May 2022 01:05:51 GMT  
		Size: 28.9 MB (28921122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e23defdefe7366c4546b3284b11bdbedcf73c55c4cad0c49a2e12b6bc971f653`  
		Last Modified: Wed, 11 May 2022 20:05:07 GMT  
		Size: 4.9 KB (4893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aed101d7cb94db52f647e3cf585d3a7702b5a01cb3f7c3fc86aedcd94fb5b01`  
		Last Modified: Wed, 11 May 2022 20:05:07 GMT  
		Size: 316.6 KB (316610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80e354b9ae9a23ca02681ddaca03fe3a6fa45069b80a683e38123aa3a0174fab`  
		Last Modified: Wed, 11 May 2022 20:05:08 GMT  
		Size: 1.2 MB (1226962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d82b2d2d5ab7db68fddbbf26596ed21c9c4506e0355be942188f9a81557bdd`  
		Last Modified: Wed, 11 May 2022 20:05:07 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd35d60f098711fce5b4a2d107b57cfe22a70cbb6bf47476c42ea4d975b6c3f7`  
		Last Modified: Wed, 11 May 2022 20:05:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; arm variant v7

```console
$ docker pull memcached@sha256:34dee5b2772158236707bc1811db77d4adc27d86ca6b1b096fb444a8cfef133e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28091607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad29267829b7cd5d6051ca12869e51112bded24fc2e06656b673942a215f1c84`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 20 Apr 2022 13:27:18 GMT
ADD file:1a0e290eb32b3533f9d1684c683ad866b5003579790b25ad61b2044dc6c20bbb in / 
# Wed, 20 Apr 2022 13:27:18 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 21:47:36 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 20 Apr 2022 21:47:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 21:47:45 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 20 Apr 2022 21:47:45 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 20 Apr 2022 21:51:42 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 20 Apr 2022 21:51:42 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 20 Apr 2022 21:51:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 20 Apr 2022 21:51:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Apr 2022 21:51:45 GMT
USER memcache
# Wed, 20 Apr 2022 21:51:45 GMT
EXPOSE 11211
# Wed, 20 Apr 2022 21:51:46 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a6b2963233cd14b47391f0e25f2a485bbeabb87e771a71b73e5cde7c013963da`  
		Last Modified: Wed, 20 Apr 2022 13:43:41 GMT  
		Size: 26.6 MB (26575758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4b149950ca557655b7e9b7229a81d7d772f2aad316a5ce7de452664795a377`  
		Last Modified: Wed, 20 Apr 2022 22:04:23 GMT  
		Size: 4.9 KB (4893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d14f3b12cc24aac4e3614237409e18959637d8420b534524bc1fe63e7456a660`  
		Last Modified: Wed, 20 Apr 2022 22:04:23 GMT  
		Size: 312.1 KB (312059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca5c1518bd4380c5c22f884d402b699c75cb53de72de7d5b2a53e99d8ba56d9e`  
		Last Modified: Wed, 20 Apr 2022 22:04:24 GMT  
		Size: 1.2 MB (1198488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd1a54f20b40e9c7302a4ab0c46cc590140bde81aba4ab1d149dd8b2b3edade`  
		Last Modified: Wed, 20 Apr 2022 22:04:23 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6e66d52d7551a05a10e5a70971eef4ad0803f499c934fd1ec734a144e5bc64`  
		Last Modified: Wed, 20 Apr 2022 22:04:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:6c452eece1271128806922efd79c0ef0f809e6705d855d6a271f5208d2a2117d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31444857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d45eed3b8e469acc08e97e874bb1e8b4f004720606f20212dad652f79ca29db4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 11 May 2022 00:46:59 GMT
ADD file:158a0e401328bd7c0d49b9e8539186098967218f1b1a8c811f4398d29b74397f in / 
# Wed, 11 May 2022 00:47:00 GMT
CMD ["bash"]
# Wed, 11 May 2022 02:27:34 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 11 May 2022 02:27:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:27:38 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 11 May 2022 02:27:39 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 11 May 2022 02:30:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 May 2022 02:30:13 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 May 2022 02:30:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 02:30:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 02:30:15 GMT
USER memcache
# Wed, 11 May 2022 02:30:16 GMT
EXPOSE 11211
# Wed, 11 May 2022 02:30:17 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:dfdd5ffb257742b891ccad9400a77dad2a6260b2451e0f5e48a9ade1d17a87ec`  
		Last Modified: Wed, 11 May 2022 00:53:46 GMT  
		Size: 30.1 MB (30065693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:921e9eec57430f29a509862965b1bc0f909703c8c5e73b2345205cbd6b715910`  
		Last Modified: Wed, 11 May 2022 02:31:07 GMT  
		Size: 4.9 KB (4900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:984aa2c2269106d51c47bed797929d496825d1dee8883d84918fd98cd809ba76`  
		Last Modified: Wed, 11 May 2022 02:31:07 GMT  
		Size: 119.2 KB (119215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b52324e4c1cc245d2131fae3776a0359730099f17e8039fa1db0d0b6310a195`  
		Last Modified: Wed, 11 May 2022 02:31:08 GMT  
		Size: 1.3 MB (1254642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70bc38e444a829155cb5ad8ca3f2b8cc68a6065e19b795707656cec98edadbfc`  
		Last Modified: Wed, 11 May 2022 02:31:07 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b29514622ffb8a37130cc9662034040cbc8ff1d5c7b8ce620f49c0d26b24b73`  
		Last Modified: Wed, 11 May 2022 02:31:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; 386

```console
$ docker pull memcached@sha256:faedc990d98e8f3b6058c1e3f9ace6816b59338aaf906a8099a0b1141713d345
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33778000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74fb9295e5de207e5aade7877e8b45371b49a320bf3eafbfe65ea15c6f70dd59`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 11 May 2022 01:39:14 GMT
ADD file:9eecb0fd311177f9d226e914c411aef49b5de1930e73019d2ee24afed515b5a2 in / 
# Wed, 11 May 2022 01:39:14 GMT
CMD ["bash"]
# Wed, 11 May 2022 04:32:45 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 11 May 2022 04:32:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 04:32:49 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 11 May 2022 04:32:50 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 11 May 2022 04:35:41 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 May 2022 04:35:43 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 May 2022 04:35:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 04:35:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 04:35:45 GMT
USER memcache
# Wed, 11 May 2022 04:35:46 GMT
EXPOSE 11211
# Wed, 11 May 2022 04:35:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:91c5bdbe4bf9f1970dd54ba71e2523649adce4e5240c2ff8a87711bf389ecba3`  
		Last Modified: Wed, 11 May 2022 01:46:25 GMT  
		Size: 32.4 MB (32389776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cbc080a4e6972a45023b1c0d8d9f74e9df257677ec7503a9f8756eabb61b5e0`  
		Last Modified: Wed, 11 May 2022 04:36:36 GMT  
		Size: 4.8 KB (4771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdfcc6e2f39957ee91e94aa2f1264a35ccef2b3aed8ae29d859144d763ed06ab`  
		Last Modified: Wed, 11 May 2022 04:36:36 GMT  
		Size: 130.1 KB (130140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a68472399b32a22e31b1b551482a4fec929210d4db3da6b3010fdb3a97bf0944`  
		Last Modified: Wed, 11 May 2022 04:36:37 GMT  
		Size: 1.3 MB (1252905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a1040db24a5a1a06568a3d81752b73f002172ebec23d3ace2181c365e6216c9`  
		Last Modified: Wed, 11 May 2022 04:36:36 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496cfb26b818ba873c9dbd7203c2551d9c1503db7a8281c82b03ecd7987dfe44`  
		Last Modified: Wed, 11 May 2022 04:36:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; mips64le

```console
$ docker pull memcached@sha256:d4d70ee02bd6a268e51e7cb45ae2ab6028a3f5546e3566abea4839b7bc0b2795
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31014729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5edfa57d6aec6089194206346467a5708554650f75a703542020f03dda6cfb13`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 11 May 2022 02:23:35 GMT
ADD file:d47dce2adbc9352ef1d437730bab3b579dd8d2bf29dd60cd8a8b65396b39e36e in / 
# Wed, 11 May 2022 02:23:40 GMT
CMD ["bash"]
# Wed, 11 May 2022 04:26:13 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 11 May 2022 04:26:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 04:26:33 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 11 May 2022 04:26:36 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 11 May 2022 04:33:31 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 May 2022 04:33:33 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 May 2022 04:33:38 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 04:33:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 04:33:43 GMT
USER memcache
# Wed, 11 May 2022 04:33:45 GMT
EXPOSE 11211
# Wed, 11 May 2022 04:33:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:438a36bf0b6e75ff6f0fbb2b7669dfb86361416f4d808912d30cf5b91ad2eea9`  
		Last Modified: Wed, 11 May 2022 02:33:43 GMT  
		Size: 29.6 MB (29641051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2947248cd8e754e130fecb9083b0ad0025e50361a44987eadfb6edfeb2e3908c`  
		Last Modified: Wed, 11 May 2022 04:34:05 GMT  
		Size: 4.9 KB (4861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3849c71c1ab16dd8196e74fd37ae70b3a0b89a3b07a9cb7f76535725af27a86a`  
		Last Modified: Wed, 11 May 2022 04:34:05 GMT  
		Size: 117.2 KB (117156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f24b722d80efb82b9982c69a407116125ad8a340447344e252517f9798849b9`  
		Last Modified: Wed, 11 May 2022 04:34:06 GMT  
		Size: 1.3 MB (1251254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f4827b1598450f78ff6da5317e269d8fdc544d21ff25409586a2db03053022`  
		Last Modified: Wed, 11 May 2022 04:34:05 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:090d97f72bbcf506ab0dc4d8e19c3a1522513237327ced2e711f0613fb262865`  
		Last Modified: Wed, 11 May 2022 04:34:05 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; ppc64le

```console
$ docker pull memcached@sha256:673643121e94f08dd12197b69994ec2cad834c15326b37ba83861eb00aa22134
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36971800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:821c76dba347fd635474ef0126da0d404cc404e989635b028d0da3c2dfb273b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 11 May 2022 01:32:29 GMT
ADD file:1e94716789ec21981460f74be38a668bc212bd804c1d41cecf90036a5bccac5a in / 
# Wed, 11 May 2022 01:32:34 GMT
CMD ["bash"]
# Wed, 11 May 2022 07:51:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 11 May 2022 07:51:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 07:51:40 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 11 May 2022 07:51:48 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 11 May 2022 07:57:31 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 May 2022 07:57:33 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 May 2022 07:57:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 07:57:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 07:57:49 GMT
USER memcache
# Wed, 11 May 2022 07:57:55 GMT
EXPOSE 11211
# Wed, 11 May 2022 07:58:00 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2533109ed11eefd6415e0370d6d7a3ea879b582b1887c98b819a598ad18fca24`  
		Last Modified: Wed, 11 May 2022 01:43:03 GMT  
		Size: 35.3 MB (35286467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:103a6713e9bf2853760692eb30b886453378b61e3fb83321c0ce1fec39bdf2f2`  
		Last Modified: Wed, 11 May 2022 07:59:13 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9173dced38a5c576a66100ed6df59833b82ee6847ed29531d690b7377a72e02d`  
		Last Modified: Wed, 11 May 2022 07:59:13 GMT  
		Size: 356.9 KB (356938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e15378aab9e7b0eefd835da5eeee5fe567c111dcf6df814b34f6755cf27c45`  
		Last Modified: Wed, 11 May 2022 07:59:13 GMT  
		Size: 1.3 MB (1323008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523888230dfa0221ad182120061be4802ac72d7a19047277ffc452c5003537b5`  
		Last Modified: Wed, 11 May 2022 07:59:13 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12893f041469d0edbc3132e6af823296c231a18db48dc29c665658f6ba859c9f`  
		Last Modified: Wed, 11 May 2022 07:59:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; s390x

```console
$ docker pull memcached@sha256:d0221a850100573af43f6113f62398369ddaa506aef1fd1e114da8fdd4403330
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31225739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37e72a40047bd848bbedd03871f17d8132f625301f2203038b265841fa1a660f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 11 May 2022 00:44:17 GMT
ADD file:d93a1cf64a813d01774cd628dfd683c006e20159e2ab3464c2159c8d9897c725 in / 
# Wed, 11 May 2022 00:44:19 GMT
CMD ["bash"]
# Wed, 11 May 2022 02:35:31 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 11 May 2022 02:35:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:35:34 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 11 May 2022 02:35:34 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 11 May 2022 02:39:02 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 May 2022 02:39:03 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 May 2022 02:39:03 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 02:39:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 02:39:03 GMT
USER memcache
# Wed, 11 May 2022 02:39:03 GMT
EXPOSE 11211
# Wed, 11 May 2022 02:39:04 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9f3750f6094217808e26d471752341db88153c8d5b5f9bb11577b74671303bbc`  
		Last Modified: Wed, 11 May 2022 00:50:03 GMT  
		Size: 29.7 MB (29654739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29541285df59f95a596b1911b49171e64e2361189a163533e77dbf2961b8f685`  
		Last Modified: Wed, 11 May 2022 02:40:04 GMT  
		Size: 5.0 KB (5026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c94a32e11bca5f817bc7015ceff49279fcd263d523198a38cc02607b7899e261`  
		Last Modified: Wed, 11 May 2022 02:40:04 GMT  
		Size: 324.2 KB (324197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57395e3cd66c2852ddaac636856f0245c1cfdca358d6bb75128950b9d9042481`  
		Last Modified: Wed, 11 May 2022 02:40:04 GMT  
		Size: 1.2 MB (1241369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ed03e37cb4ad7ab6dfc00b4938e9e5ec27777eb89fe1918ffc45a5a8de10c0`  
		Last Modified: Wed, 11 May 2022 02:40:04 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79cc46e5a2551dd05d1dcb476692b2a5d1c7e5181f253ad3938c179835018b95`  
		Last Modified: Wed, 11 May 2022 02:40:03 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6`

```console
$ docker pull memcached@sha256:05917d8f91b97eff3ffb98497dd139c65f61c2107649cf73db6cced7e7667b94
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

### `memcached:1.6` - linux; amd64

```console
$ docker pull memcached@sha256:58a41bfdd7492d7d9be5ea8ab1abeffa106a2193e98e6646be91d06ad37d0675
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32968652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:065555a745051537085b4135608198e45686d4574eda4d7093537d1107a1feff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 11 May 2022 01:20:16 GMT
ADD file:4a0bb88956083aa56032fdd9601d9b66c39b18c896ba35ea33594cd75621640a in / 
# Wed, 11 May 2022 01:20:16 GMT
CMD ["bash"]
# Wed, 11 May 2022 04:44:00 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 11 May 2022 04:44:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 04:44:03 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 11 May 2022 04:44:03 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 11 May 2022 04:46:42 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 May 2022 04:46:42 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 May 2022 04:46:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 04:46:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 04:46:43 GMT
USER memcache
# Wed, 11 May 2022 04:46:43 GMT
EXPOSE 11211
# Wed, 11 May 2022 04:46:43 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:214ca5fb90323fe769c63a12af092f2572bf1c6b300263e09883909fc865d260`  
		Last Modified: Wed, 11 May 2022 01:25:13 GMT  
		Size: 31.4 MB (31379476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae8d4b1feabc5879929064e635eb9f14ef5b8a15bac772048359ca7ff051d1c`  
		Last Modified: Wed, 11 May 2022 04:47:13 GMT  
		Size: 5.0 KB (4975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dc491b9af677c0a71fa36fcbf2faea8087acafa69e2d760fcaea4f26fb5eb2a`  
		Last Modified: Wed, 11 May 2022 04:47:14 GMT  
		Size: 328.1 KB (328091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c355a147dff081cfbbf9d104870e2195eb0213138ae88d87a585b466fc521d4a`  
		Last Modified: Wed, 11 May 2022 04:47:14 GMT  
		Size: 1.3 MB (1255702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0cc0d566fb2a731f9d4dd270354fe902ec4b175b95e3552e17d53a76601b28d`  
		Last Modified: Wed, 11 May 2022 04:47:13 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d5c91075c8421465ad8ef2fe32f6daab4ff01b837e03aee3568d39c64cb2d3`  
		Last Modified: Wed, 11 May 2022 04:47:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm variant v5

```console
$ docker pull memcached@sha256:7114dc5aaa1603875d79f65e4d27cf83fd5c6ff279092e5019313c2e676e8563
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30469996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:711c043049190c6786a1fe335232c7bee5a0c58134e9481f385ae99e18cff3a2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 11 May 2022 00:50:34 GMT
ADD file:72357b75d7e4546f06abf4648ab600980e742a3017f36da3c7a6c086f2f5fb56 in / 
# Wed, 11 May 2022 00:50:35 GMT
CMD ["bash"]
# Wed, 11 May 2022 19:59:38 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 11 May 2022 19:59:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 19:59:48 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 11 May 2022 19:59:49 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 11 May 2022 20:04:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 May 2022 20:04:12 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 May 2022 20:04:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 20:04:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 20:04:14 GMT
USER memcache
# Wed, 11 May 2022 20:04:15 GMT
EXPOSE 11211
# Wed, 11 May 2022 20:04:15 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f7b69be15db1cb94a249f74b27edd4f5e5923a8701b026179a593f6888e897aa`  
		Last Modified: Wed, 11 May 2022 01:05:51 GMT  
		Size: 28.9 MB (28921122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e23defdefe7366c4546b3284b11bdbedcf73c55c4cad0c49a2e12b6bc971f653`  
		Last Modified: Wed, 11 May 2022 20:05:07 GMT  
		Size: 4.9 KB (4893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aed101d7cb94db52f647e3cf585d3a7702b5a01cb3f7c3fc86aedcd94fb5b01`  
		Last Modified: Wed, 11 May 2022 20:05:07 GMT  
		Size: 316.6 KB (316610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80e354b9ae9a23ca02681ddaca03fe3a6fa45069b80a683e38123aa3a0174fab`  
		Last Modified: Wed, 11 May 2022 20:05:08 GMT  
		Size: 1.2 MB (1226962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d82b2d2d5ab7db68fddbbf26596ed21c9c4506e0355be942188f9a81557bdd`  
		Last Modified: Wed, 11 May 2022 20:05:07 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd35d60f098711fce5b4a2d107b57cfe22a70cbb6bf47476c42ea4d975b6c3f7`  
		Last Modified: Wed, 11 May 2022 20:05:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm variant v7

```console
$ docker pull memcached@sha256:34dee5b2772158236707bc1811db77d4adc27d86ca6b1b096fb444a8cfef133e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28091607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad29267829b7cd5d6051ca12869e51112bded24fc2e06656b673942a215f1c84`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 20 Apr 2022 13:27:18 GMT
ADD file:1a0e290eb32b3533f9d1684c683ad866b5003579790b25ad61b2044dc6c20bbb in / 
# Wed, 20 Apr 2022 13:27:18 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 21:47:36 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 20 Apr 2022 21:47:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 21:47:45 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 20 Apr 2022 21:47:45 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 20 Apr 2022 21:51:42 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 20 Apr 2022 21:51:42 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 20 Apr 2022 21:51:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 20 Apr 2022 21:51:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Apr 2022 21:51:45 GMT
USER memcache
# Wed, 20 Apr 2022 21:51:45 GMT
EXPOSE 11211
# Wed, 20 Apr 2022 21:51:46 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a6b2963233cd14b47391f0e25f2a485bbeabb87e771a71b73e5cde7c013963da`  
		Last Modified: Wed, 20 Apr 2022 13:43:41 GMT  
		Size: 26.6 MB (26575758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4b149950ca557655b7e9b7229a81d7d772f2aad316a5ce7de452664795a377`  
		Last Modified: Wed, 20 Apr 2022 22:04:23 GMT  
		Size: 4.9 KB (4893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d14f3b12cc24aac4e3614237409e18959637d8420b534524bc1fe63e7456a660`  
		Last Modified: Wed, 20 Apr 2022 22:04:23 GMT  
		Size: 312.1 KB (312059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca5c1518bd4380c5c22f884d402b699c75cb53de72de7d5b2a53e99d8ba56d9e`  
		Last Modified: Wed, 20 Apr 2022 22:04:24 GMT  
		Size: 1.2 MB (1198488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd1a54f20b40e9c7302a4ab0c46cc590140bde81aba4ab1d149dd8b2b3edade`  
		Last Modified: Wed, 20 Apr 2022 22:04:23 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6e66d52d7551a05a10e5a70971eef4ad0803f499c934fd1ec734a144e5bc64`  
		Last Modified: Wed, 20 Apr 2022 22:04:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:6c452eece1271128806922efd79c0ef0f809e6705d855d6a271f5208d2a2117d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31444857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d45eed3b8e469acc08e97e874bb1e8b4f004720606f20212dad652f79ca29db4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 11 May 2022 00:46:59 GMT
ADD file:158a0e401328bd7c0d49b9e8539186098967218f1b1a8c811f4398d29b74397f in / 
# Wed, 11 May 2022 00:47:00 GMT
CMD ["bash"]
# Wed, 11 May 2022 02:27:34 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 11 May 2022 02:27:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:27:38 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 11 May 2022 02:27:39 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 11 May 2022 02:30:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 May 2022 02:30:13 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 May 2022 02:30:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 02:30:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 02:30:15 GMT
USER memcache
# Wed, 11 May 2022 02:30:16 GMT
EXPOSE 11211
# Wed, 11 May 2022 02:30:17 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:dfdd5ffb257742b891ccad9400a77dad2a6260b2451e0f5e48a9ade1d17a87ec`  
		Last Modified: Wed, 11 May 2022 00:53:46 GMT  
		Size: 30.1 MB (30065693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:921e9eec57430f29a509862965b1bc0f909703c8c5e73b2345205cbd6b715910`  
		Last Modified: Wed, 11 May 2022 02:31:07 GMT  
		Size: 4.9 KB (4900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:984aa2c2269106d51c47bed797929d496825d1dee8883d84918fd98cd809ba76`  
		Last Modified: Wed, 11 May 2022 02:31:07 GMT  
		Size: 119.2 KB (119215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b52324e4c1cc245d2131fae3776a0359730099f17e8039fa1db0d0b6310a195`  
		Last Modified: Wed, 11 May 2022 02:31:08 GMT  
		Size: 1.3 MB (1254642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70bc38e444a829155cb5ad8ca3f2b8cc68a6065e19b795707656cec98edadbfc`  
		Last Modified: Wed, 11 May 2022 02:31:07 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b29514622ffb8a37130cc9662034040cbc8ff1d5c7b8ce620f49c0d26b24b73`  
		Last Modified: Wed, 11 May 2022 02:31:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; 386

```console
$ docker pull memcached@sha256:faedc990d98e8f3b6058c1e3f9ace6816b59338aaf906a8099a0b1141713d345
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33778000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74fb9295e5de207e5aade7877e8b45371b49a320bf3eafbfe65ea15c6f70dd59`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 11 May 2022 01:39:14 GMT
ADD file:9eecb0fd311177f9d226e914c411aef49b5de1930e73019d2ee24afed515b5a2 in / 
# Wed, 11 May 2022 01:39:14 GMT
CMD ["bash"]
# Wed, 11 May 2022 04:32:45 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 11 May 2022 04:32:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 04:32:49 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 11 May 2022 04:32:50 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 11 May 2022 04:35:41 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 May 2022 04:35:43 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 May 2022 04:35:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 04:35:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 04:35:45 GMT
USER memcache
# Wed, 11 May 2022 04:35:46 GMT
EXPOSE 11211
# Wed, 11 May 2022 04:35:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:91c5bdbe4bf9f1970dd54ba71e2523649adce4e5240c2ff8a87711bf389ecba3`  
		Last Modified: Wed, 11 May 2022 01:46:25 GMT  
		Size: 32.4 MB (32389776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cbc080a4e6972a45023b1c0d8d9f74e9df257677ec7503a9f8756eabb61b5e0`  
		Last Modified: Wed, 11 May 2022 04:36:36 GMT  
		Size: 4.8 KB (4771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdfcc6e2f39957ee91e94aa2f1264a35ccef2b3aed8ae29d859144d763ed06ab`  
		Last Modified: Wed, 11 May 2022 04:36:36 GMT  
		Size: 130.1 KB (130140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a68472399b32a22e31b1b551482a4fec929210d4db3da6b3010fdb3a97bf0944`  
		Last Modified: Wed, 11 May 2022 04:36:37 GMT  
		Size: 1.3 MB (1252905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a1040db24a5a1a06568a3d81752b73f002172ebec23d3ace2181c365e6216c9`  
		Last Modified: Wed, 11 May 2022 04:36:36 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496cfb26b818ba873c9dbd7203c2551d9c1503db7a8281c82b03ecd7987dfe44`  
		Last Modified: Wed, 11 May 2022 04:36:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; mips64le

```console
$ docker pull memcached@sha256:d4d70ee02bd6a268e51e7cb45ae2ab6028a3f5546e3566abea4839b7bc0b2795
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31014729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5edfa57d6aec6089194206346467a5708554650f75a703542020f03dda6cfb13`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 11 May 2022 02:23:35 GMT
ADD file:d47dce2adbc9352ef1d437730bab3b579dd8d2bf29dd60cd8a8b65396b39e36e in / 
# Wed, 11 May 2022 02:23:40 GMT
CMD ["bash"]
# Wed, 11 May 2022 04:26:13 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 11 May 2022 04:26:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 04:26:33 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 11 May 2022 04:26:36 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 11 May 2022 04:33:31 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 May 2022 04:33:33 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 May 2022 04:33:38 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 04:33:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 04:33:43 GMT
USER memcache
# Wed, 11 May 2022 04:33:45 GMT
EXPOSE 11211
# Wed, 11 May 2022 04:33:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:438a36bf0b6e75ff6f0fbb2b7669dfb86361416f4d808912d30cf5b91ad2eea9`  
		Last Modified: Wed, 11 May 2022 02:33:43 GMT  
		Size: 29.6 MB (29641051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2947248cd8e754e130fecb9083b0ad0025e50361a44987eadfb6edfeb2e3908c`  
		Last Modified: Wed, 11 May 2022 04:34:05 GMT  
		Size: 4.9 KB (4861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3849c71c1ab16dd8196e74fd37ae70b3a0b89a3b07a9cb7f76535725af27a86a`  
		Last Modified: Wed, 11 May 2022 04:34:05 GMT  
		Size: 117.2 KB (117156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f24b722d80efb82b9982c69a407116125ad8a340447344e252517f9798849b9`  
		Last Modified: Wed, 11 May 2022 04:34:06 GMT  
		Size: 1.3 MB (1251254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f4827b1598450f78ff6da5317e269d8fdc544d21ff25409586a2db03053022`  
		Last Modified: Wed, 11 May 2022 04:34:05 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:090d97f72bbcf506ab0dc4d8e19c3a1522513237327ced2e711f0613fb262865`  
		Last Modified: Wed, 11 May 2022 04:34:05 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; ppc64le

```console
$ docker pull memcached@sha256:673643121e94f08dd12197b69994ec2cad834c15326b37ba83861eb00aa22134
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36971800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:821c76dba347fd635474ef0126da0d404cc404e989635b028d0da3c2dfb273b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 11 May 2022 01:32:29 GMT
ADD file:1e94716789ec21981460f74be38a668bc212bd804c1d41cecf90036a5bccac5a in / 
# Wed, 11 May 2022 01:32:34 GMT
CMD ["bash"]
# Wed, 11 May 2022 07:51:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 11 May 2022 07:51:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 07:51:40 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 11 May 2022 07:51:48 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 11 May 2022 07:57:31 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 May 2022 07:57:33 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 May 2022 07:57:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 07:57:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 07:57:49 GMT
USER memcache
# Wed, 11 May 2022 07:57:55 GMT
EXPOSE 11211
# Wed, 11 May 2022 07:58:00 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2533109ed11eefd6415e0370d6d7a3ea879b582b1887c98b819a598ad18fca24`  
		Last Modified: Wed, 11 May 2022 01:43:03 GMT  
		Size: 35.3 MB (35286467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:103a6713e9bf2853760692eb30b886453378b61e3fb83321c0ce1fec39bdf2f2`  
		Last Modified: Wed, 11 May 2022 07:59:13 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9173dced38a5c576a66100ed6df59833b82ee6847ed29531d690b7377a72e02d`  
		Last Modified: Wed, 11 May 2022 07:59:13 GMT  
		Size: 356.9 KB (356938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e15378aab9e7b0eefd835da5eeee5fe567c111dcf6df814b34f6755cf27c45`  
		Last Modified: Wed, 11 May 2022 07:59:13 GMT  
		Size: 1.3 MB (1323008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523888230dfa0221ad182120061be4802ac72d7a19047277ffc452c5003537b5`  
		Last Modified: Wed, 11 May 2022 07:59:13 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12893f041469d0edbc3132e6af823296c231a18db48dc29c665658f6ba859c9f`  
		Last Modified: Wed, 11 May 2022 07:59:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; s390x

```console
$ docker pull memcached@sha256:d0221a850100573af43f6113f62398369ddaa506aef1fd1e114da8fdd4403330
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31225739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37e72a40047bd848bbedd03871f17d8132f625301f2203038b265841fa1a660f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 11 May 2022 00:44:17 GMT
ADD file:d93a1cf64a813d01774cd628dfd683c006e20159e2ab3464c2159c8d9897c725 in / 
# Wed, 11 May 2022 00:44:19 GMT
CMD ["bash"]
# Wed, 11 May 2022 02:35:31 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 11 May 2022 02:35:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:35:34 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 11 May 2022 02:35:34 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 11 May 2022 02:39:02 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 May 2022 02:39:03 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 May 2022 02:39:03 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 02:39:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 02:39:03 GMT
USER memcache
# Wed, 11 May 2022 02:39:03 GMT
EXPOSE 11211
# Wed, 11 May 2022 02:39:04 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9f3750f6094217808e26d471752341db88153c8d5b5f9bb11577b74671303bbc`  
		Last Modified: Wed, 11 May 2022 00:50:03 GMT  
		Size: 29.7 MB (29654739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29541285df59f95a596b1911b49171e64e2361189a163533e77dbf2961b8f685`  
		Last Modified: Wed, 11 May 2022 02:40:04 GMT  
		Size: 5.0 KB (5026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c94a32e11bca5f817bc7015ceff49279fcd263d523198a38cc02607b7899e261`  
		Last Modified: Wed, 11 May 2022 02:40:04 GMT  
		Size: 324.2 KB (324197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57395e3cd66c2852ddaac636856f0245c1cfdca358d6bb75128950b9d9042481`  
		Last Modified: Wed, 11 May 2022 02:40:04 GMT  
		Size: 1.2 MB (1241369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ed03e37cb4ad7ab6dfc00b4938e9e5ec27777eb89fe1918ffc45a5a8de10c0`  
		Last Modified: Wed, 11 May 2022 02:40:04 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79cc46e5a2551dd05d1dcb476692b2a5d1c7e5181f253ad3938c179835018b95`  
		Last Modified: Wed, 11 May 2022 02:40:03 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6-alpine`

```console
$ docker pull memcached@sha256:0374a1e43929f2da9d7acf6887903eb3337ea92f0b8fd080aec28d2b902065aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1.6-alpine` - linux; amd64

```console
$ docker pull memcached@sha256:fbb3eda59b2f6851b1335f6fd43fa5a371ac197b06f84c0363341b7cd1c066f1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3864898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bcea36e93e267587df645dc2c39d08513419e129eb5b28db4a204207d64a9ea6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 09:54:14 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 05 Apr 2022 09:54:15 GMT
RUN apk add --no-cache libsasl
# Tue, 05 Apr 2022 09:54:15 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 05 Apr 2022 09:54:15 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 05 Apr 2022 09:57:57 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 05 Apr 2022 09:57:57 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 05 Apr 2022 09:57:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 05 Apr 2022 09:57:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 09:57:58 GMT
USER memcache
# Tue, 05 Apr 2022 09:57:58 GMT
EXPOSE 11211
# Tue, 05 Apr 2022 09:57:58 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c437462196847904d5021a85f817fecbb0b84eca04e4677f3a907f95125ebd3`  
		Last Modified: Tue, 05 Apr 2022 09:58:27 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37749f62d258e02c4f026b7ed0cb874d23b47abaa2c5860e41b3c099fdeb1d15`  
		Last Modified: Tue, 05 Apr 2022 09:58:27 GMT  
		Size: 109.2 KB (109172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf6c1e9f5167a143f222aea98c5b9c1d58ad0f9eed19d753fa1c4ffdfdd0269`  
		Last Modified: Tue, 05 Apr 2022 09:58:27 GMT  
		Size: 939.5 KB (939497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550e19164877083e509bb0c014a831674a7b77ddcf111d980a4f2b1bd1a78171`  
		Last Modified: Tue, 05 Apr 2022 09:58:27 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:515f37e9ad844fe3fdd82c3504b1c092e11e2c8f5f8395bc8944c96c768f3d3c`  
		Last Modified: Tue, 05 Apr 2022 09:58:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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
$ docker pull memcached@sha256:d38012edd86b9a7abab01b390d4bbce8c39201ebedfd0066fcff6b6fb20cf178
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3757025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e0f3d4ef24801f58b76d5d0e24224de96c6e02fba4eccb3fa2e037e94403f0a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:15:56 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 05 Apr 2022 04:15:57 GMT
RUN apk add --no-cache libsasl
# Tue, 05 Apr 2022 04:15:58 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 05 Apr 2022 04:15:59 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 05 Apr 2022 04:18:36 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 05 Apr 2022 04:18:37 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 05 Apr 2022 04:18:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 05 Apr 2022 04:18:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 04:18:39 GMT
USER memcache
# Tue, 05 Apr 2022 04:18:40 GMT
EXPOSE 11211
# Tue, 05 Apr 2022 04:18:41 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa012cdcd391bd8cd78796fe53eb96b7585962832b802667f44cedd88405d0cc`  
		Last Modified: Tue, 05 Apr 2022 04:19:28 GMT  
		Size: 1.2 KB (1238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca8ad568702372595d83e4a4b906e000230b00315e1fd6ef6d219697badb387`  
		Last Modified: Tue, 05 Apr 2022 04:19:28 GMT  
		Size: 110.5 KB (110499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:265ae8d237ddc109ffe7e544e93a0dc1cea5bfe3fa5685fca792afda6d67ed0f`  
		Last Modified: Tue, 05 Apr 2022 04:19:29 GMT  
		Size: 928.4 KB (928406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce17e42e65242140f2a8f7c6d0a16bf4f1b64b0ba276ed8341905ed6f63e4a7b`  
		Last Modified: Tue, 05 Apr 2022 04:19:28 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30070b7f5a7be9b35fb6b8c7f1b6cb0de4508d927cc49caf12b3f6e220b0cc60`  
		Last Modified: Tue, 05 Apr 2022 04:19:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; 386

```console
$ docker pull memcached@sha256:5378334a3366058f6987024a1963dceafda46b182d6236b4685f816238f99992
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3888728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be3d8aa97e2099f400479214a98c34c3a23c21939afde5c6611961b33539a8bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:25 GMT
ADD file:7d51a0f8691eb78c9062fd31984423a93d276a67b4ed5d1a706e1c2cd9fea23a in / 
# Mon, 04 Apr 2022 23:38:25 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:52:17 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 05 Apr 2022 03:52:18 GMT
RUN apk add --no-cache libsasl
# Tue, 05 Apr 2022 03:52:19 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 05 Apr 2022 03:52:20 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 05 Apr 2022 03:55:15 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 05 Apr 2022 03:55:17 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 05 Apr 2022 03:55:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 05 Apr 2022 03:55:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 03:55:19 GMT
USER memcache
# Tue, 05 Apr 2022 03:55:20 GMT
EXPOSE 11211
# Tue, 05 Apr 2022 03:55:21 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:73b28a5955ec7fb46f2cf0434e4901a889f7dda3f8c9ec496300feb256c7eda8`  
		Last Modified: Mon, 04 Apr 2022 19:10:03 GMT  
		Size: 2.8 MB (2818974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06cddc8f8c3aabebd92d18ccbc0c9181ed94cc4b15b5adbda9e2bfdf4b8f38e9`  
		Last Modified: Tue, 05 Apr 2022 03:56:08 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad8594347186db0e9366f74b1e03bd14ed234378b2d1238a6b56504a86608fa6`  
		Last Modified: Tue, 05 Apr 2022 03:56:08 GMT  
		Size: 120.9 KB (120869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d7907ab18015191139b22c9b7b25c6a23d1c569470a49f2eb3e1ef985c4450`  
		Last Modified: Tue, 05 Apr 2022 03:56:08 GMT  
		Size: 947.2 KB (947242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3d6dff2eb04a8a959a2e8d101ca3da2646db4b2125b02fd6505c61ce53215b`  
		Last Modified: Tue, 05 Apr 2022 03:56:08 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:845b50269336006037a46780211bf0b2b95df971864d348d10c893aa2bf3afe3`  
		Last Modified: Tue, 05 Apr 2022 03:56:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:d1110704ee41f1dce802400ce09904c39aff25c66c1e1b87c64781b0bd9527d4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3905105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1827e9495120e553b560bd77e162a97bfdb923a96c36b2dea8afd967fdc57bd1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:30 GMT
ADD file:960cf6f9d3d1cfcb36c2d67dd4c3eaba7db1d0c7afe97968512248d7f234ad47 in / 
# Tue, 05 Apr 2022 00:23:32 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 10:09:23 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 05 Apr 2022 10:09:31 GMT
RUN apk add --no-cache libsasl
# Tue, 05 Apr 2022 10:09:35 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 05 Apr 2022 10:09:41 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 05 Apr 2022 10:12:56 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 05 Apr 2022 10:12:58 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 05 Apr 2022 10:13:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 05 Apr 2022 10:13:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 10:13:10 GMT
USER memcache
# Tue, 05 Apr 2022 10:13:12 GMT
EXPOSE 11211
# Tue, 05 Apr 2022 10:13:14 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1877acf2d48ed8bcb5bd9756a95aca0c077457be7cf4fcef25807f4e9be88db1`  
		Last Modified: Mon, 04 Apr 2022 19:09:49 GMT  
		Size: 2.8 MB (2811186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8124818eb8eba84f8929c5e21fa177a0224a632a260382b31fd9ea53de0cb63`  
		Last Modified: Tue, 05 Apr 2022 10:14:09 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65727b8884a0072f667d76a190572aecbef43ea2013aa1fab131f8ad94cf6027`  
		Last Modified: Tue, 05 Apr 2022 10:14:09 GMT  
		Size: 126.2 KB (126153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fdd85c6abf5a16922e7e67ae0f58814880550c8e561aa25fe98f824c65e283f`  
		Last Modified: Tue, 05 Apr 2022 10:14:09 GMT  
		Size: 966.1 KB (966088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72641c2cb945038b7f950ba927f9377d909670cd2c8a2f99f0027cfe6f34d41f`  
		Last Modified: Tue, 05 Apr 2022 10:14:09 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27047ea6a5173f1f7f40a46c10833cfbf360f9ac71f5595dd2b745afc3f9f3bb`  
		Last Modified: Tue, 05 Apr 2022 10:14:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; s390x

```console
$ docker pull memcached@sha256:f4d6b61f33632664a2176b827e6f04dc9b43bece1e1225f1c27d3f218fcaf90c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3650153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d81b27c0ae4d75825efc6c14a9b31769a43cebc314ab07e25b9024fe3b7d6bf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:18:54 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 05 Apr 2022 11:18:55 GMT
RUN apk add --no-cache libsasl
# Tue, 05 Apr 2022 11:18:55 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 05 Apr 2022 11:18:55 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 05 Apr 2022 11:22:16 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 05 Apr 2022 11:22:16 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 05 Apr 2022 11:22:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 05 Apr 2022 11:22:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 11:22:17 GMT
USER memcache
# Tue, 05 Apr 2022 11:22:17 GMT
EXPOSE 11211
# Tue, 05 Apr 2022 11:22:17 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d92848f08937ad9e3c8df84e91a6ae677af747e7ae736062bf8303e6f98a5a`  
		Last Modified: Tue, 05 Apr 2022 11:23:08 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee4699d5d9185c820000eb9490520b6c45f7c7df9e07c67d79ec6efac05ff170`  
		Last Modified: Tue, 05 Apr 2022 11:23:08 GMT  
		Size: 113.5 KB (113464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c834b41bef6837d1312846d4839e66a0070dd934cb4388ff09a93112f6cdc0`  
		Last Modified: Tue, 05 Apr 2022 11:23:09 GMT  
		Size: 934.6 KB (934639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd760c99b09ff84bd3f703d93a143abd83f2ecfc7c941856bdd4222a4da2b7a`  
		Last Modified: Tue, 05 Apr 2022 11:23:08 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b4795384f4f0fbaa99dd9e3683dfd3639ccbcd001144f0b8d1f050c3a765283`  
		Last Modified: Tue, 05 Apr 2022 11:23:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6-alpine3.15`

```console
$ docker pull memcached@sha256:06bc630f006be575ae4e8a55e515a66daba0ed432f0e46ecfacf654daf4f07e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1.6-alpine3.15` - linux; amd64

```console
$ docker pull memcached@sha256:fbb3eda59b2f6851b1335f6fd43fa5a371ac197b06f84c0363341b7cd1c066f1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3864898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bcea36e93e267587df645dc2c39d08513419e129eb5b28db4a204207d64a9ea6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 09:54:14 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 05 Apr 2022 09:54:15 GMT
RUN apk add --no-cache libsasl
# Tue, 05 Apr 2022 09:54:15 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 05 Apr 2022 09:54:15 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 05 Apr 2022 09:57:57 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 05 Apr 2022 09:57:57 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 05 Apr 2022 09:57:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 05 Apr 2022 09:57:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 09:57:58 GMT
USER memcache
# Tue, 05 Apr 2022 09:57:58 GMT
EXPOSE 11211
# Tue, 05 Apr 2022 09:57:58 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c437462196847904d5021a85f817fecbb0b84eca04e4677f3a907f95125ebd3`  
		Last Modified: Tue, 05 Apr 2022 09:58:27 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37749f62d258e02c4f026b7ed0cb874d23b47abaa2c5860e41b3c099fdeb1d15`  
		Last Modified: Tue, 05 Apr 2022 09:58:27 GMT  
		Size: 109.2 KB (109172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf6c1e9f5167a143f222aea98c5b9c1d58ad0f9eed19d753fa1c4ffdfdd0269`  
		Last Modified: Tue, 05 Apr 2022 09:58:27 GMT  
		Size: 939.5 KB (939497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550e19164877083e509bb0c014a831674a7b77ddcf111d980a4f2b1bd1a78171`  
		Last Modified: Tue, 05 Apr 2022 09:58:27 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:515f37e9ad844fe3fdd82c3504b1c092e11e2c8f5f8395bc8944c96c768f3d3c`  
		Last Modified: Tue, 05 Apr 2022 09:58:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:d38012edd86b9a7abab01b390d4bbce8c39201ebedfd0066fcff6b6fb20cf178
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3757025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e0f3d4ef24801f58b76d5d0e24224de96c6e02fba4eccb3fa2e037e94403f0a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:15:56 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 05 Apr 2022 04:15:57 GMT
RUN apk add --no-cache libsasl
# Tue, 05 Apr 2022 04:15:58 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 05 Apr 2022 04:15:59 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 05 Apr 2022 04:18:36 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 05 Apr 2022 04:18:37 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 05 Apr 2022 04:18:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 05 Apr 2022 04:18:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 04:18:39 GMT
USER memcache
# Tue, 05 Apr 2022 04:18:40 GMT
EXPOSE 11211
# Tue, 05 Apr 2022 04:18:41 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa012cdcd391bd8cd78796fe53eb96b7585962832b802667f44cedd88405d0cc`  
		Last Modified: Tue, 05 Apr 2022 04:19:28 GMT  
		Size: 1.2 KB (1238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca8ad568702372595d83e4a4b906e000230b00315e1fd6ef6d219697badb387`  
		Last Modified: Tue, 05 Apr 2022 04:19:28 GMT  
		Size: 110.5 KB (110499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:265ae8d237ddc109ffe7e544e93a0dc1cea5bfe3fa5685fca792afda6d67ed0f`  
		Last Modified: Tue, 05 Apr 2022 04:19:29 GMT  
		Size: 928.4 KB (928406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce17e42e65242140f2a8f7c6d0a16bf4f1b64b0ba276ed8341905ed6f63e4a7b`  
		Last Modified: Tue, 05 Apr 2022 04:19:28 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30070b7f5a7be9b35fb6b8c7f1b6cb0de4508d927cc49caf12b3f6e220b0cc60`  
		Last Modified: Tue, 05 Apr 2022 04:19:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine3.15` - linux; 386

```console
$ docker pull memcached@sha256:5378334a3366058f6987024a1963dceafda46b182d6236b4685f816238f99992
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3888728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be3d8aa97e2099f400479214a98c34c3a23c21939afde5c6611961b33539a8bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:25 GMT
ADD file:7d51a0f8691eb78c9062fd31984423a93d276a67b4ed5d1a706e1c2cd9fea23a in / 
# Mon, 04 Apr 2022 23:38:25 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:52:17 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 05 Apr 2022 03:52:18 GMT
RUN apk add --no-cache libsasl
# Tue, 05 Apr 2022 03:52:19 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 05 Apr 2022 03:52:20 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 05 Apr 2022 03:55:15 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 05 Apr 2022 03:55:17 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 05 Apr 2022 03:55:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 05 Apr 2022 03:55:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 03:55:19 GMT
USER memcache
# Tue, 05 Apr 2022 03:55:20 GMT
EXPOSE 11211
# Tue, 05 Apr 2022 03:55:21 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:73b28a5955ec7fb46f2cf0434e4901a889f7dda3f8c9ec496300feb256c7eda8`  
		Last Modified: Mon, 04 Apr 2022 19:10:03 GMT  
		Size: 2.8 MB (2818974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06cddc8f8c3aabebd92d18ccbc0c9181ed94cc4b15b5adbda9e2bfdf4b8f38e9`  
		Last Modified: Tue, 05 Apr 2022 03:56:08 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad8594347186db0e9366f74b1e03bd14ed234378b2d1238a6b56504a86608fa6`  
		Last Modified: Tue, 05 Apr 2022 03:56:08 GMT  
		Size: 120.9 KB (120869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d7907ab18015191139b22c9b7b25c6a23d1c569470a49f2eb3e1ef985c4450`  
		Last Modified: Tue, 05 Apr 2022 03:56:08 GMT  
		Size: 947.2 KB (947242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3d6dff2eb04a8a959a2e8d101ca3da2646db4b2125b02fd6505c61ce53215b`  
		Last Modified: Tue, 05 Apr 2022 03:56:08 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:845b50269336006037a46780211bf0b2b95df971864d348d10c893aa2bf3afe3`  
		Last Modified: Tue, 05 Apr 2022 03:56:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine3.15` - linux; ppc64le

```console
$ docker pull memcached@sha256:d1110704ee41f1dce802400ce09904c39aff25c66c1e1b87c64781b0bd9527d4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3905105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1827e9495120e553b560bd77e162a97bfdb923a96c36b2dea8afd967fdc57bd1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:30 GMT
ADD file:960cf6f9d3d1cfcb36c2d67dd4c3eaba7db1d0c7afe97968512248d7f234ad47 in / 
# Tue, 05 Apr 2022 00:23:32 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 10:09:23 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 05 Apr 2022 10:09:31 GMT
RUN apk add --no-cache libsasl
# Tue, 05 Apr 2022 10:09:35 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 05 Apr 2022 10:09:41 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 05 Apr 2022 10:12:56 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 05 Apr 2022 10:12:58 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 05 Apr 2022 10:13:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 05 Apr 2022 10:13:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 10:13:10 GMT
USER memcache
# Tue, 05 Apr 2022 10:13:12 GMT
EXPOSE 11211
# Tue, 05 Apr 2022 10:13:14 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1877acf2d48ed8bcb5bd9756a95aca0c077457be7cf4fcef25807f4e9be88db1`  
		Last Modified: Mon, 04 Apr 2022 19:09:49 GMT  
		Size: 2.8 MB (2811186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8124818eb8eba84f8929c5e21fa177a0224a632a260382b31fd9ea53de0cb63`  
		Last Modified: Tue, 05 Apr 2022 10:14:09 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65727b8884a0072f667d76a190572aecbef43ea2013aa1fab131f8ad94cf6027`  
		Last Modified: Tue, 05 Apr 2022 10:14:09 GMT  
		Size: 126.2 KB (126153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fdd85c6abf5a16922e7e67ae0f58814880550c8e561aa25fe98f824c65e283f`  
		Last Modified: Tue, 05 Apr 2022 10:14:09 GMT  
		Size: 966.1 KB (966088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72641c2cb945038b7f950ba927f9377d909670cd2c8a2f99f0027cfe6f34d41f`  
		Last Modified: Tue, 05 Apr 2022 10:14:09 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27047ea6a5173f1f7f40a46c10833cfbf360f9ac71f5595dd2b745afc3f9f3bb`  
		Last Modified: Tue, 05 Apr 2022 10:14:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine3.15` - linux; s390x

```console
$ docker pull memcached@sha256:f4d6b61f33632664a2176b827e6f04dc9b43bece1e1225f1c27d3f218fcaf90c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3650153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d81b27c0ae4d75825efc6c14a9b31769a43cebc314ab07e25b9024fe3b7d6bf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:18:54 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 05 Apr 2022 11:18:55 GMT
RUN apk add --no-cache libsasl
# Tue, 05 Apr 2022 11:18:55 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 05 Apr 2022 11:18:55 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 05 Apr 2022 11:22:16 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 05 Apr 2022 11:22:16 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 05 Apr 2022 11:22:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 05 Apr 2022 11:22:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 11:22:17 GMT
USER memcache
# Tue, 05 Apr 2022 11:22:17 GMT
EXPOSE 11211
# Tue, 05 Apr 2022 11:22:17 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d92848f08937ad9e3c8df84e91a6ae677af747e7ae736062bf8303e6f98a5a`  
		Last Modified: Tue, 05 Apr 2022 11:23:08 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee4699d5d9185c820000eb9490520b6c45f7c7df9e07c67d79ec6efac05ff170`  
		Last Modified: Tue, 05 Apr 2022 11:23:08 GMT  
		Size: 113.5 KB (113464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c834b41bef6837d1312846d4839e66a0070dd934cb4388ff09a93112f6cdc0`  
		Last Modified: Tue, 05 Apr 2022 11:23:09 GMT  
		Size: 934.6 KB (934639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd760c99b09ff84bd3f703d93a143abd83f2ecfc7c941856bdd4222a4da2b7a`  
		Last Modified: Tue, 05 Apr 2022 11:23:08 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b4795384f4f0fbaa99dd9e3683dfd3639ccbcd001144f0b8d1f050c3a765283`  
		Last Modified: Tue, 05 Apr 2022 11:23:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6-bullseye`

```console
$ docker pull memcached@sha256:05917d8f91b97eff3ffb98497dd139c65f61c2107649cf73db6cced7e7667b94
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

### `memcached:1.6-bullseye` - linux; amd64

```console
$ docker pull memcached@sha256:58a41bfdd7492d7d9be5ea8ab1abeffa106a2193e98e6646be91d06ad37d0675
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32968652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:065555a745051537085b4135608198e45686d4574eda4d7093537d1107a1feff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 11 May 2022 01:20:16 GMT
ADD file:4a0bb88956083aa56032fdd9601d9b66c39b18c896ba35ea33594cd75621640a in / 
# Wed, 11 May 2022 01:20:16 GMT
CMD ["bash"]
# Wed, 11 May 2022 04:44:00 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 11 May 2022 04:44:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 04:44:03 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 11 May 2022 04:44:03 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 11 May 2022 04:46:42 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 May 2022 04:46:42 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 May 2022 04:46:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 04:46:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 04:46:43 GMT
USER memcache
# Wed, 11 May 2022 04:46:43 GMT
EXPOSE 11211
# Wed, 11 May 2022 04:46:43 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:214ca5fb90323fe769c63a12af092f2572bf1c6b300263e09883909fc865d260`  
		Last Modified: Wed, 11 May 2022 01:25:13 GMT  
		Size: 31.4 MB (31379476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae8d4b1feabc5879929064e635eb9f14ef5b8a15bac772048359ca7ff051d1c`  
		Last Modified: Wed, 11 May 2022 04:47:13 GMT  
		Size: 5.0 KB (4975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dc491b9af677c0a71fa36fcbf2faea8087acafa69e2d760fcaea4f26fb5eb2a`  
		Last Modified: Wed, 11 May 2022 04:47:14 GMT  
		Size: 328.1 KB (328091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c355a147dff081cfbbf9d104870e2195eb0213138ae88d87a585b466fc521d4a`  
		Last Modified: Wed, 11 May 2022 04:47:14 GMT  
		Size: 1.3 MB (1255702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0cc0d566fb2a731f9d4dd270354fe902ec4b175b95e3552e17d53a76601b28d`  
		Last Modified: Wed, 11 May 2022 04:47:13 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d5c91075c8421465ad8ef2fe32f6daab4ff01b837e03aee3568d39c64cb2d3`  
		Last Modified: Wed, 11 May 2022 04:47:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bullseye` - linux; arm variant v5

```console
$ docker pull memcached@sha256:7114dc5aaa1603875d79f65e4d27cf83fd5c6ff279092e5019313c2e676e8563
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30469996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:711c043049190c6786a1fe335232c7bee5a0c58134e9481f385ae99e18cff3a2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 11 May 2022 00:50:34 GMT
ADD file:72357b75d7e4546f06abf4648ab600980e742a3017f36da3c7a6c086f2f5fb56 in / 
# Wed, 11 May 2022 00:50:35 GMT
CMD ["bash"]
# Wed, 11 May 2022 19:59:38 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 11 May 2022 19:59:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 19:59:48 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 11 May 2022 19:59:49 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 11 May 2022 20:04:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 May 2022 20:04:12 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 May 2022 20:04:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 20:04:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 20:04:14 GMT
USER memcache
# Wed, 11 May 2022 20:04:15 GMT
EXPOSE 11211
# Wed, 11 May 2022 20:04:15 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f7b69be15db1cb94a249f74b27edd4f5e5923a8701b026179a593f6888e897aa`  
		Last Modified: Wed, 11 May 2022 01:05:51 GMT  
		Size: 28.9 MB (28921122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e23defdefe7366c4546b3284b11bdbedcf73c55c4cad0c49a2e12b6bc971f653`  
		Last Modified: Wed, 11 May 2022 20:05:07 GMT  
		Size: 4.9 KB (4893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aed101d7cb94db52f647e3cf585d3a7702b5a01cb3f7c3fc86aedcd94fb5b01`  
		Last Modified: Wed, 11 May 2022 20:05:07 GMT  
		Size: 316.6 KB (316610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80e354b9ae9a23ca02681ddaca03fe3a6fa45069b80a683e38123aa3a0174fab`  
		Last Modified: Wed, 11 May 2022 20:05:08 GMT  
		Size: 1.2 MB (1226962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d82b2d2d5ab7db68fddbbf26596ed21c9c4506e0355be942188f9a81557bdd`  
		Last Modified: Wed, 11 May 2022 20:05:07 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd35d60f098711fce5b4a2d107b57cfe22a70cbb6bf47476c42ea4d975b6c3f7`  
		Last Modified: Wed, 11 May 2022 20:05:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bullseye` - linux; arm variant v7

```console
$ docker pull memcached@sha256:34dee5b2772158236707bc1811db77d4adc27d86ca6b1b096fb444a8cfef133e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28091607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad29267829b7cd5d6051ca12869e51112bded24fc2e06656b673942a215f1c84`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 20 Apr 2022 13:27:18 GMT
ADD file:1a0e290eb32b3533f9d1684c683ad866b5003579790b25ad61b2044dc6c20bbb in / 
# Wed, 20 Apr 2022 13:27:18 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 21:47:36 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 20 Apr 2022 21:47:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 21:47:45 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 20 Apr 2022 21:47:45 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 20 Apr 2022 21:51:42 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 20 Apr 2022 21:51:42 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 20 Apr 2022 21:51:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 20 Apr 2022 21:51:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Apr 2022 21:51:45 GMT
USER memcache
# Wed, 20 Apr 2022 21:51:45 GMT
EXPOSE 11211
# Wed, 20 Apr 2022 21:51:46 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a6b2963233cd14b47391f0e25f2a485bbeabb87e771a71b73e5cde7c013963da`  
		Last Modified: Wed, 20 Apr 2022 13:43:41 GMT  
		Size: 26.6 MB (26575758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4b149950ca557655b7e9b7229a81d7d772f2aad316a5ce7de452664795a377`  
		Last Modified: Wed, 20 Apr 2022 22:04:23 GMT  
		Size: 4.9 KB (4893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d14f3b12cc24aac4e3614237409e18959637d8420b534524bc1fe63e7456a660`  
		Last Modified: Wed, 20 Apr 2022 22:04:23 GMT  
		Size: 312.1 KB (312059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca5c1518bd4380c5c22f884d402b699c75cb53de72de7d5b2a53e99d8ba56d9e`  
		Last Modified: Wed, 20 Apr 2022 22:04:24 GMT  
		Size: 1.2 MB (1198488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd1a54f20b40e9c7302a4ab0c46cc590140bde81aba4ab1d149dd8b2b3edade`  
		Last Modified: Wed, 20 Apr 2022 22:04:23 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6e66d52d7551a05a10e5a70971eef4ad0803f499c934fd1ec734a144e5bc64`  
		Last Modified: Wed, 20 Apr 2022 22:04:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bullseye` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:6c452eece1271128806922efd79c0ef0f809e6705d855d6a271f5208d2a2117d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31444857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d45eed3b8e469acc08e97e874bb1e8b4f004720606f20212dad652f79ca29db4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 11 May 2022 00:46:59 GMT
ADD file:158a0e401328bd7c0d49b9e8539186098967218f1b1a8c811f4398d29b74397f in / 
# Wed, 11 May 2022 00:47:00 GMT
CMD ["bash"]
# Wed, 11 May 2022 02:27:34 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 11 May 2022 02:27:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:27:38 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 11 May 2022 02:27:39 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 11 May 2022 02:30:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 May 2022 02:30:13 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 May 2022 02:30:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 02:30:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 02:30:15 GMT
USER memcache
# Wed, 11 May 2022 02:30:16 GMT
EXPOSE 11211
# Wed, 11 May 2022 02:30:17 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:dfdd5ffb257742b891ccad9400a77dad2a6260b2451e0f5e48a9ade1d17a87ec`  
		Last Modified: Wed, 11 May 2022 00:53:46 GMT  
		Size: 30.1 MB (30065693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:921e9eec57430f29a509862965b1bc0f909703c8c5e73b2345205cbd6b715910`  
		Last Modified: Wed, 11 May 2022 02:31:07 GMT  
		Size: 4.9 KB (4900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:984aa2c2269106d51c47bed797929d496825d1dee8883d84918fd98cd809ba76`  
		Last Modified: Wed, 11 May 2022 02:31:07 GMT  
		Size: 119.2 KB (119215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b52324e4c1cc245d2131fae3776a0359730099f17e8039fa1db0d0b6310a195`  
		Last Modified: Wed, 11 May 2022 02:31:08 GMT  
		Size: 1.3 MB (1254642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70bc38e444a829155cb5ad8ca3f2b8cc68a6065e19b795707656cec98edadbfc`  
		Last Modified: Wed, 11 May 2022 02:31:07 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b29514622ffb8a37130cc9662034040cbc8ff1d5c7b8ce620f49c0d26b24b73`  
		Last Modified: Wed, 11 May 2022 02:31:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bullseye` - linux; 386

```console
$ docker pull memcached@sha256:faedc990d98e8f3b6058c1e3f9ace6816b59338aaf906a8099a0b1141713d345
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33778000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74fb9295e5de207e5aade7877e8b45371b49a320bf3eafbfe65ea15c6f70dd59`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 11 May 2022 01:39:14 GMT
ADD file:9eecb0fd311177f9d226e914c411aef49b5de1930e73019d2ee24afed515b5a2 in / 
# Wed, 11 May 2022 01:39:14 GMT
CMD ["bash"]
# Wed, 11 May 2022 04:32:45 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 11 May 2022 04:32:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 04:32:49 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 11 May 2022 04:32:50 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 11 May 2022 04:35:41 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 May 2022 04:35:43 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 May 2022 04:35:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 04:35:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 04:35:45 GMT
USER memcache
# Wed, 11 May 2022 04:35:46 GMT
EXPOSE 11211
# Wed, 11 May 2022 04:35:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:91c5bdbe4bf9f1970dd54ba71e2523649adce4e5240c2ff8a87711bf389ecba3`  
		Last Modified: Wed, 11 May 2022 01:46:25 GMT  
		Size: 32.4 MB (32389776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cbc080a4e6972a45023b1c0d8d9f74e9df257677ec7503a9f8756eabb61b5e0`  
		Last Modified: Wed, 11 May 2022 04:36:36 GMT  
		Size: 4.8 KB (4771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdfcc6e2f39957ee91e94aa2f1264a35ccef2b3aed8ae29d859144d763ed06ab`  
		Last Modified: Wed, 11 May 2022 04:36:36 GMT  
		Size: 130.1 KB (130140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a68472399b32a22e31b1b551482a4fec929210d4db3da6b3010fdb3a97bf0944`  
		Last Modified: Wed, 11 May 2022 04:36:37 GMT  
		Size: 1.3 MB (1252905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a1040db24a5a1a06568a3d81752b73f002172ebec23d3ace2181c365e6216c9`  
		Last Modified: Wed, 11 May 2022 04:36:36 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496cfb26b818ba873c9dbd7203c2551d9c1503db7a8281c82b03ecd7987dfe44`  
		Last Modified: Wed, 11 May 2022 04:36:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bullseye` - linux; mips64le

```console
$ docker pull memcached@sha256:d4d70ee02bd6a268e51e7cb45ae2ab6028a3f5546e3566abea4839b7bc0b2795
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31014729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5edfa57d6aec6089194206346467a5708554650f75a703542020f03dda6cfb13`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 11 May 2022 02:23:35 GMT
ADD file:d47dce2adbc9352ef1d437730bab3b579dd8d2bf29dd60cd8a8b65396b39e36e in / 
# Wed, 11 May 2022 02:23:40 GMT
CMD ["bash"]
# Wed, 11 May 2022 04:26:13 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 11 May 2022 04:26:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 04:26:33 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 11 May 2022 04:26:36 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 11 May 2022 04:33:31 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 May 2022 04:33:33 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 May 2022 04:33:38 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 04:33:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 04:33:43 GMT
USER memcache
# Wed, 11 May 2022 04:33:45 GMT
EXPOSE 11211
# Wed, 11 May 2022 04:33:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:438a36bf0b6e75ff6f0fbb2b7669dfb86361416f4d808912d30cf5b91ad2eea9`  
		Last Modified: Wed, 11 May 2022 02:33:43 GMT  
		Size: 29.6 MB (29641051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2947248cd8e754e130fecb9083b0ad0025e50361a44987eadfb6edfeb2e3908c`  
		Last Modified: Wed, 11 May 2022 04:34:05 GMT  
		Size: 4.9 KB (4861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3849c71c1ab16dd8196e74fd37ae70b3a0b89a3b07a9cb7f76535725af27a86a`  
		Last Modified: Wed, 11 May 2022 04:34:05 GMT  
		Size: 117.2 KB (117156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f24b722d80efb82b9982c69a407116125ad8a340447344e252517f9798849b9`  
		Last Modified: Wed, 11 May 2022 04:34:06 GMT  
		Size: 1.3 MB (1251254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f4827b1598450f78ff6da5317e269d8fdc544d21ff25409586a2db03053022`  
		Last Modified: Wed, 11 May 2022 04:34:05 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:090d97f72bbcf506ab0dc4d8e19c3a1522513237327ced2e711f0613fb262865`  
		Last Modified: Wed, 11 May 2022 04:34:05 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bullseye` - linux; ppc64le

```console
$ docker pull memcached@sha256:673643121e94f08dd12197b69994ec2cad834c15326b37ba83861eb00aa22134
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36971800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:821c76dba347fd635474ef0126da0d404cc404e989635b028d0da3c2dfb273b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 11 May 2022 01:32:29 GMT
ADD file:1e94716789ec21981460f74be38a668bc212bd804c1d41cecf90036a5bccac5a in / 
# Wed, 11 May 2022 01:32:34 GMT
CMD ["bash"]
# Wed, 11 May 2022 07:51:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 11 May 2022 07:51:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 07:51:40 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 11 May 2022 07:51:48 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 11 May 2022 07:57:31 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 May 2022 07:57:33 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 May 2022 07:57:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 07:57:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 07:57:49 GMT
USER memcache
# Wed, 11 May 2022 07:57:55 GMT
EXPOSE 11211
# Wed, 11 May 2022 07:58:00 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2533109ed11eefd6415e0370d6d7a3ea879b582b1887c98b819a598ad18fca24`  
		Last Modified: Wed, 11 May 2022 01:43:03 GMT  
		Size: 35.3 MB (35286467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:103a6713e9bf2853760692eb30b886453378b61e3fb83321c0ce1fec39bdf2f2`  
		Last Modified: Wed, 11 May 2022 07:59:13 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9173dced38a5c576a66100ed6df59833b82ee6847ed29531d690b7377a72e02d`  
		Last Modified: Wed, 11 May 2022 07:59:13 GMT  
		Size: 356.9 KB (356938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e15378aab9e7b0eefd835da5eeee5fe567c111dcf6df814b34f6755cf27c45`  
		Last Modified: Wed, 11 May 2022 07:59:13 GMT  
		Size: 1.3 MB (1323008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523888230dfa0221ad182120061be4802ac72d7a19047277ffc452c5003537b5`  
		Last Modified: Wed, 11 May 2022 07:59:13 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12893f041469d0edbc3132e6af823296c231a18db48dc29c665658f6ba859c9f`  
		Last Modified: Wed, 11 May 2022 07:59:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bullseye` - linux; s390x

```console
$ docker pull memcached@sha256:d0221a850100573af43f6113f62398369ddaa506aef1fd1e114da8fdd4403330
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31225739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37e72a40047bd848bbedd03871f17d8132f625301f2203038b265841fa1a660f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 11 May 2022 00:44:17 GMT
ADD file:d93a1cf64a813d01774cd628dfd683c006e20159e2ab3464c2159c8d9897c725 in / 
# Wed, 11 May 2022 00:44:19 GMT
CMD ["bash"]
# Wed, 11 May 2022 02:35:31 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 11 May 2022 02:35:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:35:34 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 11 May 2022 02:35:34 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 11 May 2022 02:39:02 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 May 2022 02:39:03 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 May 2022 02:39:03 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 02:39:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 02:39:03 GMT
USER memcache
# Wed, 11 May 2022 02:39:03 GMT
EXPOSE 11211
# Wed, 11 May 2022 02:39:04 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9f3750f6094217808e26d471752341db88153c8d5b5f9bb11577b74671303bbc`  
		Last Modified: Wed, 11 May 2022 00:50:03 GMT  
		Size: 29.7 MB (29654739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29541285df59f95a596b1911b49171e64e2361189a163533e77dbf2961b8f685`  
		Last Modified: Wed, 11 May 2022 02:40:04 GMT  
		Size: 5.0 KB (5026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c94a32e11bca5f817bc7015ceff49279fcd263d523198a38cc02607b7899e261`  
		Last Modified: Wed, 11 May 2022 02:40:04 GMT  
		Size: 324.2 KB (324197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57395e3cd66c2852ddaac636856f0245c1cfdca358d6bb75128950b9d9042481`  
		Last Modified: Wed, 11 May 2022 02:40:04 GMT  
		Size: 1.2 MB (1241369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ed03e37cb4ad7ab6dfc00b4938e9e5ec27777eb89fe1918ffc45a5a8de10c0`  
		Last Modified: Wed, 11 May 2022 02:40:04 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79cc46e5a2551dd05d1dcb476692b2a5d1c7e5181f253ad3938c179835018b95`  
		Last Modified: Wed, 11 May 2022 02:40:03 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.15`

```console
$ docker pull memcached@sha256:05917d8f91b97eff3ffb98497dd139c65f61c2107649cf73db6cced7e7667b94
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

### `memcached:1.6.15` - linux; amd64

```console
$ docker pull memcached@sha256:58a41bfdd7492d7d9be5ea8ab1abeffa106a2193e98e6646be91d06ad37d0675
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32968652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:065555a745051537085b4135608198e45686d4574eda4d7093537d1107a1feff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 11 May 2022 01:20:16 GMT
ADD file:4a0bb88956083aa56032fdd9601d9b66c39b18c896ba35ea33594cd75621640a in / 
# Wed, 11 May 2022 01:20:16 GMT
CMD ["bash"]
# Wed, 11 May 2022 04:44:00 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 11 May 2022 04:44:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 04:44:03 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 11 May 2022 04:44:03 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 11 May 2022 04:46:42 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 May 2022 04:46:42 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 May 2022 04:46:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 04:46:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 04:46:43 GMT
USER memcache
# Wed, 11 May 2022 04:46:43 GMT
EXPOSE 11211
# Wed, 11 May 2022 04:46:43 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:214ca5fb90323fe769c63a12af092f2572bf1c6b300263e09883909fc865d260`  
		Last Modified: Wed, 11 May 2022 01:25:13 GMT  
		Size: 31.4 MB (31379476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae8d4b1feabc5879929064e635eb9f14ef5b8a15bac772048359ca7ff051d1c`  
		Last Modified: Wed, 11 May 2022 04:47:13 GMT  
		Size: 5.0 KB (4975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dc491b9af677c0a71fa36fcbf2faea8087acafa69e2d760fcaea4f26fb5eb2a`  
		Last Modified: Wed, 11 May 2022 04:47:14 GMT  
		Size: 328.1 KB (328091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c355a147dff081cfbbf9d104870e2195eb0213138ae88d87a585b466fc521d4a`  
		Last Modified: Wed, 11 May 2022 04:47:14 GMT  
		Size: 1.3 MB (1255702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0cc0d566fb2a731f9d4dd270354fe902ec4b175b95e3552e17d53a76601b28d`  
		Last Modified: Wed, 11 May 2022 04:47:13 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d5c91075c8421465ad8ef2fe32f6daab4ff01b837e03aee3568d39c64cb2d3`  
		Last Modified: Wed, 11 May 2022 04:47:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.15` - linux; arm variant v5

```console
$ docker pull memcached@sha256:7114dc5aaa1603875d79f65e4d27cf83fd5c6ff279092e5019313c2e676e8563
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30469996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:711c043049190c6786a1fe335232c7bee5a0c58134e9481f385ae99e18cff3a2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 11 May 2022 00:50:34 GMT
ADD file:72357b75d7e4546f06abf4648ab600980e742a3017f36da3c7a6c086f2f5fb56 in / 
# Wed, 11 May 2022 00:50:35 GMT
CMD ["bash"]
# Wed, 11 May 2022 19:59:38 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 11 May 2022 19:59:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 19:59:48 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 11 May 2022 19:59:49 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 11 May 2022 20:04:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 May 2022 20:04:12 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 May 2022 20:04:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 20:04:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 20:04:14 GMT
USER memcache
# Wed, 11 May 2022 20:04:15 GMT
EXPOSE 11211
# Wed, 11 May 2022 20:04:15 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f7b69be15db1cb94a249f74b27edd4f5e5923a8701b026179a593f6888e897aa`  
		Last Modified: Wed, 11 May 2022 01:05:51 GMT  
		Size: 28.9 MB (28921122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e23defdefe7366c4546b3284b11bdbedcf73c55c4cad0c49a2e12b6bc971f653`  
		Last Modified: Wed, 11 May 2022 20:05:07 GMT  
		Size: 4.9 KB (4893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aed101d7cb94db52f647e3cf585d3a7702b5a01cb3f7c3fc86aedcd94fb5b01`  
		Last Modified: Wed, 11 May 2022 20:05:07 GMT  
		Size: 316.6 KB (316610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80e354b9ae9a23ca02681ddaca03fe3a6fa45069b80a683e38123aa3a0174fab`  
		Last Modified: Wed, 11 May 2022 20:05:08 GMT  
		Size: 1.2 MB (1226962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d82b2d2d5ab7db68fddbbf26596ed21c9c4506e0355be942188f9a81557bdd`  
		Last Modified: Wed, 11 May 2022 20:05:07 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd35d60f098711fce5b4a2d107b57cfe22a70cbb6bf47476c42ea4d975b6c3f7`  
		Last Modified: Wed, 11 May 2022 20:05:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.15` - linux; arm variant v7

```console
$ docker pull memcached@sha256:34dee5b2772158236707bc1811db77d4adc27d86ca6b1b096fb444a8cfef133e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28091607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad29267829b7cd5d6051ca12869e51112bded24fc2e06656b673942a215f1c84`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 20 Apr 2022 13:27:18 GMT
ADD file:1a0e290eb32b3533f9d1684c683ad866b5003579790b25ad61b2044dc6c20bbb in / 
# Wed, 20 Apr 2022 13:27:18 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 21:47:36 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 20 Apr 2022 21:47:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 21:47:45 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 20 Apr 2022 21:47:45 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 20 Apr 2022 21:51:42 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 20 Apr 2022 21:51:42 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 20 Apr 2022 21:51:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 20 Apr 2022 21:51:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Apr 2022 21:51:45 GMT
USER memcache
# Wed, 20 Apr 2022 21:51:45 GMT
EXPOSE 11211
# Wed, 20 Apr 2022 21:51:46 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a6b2963233cd14b47391f0e25f2a485bbeabb87e771a71b73e5cde7c013963da`  
		Last Modified: Wed, 20 Apr 2022 13:43:41 GMT  
		Size: 26.6 MB (26575758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4b149950ca557655b7e9b7229a81d7d772f2aad316a5ce7de452664795a377`  
		Last Modified: Wed, 20 Apr 2022 22:04:23 GMT  
		Size: 4.9 KB (4893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d14f3b12cc24aac4e3614237409e18959637d8420b534524bc1fe63e7456a660`  
		Last Modified: Wed, 20 Apr 2022 22:04:23 GMT  
		Size: 312.1 KB (312059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca5c1518bd4380c5c22f884d402b699c75cb53de72de7d5b2a53e99d8ba56d9e`  
		Last Modified: Wed, 20 Apr 2022 22:04:24 GMT  
		Size: 1.2 MB (1198488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd1a54f20b40e9c7302a4ab0c46cc590140bde81aba4ab1d149dd8b2b3edade`  
		Last Modified: Wed, 20 Apr 2022 22:04:23 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6e66d52d7551a05a10e5a70971eef4ad0803f499c934fd1ec734a144e5bc64`  
		Last Modified: Wed, 20 Apr 2022 22:04:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.15` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:6c452eece1271128806922efd79c0ef0f809e6705d855d6a271f5208d2a2117d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31444857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d45eed3b8e469acc08e97e874bb1e8b4f004720606f20212dad652f79ca29db4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 11 May 2022 00:46:59 GMT
ADD file:158a0e401328bd7c0d49b9e8539186098967218f1b1a8c811f4398d29b74397f in / 
# Wed, 11 May 2022 00:47:00 GMT
CMD ["bash"]
# Wed, 11 May 2022 02:27:34 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 11 May 2022 02:27:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:27:38 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 11 May 2022 02:27:39 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 11 May 2022 02:30:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 May 2022 02:30:13 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 May 2022 02:30:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 02:30:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 02:30:15 GMT
USER memcache
# Wed, 11 May 2022 02:30:16 GMT
EXPOSE 11211
# Wed, 11 May 2022 02:30:17 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:dfdd5ffb257742b891ccad9400a77dad2a6260b2451e0f5e48a9ade1d17a87ec`  
		Last Modified: Wed, 11 May 2022 00:53:46 GMT  
		Size: 30.1 MB (30065693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:921e9eec57430f29a509862965b1bc0f909703c8c5e73b2345205cbd6b715910`  
		Last Modified: Wed, 11 May 2022 02:31:07 GMT  
		Size: 4.9 KB (4900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:984aa2c2269106d51c47bed797929d496825d1dee8883d84918fd98cd809ba76`  
		Last Modified: Wed, 11 May 2022 02:31:07 GMT  
		Size: 119.2 KB (119215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b52324e4c1cc245d2131fae3776a0359730099f17e8039fa1db0d0b6310a195`  
		Last Modified: Wed, 11 May 2022 02:31:08 GMT  
		Size: 1.3 MB (1254642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70bc38e444a829155cb5ad8ca3f2b8cc68a6065e19b795707656cec98edadbfc`  
		Last Modified: Wed, 11 May 2022 02:31:07 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b29514622ffb8a37130cc9662034040cbc8ff1d5c7b8ce620f49c0d26b24b73`  
		Last Modified: Wed, 11 May 2022 02:31:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.15` - linux; 386

```console
$ docker pull memcached@sha256:faedc990d98e8f3b6058c1e3f9ace6816b59338aaf906a8099a0b1141713d345
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33778000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74fb9295e5de207e5aade7877e8b45371b49a320bf3eafbfe65ea15c6f70dd59`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 11 May 2022 01:39:14 GMT
ADD file:9eecb0fd311177f9d226e914c411aef49b5de1930e73019d2ee24afed515b5a2 in / 
# Wed, 11 May 2022 01:39:14 GMT
CMD ["bash"]
# Wed, 11 May 2022 04:32:45 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 11 May 2022 04:32:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 04:32:49 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 11 May 2022 04:32:50 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 11 May 2022 04:35:41 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 May 2022 04:35:43 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 May 2022 04:35:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 04:35:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 04:35:45 GMT
USER memcache
# Wed, 11 May 2022 04:35:46 GMT
EXPOSE 11211
# Wed, 11 May 2022 04:35:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:91c5bdbe4bf9f1970dd54ba71e2523649adce4e5240c2ff8a87711bf389ecba3`  
		Last Modified: Wed, 11 May 2022 01:46:25 GMT  
		Size: 32.4 MB (32389776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cbc080a4e6972a45023b1c0d8d9f74e9df257677ec7503a9f8756eabb61b5e0`  
		Last Modified: Wed, 11 May 2022 04:36:36 GMT  
		Size: 4.8 KB (4771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdfcc6e2f39957ee91e94aa2f1264a35ccef2b3aed8ae29d859144d763ed06ab`  
		Last Modified: Wed, 11 May 2022 04:36:36 GMT  
		Size: 130.1 KB (130140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a68472399b32a22e31b1b551482a4fec929210d4db3da6b3010fdb3a97bf0944`  
		Last Modified: Wed, 11 May 2022 04:36:37 GMT  
		Size: 1.3 MB (1252905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a1040db24a5a1a06568a3d81752b73f002172ebec23d3ace2181c365e6216c9`  
		Last Modified: Wed, 11 May 2022 04:36:36 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496cfb26b818ba873c9dbd7203c2551d9c1503db7a8281c82b03ecd7987dfe44`  
		Last Modified: Wed, 11 May 2022 04:36:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.15` - linux; mips64le

```console
$ docker pull memcached@sha256:d4d70ee02bd6a268e51e7cb45ae2ab6028a3f5546e3566abea4839b7bc0b2795
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31014729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5edfa57d6aec6089194206346467a5708554650f75a703542020f03dda6cfb13`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 11 May 2022 02:23:35 GMT
ADD file:d47dce2adbc9352ef1d437730bab3b579dd8d2bf29dd60cd8a8b65396b39e36e in / 
# Wed, 11 May 2022 02:23:40 GMT
CMD ["bash"]
# Wed, 11 May 2022 04:26:13 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 11 May 2022 04:26:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 04:26:33 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 11 May 2022 04:26:36 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 11 May 2022 04:33:31 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 May 2022 04:33:33 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 May 2022 04:33:38 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 04:33:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 04:33:43 GMT
USER memcache
# Wed, 11 May 2022 04:33:45 GMT
EXPOSE 11211
# Wed, 11 May 2022 04:33:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:438a36bf0b6e75ff6f0fbb2b7669dfb86361416f4d808912d30cf5b91ad2eea9`  
		Last Modified: Wed, 11 May 2022 02:33:43 GMT  
		Size: 29.6 MB (29641051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2947248cd8e754e130fecb9083b0ad0025e50361a44987eadfb6edfeb2e3908c`  
		Last Modified: Wed, 11 May 2022 04:34:05 GMT  
		Size: 4.9 KB (4861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3849c71c1ab16dd8196e74fd37ae70b3a0b89a3b07a9cb7f76535725af27a86a`  
		Last Modified: Wed, 11 May 2022 04:34:05 GMT  
		Size: 117.2 KB (117156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f24b722d80efb82b9982c69a407116125ad8a340447344e252517f9798849b9`  
		Last Modified: Wed, 11 May 2022 04:34:06 GMT  
		Size: 1.3 MB (1251254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f4827b1598450f78ff6da5317e269d8fdc544d21ff25409586a2db03053022`  
		Last Modified: Wed, 11 May 2022 04:34:05 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:090d97f72bbcf506ab0dc4d8e19c3a1522513237327ced2e711f0613fb262865`  
		Last Modified: Wed, 11 May 2022 04:34:05 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.15` - linux; ppc64le

```console
$ docker pull memcached@sha256:673643121e94f08dd12197b69994ec2cad834c15326b37ba83861eb00aa22134
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36971800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:821c76dba347fd635474ef0126da0d404cc404e989635b028d0da3c2dfb273b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 11 May 2022 01:32:29 GMT
ADD file:1e94716789ec21981460f74be38a668bc212bd804c1d41cecf90036a5bccac5a in / 
# Wed, 11 May 2022 01:32:34 GMT
CMD ["bash"]
# Wed, 11 May 2022 07:51:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 11 May 2022 07:51:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 07:51:40 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 11 May 2022 07:51:48 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 11 May 2022 07:57:31 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 May 2022 07:57:33 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 May 2022 07:57:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 07:57:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 07:57:49 GMT
USER memcache
# Wed, 11 May 2022 07:57:55 GMT
EXPOSE 11211
# Wed, 11 May 2022 07:58:00 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2533109ed11eefd6415e0370d6d7a3ea879b582b1887c98b819a598ad18fca24`  
		Last Modified: Wed, 11 May 2022 01:43:03 GMT  
		Size: 35.3 MB (35286467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:103a6713e9bf2853760692eb30b886453378b61e3fb83321c0ce1fec39bdf2f2`  
		Last Modified: Wed, 11 May 2022 07:59:13 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9173dced38a5c576a66100ed6df59833b82ee6847ed29531d690b7377a72e02d`  
		Last Modified: Wed, 11 May 2022 07:59:13 GMT  
		Size: 356.9 KB (356938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e15378aab9e7b0eefd835da5eeee5fe567c111dcf6df814b34f6755cf27c45`  
		Last Modified: Wed, 11 May 2022 07:59:13 GMT  
		Size: 1.3 MB (1323008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523888230dfa0221ad182120061be4802ac72d7a19047277ffc452c5003537b5`  
		Last Modified: Wed, 11 May 2022 07:59:13 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12893f041469d0edbc3132e6af823296c231a18db48dc29c665658f6ba859c9f`  
		Last Modified: Wed, 11 May 2022 07:59:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.15` - linux; s390x

```console
$ docker pull memcached@sha256:d0221a850100573af43f6113f62398369ddaa506aef1fd1e114da8fdd4403330
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31225739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37e72a40047bd848bbedd03871f17d8132f625301f2203038b265841fa1a660f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 11 May 2022 00:44:17 GMT
ADD file:d93a1cf64a813d01774cd628dfd683c006e20159e2ab3464c2159c8d9897c725 in / 
# Wed, 11 May 2022 00:44:19 GMT
CMD ["bash"]
# Wed, 11 May 2022 02:35:31 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 11 May 2022 02:35:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:35:34 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 11 May 2022 02:35:34 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 11 May 2022 02:39:02 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 May 2022 02:39:03 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 May 2022 02:39:03 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 02:39:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 02:39:03 GMT
USER memcache
# Wed, 11 May 2022 02:39:03 GMT
EXPOSE 11211
# Wed, 11 May 2022 02:39:04 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9f3750f6094217808e26d471752341db88153c8d5b5f9bb11577b74671303bbc`  
		Last Modified: Wed, 11 May 2022 00:50:03 GMT  
		Size: 29.7 MB (29654739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29541285df59f95a596b1911b49171e64e2361189a163533e77dbf2961b8f685`  
		Last Modified: Wed, 11 May 2022 02:40:04 GMT  
		Size: 5.0 KB (5026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c94a32e11bca5f817bc7015ceff49279fcd263d523198a38cc02607b7899e261`  
		Last Modified: Wed, 11 May 2022 02:40:04 GMT  
		Size: 324.2 KB (324197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57395e3cd66c2852ddaac636856f0245c1cfdca358d6bb75128950b9d9042481`  
		Last Modified: Wed, 11 May 2022 02:40:04 GMT  
		Size: 1.2 MB (1241369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ed03e37cb4ad7ab6dfc00b4938e9e5ec27777eb89fe1918ffc45a5a8de10c0`  
		Last Modified: Wed, 11 May 2022 02:40:04 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79cc46e5a2551dd05d1dcb476692b2a5d1c7e5181f253ad3938c179835018b95`  
		Last Modified: Wed, 11 May 2022 02:40:03 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.15-alpine`

```console
$ docker pull memcached@sha256:06bc630f006be575ae4e8a55e515a66daba0ed432f0e46ecfacf654daf4f07e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1.6.15-alpine` - linux; amd64

```console
$ docker pull memcached@sha256:fbb3eda59b2f6851b1335f6fd43fa5a371ac197b06f84c0363341b7cd1c066f1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3864898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bcea36e93e267587df645dc2c39d08513419e129eb5b28db4a204207d64a9ea6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 09:54:14 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 05 Apr 2022 09:54:15 GMT
RUN apk add --no-cache libsasl
# Tue, 05 Apr 2022 09:54:15 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 05 Apr 2022 09:54:15 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 05 Apr 2022 09:57:57 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 05 Apr 2022 09:57:57 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 05 Apr 2022 09:57:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 05 Apr 2022 09:57:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 09:57:58 GMT
USER memcache
# Tue, 05 Apr 2022 09:57:58 GMT
EXPOSE 11211
# Tue, 05 Apr 2022 09:57:58 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c437462196847904d5021a85f817fecbb0b84eca04e4677f3a907f95125ebd3`  
		Last Modified: Tue, 05 Apr 2022 09:58:27 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37749f62d258e02c4f026b7ed0cb874d23b47abaa2c5860e41b3c099fdeb1d15`  
		Last Modified: Tue, 05 Apr 2022 09:58:27 GMT  
		Size: 109.2 KB (109172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf6c1e9f5167a143f222aea98c5b9c1d58ad0f9eed19d753fa1c4ffdfdd0269`  
		Last Modified: Tue, 05 Apr 2022 09:58:27 GMT  
		Size: 939.5 KB (939497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550e19164877083e509bb0c014a831674a7b77ddcf111d980a4f2b1bd1a78171`  
		Last Modified: Tue, 05 Apr 2022 09:58:27 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:515f37e9ad844fe3fdd82c3504b1c092e11e2c8f5f8395bc8944c96c768f3d3c`  
		Last Modified: Tue, 05 Apr 2022 09:58:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.15-alpine` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:d38012edd86b9a7abab01b390d4bbce8c39201ebedfd0066fcff6b6fb20cf178
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3757025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e0f3d4ef24801f58b76d5d0e24224de96c6e02fba4eccb3fa2e037e94403f0a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:15:56 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 05 Apr 2022 04:15:57 GMT
RUN apk add --no-cache libsasl
# Tue, 05 Apr 2022 04:15:58 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 05 Apr 2022 04:15:59 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 05 Apr 2022 04:18:36 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 05 Apr 2022 04:18:37 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 05 Apr 2022 04:18:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 05 Apr 2022 04:18:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 04:18:39 GMT
USER memcache
# Tue, 05 Apr 2022 04:18:40 GMT
EXPOSE 11211
# Tue, 05 Apr 2022 04:18:41 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa012cdcd391bd8cd78796fe53eb96b7585962832b802667f44cedd88405d0cc`  
		Last Modified: Tue, 05 Apr 2022 04:19:28 GMT  
		Size: 1.2 KB (1238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca8ad568702372595d83e4a4b906e000230b00315e1fd6ef6d219697badb387`  
		Last Modified: Tue, 05 Apr 2022 04:19:28 GMT  
		Size: 110.5 KB (110499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:265ae8d237ddc109ffe7e544e93a0dc1cea5bfe3fa5685fca792afda6d67ed0f`  
		Last Modified: Tue, 05 Apr 2022 04:19:29 GMT  
		Size: 928.4 KB (928406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce17e42e65242140f2a8f7c6d0a16bf4f1b64b0ba276ed8341905ed6f63e4a7b`  
		Last Modified: Tue, 05 Apr 2022 04:19:28 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30070b7f5a7be9b35fb6b8c7f1b6cb0de4508d927cc49caf12b3f6e220b0cc60`  
		Last Modified: Tue, 05 Apr 2022 04:19:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.15-alpine` - linux; 386

```console
$ docker pull memcached@sha256:5378334a3366058f6987024a1963dceafda46b182d6236b4685f816238f99992
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3888728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be3d8aa97e2099f400479214a98c34c3a23c21939afde5c6611961b33539a8bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:25 GMT
ADD file:7d51a0f8691eb78c9062fd31984423a93d276a67b4ed5d1a706e1c2cd9fea23a in / 
# Mon, 04 Apr 2022 23:38:25 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:52:17 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 05 Apr 2022 03:52:18 GMT
RUN apk add --no-cache libsasl
# Tue, 05 Apr 2022 03:52:19 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 05 Apr 2022 03:52:20 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 05 Apr 2022 03:55:15 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 05 Apr 2022 03:55:17 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 05 Apr 2022 03:55:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 05 Apr 2022 03:55:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 03:55:19 GMT
USER memcache
# Tue, 05 Apr 2022 03:55:20 GMT
EXPOSE 11211
# Tue, 05 Apr 2022 03:55:21 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:73b28a5955ec7fb46f2cf0434e4901a889f7dda3f8c9ec496300feb256c7eda8`  
		Last Modified: Mon, 04 Apr 2022 19:10:03 GMT  
		Size: 2.8 MB (2818974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06cddc8f8c3aabebd92d18ccbc0c9181ed94cc4b15b5adbda9e2bfdf4b8f38e9`  
		Last Modified: Tue, 05 Apr 2022 03:56:08 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad8594347186db0e9366f74b1e03bd14ed234378b2d1238a6b56504a86608fa6`  
		Last Modified: Tue, 05 Apr 2022 03:56:08 GMT  
		Size: 120.9 KB (120869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d7907ab18015191139b22c9b7b25c6a23d1c569470a49f2eb3e1ef985c4450`  
		Last Modified: Tue, 05 Apr 2022 03:56:08 GMT  
		Size: 947.2 KB (947242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3d6dff2eb04a8a959a2e8d101ca3da2646db4b2125b02fd6505c61ce53215b`  
		Last Modified: Tue, 05 Apr 2022 03:56:08 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:845b50269336006037a46780211bf0b2b95df971864d348d10c893aa2bf3afe3`  
		Last Modified: Tue, 05 Apr 2022 03:56:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.15-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:d1110704ee41f1dce802400ce09904c39aff25c66c1e1b87c64781b0bd9527d4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3905105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1827e9495120e553b560bd77e162a97bfdb923a96c36b2dea8afd967fdc57bd1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:30 GMT
ADD file:960cf6f9d3d1cfcb36c2d67dd4c3eaba7db1d0c7afe97968512248d7f234ad47 in / 
# Tue, 05 Apr 2022 00:23:32 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 10:09:23 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 05 Apr 2022 10:09:31 GMT
RUN apk add --no-cache libsasl
# Tue, 05 Apr 2022 10:09:35 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 05 Apr 2022 10:09:41 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 05 Apr 2022 10:12:56 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 05 Apr 2022 10:12:58 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 05 Apr 2022 10:13:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 05 Apr 2022 10:13:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 10:13:10 GMT
USER memcache
# Tue, 05 Apr 2022 10:13:12 GMT
EXPOSE 11211
# Tue, 05 Apr 2022 10:13:14 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1877acf2d48ed8bcb5bd9756a95aca0c077457be7cf4fcef25807f4e9be88db1`  
		Last Modified: Mon, 04 Apr 2022 19:09:49 GMT  
		Size: 2.8 MB (2811186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8124818eb8eba84f8929c5e21fa177a0224a632a260382b31fd9ea53de0cb63`  
		Last Modified: Tue, 05 Apr 2022 10:14:09 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65727b8884a0072f667d76a190572aecbef43ea2013aa1fab131f8ad94cf6027`  
		Last Modified: Tue, 05 Apr 2022 10:14:09 GMT  
		Size: 126.2 KB (126153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fdd85c6abf5a16922e7e67ae0f58814880550c8e561aa25fe98f824c65e283f`  
		Last Modified: Tue, 05 Apr 2022 10:14:09 GMT  
		Size: 966.1 KB (966088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72641c2cb945038b7f950ba927f9377d909670cd2c8a2f99f0027cfe6f34d41f`  
		Last Modified: Tue, 05 Apr 2022 10:14:09 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27047ea6a5173f1f7f40a46c10833cfbf360f9ac71f5595dd2b745afc3f9f3bb`  
		Last Modified: Tue, 05 Apr 2022 10:14:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.15-alpine` - linux; s390x

```console
$ docker pull memcached@sha256:f4d6b61f33632664a2176b827e6f04dc9b43bece1e1225f1c27d3f218fcaf90c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3650153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d81b27c0ae4d75825efc6c14a9b31769a43cebc314ab07e25b9024fe3b7d6bf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:18:54 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 05 Apr 2022 11:18:55 GMT
RUN apk add --no-cache libsasl
# Tue, 05 Apr 2022 11:18:55 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 05 Apr 2022 11:18:55 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 05 Apr 2022 11:22:16 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 05 Apr 2022 11:22:16 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 05 Apr 2022 11:22:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 05 Apr 2022 11:22:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 11:22:17 GMT
USER memcache
# Tue, 05 Apr 2022 11:22:17 GMT
EXPOSE 11211
# Tue, 05 Apr 2022 11:22:17 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d92848f08937ad9e3c8df84e91a6ae677af747e7ae736062bf8303e6f98a5a`  
		Last Modified: Tue, 05 Apr 2022 11:23:08 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee4699d5d9185c820000eb9490520b6c45f7c7df9e07c67d79ec6efac05ff170`  
		Last Modified: Tue, 05 Apr 2022 11:23:08 GMT  
		Size: 113.5 KB (113464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c834b41bef6837d1312846d4839e66a0070dd934cb4388ff09a93112f6cdc0`  
		Last Modified: Tue, 05 Apr 2022 11:23:09 GMT  
		Size: 934.6 KB (934639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd760c99b09ff84bd3f703d93a143abd83f2ecfc7c941856bdd4222a4da2b7a`  
		Last Modified: Tue, 05 Apr 2022 11:23:08 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b4795384f4f0fbaa99dd9e3683dfd3639ccbcd001144f0b8d1f050c3a765283`  
		Last Modified: Tue, 05 Apr 2022 11:23:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.15-alpine3.15`

```console
$ docker pull memcached@sha256:06bc630f006be575ae4e8a55e515a66daba0ed432f0e46ecfacf654daf4f07e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1.6.15-alpine3.15` - linux; amd64

```console
$ docker pull memcached@sha256:fbb3eda59b2f6851b1335f6fd43fa5a371ac197b06f84c0363341b7cd1c066f1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3864898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bcea36e93e267587df645dc2c39d08513419e129eb5b28db4a204207d64a9ea6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 09:54:14 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 05 Apr 2022 09:54:15 GMT
RUN apk add --no-cache libsasl
# Tue, 05 Apr 2022 09:54:15 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 05 Apr 2022 09:54:15 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 05 Apr 2022 09:57:57 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 05 Apr 2022 09:57:57 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 05 Apr 2022 09:57:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 05 Apr 2022 09:57:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 09:57:58 GMT
USER memcache
# Tue, 05 Apr 2022 09:57:58 GMT
EXPOSE 11211
# Tue, 05 Apr 2022 09:57:58 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c437462196847904d5021a85f817fecbb0b84eca04e4677f3a907f95125ebd3`  
		Last Modified: Tue, 05 Apr 2022 09:58:27 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37749f62d258e02c4f026b7ed0cb874d23b47abaa2c5860e41b3c099fdeb1d15`  
		Last Modified: Tue, 05 Apr 2022 09:58:27 GMT  
		Size: 109.2 KB (109172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf6c1e9f5167a143f222aea98c5b9c1d58ad0f9eed19d753fa1c4ffdfdd0269`  
		Last Modified: Tue, 05 Apr 2022 09:58:27 GMT  
		Size: 939.5 KB (939497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550e19164877083e509bb0c014a831674a7b77ddcf111d980a4f2b1bd1a78171`  
		Last Modified: Tue, 05 Apr 2022 09:58:27 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:515f37e9ad844fe3fdd82c3504b1c092e11e2c8f5f8395bc8944c96c768f3d3c`  
		Last Modified: Tue, 05 Apr 2022 09:58:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.15-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:d38012edd86b9a7abab01b390d4bbce8c39201ebedfd0066fcff6b6fb20cf178
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3757025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e0f3d4ef24801f58b76d5d0e24224de96c6e02fba4eccb3fa2e037e94403f0a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:15:56 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 05 Apr 2022 04:15:57 GMT
RUN apk add --no-cache libsasl
# Tue, 05 Apr 2022 04:15:58 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 05 Apr 2022 04:15:59 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 05 Apr 2022 04:18:36 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 05 Apr 2022 04:18:37 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 05 Apr 2022 04:18:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 05 Apr 2022 04:18:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 04:18:39 GMT
USER memcache
# Tue, 05 Apr 2022 04:18:40 GMT
EXPOSE 11211
# Tue, 05 Apr 2022 04:18:41 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa012cdcd391bd8cd78796fe53eb96b7585962832b802667f44cedd88405d0cc`  
		Last Modified: Tue, 05 Apr 2022 04:19:28 GMT  
		Size: 1.2 KB (1238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca8ad568702372595d83e4a4b906e000230b00315e1fd6ef6d219697badb387`  
		Last Modified: Tue, 05 Apr 2022 04:19:28 GMT  
		Size: 110.5 KB (110499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:265ae8d237ddc109ffe7e544e93a0dc1cea5bfe3fa5685fca792afda6d67ed0f`  
		Last Modified: Tue, 05 Apr 2022 04:19:29 GMT  
		Size: 928.4 KB (928406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce17e42e65242140f2a8f7c6d0a16bf4f1b64b0ba276ed8341905ed6f63e4a7b`  
		Last Modified: Tue, 05 Apr 2022 04:19:28 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30070b7f5a7be9b35fb6b8c7f1b6cb0de4508d927cc49caf12b3f6e220b0cc60`  
		Last Modified: Tue, 05 Apr 2022 04:19:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.15-alpine3.15` - linux; 386

```console
$ docker pull memcached@sha256:5378334a3366058f6987024a1963dceafda46b182d6236b4685f816238f99992
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3888728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be3d8aa97e2099f400479214a98c34c3a23c21939afde5c6611961b33539a8bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:25 GMT
ADD file:7d51a0f8691eb78c9062fd31984423a93d276a67b4ed5d1a706e1c2cd9fea23a in / 
# Mon, 04 Apr 2022 23:38:25 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:52:17 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 05 Apr 2022 03:52:18 GMT
RUN apk add --no-cache libsasl
# Tue, 05 Apr 2022 03:52:19 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 05 Apr 2022 03:52:20 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 05 Apr 2022 03:55:15 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 05 Apr 2022 03:55:17 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 05 Apr 2022 03:55:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 05 Apr 2022 03:55:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 03:55:19 GMT
USER memcache
# Tue, 05 Apr 2022 03:55:20 GMT
EXPOSE 11211
# Tue, 05 Apr 2022 03:55:21 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:73b28a5955ec7fb46f2cf0434e4901a889f7dda3f8c9ec496300feb256c7eda8`  
		Last Modified: Mon, 04 Apr 2022 19:10:03 GMT  
		Size: 2.8 MB (2818974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06cddc8f8c3aabebd92d18ccbc0c9181ed94cc4b15b5adbda9e2bfdf4b8f38e9`  
		Last Modified: Tue, 05 Apr 2022 03:56:08 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad8594347186db0e9366f74b1e03bd14ed234378b2d1238a6b56504a86608fa6`  
		Last Modified: Tue, 05 Apr 2022 03:56:08 GMT  
		Size: 120.9 KB (120869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d7907ab18015191139b22c9b7b25c6a23d1c569470a49f2eb3e1ef985c4450`  
		Last Modified: Tue, 05 Apr 2022 03:56:08 GMT  
		Size: 947.2 KB (947242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3d6dff2eb04a8a959a2e8d101ca3da2646db4b2125b02fd6505c61ce53215b`  
		Last Modified: Tue, 05 Apr 2022 03:56:08 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:845b50269336006037a46780211bf0b2b95df971864d348d10c893aa2bf3afe3`  
		Last Modified: Tue, 05 Apr 2022 03:56:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.15-alpine3.15` - linux; ppc64le

```console
$ docker pull memcached@sha256:d1110704ee41f1dce802400ce09904c39aff25c66c1e1b87c64781b0bd9527d4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3905105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1827e9495120e553b560bd77e162a97bfdb923a96c36b2dea8afd967fdc57bd1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:30 GMT
ADD file:960cf6f9d3d1cfcb36c2d67dd4c3eaba7db1d0c7afe97968512248d7f234ad47 in / 
# Tue, 05 Apr 2022 00:23:32 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 10:09:23 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 05 Apr 2022 10:09:31 GMT
RUN apk add --no-cache libsasl
# Tue, 05 Apr 2022 10:09:35 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 05 Apr 2022 10:09:41 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 05 Apr 2022 10:12:56 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 05 Apr 2022 10:12:58 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 05 Apr 2022 10:13:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 05 Apr 2022 10:13:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 10:13:10 GMT
USER memcache
# Tue, 05 Apr 2022 10:13:12 GMT
EXPOSE 11211
# Tue, 05 Apr 2022 10:13:14 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1877acf2d48ed8bcb5bd9756a95aca0c077457be7cf4fcef25807f4e9be88db1`  
		Last Modified: Mon, 04 Apr 2022 19:09:49 GMT  
		Size: 2.8 MB (2811186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8124818eb8eba84f8929c5e21fa177a0224a632a260382b31fd9ea53de0cb63`  
		Last Modified: Tue, 05 Apr 2022 10:14:09 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65727b8884a0072f667d76a190572aecbef43ea2013aa1fab131f8ad94cf6027`  
		Last Modified: Tue, 05 Apr 2022 10:14:09 GMT  
		Size: 126.2 KB (126153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fdd85c6abf5a16922e7e67ae0f58814880550c8e561aa25fe98f824c65e283f`  
		Last Modified: Tue, 05 Apr 2022 10:14:09 GMT  
		Size: 966.1 KB (966088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72641c2cb945038b7f950ba927f9377d909670cd2c8a2f99f0027cfe6f34d41f`  
		Last Modified: Tue, 05 Apr 2022 10:14:09 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27047ea6a5173f1f7f40a46c10833cfbf360f9ac71f5595dd2b745afc3f9f3bb`  
		Last Modified: Tue, 05 Apr 2022 10:14:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.15-alpine3.15` - linux; s390x

```console
$ docker pull memcached@sha256:f4d6b61f33632664a2176b827e6f04dc9b43bece1e1225f1c27d3f218fcaf90c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3650153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d81b27c0ae4d75825efc6c14a9b31769a43cebc314ab07e25b9024fe3b7d6bf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:18:54 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 05 Apr 2022 11:18:55 GMT
RUN apk add --no-cache libsasl
# Tue, 05 Apr 2022 11:18:55 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 05 Apr 2022 11:18:55 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 05 Apr 2022 11:22:16 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 05 Apr 2022 11:22:16 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 05 Apr 2022 11:22:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 05 Apr 2022 11:22:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 11:22:17 GMT
USER memcache
# Tue, 05 Apr 2022 11:22:17 GMT
EXPOSE 11211
# Tue, 05 Apr 2022 11:22:17 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d92848f08937ad9e3c8df84e91a6ae677af747e7ae736062bf8303e6f98a5a`  
		Last Modified: Tue, 05 Apr 2022 11:23:08 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee4699d5d9185c820000eb9490520b6c45f7c7df9e07c67d79ec6efac05ff170`  
		Last Modified: Tue, 05 Apr 2022 11:23:08 GMT  
		Size: 113.5 KB (113464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c834b41bef6837d1312846d4839e66a0070dd934cb4388ff09a93112f6cdc0`  
		Last Modified: Tue, 05 Apr 2022 11:23:09 GMT  
		Size: 934.6 KB (934639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd760c99b09ff84bd3f703d93a143abd83f2ecfc7c941856bdd4222a4da2b7a`  
		Last Modified: Tue, 05 Apr 2022 11:23:08 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b4795384f4f0fbaa99dd9e3683dfd3639ccbcd001144f0b8d1f050c3a765283`  
		Last Modified: Tue, 05 Apr 2022 11:23:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.15-bullseye`

```console
$ docker pull memcached@sha256:05917d8f91b97eff3ffb98497dd139c65f61c2107649cf73db6cced7e7667b94
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

### `memcached:1.6.15-bullseye` - linux; amd64

```console
$ docker pull memcached@sha256:58a41bfdd7492d7d9be5ea8ab1abeffa106a2193e98e6646be91d06ad37d0675
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32968652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:065555a745051537085b4135608198e45686d4574eda4d7093537d1107a1feff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 11 May 2022 01:20:16 GMT
ADD file:4a0bb88956083aa56032fdd9601d9b66c39b18c896ba35ea33594cd75621640a in / 
# Wed, 11 May 2022 01:20:16 GMT
CMD ["bash"]
# Wed, 11 May 2022 04:44:00 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 11 May 2022 04:44:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 04:44:03 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 11 May 2022 04:44:03 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 11 May 2022 04:46:42 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 May 2022 04:46:42 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 May 2022 04:46:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 04:46:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 04:46:43 GMT
USER memcache
# Wed, 11 May 2022 04:46:43 GMT
EXPOSE 11211
# Wed, 11 May 2022 04:46:43 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:214ca5fb90323fe769c63a12af092f2572bf1c6b300263e09883909fc865d260`  
		Last Modified: Wed, 11 May 2022 01:25:13 GMT  
		Size: 31.4 MB (31379476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae8d4b1feabc5879929064e635eb9f14ef5b8a15bac772048359ca7ff051d1c`  
		Last Modified: Wed, 11 May 2022 04:47:13 GMT  
		Size: 5.0 KB (4975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dc491b9af677c0a71fa36fcbf2faea8087acafa69e2d760fcaea4f26fb5eb2a`  
		Last Modified: Wed, 11 May 2022 04:47:14 GMT  
		Size: 328.1 KB (328091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c355a147dff081cfbbf9d104870e2195eb0213138ae88d87a585b466fc521d4a`  
		Last Modified: Wed, 11 May 2022 04:47:14 GMT  
		Size: 1.3 MB (1255702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0cc0d566fb2a731f9d4dd270354fe902ec4b175b95e3552e17d53a76601b28d`  
		Last Modified: Wed, 11 May 2022 04:47:13 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d5c91075c8421465ad8ef2fe32f6daab4ff01b837e03aee3568d39c64cb2d3`  
		Last Modified: Wed, 11 May 2022 04:47:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.15-bullseye` - linux; arm variant v5

```console
$ docker pull memcached@sha256:7114dc5aaa1603875d79f65e4d27cf83fd5c6ff279092e5019313c2e676e8563
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30469996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:711c043049190c6786a1fe335232c7bee5a0c58134e9481f385ae99e18cff3a2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 11 May 2022 00:50:34 GMT
ADD file:72357b75d7e4546f06abf4648ab600980e742a3017f36da3c7a6c086f2f5fb56 in / 
# Wed, 11 May 2022 00:50:35 GMT
CMD ["bash"]
# Wed, 11 May 2022 19:59:38 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 11 May 2022 19:59:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 19:59:48 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 11 May 2022 19:59:49 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 11 May 2022 20:04:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 May 2022 20:04:12 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 May 2022 20:04:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 20:04:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 20:04:14 GMT
USER memcache
# Wed, 11 May 2022 20:04:15 GMT
EXPOSE 11211
# Wed, 11 May 2022 20:04:15 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f7b69be15db1cb94a249f74b27edd4f5e5923a8701b026179a593f6888e897aa`  
		Last Modified: Wed, 11 May 2022 01:05:51 GMT  
		Size: 28.9 MB (28921122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e23defdefe7366c4546b3284b11bdbedcf73c55c4cad0c49a2e12b6bc971f653`  
		Last Modified: Wed, 11 May 2022 20:05:07 GMT  
		Size: 4.9 KB (4893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aed101d7cb94db52f647e3cf585d3a7702b5a01cb3f7c3fc86aedcd94fb5b01`  
		Last Modified: Wed, 11 May 2022 20:05:07 GMT  
		Size: 316.6 KB (316610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80e354b9ae9a23ca02681ddaca03fe3a6fa45069b80a683e38123aa3a0174fab`  
		Last Modified: Wed, 11 May 2022 20:05:08 GMT  
		Size: 1.2 MB (1226962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d82b2d2d5ab7db68fddbbf26596ed21c9c4506e0355be942188f9a81557bdd`  
		Last Modified: Wed, 11 May 2022 20:05:07 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd35d60f098711fce5b4a2d107b57cfe22a70cbb6bf47476c42ea4d975b6c3f7`  
		Last Modified: Wed, 11 May 2022 20:05:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.15-bullseye` - linux; arm variant v7

```console
$ docker pull memcached@sha256:34dee5b2772158236707bc1811db77d4adc27d86ca6b1b096fb444a8cfef133e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28091607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad29267829b7cd5d6051ca12869e51112bded24fc2e06656b673942a215f1c84`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 20 Apr 2022 13:27:18 GMT
ADD file:1a0e290eb32b3533f9d1684c683ad866b5003579790b25ad61b2044dc6c20bbb in / 
# Wed, 20 Apr 2022 13:27:18 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 21:47:36 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 20 Apr 2022 21:47:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 21:47:45 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 20 Apr 2022 21:47:45 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 20 Apr 2022 21:51:42 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 20 Apr 2022 21:51:42 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 20 Apr 2022 21:51:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 20 Apr 2022 21:51:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Apr 2022 21:51:45 GMT
USER memcache
# Wed, 20 Apr 2022 21:51:45 GMT
EXPOSE 11211
# Wed, 20 Apr 2022 21:51:46 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a6b2963233cd14b47391f0e25f2a485bbeabb87e771a71b73e5cde7c013963da`  
		Last Modified: Wed, 20 Apr 2022 13:43:41 GMT  
		Size: 26.6 MB (26575758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4b149950ca557655b7e9b7229a81d7d772f2aad316a5ce7de452664795a377`  
		Last Modified: Wed, 20 Apr 2022 22:04:23 GMT  
		Size: 4.9 KB (4893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d14f3b12cc24aac4e3614237409e18959637d8420b534524bc1fe63e7456a660`  
		Last Modified: Wed, 20 Apr 2022 22:04:23 GMT  
		Size: 312.1 KB (312059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca5c1518bd4380c5c22f884d402b699c75cb53de72de7d5b2a53e99d8ba56d9e`  
		Last Modified: Wed, 20 Apr 2022 22:04:24 GMT  
		Size: 1.2 MB (1198488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd1a54f20b40e9c7302a4ab0c46cc590140bde81aba4ab1d149dd8b2b3edade`  
		Last Modified: Wed, 20 Apr 2022 22:04:23 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6e66d52d7551a05a10e5a70971eef4ad0803f499c934fd1ec734a144e5bc64`  
		Last Modified: Wed, 20 Apr 2022 22:04:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.15-bullseye` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:6c452eece1271128806922efd79c0ef0f809e6705d855d6a271f5208d2a2117d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31444857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d45eed3b8e469acc08e97e874bb1e8b4f004720606f20212dad652f79ca29db4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 11 May 2022 00:46:59 GMT
ADD file:158a0e401328bd7c0d49b9e8539186098967218f1b1a8c811f4398d29b74397f in / 
# Wed, 11 May 2022 00:47:00 GMT
CMD ["bash"]
# Wed, 11 May 2022 02:27:34 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 11 May 2022 02:27:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:27:38 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 11 May 2022 02:27:39 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 11 May 2022 02:30:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 May 2022 02:30:13 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 May 2022 02:30:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 02:30:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 02:30:15 GMT
USER memcache
# Wed, 11 May 2022 02:30:16 GMT
EXPOSE 11211
# Wed, 11 May 2022 02:30:17 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:dfdd5ffb257742b891ccad9400a77dad2a6260b2451e0f5e48a9ade1d17a87ec`  
		Last Modified: Wed, 11 May 2022 00:53:46 GMT  
		Size: 30.1 MB (30065693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:921e9eec57430f29a509862965b1bc0f909703c8c5e73b2345205cbd6b715910`  
		Last Modified: Wed, 11 May 2022 02:31:07 GMT  
		Size: 4.9 KB (4900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:984aa2c2269106d51c47bed797929d496825d1dee8883d84918fd98cd809ba76`  
		Last Modified: Wed, 11 May 2022 02:31:07 GMT  
		Size: 119.2 KB (119215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b52324e4c1cc245d2131fae3776a0359730099f17e8039fa1db0d0b6310a195`  
		Last Modified: Wed, 11 May 2022 02:31:08 GMT  
		Size: 1.3 MB (1254642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70bc38e444a829155cb5ad8ca3f2b8cc68a6065e19b795707656cec98edadbfc`  
		Last Modified: Wed, 11 May 2022 02:31:07 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b29514622ffb8a37130cc9662034040cbc8ff1d5c7b8ce620f49c0d26b24b73`  
		Last Modified: Wed, 11 May 2022 02:31:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.15-bullseye` - linux; 386

```console
$ docker pull memcached@sha256:faedc990d98e8f3b6058c1e3f9ace6816b59338aaf906a8099a0b1141713d345
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33778000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74fb9295e5de207e5aade7877e8b45371b49a320bf3eafbfe65ea15c6f70dd59`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 11 May 2022 01:39:14 GMT
ADD file:9eecb0fd311177f9d226e914c411aef49b5de1930e73019d2ee24afed515b5a2 in / 
# Wed, 11 May 2022 01:39:14 GMT
CMD ["bash"]
# Wed, 11 May 2022 04:32:45 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 11 May 2022 04:32:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 04:32:49 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 11 May 2022 04:32:50 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 11 May 2022 04:35:41 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 May 2022 04:35:43 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 May 2022 04:35:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 04:35:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 04:35:45 GMT
USER memcache
# Wed, 11 May 2022 04:35:46 GMT
EXPOSE 11211
# Wed, 11 May 2022 04:35:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:91c5bdbe4bf9f1970dd54ba71e2523649adce4e5240c2ff8a87711bf389ecba3`  
		Last Modified: Wed, 11 May 2022 01:46:25 GMT  
		Size: 32.4 MB (32389776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cbc080a4e6972a45023b1c0d8d9f74e9df257677ec7503a9f8756eabb61b5e0`  
		Last Modified: Wed, 11 May 2022 04:36:36 GMT  
		Size: 4.8 KB (4771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdfcc6e2f39957ee91e94aa2f1264a35ccef2b3aed8ae29d859144d763ed06ab`  
		Last Modified: Wed, 11 May 2022 04:36:36 GMT  
		Size: 130.1 KB (130140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a68472399b32a22e31b1b551482a4fec929210d4db3da6b3010fdb3a97bf0944`  
		Last Modified: Wed, 11 May 2022 04:36:37 GMT  
		Size: 1.3 MB (1252905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a1040db24a5a1a06568a3d81752b73f002172ebec23d3ace2181c365e6216c9`  
		Last Modified: Wed, 11 May 2022 04:36:36 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496cfb26b818ba873c9dbd7203c2551d9c1503db7a8281c82b03ecd7987dfe44`  
		Last Modified: Wed, 11 May 2022 04:36:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.15-bullseye` - linux; mips64le

```console
$ docker pull memcached@sha256:d4d70ee02bd6a268e51e7cb45ae2ab6028a3f5546e3566abea4839b7bc0b2795
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31014729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5edfa57d6aec6089194206346467a5708554650f75a703542020f03dda6cfb13`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 11 May 2022 02:23:35 GMT
ADD file:d47dce2adbc9352ef1d437730bab3b579dd8d2bf29dd60cd8a8b65396b39e36e in / 
# Wed, 11 May 2022 02:23:40 GMT
CMD ["bash"]
# Wed, 11 May 2022 04:26:13 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 11 May 2022 04:26:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 04:26:33 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 11 May 2022 04:26:36 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 11 May 2022 04:33:31 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 May 2022 04:33:33 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 May 2022 04:33:38 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 04:33:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 04:33:43 GMT
USER memcache
# Wed, 11 May 2022 04:33:45 GMT
EXPOSE 11211
# Wed, 11 May 2022 04:33:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:438a36bf0b6e75ff6f0fbb2b7669dfb86361416f4d808912d30cf5b91ad2eea9`  
		Last Modified: Wed, 11 May 2022 02:33:43 GMT  
		Size: 29.6 MB (29641051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2947248cd8e754e130fecb9083b0ad0025e50361a44987eadfb6edfeb2e3908c`  
		Last Modified: Wed, 11 May 2022 04:34:05 GMT  
		Size: 4.9 KB (4861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3849c71c1ab16dd8196e74fd37ae70b3a0b89a3b07a9cb7f76535725af27a86a`  
		Last Modified: Wed, 11 May 2022 04:34:05 GMT  
		Size: 117.2 KB (117156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f24b722d80efb82b9982c69a407116125ad8a340447344e252517f9798849b9`  
		Last Modified: Wed, 11 May 2022 04:34:06 GMT  
		Size: 1.3 MB (1251254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f4827b1598450f78ff6da5317e269d8fdc544d21ff25409586a2db03053022`  
		Last Modified: Wed, 11 May 2022 04:34:05 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:090d97f72bbcf506ab0dc4d8e19c3a1522513237327ced2e711f0613fb262865`  
		Last Modified: Wed, 11 May 2022 04:34:05 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.15-bullseye` - linux; ppc64le

```console
$ docker pull memcached@sha256:673643121e94f08dd12197b69994ec2cad834c15326b37ba83861eb00aa22134
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36971800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:821c76dba347fd635474ef0126da0d404cc404e989635b028d0da3c2dfb273b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 11 May 2022 01:32:29 GMT
ADD file:1e94716789ec21981460f74be38a668bc212bd804c1d41cecf90036a5bccac5a in / 
# Wed, 11 May 2022 01:32:34 GMT
CMD ["bash"]
# Wed, 11 May 2022 07:51:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 11 May 2022 07:51:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 07:51:40 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 11 May 2022 07:51:48 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 11 May 2022 07:57:31 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 May 2022 07:57:33 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 May 2022 07:57:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 07:57:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 07:57:49 GMT
USER memcache
# Wed, 11 May 2022 07:57:55 GMT
EXPOSE 11211
# Wed, 11 May 2022 07:58:00 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2533109ed11eefd6415e0370d6d7a3ea879b582b1887c98b819a598ad18fca24`  
		Last Modified: Wed, 11 May 2022 01:43:03 GMT  
		Size: 35.3 MB (35286467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:103a6713e9bf2853760692eb30b886453378b61e3fb83321c0ce1fec39bdf2f2`  
		Last Modified: Wed, 11 May 2022 07:59:13 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9173dced38a5c576a66100ed6df59833b82ee6847ed29531d690b7377a72e02d`  
		Last Modified: Wed, 11 May 2022 07:59:13 GMT  
		Size: 356.9 KB (356938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e15378aab9e7b0eefd835da5eeee5fe567c111dcf6df814b34f6755cf27c45`  
		Last Modified: Wed, 11 May 2022 07:59:13 GMT  
		Size: 1.3 MB (1323008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523888230dfa0221ad182120061be4802ac72d7a19047277ffc452c5003537b5`  
		Last Modified: Wed, 11 May 2022 07:59:13 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12893f041469d0edbc3132e6af823296c231a18db48dc29c665658f6ba859c9f`  
		Last Modified: Wed, 11 May 2022 07:59:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.15-bullseye` - linux; s390x

```console
$ docker pull memcached@sha256:d0221a850100573af43f6113f62398369ddaa506aef1fd1e114da8fdd4403330
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31225739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37e72a40047bd848bbedd03871f17d8132f625301f2203038b265841fa1a660f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 11 May 2022 00:44:17 GMT
ADD file:d93a1cf64a813d01774cd628dfd683c006e20159e2ab3464c2159c8d9897c725 in / 
# Wed, 11 May 2022 00:44:19 GMT
CMD ["bash"]
# Wed, 11 May 2022 02:35:31 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 11 May 2022 02:35:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:35:34 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 11 May 2022 02:35:34 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 11 May 2022 02:39:02 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 May 2022 02:39:03 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 May 2022 02:39:03 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 02:39:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 02:39:03 GMT
USER memcache
# Wed, 11 May 2022 02:39:03 GMT
EXPOSE 11211
# Wed, 11 May 2022 02:39:04 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9f3750f6094217808e26d471752341db88153c8d5b5f9bb11577b74671303bbc`  
		Last Modified: Wed, 11 May 2022 00:50:03 GMT  
		Size: 29.7 MB (29654739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29541285df59f95a596b1911b49171e64e2361189a163533e77dbf2961b8f685`  
		Last Modified: Wed, 11 May 2022 02:40:04 GMT  
		Size: 5.0 KB (5026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c94a32e11bca5f817bc7015ceff49279fcd263d523198a38cc02607b7899e261`  
		Last Modified: Wed, 11 May 2022 02:40:04 GMT  
		Size: 324.2 KB (324197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57395e3cd66c2852ddaac636856f0245c1cfdca358d6bb75128950b9d9042481`  
		Last Modified: Wed, 11 May 2022 02:40:04 GMT  
		Size: 1.2 MB (1241369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ed03e37cb4ad7ab6dfc00b4938e9e5ec27777eb89fe1918ffc45a5a8de10c0`  
		Last Modified: Wed, 11 May 2022 02:40:04 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79cc46e5a2551dd05d1dcb476692b2a5d1c7e5181f253ad3938c179835018b95`  
		Last Modified: Wed, 11 May 2022 02:40:03 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:alpine`

```console
$ docker pull memcached@sha256:0374a1e43929f2da9d7acf6887903eb3337ea92f0b8fd080aec28d2b902065aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `memcached:alpine` - linux; amd64

```console
$ docker pull memcached@sha256:fbb3eda59b2f6851b1335f6fd43fa5a371ac197b06f84c0363341b7cd1c066f1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3864898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bcea36e93e267587df645dc2c39d08513419e129eb5b28db4a204207d64a9ea6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 09:54:14 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 05 Apr 2022 09:54:15 GMT
RUN apk add --no-cache libsasl
# Tue, 05 Apr 2022 09:54:15 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 05 Apr 2022 09:54:15 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 05 Apr 2022 09:57:57 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 05 Apr 2022 09:57:57 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 05 Apr 2022 09:57:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 05 Apr 2022 09:57:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 09:57:58 GMT
USER memcache
# Tue, 05 Apr 2022 09:57:58 GMT
EXPOSE 11211
# Tue, 05 Apr 2022 09:57:58 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c437462196847904d5021a85f817fecbb0b84eca04e4677f3a907f95125ebd3`  
		Last Modified: Tue, 05 Apr 2022 09:58:27 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37749f62d258e02c4f026b7ed0cb874d23b47abaa2c5860e41b3c099fdeb1d15`  
		Last Modified: Tue, 05 Apr 2022 09:58:27 GMT  
		Size: 109.2 KB (109172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf6c1e9f5167a143f222aea98c5b9c1d58ad0f9eed19d753fa1c4ffdfdd0269`  
		Last Modified: Tue, 05 Apr 2022 09:58:27 GMT  
		Size: 939.5 KB (939497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550e19164877083e509bb0c014a831674a7b77ddcf111d980a4f2b1bd1a78171`  
		Last Modified: Tue, 05 Apr 2022 09:58:27 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:515f37e9ad844fe3fdd82c3504b1c092e11e2c8f5f8395bc8944c96c768f3d3c`  
		Last Modified: Tue, 05 Apr 2022 09:58:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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
$ docker pull memcached@sha256:d38012edd86b9a7abab01b390d4bbce8c39201ebedfd0066fcff6b6fb20cf178
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3757025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e0f3d4ef24801f58b76d5d0e24224de96c6e02fba4eccb3fa2e037e94403f0a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:15:56 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 05 Apr 2022 04:15:57 GMT
RUN apk add --no-cache libsasl
# Tue, 05 Apr 2022 04:15:58 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 05 Apr 2022 04:15:59 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 05 Apr 2022 04:18:36 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 05 Apr 2022 04:18:37 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 05 Apr 2022 04:18:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 05 Apr 2022 04:18:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 04:18:39 GMT
USER memcache
# Tue, 05 Apr 2022 04:18:40 GMT
EXPOSE 11211
# Tue, 05 Apr 2022 04:18:41 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa012cdcd391bd8cd78796fe53eb96b7585962832b802667f44cedd88405d0cc`  
		Last Modified: Tue, 05 Apr 2022 04:19:28 GMT  
		Size: 1.2 KB (1238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca8ad568702372595d83e4a4b906e000230b00315e1fd6ef6d219697badb387`  
		Last Modified: Tue, 05 Apr 2022 04:19:28 GMT  
		Size: 110.5 KB (110499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:265ae8d237ddc109ffe7e544e93a0dc1cea5bfe3fa5685fca792afda6d67ed0f`  
		Last Modified: Tue, 05 Apr 2022 04:19:29 GMT  
		Size: 928.4 KB (928406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce17e42e65242140f2a8f7c6d0a16bf4f1b64b0ba276ed8341905ed6f63e4a7b`  
		Last Modified: Tue, 05 Apr 2022 04:19:28 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30070b7f5a7be9b35fb6b8c7f1b6cb0de4508d927cc49caf12b3f6e220b0cc60`  
		Last Modified: Tue, 05 Apr 2022 04:19:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; 386

```console
$ docker pull memcached@sha256:5378334a3366058f6987024a1963dceafda46b182d6236b4685f816238f99992
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3888728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be3d8aa97e2099f400479214a98c34c3a23c21939afde5c6611961b33539a8bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:25 GMT
ADD file:7d51a0f8691eb78c9062fd31984423a93d276a67b4ed5d1a706e1c2cd9fea23a in / 
# Mon, 04 Apr 2022 23:38:25 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:52:17 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 05 Apr 2022 03:52:18 GMT
RUN apk add --no-cache libsasl
# Tue, 05 Apr 2022 03:52:19 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 05 Apr 2022 03:52:20 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 05 Apr 2022 03:55:15 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 05 Apr 2022 03:55:17 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 05 Apr 2022 03:55:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 05 Apr 2022 03:55:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 03:55:19 GMT
USER memcache
# Tue, 05 Apr 2022 03:55:20 GMT
EXPOSE 11211
# Tue, 05 Apr 2022 03:55:21 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:73b28a5955ec7fb46f2cf0434e4901a889f7dda3f8c9ec496300feb256c7eda8`  
		Last Modified: Mon, 04 Apr 2022 19:10:03 GMT  
		Size: 2.8 MB (2818974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06cddc8f8c3aabebd92d18ccbc0c9181ed94cc4b15b5adbda9e2bfdf4b8f38e9`  
		Last Modified: Tue, 05 Apr 2022 03:56:08 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad8594347186db0e9366f74b1e03bd14ed234378b2d1238a6b56504a86608fa6`  
		Last Modified: Tue, 05 Apr 2022 03:56:08 GMT  
		Size: 120.9 KB (120869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d7907ab18015191139b22c9b7b25c6a23d1c569470a49f2eb3e1ef985c4450`  
		Last Modified: Tue, 05 Apr 2022 03:56:08 GMT  
		Size: 947.2 KB (947242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3d6dff2eb04a8a959a2e8d101ca3da2646db4b2125b02fd6505c61ce53215b`  
		Last Modified: Tue, 05 Apr 2022 03:56:08 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:845b50269336006037a46780211bf0b2b95df971864d348d10c893aa2bf3afe3`  
		Last Modified: Tue, 05 Apr 2022 03:56:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:d1110704ee41f1dce802400ce09904c39aff25c66c1e1b87c64781b0bd9527d4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3905105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1827e9495120e553b560bd77e162a97bfdb923a96c36b2dea8afd967fdc57bd1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:30 GMT
ADD file:960cf6f9d3d1cfcb36c2d67dd4c3eaba7db1d0c7afe97968512248d7f234ad47 in / 
# Tue, 05 Apr 2022 00:23:32 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 10:09:23 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 05 Apr 2022 10:09:31 GMT
RUN apk add --no-cache libsasl
# Tue, 05 Apr 2022 10:09:35 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 05 Apr 2022 10:09:41 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 05 Apr 2022 10:12:56 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 05 Apr 2022 10:12:58 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 05 Apr 2022 10:13:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 05 Apr 2022 10:13:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 10:13:10 GMT
USER memcache
# Tue, 05 Apr 2022 10:13:12 GMT
EXPOSE 11211
# Tue, 05 Apr 2022 10:13:14 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1877acf2d48ed8bcb5bd9756a95aca0c077457be7cf4fcef25807f4e9be88db1`  
		Last Modified: Mon, 04 Apr 2022 19:09:49 GMT  
		Size: 2.8 MB (2811186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8124818eb8eba84f8929c5e21fa177a0224a632a260382b31fd9ea53de0cb63`  
		Last Modified: Tue, 05 Apr 2022 10:14:09 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65727b8884a0072f667d76a190572aecbef43ea2013aa1fab131f8ad94cf6027`  
		Last Modified: Tue, 05 Apr 2022 10:14:09 GMT  
		Size: 126.2 KB (126153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fdd85c6abf5a16922e7e67ae0f58814880550c8e561aa25fe98f824c65e283f`  
		Last Modified: Tue, 05 Apr 2022 10:14:09 GMT  
		Size: 966.1 KB (966088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72641c2cb945038b7f950ba927f9377d909670cd2c8a2f99f0027cfe6f34d41f`  
		Last Modified: Tue, 05 Apr 2022 10:14:09 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27047ea6a5173f1f7f40a46c10833cfbf360f9ac71f5595dd2b745afc3f9f3bb`  
		Last Modified: Tue, 05 Apr 2022 10:14:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; s390x

```console
$ docker pull memcached@sha256:f4d6b61f33632664a2176b827e6f04dc9b43bece1e1225f1c27d3f218fcaf90c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3650153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d81b27c0ae4d75825efc6c14a9b31769a43cebc314ab07e25b9024fe3b7d6bf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:18:54 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 05 Apr 2022 11:18:55 GMT
RUN apk add --no-cache libsasl
# Tue, 05 Apr 2022 11:18:55 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 05 Apr 2022 11:18:55 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 05 Apr 2022 11:22:16 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 05 Apr 2022 11:22:16 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 05 Apr 2022 11:22:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 05 Apr 2022 11:22:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 11:22:17 GMT
USER memcache
# Tue, 05 Apr 2022 11:22:17 GMT
EXPOSE 11211
# Tue, 05 Apr 2022 11:22:17 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d92848f08937ad9e3c8df84e91a6ae677af747e7ae736062bf8303e6f98a5a`  
		Last Modified: Tue, 05 Apr 2022 11:23:08 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee4699d5d9185c820000eb9490520b6c45f7c7df9e07c67d79ec6efac05ff170`  
		Last Modified: Tue, 05 Apr 2022 11:23:08 GMT  
		Size: 113.5 KB (113464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c834b41bef6837d1312846d4839e66a0070dd934cb4388ff09a93112f6cdc0`  
		Last Modified: Tue, 05 Apr 2022 11:23:09 GMT  
		Size: 934.6 KB (934639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd760c99b09ff84bd3f703d93a143abd83f2ecfc7c941856bdd4222a4da2b7a`  
		Last Modified: Tue, 05 Apr 2022 11:23:08 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b4795384f4f0fbaa99dd9e3683dfd3639ccbcd001144f0b8d1f050c3a765283`  
		Last Modified: Tue, 05 Apr 2022 11:23:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:alpine3.15`

```console
$ docker pull memcached@sha256:06bc630f006be575ae4e8a55e515a66daba0ed432f0e46ecfacf654daf4f07e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `memcached:alpine3.15` - linux; amd64

```console
$ docker pull memcached@sha256:fbb3eda59b2f6851b1335f6fd43fa5a371ac197b06f84c0363341b7cd1c066f1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3864898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bcea36e93e267587df645dc2c39d08513419e129eb5b28db4a204207d64a9ea6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 09:54:14 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 05 Apr 2022 09:54:15 GMT
RUN apk add --no-cache libsasl
# Tue, 05 Apr 2022 09:54:15 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 05 Apr 2022 09:54:15 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 05 Apr 2022 09:57:57 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 05 Apr 2022 09:57:57 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 05 Apr 2022 09:57:58 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 05 Apr 2022 09:57:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 09:57:58 GMT
USER memcache
# Tue, 05 Apr 2022 09:57:58 GMT
EXPOSE 11211
# Tue, 05 Apr 2022 09:57:58 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c437462196847904d5021a85f817fecbb0b84eca04e4677f3a907f95125ebd3`  
		Last Modified: Tue, 05 Apr 2022 09:58:27 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37749f62d258e02c4f026b7ed0cb874d23b47abaa2c5860e41b3c099fdeb1d15`  
		Last Modified: Tue, 05 Apr 2022 09:58:27 GMT  
		Size: 109.2 KB (109172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf6c1e9f5167a143f222aea98c5b9c1d58ad0f9eed19d753fa1c4ffdfdd0269`  
		Last Modified: Tue, 05 Apr 2022 09:58:27 GMT  
		Size: 939.5 KB (939497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550e19164877083e509bb0c014a831674a7b77ddcf111d980a4f2b1bd1a78171`  
		Last Modified: Tue, 05 Apr 2022 09:58:27 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:515f37e9ad844fe3fdd82c3504b1c092e11e2c8f5f8395bc8944c96c768f3d3c`  
		Last Modified: Tue, 05 Apr 2022 09:58:27 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine3.15` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:d38012edd86b9a7abab01b390d4bbce8c39201ebedfd0066fcff6b6fb20cf178
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3757025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e0f3d4ef24801f58b76d5d0e24224de96c6e02fba4eccb3fa2e037e94403f0a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:15:56 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 05 Apr 2022 04:15:57 GMT
RUN apk add --no-cache libsasl
# Tue, 05 Apr 2022 04:15:58 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 05 Apr 2022 04:15:59 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 05 Apr 2022 04:18:36 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 05 Apr 2022 04:18:37 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 05 Apr 2022 04:18:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 05 Apr 2022 04:18:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 04:18:39 GMT
USER memcache
# Tue, 05 Apr 2022 04:18:40 GMT
EXPOSE 11211
# Tue, 05 Apr 2022 04:18:41 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa012cdcd391bd8cd78796fe53eb96b7585962832b802667f44cedd88405d0cc`  
		Last Modified: Tue, 05 Apr 2022 04:19:28 GMT  
		Size: 1.2 KB (1238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca8ad568702372595d83e4a4b906e000230b00315e1fd6ef6d219697badb387`  
		Last Modified: Tue, 05 Apr 2022 04:19:28 GMT  
		Size: 110.5 KB (110499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:265ae8d237ddc109ffe7e544e93a0dc1cea5bfe3fa5685fca792afda6d67ed0f`  
		Last Modified: Tue, 05 Apr 2022 04:19:29 GMT  
		Size: 928.4 KB (928406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce17e42e65242140f2a8f7c6d0a16bf4f1b64b0ba276ed8341905ed6f63e4a7b`  
		Last Modified: Tue, 05 Apr 2022 04:19:28 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30070b7f5a7be9b35fb6b8c7f1b6cb0de4508d927cc49caf12b3f6e220b0cc60`  
		Last Modified: Tue, 05 Apr 2022 04:19:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine3.15` - linux; 386

```console
$ docker pull memcached@sha256:5378334a3366058f6987024a1963dceafda46b182d6236b4685f816238f99992
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3888728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be3d8aa97e2099f400479214a98c34c3a23c21939afde5c6611961b33539a8bc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:25 GMT
ADD file:7d51a0f8691eb78c9062fd31984423a93d276a67b4ed5d1a706e1c2cd9fea23a in / 
# Mon, 04 Apr 2022 23:38:25 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:52:17 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 05 Apr 2022 03:52:18 GMT
RUN apk add --no-cache libsasl
# Tue, 05 Apr 2022 03:52:19 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 05 Apr 2022 03:52:20 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 05 Apr 2022 03:55:15 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 05 Apr 2022 03:55:17 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 05 Apr 2022 03:55:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 05 Apr 2022 03:55:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 03:55:19 GMT
USER memcache
# Tue, 05 Apr 2022 03:55:20 GMT
EXPOSE 11211
# Tue, 05 Apr 2022 03:55:21 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:73b28a5955ec7fb46f2cf0434e4901a889f7dda3f8c9ec496300feb256c7eda8`  
		Last Modified: Mon, 04 Apr 2022 19:10:03 GMT  
		Size: 2.8 MB (2818974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06cddc8f8c3aabebd92d18ccbc0c9181ed94cc4b15b5adbda9e2bfdf4b8f38e9`  
		Last Modified: Tue, 05 Apr 2022 03:56:08 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad8594347186db0e9366f74b1e03bd14ed234378b2d1238a6b56504a86608fa6`  
		Last Modified: Tue, 05 Apr 2022 03:56:08 GMT  
		Size: 120.9 KB (120869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d7907ab18015191139b22c9b7b25c6a23d1c569470a49f2eb3e1ef985c4450`  
		Last Modified: Tue, 05 Apr 2022 03:56:08 GMT  
		Size: 947.2 KB (947242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3d6dff2eb04a8a959a2e8d101ca3da2646db4b2125b02fd6505c61ce53215b`  
		Last Modified: Tue, 05 Apr 2022 03:56:08 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:845b50269336006037a46780211bf0b2b95df971864d348d10c893aa2bf3afe3`  
		Last Modified: Tue, 05 Apr 2022 03:56:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine3.15` - linux; ppc64le

```console
$ docker pull memcached@sha256:d1110704ee41f1dce802400ce09904c39aff25c66c1e1b87c64781b0bd9527d4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3905105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1827e9495120e553b560bd77e162a97bfdb923a96c36b2dea8afd967fdc57bd1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:30 GMT
ADD file:960cf6f9d3d1cfcb36c2d67dd4c3eaba7db1d0c7afe97968512248d7f234ad47 in / 
# Tue, 05 Apr 2022 00:23:32 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 10:09:23 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 05 Apr 2022 10:09:31 GMT
RUN apk add --no-cache libsasl
# Tue, 05 Apr 2022 10:09:35 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 05 Apr 2022 10:09:41 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 05 Apr 2022 10:12:56 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 05 Apr 2022 10:12:58 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 05 Apr 2022 10:13:06 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 05 Apr 2022 10:13:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 10:13:10 GMT
USER memcache
# Tue, 05 Apr 2022 10:13:12 GMT
EXPOSE 11211
# Tue, 05 Apr 2022 10:13:14 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1877acf2d48ed8bcb5bd9756a95aca0c077457be7cf4fcef25807f4e9be88db1`  
		Last Modified: Mon, 04 Apr 2022 19:09:49 GMT  
		Size: 2.8 MB (2811186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8124818eb8eba84f8929c5e21fa177a0224a632a260382b31fd9ea53de0cb63`  
		Last Modified: Tue, 05 Apr 2022 10:14:09 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65727b8884a0072f667d76a190572aecbef43ea2013aa1fab131f8ad94cf6027`  
		Last Modified: Tue, 05 Apr 2022 10:14:09 GMT  
		Size: 126.2 KB (126153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fdd85c6abf5a16922e7e67ae0f58814880550c8e561aa25fe98f824c65e283f`  
		Last Modified: Tue, 05 Apr 2022 10:14:09 GMT  
		Size: 966.1 KB (966088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72641c2cb945038b7f950ba927f9377d909670cd2c8a2f99f0027cfe6f34d41f`  
		Last Modified: Tue, 05 Apr 2022 10:14:09 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27047ea6a5173f1f7f40a46c10833cfbf360f9ac71f5595dd2b745afc3f9f3bb`  
		Last Modified: Tue, 05 Apr 2022 10:14:09 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine3.15` - linux; s390x

```console
$ docker pull memcached@sha256:f4d6b61f33632664a2176b827e6f04dc9b43bece1e1225f1c27d3f218fcaf90c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.7 MB (3650153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d81b27c0ae4d75825efc6c14a9b31769a43cebc314ab07e25b9024fe3b7d6bf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:18:54 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 05 Apr 2022 11:18:55 GMT
RUN apk add --no-cache libsasl
# Tue, 05 Apr 2022 11:18:55 GMT
ENV MEMCACHED_VERSION=1.6.15
# Tue, 05 Apr 2022 11:18:55 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Tue, 05 Apr 2022 11:22:16 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 05 Apr 2022 11:22:16 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 05 Apr 2022 11:22:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 05 Apr 2022 11:22:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Apr 2022 11:22:17 GMT
USER memcache
# Tue, 05 Apr 2022 11:22:17 GMT
EXPOSE 11211
# Tue, 05 Apr 2022 11:22:17 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d92848f08937ad9e3c8df84e91a6ae677af747e7ae736062bf8303e6f98a5a`  
		Last Modified: Tue, 05 Apr 2022 11:23:08 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee4699d5d9185c820000eb9490520b6c45f7c7df9e07c67d79ec6efac05ff170`  
		Last Modified: Tue, 05 Apr 2022 11:23:08 GMT  
		Size: 113.5 KB (113464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c834b41bef6837d1312846d4839e66a0070dd934cb4388ff09a93112f6cdc0`  
		Last Modified: Tue, 05 Apr 2022 11:23:09 GMT  
		Size: 934.6 KB (934639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd760c99b09ff84bd3f703d93a143abd83f2ecfc7c941856bdd4222a4da2b7a`  
		Last Modified: Tue, 05 Apr 2022 11:23:08 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b4795384f4f0fbaa99dd9e3683dfd3639ccbcd001144f0b8d1f050c3a765283`  
		Last Modified: Tue, 05 Apr 2022 11:23:08 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:bullseye`

```console
$ docker pull memcached@sha256:05917d8f91b97eff3ffb98497dd139c65f61c2107649cf73db6cced7e7667b94
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

### `memcached:bullseye` - linux; amd64

```console
$ docker pull memcached@sha256:58a41bfdd7492d7d9be5ea8ab1abeffa106a2193e98e6646be91d06ad37d0675
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32968652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:065555a745051537085b4135608198e45686d4574eda4d7093537d1107a1feff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 11 May 2022 01:20:16 GMT
ADD file:4a0bb88956083aa56032fdd9601d9b66c39b18c896ba35ea33594cd75621640a in / 
# Wed, 11 May 2022 01:20:16 GMT
CMD ["bash"]
# Wed, 11 May 2022 04:44:00 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 11 May 2022 04:44:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 04:44:03 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 11 May 2022 04:44:03 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 11 May 2022 04:46:42 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 May 2022 04:46:42 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 May 2022 04:46:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 04:46:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 04:46:43 GMT
USER memcache
# Wed, 11 May 2022 04:46:43 GMT
EXPOSE 11211
# Wed, 11 May 2022 04:46:43 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:214ca5fb90323fe769c63a12af092f2572bf1c6b300263e09883909fc865d260`  
		Last Modified: Wed, 11 May 2022 01:25:13 GMT  
		Size: 31.4 MB (31379476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae8d4b1feabc5879929064e635eb9f14ef5b8a15bac772048359ca7ff051d1c`  
		Last Modified: Wed, 11 May 2022 04:47:13 GMT  
		Size: 5.0 KB (4975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dc491b9af677c0a71fa36fcbf2faea8087acafa69e2d760fcaea4f26fb5eb2a`  
		Last Modified: Wed, 11 May 2022 04:47:14 GMT  
		Size: 328.1 KB (328091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c355a147dff081cfbbf9d104870e2195eb0213138ae88d87a585b466fc521d4a`  
		Last Modified: Wed, 11 May 2022 04:47:14 GMT  
		Size: 1.3 MB (1255702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0cc0d566fb2a731f9d4dd270354fe902ec4b175b95e3552e17d53a76601b28d`  
		Last Modified: Wed, 11 May 2022 04:47:13 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d5c91075c8421465ad8ef2fe32f6daab4ff01b837e03aee3568d39c64cb2d3`  
		Last Modified: Wed, 11 May 2022 04:47:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; arm variant v5

```console
$ docker pull memcached@sha256:7114dc5aaa1603875d79f65e4d27cf83fd5c6ff279092e5019313c2e676e8563
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30469996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:711c043049190c6786a1fe335232c7bee5a0c58134e9481f385ae99e18cff3a2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 11 May 2022 00:50:34 GMT
ADD file:72357b75d7e4546f06abf4648ab600980e742a3017f36da3c7a6c086f2f5fb56 in / 
# Wed, 11 May 2022 00:50:35 GMT
CMD ["bash"]
# Wed, 11 May 2022 19:59:38 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 11 May 2022 19:59:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 19:59:48 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 11 May 2022 19:59:49 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 11 May 2022 20:04:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 May 2022 20:04:12 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 May 2022 20:04:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 20:04:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 20:04:14 GMT
USER memcache
# Wed, 11 May 2022 20:04:15 GMT
EXPOSE 11211
# Wed, 11 May 2022 20:04:15 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f7b69be15db1cb94a249f74b27edd4f5e5923a8701b026179a593f6888e897aa`  
		Last Modified: Wed, 11 May 2022 01:05:51 GMT  
		Size: 28.9 MB (28921122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e23defdefe7366c4546b3284b11bdbedcf73c55c4cad0c49a2e12b6bc971f653`  
		Last Modified: Wed, 11 May 2022 20:05:07 GMT  
		Size: 4.9 KB (4893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aed101d7cb94db52f647e3cf585d3a7702b5a01cb3f7c3fc86aedcd94fb5b01`  
		Last Modified: Wed, 11 May 2022 20:05:07 GMT  
		Size: 316.6 KB (316610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80e354b9ae9a23ca02681ddaca03fe3a6fa45069b80a683e38123aa3a0174fab`  
		Last Modified: Wed, 11 May 2022 20:05:08 GMT  
		Size: 1.2 MB (1226962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d82b2d2d5ab7db68fddbbf26596ed21c9c4506e0355be942188f9a81557bdd`  
		Last Modified: Wed, 11 May 2022 20:05:07 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd35d60f098711fce5b4a2d107b57cfe22a70cbb6bf47476c42ea4d975b6c3f7`  
		Last Modified: Wed, 11 May 2022 20:05:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; arm variant v7

```console
$ docker pull memcached@sha256:34dee5b2772158236707bc1811db77d4adc27d86ca6b1b096fb444a8cfef133e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28091607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad29267829b7cd5d6051ca12869e51112bded24fc2e06656b673942a215f1c84`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 20 Apr 2022 13:27:18 GMT
ADD file:1a0e290eb32b3533f9d1684c683ad866b5003579790b25ad61b2044dc6c20bbb in / 
# Wed, 20 Apr 2022 13:27:18 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 21:47:36 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 20 Apr 2022 21:47:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 21:47:45 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 20 Apr 2022 21:47:45 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 20 Apr 2022 21:51:42 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 20 Apr 2022 21:51:42 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 20 Apr 2022 21:51:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 20 Apr 2022 21:51:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Apr 2022 21:51:45 GMT
USER memcache
# Wed, 20 Apr 2022 21:51:45 GMT
EXPOSE 11211
# Wed, 20 Apr 2022 21:51:46 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a6b2963233cd14b47391f0e25f2a485bbeabb87e771a71b73e5cde7c013963da`  
		Last Modified: Wed, 20 Apr 2022 13:43:41 GMT  
		Size: 26.6 MB (26575758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4b149950ca557655b7e9b7229a81d7d772f2aad316a5ce7de452664795a377`  
		Last Modified: Wed, 20 Apr 2022 22:04:23 GMT  
		Size: 4.9 KB (4893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d14f3b12cc24aac4e3614237409e18959637d8420b534524bc1fe63e7456a660`  
		Last Modified: Wed, 20 Apr 2022 22:04:23 GMT  
		Size: 312.1 KB (312059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca5c1518bd4380c5c22f884d402b699c75cb53de72de7d5b2a53e99d8ba56d9e`  
		Last Modified: Wed, 20 Apr 2022 22:04:24 GMT  
		Size: 1.2 MB (1198488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd1a54f20b40e9c7302a4ab0c46cc590140bde81aba4ab1d149dd8b2b3edade`  
		Last Modified: Wed, 20 Apr 2022 22:04:23 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6e66d52d7551a05a10e5a70971eef4ad0803f499c934fd1ec734a144e5bc64`  
		Last Modified: Wed, 20 Apr 2022 22:04:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:6c452eece1271128806922efd79c0ef0f809e6705d855d6a271f5208d2a2117d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31444857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d45eed3b8e469acc08e97e874bb1e8b4f004720606f20212dad652f79ca29db4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 11 May 2022 00:46:59 GMT
ADD file:158a0e401328bd7c0d49b9e8539186098967218f1b1a8c811f4398d29b74397f in / 
# Wed, 11 May 2022 00:47:00 GMT
CMD ["bash"]
# Wed, 11 May 2022 02:27:34 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 11 May 2022 02:27:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:27:38 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 11 May 2022 02:27:39 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 11 May 2022 02:30:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 May 2022 02:30:13 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 May 2022 02:30:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 02:30:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 02:30:15 GMT
USER memcache
# Wed, 11 May 2022 02:30:16 GMT
EXPOSE 11211
# Wed, 11 May 2022 02:30:17 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:dfdd5ffb257742b891ccad9400a77dad2a6260b2451e0f5e48a9ade1d17a87ec`  
		Last Modified: Wed, 11 May 2022 00:53:46 GMT  
		Size: 30.1 MB (30065693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:921e9eec57430f29a509862965b1bc0f909703c8c5e73b2345205cbd6b715910`  
		Last Modified: Wed, 11 May 2022 02:31:07 GMT  
		Size: 4.9 KB (4900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:984aa2c2269106d51c47bed797929d496825d1dee8883d84918fd98cd809ba76`  
		Last Modified: Wed, 11 May 2022 02:31:07 GMT  
		Size: 119.2 KB (119215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b52324e4c1cc245d2131fae3776a0359730099f17e8039fa1db0d0b6310a195`  
		Last Modified: Wed, 11 May 2022 02:31:08 GMT  
		Size: 1.3 MB (1254642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70bc38e444a829155cb5ad8ca3f2b8cc68a6065e19b795707656cec98edadbfc`  
		Last Modified: Wed, 11 May 2022 02:31:07 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b29514622ffb8a37130cc9662034040cbc8ff1d5c7b8ce620f49c0d26b24b73`  
		Last Modified: Wed, 11 May 2022 02:31:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; 386

```console
$ docker pull memcached@sha256:faedc990d98e8f3b6058c1e3f9ace6816b59338aaf906a8099a0b1141713d345
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33778000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74fb9295e5de207e5aade7877e8b45371b49a320bf3eafbfe65ea15c6f70dd59`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 11 May 2022 01:39:14 GMT
ADD file:9eecb0fd311177f9d226e914c411aef49b5de1930e73019d2ee24afed515b5a2 in / 
# Wed, 11 May 2022 01:39:14 GMT
CMD ["bash"]
# Wed, 11 May 2022 04:32:45 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 11 May 2022 04:32:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 04:32:49 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 11 May 2022 04:32:50 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 11 May 2022 04:35:41 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 May 2022 04:35:43 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 May 2022 04:35:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 04:35:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 04:35:45 GMT
USER memcache
# Wed, 11 May 2022 04:35:46 GMT
EXPOSE 11211
# Wed, 11 May 2022 04:35:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:91c5bdbe4bf9f1970dd54ba71e2523649adce4e5240c2ff8a87711bf389ecba3`  
		Last Modified: Wed, 11 May 2022 01:46:25 GMT  
		Size: 32.4 MB (32389776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cbc080a4e6972a45023b1c0d8d9f74e9df257677ec7503a9f8756eabb61b5e0`  
		Last Modified: Wed, 11 May 2022 04:36:36 GMT  
		Size: 4.8 KB (4771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdfcc6e2f39957ee91e94aa2f1264a35ccef2b3aed8ae29d859144d763ed06ab`  
		Last Modified: Wed, 11 May 2022 04:36:36 GMT  
		Size: 130.1 KB (130140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a68472399b32a22e31b1b551482a4fec929210d4db3da6b3010fdb3a97bf0944`  
		Last Modified: Wed, 11 May 2022 04:36:37 GMT  
		Size: 1.3 MB (1252905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a1040db24a5a1a06568a3d81752b73f002172ebec23d3ace2181c365e6216c9`  
		Last Modified: Wed, 11 May 2022 04:36:36 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496cfb26b818ba873c9dbd7203c2551d9c1503db7a8281c82b03ecd7987dfe44`  
		Last Modified: Wed, 11 May 2022 04:36:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; mips64le

```console
$ docker pull memcached@sha256:d4d70ee02bd6a268e51e7cb45ae2ab6028a3f5546e3566abea4839b7bc0b2795
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31014729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5edfa57d6aec6089194206346467a5708554650f75a703542020f03dda6cfb13`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 11 May 2022 02:23:35 GMT
ADD file:d47dce2adbc9352ef1d437730bab3b579dd8d2bf29dd60cd8a8b65396b39e36e in / 
# Wed, 11 May 2022 02:23:40 GMT
CMD ["bash"]
# Wed, 11 May 2022 04:26:13 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 11 May 2022 04:26:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 04:26:33 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 11 May 2022 04:26:36 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 11 May 2022 04:33:31 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 May 2022 04:33:33 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 May 2022 04:33:38 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 04:33:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 04:33:43 GMT
USER memcache
# Wed, 11 May 2022 04:33:45 GMT
EXPOSE 11211
# Wed, 11 May 2022 04:33:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:438a36bf0b6e75ff6f0fbb2b7669dfb86361416f4d808912d30cf5b91ad2eea9`  
		Last Modified: Wed, 11 May 2022 02:33:43 GMT  
		Size: 29.6 MB (29641051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2947248cd8e754e130fecb9083b0ad0025e50361a44987eadfb6edfeb2e3908c`  
		Last Modified: Wed, 11 May 2022 04:34:05 GMT  
		Size: 4.9 KB (4861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3849c71c1ab16dd8196e74fd37ae70b3a0b89a3b07a9cb7f76535725af27a86a`  
		Last Modified: Wed, 11 May 2022 04:34:05 GMT  
		Size: 117.2 KB (117156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f24b722d80efb82b9982c69a407116125ad8a340447344e252517f9798849b9`  
		Last Modified: Wed, 11 May 2022 04:34:06 GMT  
		Size: 1.3 MB (1251254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f4827b1598450f78ff6da5317e269d8fdc544d21ff25409586a2db03053022`  
		Last Modified: Wed, 11 May 2022 04:34:05 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:090d97f72bbcf506ab0dc4d8e19c3a1522513237327ced2e711f0613fb262865`  
		Last Modified: Wed, 11 May 2022 04:34:05 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; ppc64le

```console
$ docker pull memcached@sha256:673643121e94f08dd12197b69994ec2cad834c15326b37ba83861eb00aa22134
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36971800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:821c76dba347fd635474ef0126da0d404cc404e989635b028d0da3c2dfb273b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 11 May 2022 01:32:29 GMT
ADD file:1e94716789ec21981460f74be38a668bc212bd804c1d41cecf90036a5bccac5a in / 
# Wed, 11 May 2022 01:32:34 GMT
CMD ["bash"]
# Wed, 11 May 2022 07:51:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 11 May 2022 07:51:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 07:51:40 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 11 May 2022 07:51:48 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 11 May 2022 07:57:31 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 May 2022 07:57:33 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 May 2022 07:57:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 07:57:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 07:57:49 GMT
USER memcache
# Wed, 11 May 2022 07:57:55 GMT
EXPOSE 11211
# Wed, 11 May 2022 07:58:00 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2533109ed11eefd6415e0370d6d7a3ea879b582b1887c98b819a598ad18fca24`  
		Last Modified: Wed, 11 May 2022 01:43:03 GMT  
		Size: 35.3 MB (35286467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:103a6713e9bf2853760692eb30b886453378b61e3fb83321c0ce1fec39bdf2f2`  
		Last Modified: Wed, 11 May 2022 07:59:13 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9173dced38a5c576a66100ed6df59833b82ee6847ed29531d690b7377a72e02d`  
		Last Modified: Wed, 11 May 2022 07:59:13 GMT  
		Size: 356.9 KB (356938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e15378aab9e7b0eefd835da5eeee5fe567c111dcf6df814b34f6755cf27c45`  
		Last Modified: Wed, 11 May 2022 07:59:13 GMT  
		Size: 1.3 MB (1323008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523888230dfa0221ad182120061be4802ac72d7a19047277ffc452c5003537b5`  
		Last Modified: Wed, 11 May 2022 07:59:13 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12893f041469d0edbc3132e6af823296c231a18db48dc29c665658f6ba859c9f`  
		Last Modified: Wed, 11 May 2022 07:59:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; s390x

```console
$ docker pull memcached@sha256:d0221a850100573af43f6113f62398369ddaa506aef1fd1e114da8fdd4403330
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31225739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37e72a40047bd848bbedd03871f17d8132f625301f2203038b265841fa1a660f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 11 May 2022 00:44:17 GMT
ADD file:d93a1cf64a813d01774cd628dfd683c006e20159e2ab3464c2159c8d9897c725 in / 
# Wed, 11 May 2022 00:44:19 GMT
CMD ["bash"]
# Wed, 11 May 2022 02:35:31 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 11 May 2022 02:35:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:35:34 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 11 May 2022 02:35:34 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 11 May 2022 02:39:02 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 May 2022 02:39:03 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 May 2022 02:39:03 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 02:39:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 02:39:03 GMT
USER memcache
# Wed, 11 May 2022 02:39:03 GMT
EXPOSE 11211
# Wed, 11 May 2022 02:39:04 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9f3750f6094217808e26d471752341db88153c8d5b5f9bb11577b74671303bbc`  
		Last Modified: Wed, 11 May 2022 00:50:03 GMT  
		Size: 29.7 MB (29654739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29541285df59f95a596b1911b49171e64e2361189a163533e77dbf2961b8f685`  
		Last Modified: Wed, 11 May 2022 02:40:04 GMT  
		Size: 5.0 KB (5026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c94a32e11bca5f817bc7015ceff49279fcd263d523198a38cc02607b7899e261`  
		Last Modified: Wed, 11 May 2022 02:40:04 GMT  
		Size: 324.2 KB (324197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57395e3cd66c2852ddaac636856f0245c1cfdca358d6bb75128950b9d9042481`  
		Last Modified: Wed, 11 May 2022 02:40:04 GMT  
		Size: 1.2 MB (1241369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ed03e37cb4ad7ab6dfc00b4938e9e5ec27777eb89fe1918ffc45a5a8de10c0`  
		Last Modified: Wed, 11 May 2022 02:40:04 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79cc46e5a2551dd05d1dcb476692b2a5d1c7e5181f253ad3938c179835018b95`  
		Last Modified: Wed, 11 May 2022 02:40:03 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:latest`

```console
$ docker pull memcached@sha256:05917d8f91b97eff3ffb98497dd139c65f61c2107649cf73db6cced7e7667b94
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

### `memcached:latest` - linux; amd64

```console
$ docker pull memcached@sha256:58a41bfdd7492d7d9be5ea8ab1abeffa106a2193e98e6646be91d06ad37d0675
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32968652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:065555a745051537085b4135608198e45686d4574eda4d7093537d1107a1feff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 11 May 2022 01:20:16 GMT
ADD file:4a0bb88956083aa56032fdd9601d9b66c39b18c896ba35ea33594cd75621640a in / 
# Wed, 11 May 2022 01:20:16 GMT
CMD ["bash"]
# Wed, 11 May 2022 04:44:00 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 11 May 2022 04:44:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 04:44:03 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 11 May 2022 04:44:03 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 11 May 2022 04:46:42 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 May 2022 04:46:42 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 May 2022 04:46:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 04:46:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 04:46:43 GMT
USER memcache
# Wed, 11 May 2022 04:46:43 GMT
EXPOSE 11211
# Wed, 11 May 2022 04:46:43 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:214ca5fb90323fe769c63a12af092f2572bf1c6b300263e09883909fc865d260`  
		Last Modified: Wed, 11 May 2022 01:25:13 GMT  
		Size: 31.4 MB (31379476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae8d4b1feabc5879929064e635eb9f14ef5b8a15bac772048359ca7ff051d1c`  
		Last Modified: Wed, 11 May 2022 04:47:13 GMT  
		Size: 5.0 KB (4975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dc491b9af677c0a71fa36fcbf2faea8087acafa69e2d760fcaea4f26fb5eb2a`  
		Last Modified: Wed, 11 May 2022 04:47:14 GMT  
		Size: 328.1 KB (328091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c355a147dff081cfbbf9d104870e2195eb0213138ae88d87a585b466fc521d4a`  
		Last Modified: Wed, 11 May 2022 04:47:14 GMT  
		Size: 1.3 MB (1255702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0cc0d566fb2a731f9d4dd270354fe902ec4b175b95e3552e17d53a76601b28d`  
		Last Modified: Wed, 11 May 2022 04:47:13 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d5c91075c8421465ad8ef2fe32f6daab4ff01b837e03aee3568d39c64cb2d3`  
		Last Modified: Wed, 11 May 2022 04:47:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm variant v5

```console
$ docker pull memcached@sha256:7114dc5aaa1603875d79f65e4d27cf83fd5c6ff279092e5019313c2e676e8563
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30469996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:711c043049190c6786a1fe335232c7bee5a0c58134e9481f385ae99e18cff3a2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 11 May 2022 00:50:34 GMT
ADD file:72357b75d7e4546f06abf4648ab600980e742a3017f36da3c7a6c086f2f5fb56 in / 
# Wed, 11 May 2022 00:50:35 GMT
CMD ["bash"]
# Wed, 11 May 2022 19:59:38 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 11 May 2022 19:59:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 19:59:48 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 11 May 2022 19:59:49 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 11 May 2022 20:04:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 May 2022 20:04:12 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 May 2022 20:04:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 20:04:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 20:04:14 GMT
USER memcache
# Wed, 11 May 2022 20:04:15 GMT
EXPOSE 11211
# Wed, 11 May 2022 20:04:15 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f7b69be15db1cb94a249f74b27edd4f5e5923a8701b026179a593f6888e897aa`  
		Last Modified: Wed, 11 May 2022 01:05:51 GMT  
		Size: 28.9 MB (28921122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e23defdefe7366c4546b3284b11bdbedcf73c55c4cad0c49a2e12b6bc971f653`  
		Last Modified: Wed, 11 May 2022 20:05:07 GMT  
		Size: 4.9 KB (4893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aed101d7cb94db52f647e3cf585d3a7702b5a01cb3f7c3fc86aedcd94fb5b01`  
		Last Modified: Wed, 11 May 2022 20:05:07 GMT  
		Size: 316.6 KB (316610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80e354b9ae9a23ca02681ddaca03fe3a6fa45069b80a683e38123aa3a0174fab`  
		Last Modified: Wed, 11 May 2022 20:05:08 GMT  
		Size: 1.2 MB (1226962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d82b2d2d5ab7db68fddbbf26596ed21c9c4506e0355be942188f9a81557bdd`  
		Last Modified: Wed, 11 May 2022 20:05:07 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd35d60f098711fce5b4a2d107b57cfe22a70cbb6bf47476c42ea4d975b6c3f7`  
		Last Modified: Wed, 11 May 2022 20:05:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm variant v7

```console
$ docker pull memcached@sha256:34dee5b2772158236707bc1811db77d4adc27d86ca6b1b096fb444a8cfef133e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28091607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad29267829b7cd5d6051ca12869e51112bded24fc2e06656b673942a215f1c84`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 20 Apr 2022 13:27:18 GMT
ADD file:1a0e290eb32b3533f9d1684c683ad866b5003579790b25ad61b2044dc6c20bbb in / 
# Wed, 20 Apr 2022 13:27:18 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 21:47:36 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 20 Apr 2022 21:47:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 21:47:45 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 20 Apr 2022 21:47:45 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 20 Apr 2022 21:51:42 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 20 Apr 2022 21:51:42 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 20 Apr 2022 21:51:44 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 20 Apr 2022 21:51:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Apr 2022 21:51:45 GMT
USER memcache
# Wed, 20 Apr 2022 21:51:45 GMT
EXPOSE 11211
# Wed, 20 Apr 2022 21:51:46 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a6b2963233cd14b47391f0e25f2a485bbeabb87e771a71b73e5cde7c013963da`  
		Last Modified: Wed, 20 Apr 2022 13:43:41 GMT  
		Size: 26.6 MB (26575758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4b149950ca557655b7e9b7229a81d7d772f2aad316a5ce7de452664795a377`  
		Last Modified: Wed, 20 Apr 2022 22:04:23 GMT  
		Size: 4.9 KB (4893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d14f3b12cc24aac4e3614237409e18959637d8420b534524bc1fe63e7456a660`  
		Last Modified: Wed, 20 Apr 2022 22:04:23 GMT  
		Size: 312.1 KB (312059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca5c1518bd4380c5c22f884d402b699c75cb53de72de7d5b2a53e99d8ba56d9e`  
		Last Modified: Wed, 20 Apr 2022 22:04:24 GMT  
		Size: 1.2 MB (1198488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd1a54f20b40e9c7302a4ab0c46cc590140bde81aba4ab1d149dd8b2b3edade`  
		Last Modified: Wed, 20 Apr 2022 22:04:23 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6e66d52d7551a05a10e5a70971eef4ad0803f499c934fd1ec734a144e5bc64`  
		Last Modified: Wed, 20 Apr 2022 22:04:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:6c452eece1271128806922efd79c0ef0f809e6705d855d6a271f5208d2a2117d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31444857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d45eed3b8e469acc08e97e874bb1e8b4f004720606f20212dad652f79ca29db4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 11 May 2022 00:46:59 GMT
ADD file:158a0e401328bd7c0d49b9e8539186098967218f1b1a8c811f4398d29b74397f in / 
# Wed, 11 May 2022 00:47:00 GMT
CMD ["bash"]
# Wed, 11 May 2022 02:27:34 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 11 May 2022 02:27:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:27:38 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 11 May 2022 02:27:39 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 11 May 2022 02:30:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 May 2022 02:30:13 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 May 2022 02:30:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 02:30:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 02:30:15 GMT
USER memcache
# Wed, 11 May 2022 02:30:16 GMT
EXPOSE 11211
# Wed, 11 May 2022 02:30:17 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:dfdd5ffb257742b891ccad9400a77dad2a6260b2451e0f5e48a9ade1d17a87ec`  
		Last Modified: Wed, 11 May 2022 00:53:46 GMT  
		Size: 30.1 MB (30065693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:921e9eec57430f29a509862965b1bc0f909703c8c5e73b2345205cbd6b715910`  
		Last Modified: Wed, 11 May 2022 02:31:07 GMT  
		Size: 4.9 KB (4900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:984aa2c2269106d51c47bed797929d496825d1dee8883d84918fd98cd809ba76`  
		Last Modified: Wed, 11 May 2022 02:31:07 GMT  
		Size: 119.2 KB (119215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b52324e4c1cc245d2131fae3776a0359730099f17e8039fa1db0d0b6310a195`  
		Last Modified: Wed, 11 May 2022 02:31:08 GMT  
		Size: 1.3 MB (1254642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70bc38e444a829155cb5ad8ca3f2b8cc68a6065e19b795707656cec98edadbfc`  
		Last Modified: Wed, 11 May 2022 02:31:07 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b29514622ffb8a37130cc9662034040cbc8ff1d5c7b8ce620f49c0d26b24b73`  
		Last Modified: Wed, 11 May 2022 02:31:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; 386

```console
$ docker pull memcached@sha256:faedc990d98e8f3b6058c1e3f9ace6816b59338aaf906a8099a0b1141713d345
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33778000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74fb9295e5de207e5aade7877e8b45371b49a320bf3eafbfe65ea15c6f70dd59`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 11 May 2022 01:39:14 GMT
ADD file:9eecb0fd311177f9d226e914c411aef49b5de1930e73019d2ee24afed515b5a2 in / 
# Wed, 11 May 2022 01:39:14 GMT
CMD ["bash"]
# Wed, 11 May 2022 04:32:45 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 11 May 2022 04:32:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 04:32:49 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 11 May 2022 04:32:50 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 11 May 2022 04:35:41 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 May 2022 04:35:43 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 May 2022 04:35:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 04:35:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 04:35:45 GMT
USER memcache
# Wed, 11 May 2022 04:35:46 GMT
EXPOSE 11211
# Wed, 11 May 2022 04:35:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:91c5bdbe4bf9f1970dd54ba71e2523649adce4e5240c2ff8a87711bf389ecba3`  
		Last Modified: Wed, 11 May 2022 01:46:25 GMT  
		Size: 32.4 MB (32389776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cbc080a4e6972a45023b1c0d8d9f74e9df257677ec7503a9f8756eabb61b5e0`  
		Last Modified: Wed, 11 May 2022 04:36:36 GMT  
		Size: 4.8 KB (4771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdfcc6e2f39957ee91e94aa2f1264a35ccef2b3aed8ae29d859144d763ed06ab`  
		Last Modified: Wed, 11 May 2022 04:36:36 GMT  
		Size: 130.1 KB (130140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a68472399b32a22e31b1b551482a4fec929210d4db3da6b3010fdb3a97bf0944`  
		Last Modified: Wed, 11 May 2022 04:36:37 GMT  
		Size: 1.3 MB (1252905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a1040db24a5a1a06568a3d81752b73f002172ebec23d3ace2181c365e6216c9`  
		Last Modified: Wed, 11 May 2022 04:36:36 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496cfb26b818ba873c9dbd7203c2551d9c1503db7a8281c82b03ecd7987dfe44`  
		Last Modified: Wed, 11 May 2022 04:36:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; mips64le

```console
$ docker pull memcached@sha256:d4d70ee02bd6a268e51e7cb45ae2ab6028a3f5546e3566abea4839b7bc0b2795
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31014729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5edfa57d6aec6089194206346467a5708554650f75a703542020f03dda6cfb13`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 11 May 2022 02:23:35 GMT
ADD file:d47dce2adbc9352ef1d437730bab3b579dd8d2bf29dd60cd8a8b65396b39e36e in / 
# Wed, 11 May 2022 02:23:40 GMT
CMD ["bash"]
# Wed, 11 May 2022 04:26:13 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 11 May 2022 04:26:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 04:26:33 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 11 May 2022 04:26:36 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 11 May 2022 04:33:31 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 May 2022 04:33:33 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 May 2022 04:33:38 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 04:33:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 04:33:43 GMT
USER memcache
# Wed, 11 May 2022 04:33:45 GMT
EXPOSE 11211
# Wed, 11 May 2022 04:33:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:438a36bf0b6e75ff6f0fbb2b7669dfb86361416f4d808912d30cf5b91ad2eea9`  
		Last Modified: Wed, 11 May 2022 02:33:43 GMT  
		Size: 29.6 MB (29641051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2947248cd8e754e130fecb9083b0ad0025e50361a44987eadfb6edfeb2e3908c`  
		Last Modified: Wed, 11 May 2022 04:34:05 GMT  
		Size: 4.9 KB (4861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3849c71c1ab16dd8196e74fd37ae70b3a0b89a3b07a9cb7f76535725af27a86a`  
		Last Modified: Wed, 11 May 2022 04:34:05 GMT  
		Size: 117.2 KB (117156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f24b722d80efb82b9982c69a407116125ad8a340447344e252517f9798849b9`  
		Last Modified: Wed, 11 May 2022 04:34:06 GMT  
		Size: 1.3 MB (1251254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f4827b1598450f78ff6da5317e269d8fdc544d21ff25409586a2db03053022`  
		Last Modified: Wed, 11 May 2022 04:34:05 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:090d97f72bbcf506ab0dc4d8e19c3a1522513237327ced2e711f0613fb262865`  
		Last Modified: Wed, 11 May 2022 04:34:05 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; ppc64le

```console
$ docker pull memcached@sha256:673643121e94f08dd12197b69994ec2cad834c15326b37ba83861eb00aa22134
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36971800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:821c76dba347fd635474ef0126da0d404cc404e989635b028d0da3c2dfb273b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 11 May 2022 01:32:29 GMT
ADD file:1e94716789ec21981460f74be38a668bc212bd804c1d41cecf90036a5bccac5a in / 
# Wed, 11 May 2022 01:32:34 GMT
CMD ["bash"]
# Wed, 11 May 2022 07:51:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 11 May 2022 07:51:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 07:51:40 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 11 May 2022 07:51:48 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 11 May 2022 07:57:31 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 May 2022 07:57:33 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 May 2022 07:57:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 07:57:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 07:57:49 GMT
USER memcache
# Wed, 11 May 2022 07:57:55 GMT
EXPOSE 11211
# Wed, 11 May 2022 07:58:00 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2533109ed11eefd6415e0370d6d7a3ea879b582b1887c98b819a598ad18fca24`  
		Last Modified: Wed, 11 May 2022 01:43:03 GMT  
		Size: 35.3 MB (35286467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:103a6713e9bf2853760692eb30b886453378b61e3fb83321c0ce1fec39bdf2f2`  
		Last Modified: Wed, 11 May 2022 07:59:13 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9173dced38a5c576a66100ed6df59833b82ee6847ed29531d690b7377a72e02d`  
		Last Modified: Wed, 11 May 2022 07:59:13 GMT  
		Size: 356.9 KB (356938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9e15378aab9e7b0eefd835da5eeee5fe567c111dcf6df814b34f6755cf27c45`  
		Last Modified: Wed, 11 May 2022 07:59:13 GMT  
		Size: 1.3 MB (1323008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523888230dfa0221ad182120061be4802ac72d7a19047277ffc452c5003537b5`  
		Last Modified: Wed, 11 May 2022 07:59:13 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12893f041469d0edbc3132e6af823296c231a18db48dc29c665658f6ba859c9f`  
		Last Modified: Wed, 11 May 2022 07:59:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; s390x

```console
$ docker pull memcached@sha256:d0221a850100573af43f6113f62398369ddaa506aef1fd1e114da8fdd4403330
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31225739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37e72a40047bd848bbedd03871f17d8132f625301f2203038b265841fa1a660f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 11 May 2022 00:44:17 GMT
ADD file:d93a1cf64a813d01774cd628dfd683c006e20159e2ab3464c2159c8d9897c725 in / 
# Wed, 11 May 2022 00:44:19 GMT
CMD ["bash"]
# Wed, 11 May 2022 02:35:31 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 11 May 2022 02:35:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:35:34 GMT
ENV MEMCACHED_VERSION=1.6.15
# Wed, 11 May 2022 02:35:34 GMT
ENV MEMCACHED_SHA1=badcfa0d65f5797cc9c2f957f3fbfedbd8c13411
# Wed, 11 May 2022 02:39:02 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 11 May 2022 02:39:03 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 11 May 2022 02:39:03 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 11 May 2022 02:39:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 02:39:03 GMT
USER memcache
# Wed, 11 May 2022 02:39:03 GMT
EXPOSE 11211
# Wed, 11 May 2022 02:39:04 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9f3750f6094217808e26d471752341db88153c8d5b5f9bb11577b74671303bbc`  
		Last Modified: Wed, 11 May 2022 00:50:03 GMT  
		Size: 29.7 MB (29654739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29541285df59f95a596b1911b49171e64e2361189a163533e77dbf2961b8f685`  
		Last Modified: Wed, 11 May 2022 02:40:04 GMT  
		Size: 5.0 KB (5026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c94a32e11bca5f817bc7015ceff49279fcd263d523198a38cc02607b7899e261`  
		Last Modified: Wed, 11 May 2022 02:40:04 GMT  
		Size: 324.2 KB (324197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57395e3cd66c2852ddaac636856f0245c1cfdca358d6bb75128950b9d9042481`  
		Last Modified: Wed, 11 May 2022 02:40:04 GMT  
		Size: 1.2 MB (1241369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ed03e37cb4ad7ab6dfc00b4938e9e5ec27777eb89fe1918ffc45a5a8de10c0`  
		Last Modified: Wed, 11 May 2022 02:40:04 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79cc46e5a2551dd05d1dcb476692b2a5d1c7e5181f253ad3938c179835018b95`  
		Last Modified: Wed, 11 May 2022 02:40:03 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
