<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `memcached`

-	[`memcached:1`](#memcached1)
-	[`memcached:1-alpine`](#memcached1-alpine)
-	[`memcached:1-alpine3.16`](#memcached1-alpine316)
-	[`memcached:1-bullseye`](#memcached1-bullseye)
-	[`memcached:1.6`](#memcached16)
-	[`memcached:1.6-alpine`](#memcached16-alpine)
-	[`memcached:1.6-alpine3.16`](#memcached16-alpine316)
-	[`memcached:1.6-bullseye`](#memcached16-bullseye)
-	[`memcached:1.6.17`](#memcached1617)
-	[`memcached:1.6.17-alpine`](#memcached1617-alpine)
-	[`memcached:1.6.17-alpine3.16`](#memcached1617-alpine316)
-	[`memcached:1.6.17-bullseye`](#memcached1617-bullseye)
-	[`memcached:alpine`](#memcachedalpine)
-	[`memcached:alpine3.16`](#memcachedalpine316)
-	[`memcached:bullseye`](#memcachedbullseye)
-	[`memcached:latest`](#memcachedlatest)

## `memcached:1`

```console
$ docker pull memcached@sha256:32b63986179511a820e33f0335381897731f15c802aa1d2707e9891aca1403a5
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
$ docker pull memcached@sha256:931b3d5a0c377a1ffba03d7692e157961e2802cd2fe528801182e80b099fcad8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (33009876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bdad48377094436fa7ba308ceb1b2bbce918630232e753085668b4e28281114`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:39 GMT
ADD file:b78b777208be08edd8f297035cdfbacddb45170ad778fd643c792ee045187e39 in / 
# Tue, 04 Oct 2022 23:26:39 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:17:54 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 04:17:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:17:57 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 04:17:57 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 04:20:39 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 04:20:39 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 04:20:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 04:20:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 04:20:40 GMT
USER memcache
# Wed, 05 Oct 2022 04:20:40 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 04:20:40 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:bd159e379b3b1bc0134341e4ffdeab5f966ec422ae04818bb69ecef08a823b05`  
		Last Modified: Tue, 04 Oct 2022 23:30:54 GMT  
		Size: 31.4 MB (31420102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ba15a7daa0d15e5ba45e9a9fdc332fce5b82c224ba42834aea059a6f245cf0`  
		Last Modified: Wed, 05 Oct 2022 04:21:07 GMT  
		Size: 5.0 KB (4983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7285127ceb5872fecb20531ce255b227f193cf0f6fceec79c876e4b8ebff29be`  
		Last Modified: Wed, 05 Oct 2022 04:21:08 GMT  
		Size: 328.1 KB (328117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e838e946498e1c28405bc1ae35d0fb6dafb97f0f47a462256719329c40afe865`  
		Last Modified: Wed, 05 Oct 2022 04:21:08 GMT  
		Size: 1.3 MB (1256265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd912af099a0b3bb0a430c2768ef0d784cab1d86924c157e945a751e12670e1d`  
		Last Modified: Wed, 05 Oct 2022 04:21:07 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60814b5c0f0d9e77d568f57890e62e11d94773423f772a3120117016d0de3294`  
		Last Modified: Wed, 05 Oct 2022 04:21:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm variant v5

```console
$ docker pull memcached@sha256:a84f9fc0812c5f2e6d4575b277b7421022c21829d34d89128c0058f22caf890e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30467657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:449c07e8773b5918abc8cf6d2542c0f1a102b52a38606808b8c1365296278cbc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Oct 2022 23:49:11 GMT
ADD file:effb9e2e2f8c7539e1a2200d069a2592e8ba20c9d034b5a73fbf173b6987193c in / 
# Tue, 04 Oct 2022 23:49:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:53:06 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 01:53:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:53:12 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 01:53:12 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 01:59:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 01:59:12 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 01:59:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 01:59:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 01:59:13 GMT
USER memcache
# Wed, 05 Oct 2022 01:59:13 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 01:59:13 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:7b9558bbfd8050a8e6af6e60560101c49bd53f81df6fa068419b44d028e465eb`  
		Last Modified: Tue, 04 Oct 2022 23:53:54 GMT  
		Size: 28.9 MB (28918381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f7663872748bf22ac651be2e08927fdd98e08f447cb7bcc3862ff485c6d5ddd`  
		Last Modified: Wed, 05 Oct 2022 01:59:52 GMT  
		Size: 4.9 KB (4897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b071b414257fa2a96433371bc4d51ce61fdac16c63b3f3c5e55c9818fa0529f`  
		Last Modified: Wed, 05 Oct 2022 01:59:52 GMT  
		Size: 316.6 KB (316627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f813defd9f0615e613628e02e7dadc2cbecc6b31ae8151aefb81d6a72922c9`  
		Last Modified: Wed, 05 Oct 2022 01:59:52 GMT  
		Size: 1.2 MB (1227346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb16c09a595afd6523b77641de3a45962bd09b125d8ba26b64c7ce6a17137a63`  
		Last Modified: Wed, 05 Oct 2022 01:59:52 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c54c4bbaf374145c3304bfe33479e0b53e0047102ae2488c8190de918a16e3e1`  
		Last Modified: Wed, 05 Oct 2022 01:59:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm variant v7

```console
$ docker pull memcached@sha256:c809ce19f7998cea0a39f8a4d06573b6f886a9c98b5da65ebb6efb13e8886d5e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28095847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9ba6ef519428019c76007d4e4e34b0d8e293799d94f152576aeb3a23fca1d0a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Oct 2022 23:58:46 GMT
ADD file:ca1bf27f17594a91224a252bd446f97c3b898210c571f2f26fa2e723d2bf521e in / 
# Tue, 04 Oct 2022 23:58:46 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 05:07:01 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 05:07:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 05:07:05 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 05:07:05 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 05:12:39 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 05:12:39 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 05:12:39 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 05:12:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 05:12:39 GMT
USER memcache
# Wed, 05 Oct 2022 05:12:39 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 05:12:40 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2bc64aeac2e429577e497affc8a416d2fc59158aa967f07aced793368e19455f`  
		Last Modified: Wed, 05 Oct 2022 00:05:09 GMT  
		Size: 26.6 MB (26579199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7e548f4109245b4d3d68767b83de82ac836ac9d5cc1bc081a219d32dbbeda54`  
		Last Modified: Wed, 05 Oct 2022 08:13:34 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:697369682782d1b2dbc043f43ca3316b0db3fa9ea73f7db3dbc467bac02eb162`  
		Last Modified: Wed, 05 Oct 2022 08:13:34 GMT  
		Size: 312.1 KB (312059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dfb70795c00f40a530881bffe5c831e6db14159082a026ea6998712e348984a`  
		Last Modified: Wed, 05 Oct 2022 08:13:35 GMT  
		Size: 1.2 MB (1199286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:476c14bf2670ef65dcc686dfa808de6890eff3c4910ef826bb7faf2291852c8e`  
		Last Modified: Wed, 05 Oct 2022 08:13:34 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d568980c19cf77318fcb8d77bacb59d6693b433e7181df0f3caef176b52a3191`  
		Last Modified: Wed, 05 Oct 2022 08:13:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:d3f458555a9a339d16f76ef8013aa925929005de7217194985f7efa465554cad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31445121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6406224fb2a1c7a535f7f3e81b89efa7325ae81d6b21d9d6bc5d27f41395d88a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:05:55 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 03:05:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:05:59 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 03:06:00 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 03:08:31 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 03:08:33 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 03:08:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 03:08:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 03:08:35 GMT
USER memcache
# Wed, 05 Oct 2022 03:08:36 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 03:08:37 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d51bfc33abb0dd79aa4c51b1f9c4cfd1190791ddeea14d61e1b8e5f5d996da7`  
		Last Modified: Wed, 05 Oct 2022 03:09:28 GMT  
		Size: 4.9 KB (4907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e37070a0cb39b1adff15bff570c77cd0bbe4459d214fc5722701da4f7c5b402`  
		Last Modified: Wed, 05 Oct 2022 03:09:29 GMT  
		Size: 119.3 KB (119254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078e83a26c52c9ff73f62179ba3a9b4b9cdbe0d927d4245a2f3c14d96d909d11`  
		Last Modified: Wed, 05 Oct 2022 03:09:29 GMT  
		Size: 1.3 MB (1256157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f353bbcc7b933af6761691a3ba35fb1b80b182162960769306c81729487de9cf`  
		Last Modified: Wed, 05 Oct 2022 03:09:29 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78a605409bcc6452727b4f53d4b26811dcdc8b176a88c568b56302f9e39ff85`  
		Last Modified: Wed, 05 Oct 2022 03:09:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; 386

```console
$ docker pull memcached@sha256:95ab1613d2fcc9c5a7eba541a7dfb13495fa99b5d77d4656da4630b78bf74c5a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33785263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93de9a3d72d17c99080504de246a0b51465565d26793ad487cd2908476723333`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Oct 2022 23:39:40 GMT
ADD file:a66b7a182260a23fdb8b219600a8b48a5079997715006d9a5324dda11f9d0a7f in / 
# Tue, 04 Oct 2022 23:39:41 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:12:48 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 13:12:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:12:53 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 13:12:54 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 13:15:47 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 13:15:48 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 13:15:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 13:15:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 13:15:50 GMT
USER memcache
# Wed, 05 Oct 2022 13:15:51 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 13:15:52 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:711839e532aa3f129f9cfaa5125d0e379ddefd47f3da44d0674372663dfc6a9b`  
		Last Modified: Tue, 04 Oct 2022 23:45:35 GMT  
		Size: 32.4 MB (32396290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5161f80d1df63217fef9b1a73e067a92d04f472d1a4ba002103da6e1689201d2`  
		Last Modified: Wed, 05 Oct 2022 13:16:41 GMT  
		Size: 4.8 KB (4775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b8ca938e3262650de875a82b51d5429ed32858924ed01f31e08823a0110f78`  
		Last Modified: Wed, 05 Oct 2022 13:16:41 GMT  
		Size: 130.1 KB (130128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d56431e1a0c892213dfd9a453e3575db72680db48a6aed437295e181498ae6c7`  
		Last Modified: Wed, 05 Oct 2022 13:16:42 GMT  
		Size: 1.3 MB (1253663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47362ecff01e4b5783c28f0a1024c21cbacf2f17b789860e4ebf99773898229a`  
		Last Modified: Wed, 05 Oct 2022 13:16:41 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f86c83c1049b01f43ae03975626a66ecb9eae0281599db499528892e30e0269f`  
		Last Modified: Wed, 05 Oct 2022 13:16:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; mips64le

```console
$ docker pull memcached@sha256:922b5312101767b2b3fc81590e722b5e79a729452b4f0edd17a5d792aa90e1b2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31015160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ec29f9e0c7858b09669119d800f2569a6a8e381808abe1a3989aa060c7a64ea`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 05 Oct 2022 00:10:26 GMT
ADD file:48da6b2f4e0315e4f502001a00e4b2abb58d553de11a41901ba859a461052bea in / 
# Wed, 05 Oct 2022 00:10:29 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:59:00 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 03:59:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:59:18 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 03:59:21 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 04:06:17 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 04:06:19 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 04:06:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 04:06:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 04:06:29 GMT
USER memcache
# Wed, 05 Oct 2022 04:06:31 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 04:06:34 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3288c6e2e7130a1e313203f049bde0e57a05237441a3cab92c27f9ada139315b`  
		Last Modified: Wed, 05 Oct 2022 00:18:36 GMT  
		Size: 29.6 MB (29640851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaef4f8453620b9cc82968e1dbf1ed98c0e4c5e897da9cd2e4d5bc26601ef1d0`  
		Last Modified: Wed, 05 Oct 2022 04:06:52 GMT  
		Size: 4.9 KB (4864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcbc6cec97a2b18b7caa64c38f40669eb923898edf6757612abf69036cc94a9c`  
		Last Modified: Wed, 05 Oct 2022 04:06:52 GMT  
		Size: 117.2 KB (117176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b83a324f1ad5c2d5e153fcf42024969d9bbaea8df56221c47b2dcccade28696`  
		Last Modified: Wed, 05 Oct 2022 04:06:52 GMT  
		Size: 1.3 MB (1251861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f20f84bbdb83e24c72fda0fed4ef0cf58b3eee6e4f05b5f4c745e1dfb4779199`  
		Last Modified: Wed, 05 Oct 2022 04:06:52 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f4cdf4ad864d232b858c0042bc2537f61833806ddf7781642c27f0ba8c58fd`  
		Last Modified: Wed, 05 Oct 2022 04:06:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; ppc64le

```console
$ docker pull memcached@sha256:5843450835c3de77b73d275c84981ff40a8921d2fd8f63df29f20779afd4b011
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36977018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ac10fdcf830775d9abecef20325a6db9befca7259adb12da3754bd79025d14d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Oct 2022 23:18:04 GMT
ADD file:66a0f55a4b4dfbb5d64082ffdb24751f20c5773039277ba278fdb4ce4a538c33 in / 
# Tue, 04 Oct 2022 23:18:06 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 08:58:03 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 08:58:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 08:58:10 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 08:58:11 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 09:01:22 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 09:01:23 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 09:01:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 09:01:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 09:01:25 GMT
USER memcache
# Wed, 05 Oct 2022 09:01:25 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 09:01:25 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:4e001127162dd884a6f7bd2e6f74215816d325bebb3a374ae9fcee9f038f99b8`  
		Last Modified: Tue, 04 Oct 2022 23:24:13 GMT  
		Size: 35.3 MB (35290584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c333c30cea960d51a0fca6f30a61ffd7bc4ec7e6711905a2875c17661de45833`  
		Last Modified: Wed, 05 Oct 2022 09:02:24 GMT  
		Size: 5.0 KB (4981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de7f9617e3f96516ad14767e6645f8cccf14aabe76c9617293d3dbdb8d1d5013`  
		Last Modified: Wed, 05 Oct 2022 09:02:24 GMT  
		Size: 356.9 KB (356918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2668fc82899be9101fab61482fe66b640b92efae057ee88cfe0604cf0c08c270`  
		Last Modified: Wed, 05 Oct 2022 09:02:24 GMT  
		Size: 1.3 MB (1324127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617887de59cd713ef92f5af550338f216d62b3a52ff11d3db7437ae4a977677d`  
		Last Modified: Wed, 05 Oct 2022 09:02:24 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f391b42bfd5493f7f0a5e4702ef212bcbcd630dc98069b371f54008e52d555`  
		Last Modified: Wed, 05 Oct 2022 09:02:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; s390x

```console
$ docker pull memcached@sha256:a68d861d39d508e157bfec89650683c443e38e085c0bb686efd1c6f6fb771090
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31221752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f8e5591d33ad149aa1fcea8466745b9018322eb538b330f198f2a24b9b67325`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Oct 2022 23:42:42 GMT
ADD file:7acfe92be51da9cffeb5b063cc87926d1ce457729e3080de340603a38216a708 in / 
# Tue, 04 Oct 2022 23:42:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:21:53 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 01:21:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:21:56 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 01:21:56 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 01:25:31 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 01:25:31 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 01:25:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 01:25:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 01:25:32 GMT
USER memcache
# Wed, 05 Oct 2022 01:25:32 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 01:25:32 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:62990b94a520bfcf718ec711f8444f83c536af2c83c8e53fdfe1f89fdcb79826`  
		Last Modified: Tue, 04 Oct 2022 23:47:16 GMT  
		Size: 29.7 MB (29650719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e75be154924807ecff182be8b52f82593e3ac5c84f4834226f410139f250562`  
		Last Modified: Wed, 05 Oct 2022 01:26:23 GMT  
		Size: 5.0 KB (5027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c6fcd517c09d146d86a8ab0c84e0cb87c39b6d5aa6a5e4f7c2027005bc6c03`  
		Last Modified: Wed, 05 Oct 2022 01:26:23 GMT  
		Size: 324.2 KB (324212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c83fd7ffcf78cdd0c4e1cee3843ffea027ce70f87c997960ea0e14823194a62`  
		Last Modified: Wed, 05 Oct 2022 01:26:23 GMT  
		Size: 1.2 MB (1241387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b6ed6acfc224f832786cfe50858117e0ff11e69d4dfe846f50143f9479e37e`  
		Last Modified: Wed, 05 Oct 2022 01:26:23 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ebd5ba7dabf6f7077666fa277c434e6f23a6614e4dc4d5706bd30dbb2f3d80a`  
		Last Modified: Wed, 05 Oct 2022 01:26:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1-alpine`

```console
$ docker pull memcached@sha256:d1d0f8424d9564a6d28b20d441b221294ab09e586d3666e7d3329c811ac3f322
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
$ docker pull memcached@sha256:d7f1053070f1020a4fc773523705c1494bfb1edf25edf24459c81418bcddb2bf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3868456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98356558fb5c650e049187d5fbc075b7d1548df209aff29dedc7202e925ea665`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:53:39 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 09 Aug 2022 20:53:40 GMT
RUN apk add --no-cache libsasl
# Mon, 29 Aug 2022 19:59:54 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 19:59:54 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 20:02:37 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Mon, 29 Aug 2022 20:02:37 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 20:02:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 20:02:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 20:02:38 GMT
USER memcache
# Mon, 29 Aug 2022 20:02:38 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 20:02:38 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d572ef57cdf8eb58de4b4e89970c5e64c6a2f8470bbbe4746efd56927df10611`  
		Last Modified: Tue, 09 Aug 2022 20:57:08 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed8976416286665206f17c9c2ead879425c6c6c62051fa7af308abd8790c0bc`  
		Last Modified: Tue, 09 Aug 2022 20:57:08 GMT  
		Size: 108.3 KB (108322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb81a082d3307bee25bd754b44c17e3423ace86257a27e62b6492be54e6c04b3`  
		Last Modified: Mon, 29 Aug 2022 20:03:30 GMT  
		Size: 952.4 KB (952408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f0efad04b524c1b9e6115b5481dc72c9ee037e65e86b42ae61f40eb5c079b8`  
		Last Modified: Mon, 29 Aug 2022 20:03:30 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963603084de81044b37f07eb6489013949af1ab497be7ace91dd5087c64d70ce`  
		Last Modified: Mon, 29 Aug 2022 20:03:29 GMT  
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
$ docker pull memcached@sha256:fe60e76484846f910192b2d5165415ba111c556789233c183ed18880187b5fed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3758619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc1d52e69bd83adcebc7479ed25934dbd29eb32cb68b338dd65aff944de86398`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:48:03 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 09 Aug 2022 20:48:05 GMT
RUN apk add --no-cache libsasl
# Mon, 29 Aug 2022 18:51:54 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 18:51:54 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 18:54:31 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Mon, 29 Aug 2022 18:54:33 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 18:54:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 18:54:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 18:54:35 GMT
USER memcache
# Mon, 29 Aug 2022 18:54:36 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 18:54:37 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d15db589ad12df2825238bc4f6832b2c6e3d991704c9b41db7865df5d402276`  
		Last Modified: Tue, 09 Aug 2022 20:51:50 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:103b4be7608736e9e24d225ccd97cc4dfad6bacbe7bcf2ca1cd716b45ee32855`  
		Last Modified: Tue, 09 Aug 2022 20:51:50 GMT  
		Size: 109.6 KB (109566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0212e668a84adeaf525aa82fe864ac8b57acb1950c67b38f17d4007d9f9bebbf`  
		Last Modified: Mon, 29 Aug 2022 18:55:51 GMT  
		Size: 939.7 KB (939742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8a69ef314b91110c98f842b3d141768e666cf4673f4414320521338faf28d6`  
		Last Modified: Mon, 29 Aug 2022 18:55:51 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d868394810ccf1649fee843c3a0588a6775265a67dec4936a32a8ee769205eb`  
		Last Modified: Mon, 29 Aug 2022 18:55:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; 386

```console
$ docker pull memcached@sha256:562b7a7602fbdc8c555c997346529640986f1a70c5310d0e7ac7ee5be5004134
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3891424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cf987911cc9f370d9a02fd24e09b38ac92f856013a58e52ae8e1e242e8f115d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:39 GMT
ADD file:b828bc14bc5ff03c8f7310fe0aed6ac5df19a393622d5d1d779a523234d07c0a in / 
# Tue, 09 Aug 2022 17:38:39 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:31:11 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 06 Oct 2022 20:31:12 GMT
RUN apk add --no-cache libsasl
# Thu, 06 Oct 2022 20:31:13 GMT
ENV MEMCACHED_VERSION=1.6.17
# Thu, 06 Oct 2022 20:31:14 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Thu, 06 Oct 2022 20:34:15 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 06 Oct 2022 20:34:17 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 06 Oct 2022 20:34:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 06 Oct 2022 20:34:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 20:34:19 GMT
USER memcache
# Thu, 06 Oct 2022 20:34:20 GMT
EXPOSE 11211
# Thu, 06 Oct 2022 20:34:21 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6c0d3b419d848ea31ca748254611d5d5ce3b76e3d7bba520fd87400fbb75f3b9`  
		Last Modified: Tue, 09 Aug 2022 17:39:33 GMT  
		Size: 2.8 MB (2807121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c5cf4da7d47a1675ec754c4abb2f8aed348ebb76a41a3feea34b6737965077`  
		Last Modified: Thu, 06 Oct 2022 20:35:16 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd19825385b793f75ea8e660e1a32ba82a67f889d2f0fa17286da02efcc7c82`  
		Last Modified: Thu, 06 Oct 2022 20:35:17 GMT  
		Size: 119.8 KB (119834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23144451377b23ee74c09325785c2d9979f0d546d9114753499726be49f0ac35`  
		Last Modified: Thu, 06 Oct 2022 20:35:17 GMT  
		Size: 962.8 KB (962822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9862d0ec769de46de1bc8c01602342b1bbb1d2b834cf3a1aeaaa013bfebbe42c`  
		Last Modified: Thu, 06 Oct 2022 20:35:16 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28aee3d7b7e60049b472288f76c206e4acab742797abacdae0d146f1b1c987be`  
		Last Modified: Thu, 06 Oct 2022 20:35:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:933ee3008de5fff45556eed8f813dbe28c638669e4f1fae22228f1d4ae97fa5d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3913068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c35abea284c9fdadf80277c4e589f260436f39426d12485ae9fd06c66e0cab6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:58:36 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 06 Oct 2022 20:58:39 GMT
RUN apk add --no-cache libsasl
# Thu, 06 Oct 2022 20:58:39 GMT
ENV MEMCACHED_VERSION=1.6.17
# Thu, 06 Oct 2022 20:58:40 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Thu, 06 Oct 2022 21:01:52 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 06 Oct 2022 21:01:52 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 06 Oct 2022 21:01:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 06 Oct 2022 21:01:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 21:01:54 GMT
USER memcache
# Thu, 06 Oct 2022 21:01:55 GMT
EXPOSE 11211
# Thu, 06 Oct 2022 21:01:55 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a4950a8cc87dd9e5ec07268592148771ee6a96b270c2ad0cd2de4ff7b00c1a`  
		Last Modified: Thu, 06 Oct 2022 21:02:46 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c992ad9a080419adb465c5ddd18a317cb7342af149a0deab2c2c7d15bd087442`  
		Last Modified: Thu, 06 Oct 2022 21:02:47 GMT  
		Size: 126.1 KB (126070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6091cffcf047d57d7b51ecc08c3dd0d176f21102199ec0e24ee40257b838287`  
		Last Modified: Thu, 06 Oct 2022 21:02:47 GMT  
		Size: 982.0 KB (982000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b1b52d56e86ac7b75aec7089c33a24d031a269242ee0fdc7a9929f955ecbecd`  
		Last Modified: Thu, 06 Oct 2022 21:02:46 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73885207a86618904bca9142334c74041f4658a7023f9a68e109a24a4dfbfae7`  
		Last Modified: Thu, 06 Oct 2022 21:02:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; s390x

```console
$ docker pull memcached@sha256:409d3e4b8b0de5fc4e5c9f070c5496a99e2d030c2772647bb04095fe6f0757f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3646992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b6a4697fa6b2f43f9e85db112952c4b5ff69b3c9bf3ebcdf7905a11785815b5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:45:36 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 06 Oct 2022 20:45:38 GMT
RUN apk add --no-cache libsasl
# Thu, 06 Oct 2022 20:45:39 GMT
ENV MEMCACHED_VERSION=1.6.17
# Thu, 06 Oct 2022 20:45:39 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Thu, 06 Oct 2022 20:49:59 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 06 Oct 2022 20:49:59 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 06 Oct 2022 20:50:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 06 Oct 2022 20:50:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 20:50:00 GMT
USER memcache
# Thu, 06 Oct 2022 20:50:00 GMT
EXPOSE 11211
# Thu, 06 Oct 2022 20:50:01 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb7a4b531f98c3a90954f542da5d7028ec87d1ee2a74467d087d237d1a5cb62`  
		Last Modified: Thu, 06 Oct 2022 20:50:54 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:248a438b0a1fd089205148ab101aaf2457c55967afad4e042339958b0c1b6b50`  
		Last Modified: Thu, 06 Oct 2022 20:50:54 GMT  
		Size: 112.5 KB (112508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:467a2ab9413d162f0d6b5e65207d0adc2e4d105f9d4a8c3ada6852bf1c5c7e35`  
		Last Modified: Thu, 06 Oct 2022 20:50:54 GMT  
		Size: 942.2 KB (942214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20d843cc1cc32f57f16bc13ab2c98e20dc0fa2b80303702cfce0cdd39a64e4d`  
		Last Modified: Thu, 06 Oct 2022 20:50:54 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b936f167ac6d6abd85c1ebe43c570c4ce1725b0cc4b912ac38a6164606562dc4`  
		Last Modified: Thu, 06 Oct 2022 20:50:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1-alpine3.16`

```console
$ docker pull memcached@sha256:304980979f6f7d6e650ad82ab73d6b64a96c1b32800508b5c2afd9bb5341167c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1-alpine3.16` - linux; amd64

```console
$ docker pull memcached@sha256:d7f1053070f1020a4fc773523705c1494bfb1edf25edf24459c81418bcddb2bf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3868456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98356558fb5c650e049187d5fbc075b7d1548df209aff29dedc7202e925ea665`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:53:39 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 09 Aug 2022 20:53:40 GMT
RUN apk add --no-cache libsasl
# Mon, 29 Aug 2022 19:59:54 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 19:59:54 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 20:02:37 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Mon, 29 Aug 2022 20:02:37 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 20:02:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 20:02:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 20:02:38 GMT
USER memcache
# Mon, 29 Aug 2022 20:02:38 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 20:02:38 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d572ef57cdf8eb58de4b4e89970c5e64c6a2f8470bbbe4746efd56927df10611`  
		Last Modified: Tue, 09 Aug 2022 20:57:08 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed8976416286665206f17c9c2ead879425c6c6c62051fa7af308abd8790c0bc`  
		Last Modified: Tue, 09 Aug 2022 20:57:08 GMT  
		Size: 108.3 KB (108322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb81a082d3307bee25bd754b44c17e3423ace86257a27e62b6492be54e6c04b3`  
		Last Modified: Mon, 29 Aug 2022 20:03:30 GMT  
		Size: 952.4 KB (952408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f0efad04b524c1b9e6115b5481dc72c9ee037e65e86b42ae61f40eb5c079b8`  
		Last Modified: Mon, 29 Aug 2022 20:03:30 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963603084de81044b37f07eb6489013949af1ab497be7ace91dd5087c64d70ce`  
		Last Modified: Mon, 29 Aug 2022 20:03:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:fe60e76484846f910192b2d5165415ba111c556789233c183ed18880187b5fed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3758619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc1d52e69bd83adcebc7479ed25934dbd29eb32cb68b338dd65aff944de86398`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:48:03 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 09 Aug 2022 20:48:05 GMT
RUN apk add --no-cache libsasl
# Mon, 29 Aug 2022 18:51:54 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 18:51:54 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 18:54:31 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Mon, 29 Aug 2022 18:54:33 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 18:54:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 18:54:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 18:54:35 GMT
USER memcache
# Mon, 29 Aug 2022 18:54:36 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 18:54:37 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d15db589ad12df2825238bc4f6832b2c6e3d991704c9b41db7865df5d402276`  
		Last Modified: Tue, 09 Aug 2022 20:51:50 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:103b4be7608736e9e24d225ccd97cc4dfad6bacbe7bcf2ca1cd716b45ee32855`  
		Last Modified: Tue, 09 Aug 2022 20:51:50 GMT  
		Size: 109.6 KB (109566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0212e668a84adeaf525aa82fe864ac8b57acb1950c67b38f17d4007d9f9bebbf`  
		Last Modified: Mon, 29 Aug 2022 18:55:51 GMT  
		Size: 939.7 KB (939742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8a69ef314b91110c98f842b3d141768e666cf4673f4414320521338faf28d6`  
		Last Modified: Mon, 29 Aug 2022 18:55:51 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d868394810ccf1649fee843c3a0588a6775265a67dec4936a32a8ee769205eb`  
		Last Modified: Mon, 29 Aug 2022 18:55:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.16` - linux; 386

```console
$ docker pull memcached@sha256:562b7a7602fbdc8c555c997346529640986f1a70c5310d0e7ac7ee5be5004134
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3891424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cf987911cc9f370d9a02fd24e09b38ac92f856013a58e52ae8e1e242e8f115d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:39 GMT
ADD file:b828bc14bc5ff03c8f7310fe0aed6ac5df19a393622d5d1d779a523234d07c0a in / 
# Tue, 09 Aug 2022 17:38:39 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:31:11 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 06 Oct 2022 20:31:12 GMT
RUN apk add --no-cache libsasl
# Thu, 06 Oct 2022 20:31:13 GMT
ENV MEMCACHED_VERSION=1.6.17
# Thu, 06 Oct 2022 20:31:14 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Thu, 06 Oct 2022 20:34:15 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 06 Oct 2022 20:34:17 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 06 Oct 2022 20:34:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 06 Oct 2022 20:34:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 20:34:19 GMT
USER memcache
# Thu, 06 Oct 2022 20:34:20 GMT
EXPOSE 11211
# Thu, 06 Oct 2022 20:34:21 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6c0d3b419d848ea31ca748254611d5d5ce3b76e3d7bba520fd87400fbb75f3b9`  
		Last Modified: Tue, 09 Aug 2022 17:39:33 GMT  
		Size: 2.8 MB (2807121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c5cf4da7d47a1675ec754c4abb2f8aed348ebb76a41a3feea34b6737965077`  
		Last Modified: Thu, 06 Oct 2022 20:35:16 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd19825385b793f75ea8e660e1a32ba82a67f889d2f0fa17286da02efcc7c82`  
		Last Modified: Thu, 06 Oct 2022 20:35:17 GMT  
		Size: 119.8 KB (119834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23144451377b23ee74c09325785c2d9979f0d546d9114753499726be49f0ac35`  
		Last Modified: Thu, 06 Oct 2022 20:35:17 GMT  
		Size: 962.8 KB (962822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9862d0ec769de46de1bc8c01602342b1bbb1d2b834cf3a1aeaaa013bfebbe42c`  
		Last Modified: Thu, 06 Oct 2022 20:35:16 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28aee3d7b7e60049b472288f76c206e4acab742797abacdae0d146f1b1c987be`  
		Last Modified: Thu, 06 Oct 2022 20:35:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.16` - linux; ppc64le

```console
$ docker pull memcached@sha256:933ee3008de5fff45556eed8f813dbe28c638669e4f1fae22228f1d4ae97fa5d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3913068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c35abea284c9fdadf80277c4e589f260436f39426d12485ae9fd06c66e0cab6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:58:36 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 06 Oct 2022 20:58:39 GMT
RUN apk add --no-cache libsasl
# Thu, 06 Oct 2022 20:58:39 GMT
ENV MEMCACHED_VERSION=1.6.17
# Thu, 06 Oct 2022 20:58:40 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Thu, 06 Oct 2022 21:01:52 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 06 Oct 2022 21:01:52 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 06 Oct 2022 21:01:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 06 Oct 2022 21:01:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 21:01:54 GMT
USER memcache
# Thu, 06 Oct 2022 21:01:55 GMT
EXPOSE 11211
# Thu, 06 Oct 2022 21:01:55 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a4950a8cc87dd9e5ec07268592148771ee6a96b270c2ad0cd2de4ff7b00c1a`  
		Last Modified: Thu, 06 Oct 2022 21:02:46 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c992ad9a080419adb465c5ddd18a317cb7342af149a0deab2c2c7d15bd087442`  
		Last Modified: Thu, 06 Oct 2022 21:02:47 GMT  
		Size: 126.1 KB (126070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6091cffcf047d57d7b51ecc08c3dd0d176f21102199ec0e24ee40257b838287`  
		Last Modified: Thu, 06 Oct 2022 21:02:47 GMT  
		Size: 982.0 KB (982000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b1b52d56e86ac7b75aec7089c33a24d031a269242ee0fdc7a9929f955ecbecd`  
		Last Modified: Thu, 06 Oct 2022 21:02:46 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73885207a86618904bca9142334c74041f4658a7023f9a68e109a24a4dfbfae7`  
		Last Modified: Thu, 06 Oct 2022 21:02:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.16` - linux; s390x

```console
$ docker pull memcached@sha256:409d3e4b8b0de5fc4e5c9f070c5496a99e2d030c2772647bb04095fe6f0757f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3646992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b6a4697fa6b2f43f9e85db112952c4b5ff69b3c9bf3ebcdf7905a11785815b5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:45:36 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 06 Oct 2022 20:45:38 GMT
RUN apk add --no-cache libsasl
# Thu, 06 Oct 2022 20:45:39 GMT
ENV MEMCACHED_VERSION=1.6.17
# Thu, 06 Oct 2022 20:45:39 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Thu, 06 Oct 2022 20:49:59 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 06 Oct 2022 20:49:59 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 06 Oct 2022 20:50:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 06 Oct 2022 20:50:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 20:50:00 GMT
USER memcache
# Thu, 06 Oct 2022 20:50:00 GMT
EXPOSE 11211
# Thu, 06 Oct 2022 20:50:01 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb7a4b531f98c3a90954f542da5d7028ec87d1ee2a74467d087d237d1a5cb62`  
		Last Modified: Thu, 06 Oct 2022 20:50:54 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:248a438b0a1fd089205148ab101aaf2457c55967afad4e042339958b0c1b6b50`  
		Last Modified: Thu, 06 Oct 2022 20:50:54 GMT  
		Size: 112.5 KB (112508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:467a2ab9413d162f0d6b5e65207d0adc2e4d105f9d4a8c3ada6852bf1c5c7e35`  
		Last Modified: Thu, 06 Oct 2022 20:50:54 GMT  
		Size: 942.2 KB (942214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20d843cc1cc32f57f16bc13ab2c98e20dc0fa2b80303702cfce0cdd39a64e4d`  
		Last Modified: Thu, 06 Oct 2022 20:50:54 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b936f167ac6d6abd85c1ebe43c570c4ce1725b0cc4b912ac38a6164606562dc4`  
		Last Modified: Thu, 06 Oct 2022 20:50:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1-bullseye`

```console
$ docker pull memcached@sha256:32b63986179511a820e33f0335381897731f15c802aa1d2707e9891aca1403a5
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
$ docker pull memcached@sha256:931b3d5a0c377a1ffba03d7692e157961e2802cd2fe528801182e80b099fcad8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (33009876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bdad48377094436fa7ba308ceb1b2bbce918630232e753085668b4e28281114`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:39 GMT
ADD file:b78b777208be08edd8f297035cdfbacddb45170ad778fd643c792ee045187e39 in / 
# Tue, 04 Oct 2022 23:26:39 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:17:54 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 04:17:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:17:57 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 04:17:57 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 04:20:39 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 04:20:39 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 04:20:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 04:20:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 04:20:40 GMT
USER memcache
# Wed, 05 Oct 2022 04:20:40 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 04:20:40 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:bd159e379b3b1bc0134341e4ffdeab5f966ec422ae04818bb69ecef08a823b05`  
		Last Modified: Tue, 04 Oct 2022 23:30:54 GMT  
		Size: 31.4 MB (31420102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ba15a7daa0d15e5ba45e9a9fdc332fce5b82c224ba42834aea059a6f245cf0`  
		Last Modified: Wed, 05 Oct 2022 04:21:07 GMT  
		Size: 5.0 KB (4983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7285127ceb5872fecb20531ce255b227f193cf0f6fceec79c876e4b8ebff29be`  
		Last Modified: Wed, 05 Oct 2022 04:21:08 GMT  
		Size: 328.1 KB (328117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e838e946498e1c28405bc1ae35d0fb6dafb97f0f47a462256719329c40afe865`  
		Last Modified: Wed, 05 Oct 2022 04:21:08 GMT  
		Size: 1.3 MB (1256265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd912af099a0b3bb0a430c2768ef0d784cab1d86924c157e945a751e12670e1d`  
		Last Modified: Wed, 05 Oct 2022 04:21:07 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60814b5c0f0d9e77d568f57890e62e11d94773423f772a3120117016d0de3294`  
		Last Modified: Wed, 05 Oct 2022 04:21:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; arm variant v5

```console
$ docker pull memcached@sha256:a84f9fc0812c5f2e6d4575b277b7421022c21829d34d89128c0058f22caf890e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30467657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:449c07e8773b5918abc8cf6d2542c0f1a102b52a38606808b8c1365296278cbc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Oct 2022 23:49:11 GMT
ADD file:effb9e2e2f8c7539e1a2200d069a2592e8ba20c9d034b5a73fbf173b6987193c in / 
# Tue, 04 Oct 2022 23:49:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:53:06 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 01:53:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:53:12 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 01:53:12 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 01:59:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 01:59:12 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 01:59:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 01:59:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 01:59:13 GMT
USER memcache
# Wed, 05 Oct 2022 01:59:13 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 01:59:13 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:7b9558bbfd8050a8e6af6e60560101c49bd53f81df6fa068419b44d028e465eb`  
		Last Modified: Tue, 04 Oct 2022 23:53:54 GMT  
		Size: 28.9 MB (28918381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f7663872748bf22ac651be2e08927fdd98e08f447cb7bcc3862ff485c6d5ddd`  
		Last Modified: Wed, 05 Oct 2022 01:59:52 GMT  
		Size: 4.9 KB (4897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b071b414257fa2a96433371bc4d51ce61fdac16c63b3f3c5e55c9818fa0529f`  
		Last Modified: Wed, 05 Oct 2022 01:59:52 GMT  
		Size: 316.6 KB (316627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f813defd9f0615e613628e02e7dadc2cbecc6b31ae8151aefb81d6a72922c9`  
		Last Modified: Wed, 05 Oct 2022 01:59:52 GMT  
		Size: 1.2 MB (1227346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb16c09a595afd6523b77641de3a45962bd09b125d8ba26b64c7ce6a17137a63`  
		Last Modified: Wed, 05 Oct 2022 01:59:52 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c54c4bbaf374145c3304bfe33479e0b53e0047102ae2488c8190de918a16e3e1`  
		Last Modified: Wed, 05 Oct 2022 01:59:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; arm variant v7

```console
$ docker pull memcached@sha256:c809ce19f7998cea0a39f8a4d06573b6f886a9c98b5da65ebb6efb13e8886d5e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28095847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9ba6ef519428019c76007d4e4e34b0d8e293799d94f152576aeb3a23fca1d0a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Oct 2022 23:58:46 GMT
ADD file:ca1bf27f17594a91224a252bd446f97c3b898210c571f2f26fa2e723d2bf521e in / 
# Tue, 04 Oct 2022 23:58:46 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 05:07:01 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 05:07:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 05:07:05 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 05:07:05 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 05:12:39 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 05:12:39 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 05:12:39 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 05:12:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 05:12:39 GMT
USER memcache
# Wed, 05 Oct 2022 05:12:39 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 05:12:40 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2bc64aeac2e429577e497affc8a416d2fc59158aa967f07aced793368e19455f`  
		Last Modified: Wed, 05 Oct 2022 00:05:09 GMT  
		Size: 26.6 MB (26579199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7e548f4109245b4d3d68767b83de82ac836ac9d5cc1bc081a219d32dbbeda54`  
		Last Modified: Wed, 05 Oct 2022 08:13:34 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:697369682782d1b2dbc043f43ca3316b0db3fa9ea73f7db3dbc467bac02eb162`  
		Last Modified: Wed, 05 Oct 2022 08:13:34 GMT  
		Size: 312.1 KB (312059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dfb70795c00f40a530881bffe5c831e6db14159082a026ea6998712e348984a`  
		Last Modified: Wed, 05 Oct 2022 08:13:35 GMT  
		Size: 1.2 MB (1199286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:476c14bf2670ef65dcc686dfa808de6890eff3c4910ef826bb7faf2291852c8e`  
		Last Modified: Wed, 05 Oct 2022 08:13:34 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d568980c19cf77318fcb8d77bacb59d6693b433e7181df0f3caef176b52a3191`  
		Last Modified: Wed, 05 Oct 2022 08:13:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:d3f458555a9a339d16f76ef8013aa925929005de7217194985f7efa465554cad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31445121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6406224fb2a1c7a535f7f3e81b89efa7325ae81d6b21d9d6bc5d27f41395d88a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:05:55 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 03:05:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:05:59 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 03:06:00 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 03:08:31 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 03:08:33 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 03:08:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 03:08:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 03:08:35 GMT
USER memcache
# Wed, 05 Oct 2022 03:08:36 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 03:08:37 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d51bfc33abb0dd79aa4c51b1f9c4cfd1190791ddeea14d61e1b8e5f5d996da7`  
		Last Modified: Wed, 05 Oct 2022 03:09:28 GMT  
		Size: 4.9 KB (4907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e37070a0cb39b1adff15bff570c77cd0bbe4459d214fc5722701da4f7c5b402`  
		Last Modified: Wed, 05 Oct 2022 03:09:29 GMT  
		Size: 119.3 KB (119254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078e83a26c52c9ff73f62179ba3a9b4b9cdbe0d927d4245a2f3c14d96d909d11`  
		Last Modified: Wed, 05 Oct 2022 03:09:29 GMT  
		Size: 1.3 MB (1256157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f353bbcc7b933af6761691a3ba35fb1b80b182162960769306c81729487de9cf`  
		Last Modified: Wed, 05 Oct 2022 03:09:29 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78a605409bcc6452727b4f53d4b26811dcdc8b176a88c568b56302f9e39ff85`  
		Last Modified: Wed, 05 Oct 2022 03:09:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; 386

```console
$ docker pull memcached@sha256:95ab1613d2fcc9c5a7eba541a7dfb13495fa99b5d77d4656da4630b78bf74c5a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33785263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93de9a3d72d17c99080504de246a0b51465565d26793ad487cd2908476723333`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Oct 2022 23:39:40 GMT
ADD file:a66b7a182260a23fdb8b219600a8b48a5079997715006d9a5324dda11f9d0a7f in / 
# Tue, 04 Oct 2022 23:39:41 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:12:48 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 13:12:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:12:53 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 13:12:54 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 13:15:47 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 13:15:48 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 13:15:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 13:15:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 13:15:50 GMT
USER memcache
# Wed, 05 Oct 2022 13:15:51 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 13:15:52 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:711839e532aa3f129f9cfaa5125d0e379ddefd47f3da44d0674372663dfc6a9b`  
		Last Modified: Tue, 04 Oct 2022 23:45:35 GMT  
		Size: 32.4 MB (32396290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5161f80d1df63217fef9b1a73e067a92d04f472d1a4ba002103da6e1689201d2`  
		Last Modified: Wed, 05 Oct 2022 13:16:41 GMT  
		Size: 4.8 KB (4775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b8ca938e3262650de875a82b51d5429ed32858924ed01f31e08823a0110f78`  
		Last Modified: Wed, 05 Oct 2022 13:16:41 GMT  
		Size: 130.1 KB (130128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d56431e1a0c892213dfd9a453e3575db72680db48a6aed437295e181498ae6c7`  
		Last Modified: Wed, 05 Oct 2022 13:16:42 GMT  
		Size: 1.3 MB (1253663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47362ecff01e4b5783c28f0a1024c21cbacf2f17b789860e4ebf99773898229a`  
		Last Modified: Wed, 05 Oct 2022 13:16:41 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f86c83c1049b01f43ae03975626a66ecb9eae0281599db499528892e30e0269f`  
		Last Modified: Wed, 05 Oct 2022 13:16:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; mips64le

```console
$ docker pull memcached@sha256:922b5312101767b2b3fc81590e722b5e79a729452b4f0edd17a5d792aa90e1b2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31015160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ec29f9e0c7858b09669119d800f2569a6a8e381808abe1a3989aa060c7a64ea`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 05 Oct 2022 00:10:26 GMT
ADD file:48da6b2f4e0315e4f502001a00e4b2abb58d553de11a41901ba859a461052bea in / 
# Wed, 05 Oct 2022 00:10:29 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:59:00 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 03:59:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:59:18 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 03:59:21 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 04:06:17 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 04:06:19 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 04:06:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 04:06:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 04:06:29 GMT
USER memcache
# Wed, 05 Oct 2022 04:06:31 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 04:06:34 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3288c6e2e7130a1e313203f049bde0e57a05237441a3cab92c27f9ada139315b`  
		Last Modified: Wed, 05 Oct 2022 00:18:36 GMT  
		Size: 29.6 MB (29640851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaef4f8453620b9cc82968e1dbf1ed98c0e4c5e897da9cd2e4d5bc26601ef1d0`  
		Last Modified: Wed, 05 Oct 2022 04:06:52 GMT  
		Size: 4.9 KB (4864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcbc6cec97a2b18b7caa64c38f40669eb923898edf6757612abf69036cc94a9c`  
		Last Modified: Wed, 05 Oct 2022 04:06:52 GMT  
		Size: 117.2 KB (117176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b83a324f1ad5c2d5e153fcf42024969d9bbaea8df56221c47b2dcccade28696`  
		Last Modified: Wed, 05 Oct 2022 04:06:52 GMT  
		Size: 1.3 MB (1251861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f20f84bbdb83e24c72fda0fed4ef0cf58b3eee6e4f05b5f4c745e1dfb4779199`  
		Last Modified: Wed, 05 Oct 2022 04:06:52 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f4cdf4ad864d232b858c0042bc2537f61833806ddf7781642c27f0ba8c58fd`  
		Last Modified: Wed, 05 Oct 2022 04:06:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; ppc64le

```console
$ docker pull memcached@sha256:5843450835c3de77b73d275c84981ff40a8921d2fd8f63df29f20779afd4b011
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36977018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ac10fdcf830775d9abecef20325a6db9befca7259adb12da3754bd79025d14d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Oct 2022 23:18:04 GMT
ADD file:66a0f55a4b4dfbb5d64082ffdb24751f20c5773039277ba278fdb4ce4a538c33 in / 
# Tue, 04 Oct 2022 23:18:06 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 08:58:03 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 08:58:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 08:58:10 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 08:58:11 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 09:01:22 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 09:01:23 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 09:01:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 09:01:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 09:01:25 GMT
USER memcache
# Wed, 05 Oct 2022 09:01:25 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 09:01:25 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:4e001127162dd884a6f7bd2e6f74215816d325bebb3a374ae9fcee9f038f99b8`  
		Last Modified: Tue, 04 Oct 2022 23:24:13 GMT  
		Size: 35.3 MB (35290584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c333c30cea960d51a0fca6f30a61ffd7bc4ec7e6711905a2875c17661de45833`  
		Last Modified: Wed, 05 Oct 2022 09:02:24 GMT  
		Size: 5.0 KB (4981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de7f9617e3f96516ad14767e6645f8cccf14aabe76c9617293d3dbdb8d1d5013`  
		Last Modified: Wed, 05 Oct 2022 09:02:24 GMT  
		Size: 356.9 KB (356918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2668fc82899be9101fab61482fe66b640b92efae057ee88cfe0604cf0c08c270`  
		Last Modified: Wed, 05 Oct 2022 09:02:24 GMT  
		Size: 1.3 MB (1324127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617887de59cd713ef92f5af550338f216d62b3a52ff11d3db7437ae4a977677d`  
		Last Modified: Wed, 05 Oct 2022 09:02:24 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f391b42bfd5493f7f0a5e4702ef212bcbcd630dc98069b371f54008e52d555`  
		Last Modified: Wed, 05 Oct 2022 09:02:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; s390x

```console
$ docker pull memcached@sha256:a68d861d39d508e157bfec89650683c443e38e085c0bb686efd1c6f6fb771090
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31221752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f8e5591d33ad149aa1fcea8466745b9018322eb538b330f198f2a24b9b67325`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Oct 2022 23:42:42 GMT
ADD file:7acfe92be51da9cffeb5b063cc87926d1ce457729e3080de340603a38216a708 in / 
# Tue, 04 Oct 2022 23:42:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:21:53 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 01:21:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:21:56 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 01:21:56 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 01:25:31 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 01:25:31 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 01:25:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 01:25:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 01:25:32 GMT
USER memcache
# Wed, 05 Oct 2022 01:25:32 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 01:25:32 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:62990b94a520bfcf718ec711f8444f83c536af2c83c8e53fdfe1f89fdcb79826`  
		Last Modified: Tue, 04 Oct 2022 23:47:16 GMT  
		Size: 29.7 MB (29650719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e75be154924807ecff182be8b52f82593e3ac5c84f4834226f410139f250562`  
		Last Modified: Wed, 05 Oct 2022 01:26:23 GMT  
		Size: 5.0 KB (5027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c6fcd517c09d146d86a8ab0c84e0cb87c39b6d5aa6a5e4f7c2027005bc6c03`  
		Last Modified: Wed, 05 Oct 2022 01:26:23 GMT  
		Size: 324.2 KB (324212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c83fd7ffcf78cdd0c4e1cee3843ffea027ce70f87c997960ea0e14823194a62`  
		Last Modified: Wed, 05 Oct 2022 01:26:23 GMT  
		Size: 1.2 MB (1241387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b6ed6acfc224f832786cfe50858117e0ff11e69d4dfe846f50143f9479e37e`  
		Last Modified: Wed, 05 Oct 2022 01:26:23 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ebd5ba7dabf6f7077666fa277c434e6f23a6614e4dc4d5706bd30dbb2f3d80a`  
		Last Modified: Wed, 05 Oct 2022 01:26:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6`

```console
$ docker pull memcached@sha256:32b63986179511a820e33f0335381897731f15c802aa1d2707e9891aca1403a5
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
$ docker pull memcached@sha256:931b3d5a0c377a1ffba03d7692e157961e2802cd2fe528801182e80b099fcad8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (33009876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bdad48377094436fa7ba308ceb1b2bbce918630232e753085668b4e28281114`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:39 GMT
ADD file:b78b777208be08edd8f297035cdfbacddb45170ad778fd643c792ee045187e39 in / 
# Tue, 04 Oct 2022 23:26:39 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:17:54 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 04:17:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:17:57 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 04:17:57 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 04:20:39 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 04:20:39 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 04:20:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 04:20:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 04:20:40 GMT
USER memcache
# Wed, 05 Oct 2022 04:20:40 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 04:20:40 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:bd159e379b3b1bc0134341e4ffdeab5f966ec422ae04818bb69ecef08a823b05`  
		Last Modified: Tue, 04 Oct 2022 23:30:54 GMT  
		Size: 31.4 MB (31420102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ba15a7daa0d15e5ba45e9a9fdc332fce5b82c224ba42834aea059a6f245cf0`  
		Last Modified: Wed, 05 Oct 2022 04:21:07 GMT  
		Size: 5.0 KB (4983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7285127ceb5872fecb20531ce255b227f193cf0f6fceec79c876e4b8ebff29be`  
		Last Modified: Wed, 05 Oct 2022 04:21:08 GMT  
		Size: 328.1 KB (328117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e838e946498e1c28405bc1ae35d0fb6dafb97f0f47a462256719329c40afe865`  
		Last Modified: Wed, 05 Oct 2022 04:21:08 GMT  
		Size: 1.3 MB (1256265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd912af099a0b3bb0a430c2768ef0d784cab1d86924c157e945a751e12670e1d`  
		Last Modified: Wed, 05 Oct 2022 04:21:07 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60814b5c0f0d9e77d568f57890e62e11d94773423f772a3120117016d0de3294`  
		Last Modified: Wed, 05 Oct 2022 04:21:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm variant v5

```console
$ docker pull memcached@sha256:a84f9fc0812c5f2e6d4575b277b7421022c21829d34d89128c0058f22caf890e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30467657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:449c07e8773b5918abc8cf6d2542c0f1a102b52a38606808b8c1365296278cbc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Oct 2022 23:49:11 GMT
ADD file:effb9e2e2f8c7539e1a2200d069a2592e8ba20c9d034b5a73fbf173b6987193c in / 
# Tue, 04 Oct 2022 23:49:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:53:06 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 01:53:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:53:12 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 01:53:12 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 01:59:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 01:59:12 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 01:59:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 01:59:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 01:59:13 GMT
USER memcache
# Wed, 05 Oct 2022 01:59:13 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 01:59:13 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:7b9558bbfd8050a8e6af6e60560101c49bd53f81df6fa068419b44d028e465eb`  
		Last Modified: Tue, 04 Oct 2022 23:53:54 GMT  
		Size: 28.9 MB (28918381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f7663872748bf22ac651be2e08927fdd98e08f447cb7bcc3862ff485c6d5ddd`  
		Last Modified: Wed, 05 Oct 2022 01:59:52 GMT  
		Size: 4.9 KB (4897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b071b414257fa2a96433371bc4d51ce61fdac16c63b3f3c5e55c9818fa0529f`  
		Last Modified: Wed, 05 Oct 2022 01:59:52 GMT  
		Size: 316.6 KB (316627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f813defd9f0615e613628e02e7dadc2cbecc6b31ae8151aefb81d6a72922c9`  
		Last Modified: Wed, 05 Oct 2022 01:59:52 GMT  
		Size: 1.2 MB (1227346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb16c09a595afd6523b77641de3a45962bd09b125d8ba26b64c7ce6a17137a63`  
		Last Modified: Wed, 05 Oct 2022 01:59:52 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c54c4bbaf374145c3304bfe33479e0b53e0047102ae2488c8190de918a16e3e1`  
		Last Modified: Wed, 05 Oct 2022 01:59:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm variant v7

```console
$ docker pull memcached@sha256:c809ce19f7998cea0a39f8a4d06573b6f886a9c98b5da65ebb6efb13e8886d5e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28095847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9ba6ef519428019c76007d4e4e34b0d8e293799d94f152576aeb3a23fca1d0a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Oct 2022 23:58:46 GMT
ADD file:ca1bf27f17594a91224a252bd446f97c3b898210c571f2f26fa2e723d2bf521e in / 
# Tue, 04 Oct 2022 23:58:46 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 05:07:01 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 05:07:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 05:07:05 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 05:07:05 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 05:12:39 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 05:12:39 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 05:12:39 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 05:12:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 05:12:39 GMT
USER memcache
# Wed, 05 Oct 2022 05:12:39 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 05:12:40 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2bc64aeac2e429577e497affc8a416d2fc59158aa967f07aced793368e19455f`  
		Last Modified: Wed, 05 Oct 2022 00:05:09 GMT  
		Size: 26.6 MB (26579199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7e548f4109245b4d3d68767b83de82ac836ac9d5cc1bc081a219d32dbbeda54`  
		Last Modified: Wed, 05 Oct 2022 08:13:34 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:697369682782d1b2dbc043f43ca3316b0db3fa9ea73f7db3dbc467bac02eb162`  
		Last Modified: Wed, 05 Oct 2022 08:13:34 GMT  
		Size: 312.1 KB (312059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dfb70795c00f40a530881bffe5c831e6db14159082a026ea6998712e348984a`  
		Last Modified: Wed, 05 Oct 2022 08:13:35 GMT  
		Size: 1.2 MB (1199286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:476c14bf2670ef65dcc686dfa808de6890eff3c4910ef826bb7faf2291852c8e`  
		Last Modified: Wed, 05 Oct 2022 08:13:34 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d568980c19cf77318fcb8d77bacb59d6693b433e7181df0f3caef176b52a3191`  
		Last Modified: Wed, 05 Oct 2022 08:13:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:d3f458555a9a339d16f76ef8013aa925929005de7217194985f7efa465554cad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31445121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6406224fb2a1c7a535f7f3e81b89efa7325ae81d6b21d9d6bc5d27f41395d88a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:05:55 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 03:05:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:05:59 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 03:06:00 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 03:08:31 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 03:08:33 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 03:08:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 03:08:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 03:08:35 GMT
USER memcache
# Wed, 05 Oct 2022 03:08:36 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 03:08:37 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d51bfc33abb0dd79aa4c51b1f9c4cfd1190791ddeea14d61e1b8e5f5d996da7`  
		Last Modified: Wed, 05 Oct 2022 03:09:28 GMT  
		Size: 4.9 KB (4907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e37070a0cb39b1adff15bff570c77cd0bbe4459d214fc5722701da4f7c5b402`  
		Last Modified: Wed, 05 Oct 2022 03:09:29 GMT  
		Size: 119.3 KB (119254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078e83a26c52c9ff73f62179ba3a9b4b9cdbe0d927d4245a2f3c14d96d909d11`  
		Last Modified: Wed, 05 Oct 2022 03:09:29 GMT  
		Size: 1.3 MB (1256157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f353bbcc7b933af6761691a3ba35fb1b80b182162960769306c81729487de9cf`  
		Last Modified: Wed, 05 Oct 2022 03:09:29 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78a605409bcc6452727b4f53d4b26811dcdc8b176a88c568b56302f9e39ff85`  
		Last Modified: Wed, 05 Oct 2022 03:09:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; 386

```console
$ docker pull memcached@sha256:95ab1613d2fcc9c5a7eba541a7dfb13495fa99b5d77d4656da4630b78bf74c5a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33785263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93de9a3d72d17c99080504de246a0b51465565d26793ad487cd2908476723333`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Oct 2022 23:39:40 GMT
ADD file:a66b7a182260a23fdb8b219600a8b48a5079997715006d9a5324dda11f9d0a7f in / 
# Tue, 04 Oct 2022 23:39:41 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:12:48 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 13:12:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:12:53 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 13:12:54 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 13:15:47 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 13:15:48 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 13:15:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 13:15:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 13:15:50 GMT
USER memcache
# Wed, 05 Oct 2022 13:15:51 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 13:15:52 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:711839e532aa3f129f9cfaa5125d0e379ddefd47f3da44d0674372663dfc6a9b`  
		Last Modified: Tue, 04 Oct 2022 23:45:35 GMT  
		Size: 32.4 MB (32396290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5161f80d1df63217fef9b1a73e067a92d04f472d1a4ba002103da6e1689201d2`  
		Last Modified: Wed, 05 Oct 2022 13:16:41 GMT  
		Size: 4.8 KB (4775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b8ca938e3262650de875a82b51d5429ed32858924ed01f31e08823a0110f78`  
		Last Modified: Wed, 05 Oct 2022 13:16:41 GMT  
		Size: 130.1 KB (130128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d56431e1a0c892213dfd9a453e3575db72680db48a6aed437295e181498ae6c7`  
		Last Modified: Wed, 05 Oct 2022 13:16:42 GMT  
		Size: 1.3 MB (1253663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47362ecff01e4b5783c28f0a1024c21cbacf2f17b789860e4ebf99773898229a`  
		Last Modified: Wed, 05 Oct 2022 13:16:41 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f86c83c1049b01f43ae03975626a66ecb9eae0281599db499528892e30e0269f`  
		Last Modified: Wed, 05 Oct 2022 13:16:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; mips64le

```console
$ docker pull memcached@sha256:922b5312101767b2b3fc81590e722b5e79a729452b4f0edd17a5d792aa90e1b2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31015160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ec29f9e0c7858b09669119d800f2569a6a8e381808abe1a3989aa060c7a64ea`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 05 Oct 2022 00:10:26 GMT
ADD file:48da6b2f4e0315e4f502001a00e4b2abb58d553de11a41901ba859a461052bea in / 
# Wed, 05 Oct 2022 00:10:29 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:59:00 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 03:59:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:59:18 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 03:59:21 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 04:06:17 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 04:06:19 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 04:06:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 04:06:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 04:06:29 GMT
USER memcache
# Wed, 05 Oct 2022 04:06:31 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 04:06:34 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3288c6e2e7130a1e313203f049bde0e57a05237441a3cab92c27f9ada139315b`  
		Last Modified: Wed, 05 Oct 2022 00:18:36 GMT  
		Size: 29.6 MB (29640851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaef4f8453620b9cc82968e1dbf1ed98c0e4c5e897da9cd2e4d5bc26601ef1d0`  
		Last Modified: Wed, 05 Oct 2022 04:06:52 GMT  
		Size: 4.9 KB (4864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcbc6cec97a2b18b7caa64c38f40669eb923898edf6757612abf69036cc94a9c`  
		Last Modified: Wed, 05 Oct 2022 04:06:52 GMT  
		Size: 117.2 KB (117176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b83a324f1ad5c2d5e153fcf42024969d9bbaea8df56221c47b2dcccade28696`  
		Last Modified: Wed, 05 Oct 2022 04:06:52 GMT  
		Size: 1.3 MB (1251861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f20f84bbdb83e24c72fda0fed4ef0cf58b3eee6e4f05b5f4c745e1dfb4779199`  
		Last Modified: Wed, 05 Oct 2022 04:06:52 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f4cdf4ad864d232b858c0042bc2537f61833806ddf7781642c27f0ba8c58fd`  
		Last Modified: Wed, 05 Oct 2022 04:06:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; ppc64le

```console
$ docker pull memcached@sha256:5843450835c3de77b73d275c84981ff40a8921d2fd8f63df29f20779afd4b011
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36977018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ac10fdcf830775d9abecef20325a6db9befca7259adb12da3754bd79025d14d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Oct 2022 23:18:04 GMT
ADD file:66a0f55a4b4dfbb5d64082ffdb24751f20c5773039277ba278fdb4ce4a538c33 in / 
# Tue, 04 Oct 2022 23:18:06 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 08:58:03 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 08:58:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 08:58:10 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 08:58:11 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 09:01:22 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 09:01:23 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 09:01:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 09:01:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 09:01:25 GMT
USER memcache
# Wed, 05 Oct 2022 09:01:25 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 09:01:25 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:4e001127162dd884a6f7bd2e6f74215816d325bebb3a374ae9fcee9f038f99b8`  
		Last Modified: Tue, 04 Oct 2022 23:24:13 GMT  
		Size: 35.3 MB (35290584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c333c30cea960d51a0fca6f30a61ffd7bc4ec7e6711905a2875c17661de45833`  
		Last Modified: Wed, 05 Oct 2022 09:02:24 GMT  
		Size: 5.0 KB (4981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de7f9617e3f96516ad14767e6645f8cccf14aabe76c9617293d3dbdb8d1d5013`  
		Last Modified: Wed, 05 Oct 2022 09:02:24 GMT  
		Size: 356.9 KB (356918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2668fc82899be9101fab61482fe66b640b92efae057ee88cfe0604cf0c08c270`  
		Last Modified: Wed, 05 Oct 2022 09:02:24 GMT  
		Size: 1.3 MB (1324127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617887de59cd713ef92f5af550338f216d62b3a52ff11d3db7437ae4a977677d`  
		Last Modified: Wed, 05 Oct 2022 09:02:24 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f391b42bfd5493f7f0a5e4702ef212bcbcd630dc98069b371f54008e52d555`  
		Last Modified: Wed, 05 Oct 2022 09:02:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; s390x

```console
$ docker pull memcached@sha256:a68d861d39d508e157bfec89650683c443e38e085c0bb686efd1c6f6fb771090
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31221752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f8e5591d33ad149aa1fcea8466745b9018322eb538b330f198f2a24b9b67325`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Oct 2022 23:42:42 GMT
ADD file:7acfe92be51da9cffeb5b063cc87926d1ce457729e3080de340603a38216a708 in / 
# Tue, 04 Oct 2022 23:42:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:21:53 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 01:21:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:21:56 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 01:21:56 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 01:25:31 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 01:25:31 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 01:25:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 01:25:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 01:25:32 GMT
USER memcache
# Wed, 05 Oct 2022 01:25:32 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 01:25:32 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:62990b94a520bfcf718ec711f8444f83c536af2c83c8e53fdfe1f89fdcb79826`  
		Last Modified: Tue, 04 Oct 2022 23:47:16 GMT  
		Size: 29.7 MB (29650719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e75be154924807ecff182be8b52f82593e3ac5c84f4834226f410139f250562`  
		Last Modified: Wed, 05 Oct 2022 01:26:23 GMT  
		Size: 5.0 KB (5027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c6fcd517c09d146d86a8ab0c84e0cb87c39b6d5aa6a5e4f7c2027005bc6c03`  
		Last Modified: Wed, 05 Oct 2022 01:26:23 GMT  
		Size: 324.2 KB (324212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c83fd7ffcf78cdd0c4e1cee3843ffea027ce70f87c997960ea0e14823194a62`  
		Last Modified: Wed, 05 Oct 2022 01:26:23 GMT  
		Size: 1.2 MB (1241387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b6ed6acfc224f832786cfe50858117e0ff11e69d4dfe846f50143f9479e37e`  
		Last Modified: Wed, 05 Oct 2022 01:26:23 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ebd5ba7dabf6f7077666fa277c434e6f23a6614e4dc4d5706bd30dbb2f3d80a`  
		Last Modified: Wed, 05 Oct 2022 01:26:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6-alpine`

```console
$ docker pull memcached@sha256:d1d0f8424d9564a6d28b20d441b221294ab09e586d3666e7d3329c811ac3f322
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
$ docker pull memcached@sha256:d7f1053070f1020a4fc773523705c1494bfb1edf25edf24459c81418bcddb2bf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3868456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98356558fb5c650e049187d5fbc075b7d1548df209aff29dedc7202e925ea665`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:53:39 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 09 Aug 2022 20:53:40 GMT
RUN apk add --no-cache libsasl
# Mon, 29 Aug 2022 19:59:54 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 19:59:54 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 20:02:37 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Mon, 29 Aug 2022 20:02:37 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 20:02:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 20:02:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 20:02:38 GMT
USER memcache
# Mon, 29 Aug 2022 20:02:38 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 20:02:38 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d572ef57cdf8eb58de4b4e89970c5e64c6a2f8470bbbe4746efd56927df10611`  
		Last Modified: Tue, 09 Aug 2022 20:57:08 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed8976416286665206f17c9c2ead879425c6c6c62051fa7af308abd8790c0bc`  
		Last Modified: Tue, 09 Aug 2022 20:57:08 GMT  
		Size: 108.3 KB (108322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb81a082d3307bee25bd754b44c17e3423ace86257a27e62b6492be54e6c04b3`  
		Last Modified: Mon, 29 Aug 2022 20:03:30 GMT  
		Size: 952.4 KB (952408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f0efad04b524c1b9e6115b5481dc72c9ee037e65e86b42ae61f40eb5c079b8`  
		Last Modified: Mon, 29 Aug 2022 20:03:30 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963603084de81044b37f07eb6489013949af1ab497be7ace91dd5087c64d70ce`  
		Last Modified: Mon, 29 Aug 2022 20:03:29 GMT  
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
$ docker pull memcached@sha256:fe60e76484846f910192b2d5165415ba111c556789233c183ed18880187b5fed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3758619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc1d52e69bd83adcebc7479ed25934dbd29eb32cb68b338dd65aff944de86398`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:48:03 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 09 Aug 2022 20:48:05 GMT
RUN apk add --no-cache libsasl
# Mon, 29 Aug 2022 18:51:54 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 18:51:54 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 18:54:31 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Mon, 29 Aug 2022 18:54:33 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 18:54:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 18:54:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 18:54:35 GMT
USER memcache
# Mon, 29 Aug 2022 18:54:36 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 18:54:37 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d15db589ad12df2825238bc4f6832b2c6e3d991704c9b41db7865df5d402276`  
		Last Modified: Tue, 09 Aug 2022 20:51:50 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:103b4be7608736e9e24d225ccd97cc4dfad6bacbe7bcf2ca1cd716b45ee32855`  
		Last Modified: Tue, 09 Aug 2022 20:51:50 GMT  
		Size: 109.6 KB (109566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0212e668a84adeaf525aa82fe864ac8b57acb1950c67b38f17d4007d9f9bebbf`  
		Last Modified: Mon, 29 Aug 2022 18:55:51 GMT  
		Size: 939.7 KB (939742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8a69ef314b91110c98f842b3d141768e666cf4673f4414320521338faf28d6`  
		Last Modified: Mon, 29 Aug 2022 18:55:51 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d868394810ccf1649fee843c3a0588a6775265a67dec4936a32a8ee769205eb`  
		Last Modified: Mon, 29 Aug 2022 18:55:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; 386

```console
$ docker pull memcached@sha256:562b7a7602fbdc8c555c997346529640986f1a70c5310d0e7ac7ee5be5004134
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3891424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cf987911cc9f370d9a02fd24e09b38ac92f856013a58e52ae8e1e242e8f115d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:39 GMT
ADD file:b828bc14bc5ff03c8f7310fe0aed6ac5df19a393622d5d1d779a523234d07c0a in / 
# Tue, 09 Aug 2022 17:38:39 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:31:11 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 06 Oct 2022 20:31:12 GMT
RUN apk add --no-cache libsasl
# Thu, 06 Oct 2022 20:31:13 GMT
ENV MEMCACHED_VERSION=1.6.17
# Thu, 06 Oct 2022 20:31:14 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Thu, 06 Oct 2022 20:34:15 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 06 Oct 2022 20:34:17 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 06 Oct 2022 20:34:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 06 Oct 2022 20:34:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 20:34:19 GMT
USER memcache
# Thu, 06 Oct 2022 20:34:20 GMT
EXPOSE 11211
# Thu, 06 Oct 2022 20:34:21 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6c0d3b419d848ea31ca748254611d5d5ce3b76e3d7bba520fd87400fbb75f3b9`  
		Last Modified: Tue, 09 Aug 2022 17:39:33 GMT  
		Size: 2.8 MB (2807121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c5cf4da7d47a1675ec754c4abb2f8aed348ebb76a41a3feea34b6737965077`  
		Last Modified: Thu, 06 Oct 2022 20:35:16 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd19825385b793f75ea8e660e1a32ba82a67f889d2f0fa17286da02efcc7c82`  
		Last Modified: Thu, 06 Oct 2022 20:35:17 GMT  
		Size: 119.8 KB (119834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23144451377b23ee74c09325785c2d9979f0d546d9114753499726be49f0ac35`  
		Last Modified: Thu, 06 Oct 2022 20:35:17 GMT  
		Size: 962.8 KB (962822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9862d0ec769de46de1bc8c01602342b1bbb1d2b834cf3a1aeaaa013bfebbe42c`  
		Last Modified: Thu, 06 Oct 2022 20:35:16 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28aee3d7b7e60049b472288f76c206e4acab742797abacdae0d146f1b1c987be`  
		Last Modified: Thu, 06 Oct 2022 20:35:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:933ee3008de5fff45556eed8f813dbe28c638669e4f1fae22228f1d4ae97fa5d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3913068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c35abea284c9fdadf80277c4e589f260436f39426d12485ae9fd06c66e0cab6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:58:36 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 06 Oct 2022 20:58:39 GMT
RUN apk add --no-cache libsasl
# Thu, 06 Oct 2022 20:58:39 GMT
ENV MEMCACHED_VERSION=1.6.17
# Thu, 06 Oct 2022 20:58:40 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Thu, 06 Oct 2022 21:01:52 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 06 Oct 2022 21:01:52 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 06 Oct 2022 21:01:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 06 Oct 2022 21:01:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 21:01:54 GMT
USER memcache
# Thu, 06 Oct 2022 21:01:55 GMT
EXPOSE 11211
# Thu, 06 Oct 2022 21:01:55 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a4950a8cc87dd9e5ec07268592148771ee6a96b270c2ad0cd2de4ff7b00c1a`  
		Last Modified: Thu, 06 Oct 2022 21:02:46 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c992ad9a080419adb465c5ddd18a317cb7342af149a0deab2c2c7d15bd087442`  
		Last Modified: Thu, 06 Oct 2022 21:02:47 GMT  
		Size: 126.1 KB (126070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6091cffcf047d57d7b51ecc08c3dd0d176f21102199ec0e24ee40257b838287`  
		Last Modified: Thu, 06 Oct 2022 21:02:47 GMT  
		Size: 982.0 KB (982000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b1b52d56e86ac7b75aec7089c33a24d031a269242ee0fdc7a9929f955ecbecd`  
		Last Modified: Thu, 06 Oct 2022 21:02:46 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73885207a86618904bca9142334c74041f4658a7023f9a68e109a24a4dfbfae7`  
		Last Modified: Thu, 06 Oct 2022 21:02:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; s390x

```console
$ docker pull memcached@sha256:409d3e4b8b0de5fc4e5c9f070c5496a99e2d030c2772647bb04095fe6f0757f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3646992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b6a4697fa6b2f43f9e85db112952c4b5ff69b3c9bf3ebcdf7905a11785815b5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:45:36 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 06 Oct 2022 20:45:38 GMT
RUN apk add --no-cache libsasl
# Thu, 06 Oct 2022 20:45:39 GMT
ENV MEMCACHED_VERSION=1.6.17
# Thu, 06 Oct 2022 20:45:39 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Thu, 06 Oct 2022 20:49:59 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 06 Oct 2022 20:49:59 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 06 Oct 2022 20:50:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 06 Oct 2022 20:50:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 20:50:00 GMT
USER memcache
# Thu, 06 Oct 2022 20:50:00 GMT
EXPOSE 11211
# Thu, 06 Oct 2022 20:50:01 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb7a4b531f98c3a90954f542da5d7028ec87d1ee2a74467d087d237d1a5cb62`  
		Last Modified: Thu, 06 Oct 2022 20:50:54 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:248a438b0a1fd089205148ab101aaf2457c55967afad4e042339958b0c1b6b50`  
		Last Modified: Thu, 06 Oct 2022 20:50:54 GMT  
		Size: 112.5 KB (112508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:467a2ab9413d162f0d6b5e65207d0adc2e4d105f9d4a8c3ada6852bf1c5c7e35`  
		Last Modified: Thu, 06 Oct 2022 20:50:54 GMT  
		Size: 942.2 KB (942214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20d843cc1cc32f57f16bc13ab2c98e20dc0fa2b80303702cfce0cdd39a64e4d`  
		Last Modified: Thu, 06 Oct 2022 20:50:54 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b936f167ac6d6abd85c1ebe43c570c4ce1725b0cc4b912ac38a6164606562dc4`  
		Last Modified: Thu, 06 Oct 2022 20:50:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6-alpine3.16`

```console
$ docker pull memcached@sha256:304980979f6f7d6e650ad82ab73d6b64a96c1b32800508b5c2afd9bb5341167c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1.6-alpine3.16` - linux; amd64

```console
$ docker pull memcached@sha256:d7f1053070f1020a4fc773523705c1494bfb1edf25edf24459c81418bcddb2bf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3868456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98356558fb5c650e049187d5fbc075b7d1548df209aff29dedc7202e925ea665`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:53:39 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 09 Aug 2022 20:53:40 GMT
RUN apk add --no-cache libsasl
# Mon, 29 Aug 2022 19:59:54 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 19:59:54 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 20:02:37 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Mon, 29 Aug 2022 20:02:37 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 20:02:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 20:02:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 20:02:38 GMT
USER memcache
# Mon, 29 Aug 2022 20:02:38 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 20:02:38 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d572ef57cdf8eb58de4b4e89970c5e64c6a2f8470bbbe4746efd56927df10611`  
		Last Modified: Tue, 09 Aug 2022 20:57:08 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed8976416286665206f17c9c2ead879425c6c6c62051fa7af308abd8790c0bc`  
		Last Modified: Tue, 09 Aug 2022 20:57:08 GMT  
		Size: 108.3 KB (108322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb81a082d3307bee25bd754b44c17e3423ace86257a27e62b6492be54e6c04b3`  
		Last Modified: Mon, 29 Aug 2022 20:03:30 GMT  
		Size: 952.4 KB (952408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f0efad04b524c1b9e6115b5481dc72c9ee037e65e86b42ae61f40eb5c079b8`  
		Last Modified: Mon, 29 Aug 2022 20:03:30 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963603084de81044b37f07eb6489013949af1ab497be7ace91dd5087c64d70ce`  
		Last Modified: Mon, 29 Aug 2022 20:03:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:fe60e76484846f910192b2d5165415ba111c556789233c183ed18880187b5fed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3758619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc1d52e69bd83adcebc7479ed25934dbd29eb32cb68b338dd65aff944de86398`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:48:03 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 09 Aug 2022 20:48:05 GMT
RUN apk add --no-cache libsasl
# Mon, 29 Aug 2022 18:51:54 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 18:51:54 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 18:54:31 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Mon, 29 Aug 2022 18:54:33 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 18:54:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 18:54:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 18:54:35 GMT
USER memcache
# Mon, 29 Aug 2022 18:54:36 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 18:54:37 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d15db589ad12df2825238bc4f6832b2c6e3d991704c9b41db7865df5d402276`  
		Last Modified: Tue, 09 Aug 2022 20:51:50 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:103b4be7608736e9e24d225ccd97cc4dfad6bacbe7bcf2ca1cd716b45ee32855`  
		Last Modified: Tue, 09 Aug 2022 20:51:50 GMT  
		Size: 109.6 KB (109566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0212e668a84adeaf525aa82fe864ac8b57acb1950c67b38f17d4007d9f9bebbf`  
		Last Modified: Mon, 29 Aug 2022 18:55:51 GMT  
		Size: 939.7 KB (939742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8a69ef314b91110c98f842b3d141768e666cf4673f4414320521338faf28d6`  
		Last Modified: Mon, 29 Aug 2022 18:55:51 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d868394810ccf1649fee843c3a0588a6775265a67dec4936a32a8ee769205eb`  
		Last Modified: Mon, 29 Aug 2022 18:55:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine3.16` - linux; 386

```console
$ docker pull memcached@sha256:562b7a7602fbdc8c555c997346529640986f1a70c5310d0e7ac7ee5be5004134
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3891424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cf987911cc9f370d9a02fd24e09b38ac92f856013a58e52ae8e1e242e8f115d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:39 GMT
ADD file:b828bc14bc5ff03c8f7310fe0aed6ac5df19a393622d5d1d779a523234d07c0a in / 
# Tue, 09 Aug 2022 17:38:39 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:31:11 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 06 Oct 2022 20:31:12 GMT
RUN apk add --no-cache libsasl
# Thu, 06 Oct 2022 20:31:13 GMT
ENV MEMCACHED_VERSION=1.6.17
# Thu, 06 Oct 2022 20:31:14 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Thu, 06 Oct 2022 20:34:15 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 06 Oct 2022 20:34:17 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 06 Oct 2022 20:34:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 06 Oct 2022 20:34:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 20:34:19 GMT
USER memcache
# Thu, 06 Oct 2022 20:34:20 GMT
EXPOSE 11211
# Thu, 06 Oct 2022 20:34:21 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6c0d3b419d848ea31ca748254611d5d5ce3b76e3d7bba520fd87400fbb75f3b9`  
		Last Modified: Tue, 09 Aug 2022 17:39:33 GMT  
		Size: 2.8 MB (2807121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c5cf4da7d47a1675ec754c4abb2f8aed348ebb76a41a3feea34b6737965077`  
		Last Modified: Thu, 06 Oct 2022 20:35:16 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd19825385b793f75ea8e660e1a32ba82a67f889d2f0fa17286da02efcc7c82`  
		Last Modified: Thu, 06 Oct 2022 20:35:17 GMT  
		Size: 119.8 KB (119834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23144451377b23ee74c09325785c2d9979f0d546d9114753499726be49f0ac35`  
		Last Modified: Thu, 06 Oct 2022 20:35:17 GMT  
		Size: 962.8 KB (962822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9862d0ec769de46de1bc8c01602342b1bbb1d2b834cf3a1aeaaa013bfebbe42c`  
		Last Modified: Thu, 06 Oct 2022 20:35:16 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28aee3d7b7e60049b472288f76c206e4acab742797abacdae0d146f1b1c987be`  
		Last Modified: Thu, 06 Oct 2022 20:35:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine3.16` - linux; ppc64le

```console
$ docker pull memcached@sha256:933ee3008de5fff45556eed8f813dbe28c638669e4f1fae22228f1d4ae97fa5d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3913068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c35abea284c9fdadf80277c4e589f260436f39426d12485ae9fd06c66e0cab6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:58:36 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 06 Oct 2022 20:58:39 GMT
RUN apk add --no-cache libsasl
# Thu, 06 Oct 2022 20:58:39 GMT
ENV MEMCACHED_VERSION=1.6.17
# Thu, 06 Oct 2022 20:58:40 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Thu, 06 Oct 2022 21:01:52 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 06 Oct 2022 21:01:52 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 06 Oct 2022 21:01:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 06 Oct 2022 21:01:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 21:01:54 GMT
USER memcache
# Thu, 06 Oct 2022 21:01:55 GMT
EXPOSE 11211
# Thu, 06 Oct 2022 21:01:55 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a4950a8cc87dd9e5ec07268592148771ee6a96b270c2ad0cd2de4ff7b00c1a`  
		Last Modified: Thu, 06 Oct 2022 21:02:46 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c992ad9a080419adb465c5ddd18a317cb7342af149a0deab2c2c7d15bd087442`  
		Last Modified: Thu, 06 Oct 2022 21:02:47 GMT  
		Size: 126.1 KB (126070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6091cffcf047d57d7b51ecc08c3dd0d176f21102199ec0e24ee40257b838287`  
		Last Modified: Thu, 06 Oct 2022 21:02:47 GMT  
		Size: 982.0 KB (982000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b1b52d56e86ac7b75aec7089c33a24d031a269242ee0fdc7a9929f955ecbecd`  
		Last Modified: Thu, 06 Oct 2022 21:02:46 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73885207a86618904bca9142334c74041f4658a7023f9a68e109a24a4dfbfae7`  
		Last Modified: Thu, 06 Oct 2022 21:02:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine3.16` - linux; s390x

```console
$ docker pull memcached@sha256:409d3e4b8b0de5fc4e5c9f070c5496a99e2d030c2772647bb04095fe6f0757f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3646992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b6a4697fa6b2f43f9e85db112952c4b5ff69b3c9bf3ebcdf7905a11785815b5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:45:36 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 06 Oct 2022 20:45:38 GMT
RUN apk add --no-cache libsasl
# Thu, 06 Oct 2022 20:45:39 GMT
ENV MEMCACHED_VERSION=1.6.17
# Thu, 06 Oct 2022 20:45:39 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Thu, 06 Oct 2022 20:49:59 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 06 Oct 2022 20:49:59 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 06 Oct 2022 20:50:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 06 Oct 2022 20:50:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 20:50:00 GMT
USER memcache
# Thu, 06 Oct 2022 20:50:00 GMT
EXPOSE 11211
# Thu, 06 Oct 2022 20:50:01 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb7a4b531f98c3a90954f542da5d7028ec87d1ee2a74467d087d237d1a5cb62`  
		Last Modified: Thu, 06 Oct 2022 20:50:54 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:248a438b0a1fd089205148ab101aaf2457c55967afad4e042339958b0c1b6b50`  
		Last Modified: Thu, 06 Oct 2022 20:50:54 GMT  
		Size: 112.5 KB (112508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:467a2ab9413d162f0d6b5e65207d0adc2e4d105f9d4a8c3ada6852bf1c5c7e35`  
		Last Modified: Thu, 06 Oct 2022 20:50:54 GMT  
		Size: 942.2 KB (942214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20d843cc1cc32f57f16bc13ab2c98e20dc0fa2b80303702cfce0cdd39a64e4d`  
		Last Modified: Thu, 06 Oct 2022 20:50:54 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b936f167ac6d6abd85c1ebe43c570c4ce1725b0cc4b912ac38a6164606562dc4`  
		Last Modified: Thu, 06 Oct 2022 20:50:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6-bullseye`

```console
$ docker pull memcached@sha256:32b63986179511a820e33f0335381897731f15c802aa1d2707e9891aca1403a5
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
$ docker pull memcached@sha256:931b3d5a0c377a1ffba03d7692e157961e2802cd2fe528801182e80b099fcad8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (33009876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bdad48377094436fa7ba308ceb1b2bbce918630232e753085668b4e28281114`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:39 GMT
ADD file:b78b777208be08edd8f297035cdfbacddb45170ad778fd643c792ee045187e39 in / 
# Tue, 04 Oct 2022 23:26:39 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:17:54 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 04:17:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:17:57 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 04:17:57 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 04:20:39 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 04:20:39 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 04:20:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 04:20:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 04:20:40 GMT
USER memcache
# Wed, 05 Oct 2022 04:20:40 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 04:20:40 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:bd159e379b3b1bc0134341e4ffdeab5f966ec422ae04818bb69ecef08a823b05`  
		Last Modified: Tue, 04 Oct 2022 23:30:54 GMT  
		Size: 31.4 MB (31420102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ba15a7daa0d15e5ba45e9a9fdc332fce5b82c224ba42834aea059a6f245cf0`  
		Last Modified: Wed, 05 Oct 2022 04:21:07 GMT  
		Size: 5.0 KB (4983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7285127ceb5872fecb20531ce255b227f193cf0f6fceec79c876e4b8ebff29be`  
		Last Modified: Wed, 05 Oct 2022 04:21:08 GMT  
		Size: 328.1 KB (328117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e838e946498e1c28405bc1ae35d0fb6dafb97f0f47a462256719329c40afe865`  
		Last Modified: Wed, 05 Oct 2022 04:21:08 GMT  
		Size: 1.3 MB (1256265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd912af099a0b3bb0a430c2768ef0d784cab1d86924c157e945a751e12670e1d`  
		Last Modified: Wed, 05 Oct 2022 04:21:07 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60814b5c0f0d9e77d568f57890e62e11d94773423f772a3120117016d0de3294`  
		Last Modified: Wed, 05 Oct 2022 04:21:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bullseye` - linux; arm variant v5

```console
$ docker pull memcached@sha256:a84f9fc0812c5f2e6d4575b277b7421022c21829d34d89128c0058f22caf890e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30467657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:449c07e8773b5918abc8cf6d2542c0f1a102b52a38606808b8c1365296278cbc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Oct 2022 23:49:11 GMT
ADD file:effb9e2e2f8c7539e1a2200d069a2592e8ba20c9d034b5a73fbf173b6987193c in / 
# Tue, 04 Oct 2022 23:49:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:53:06 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 01:53:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:53:12 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 01:53:12 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 01:59:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 01:59:12 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 01:59:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 01:59:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 01:59:13 GMT
USER memcache
# Wed, 05 Oct 2022 01:59:13 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 01:59:13 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:7b9558bbfd8050a8e6af6e60560101c49bd53f81df6fa068419b44d028e465eb`  
		Last Modified: Tue, 04 Oct 2022 23:53:54 GMT  
		Size: 28.9 MB (28918381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f7663872748bf22ac651be2e08927fdd98e08f447cb7bcc3862ff485c6d5ddd`  
		Last Modified: Wed, 05 Oct 2022 01:59:52 GMT  
		Size: 4.9 KB (4897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b071b414257fa2a96433371bc4d51ce61fdac16c63b3f3c5e55c9818fa0529f`  
		Last Modified: Wed, 05 Oct 2022 01:59:52 GMT  
		Size: 316.6 KB (316627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f813defd9f0615e613628e02e7dadc2cbecc6b31ae8151aefb81d6a72922c9`  
		Last Modified: Wed, 05 Oct 2022 01:59:52 GMT  
		Size: 1.2 MB (1227346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb16c09a595afd6523b77641de3a45962bd09b125d8ba26b64c7ce6a17137a63`  
		Last Modified: Wed, 05 Oct 2022 01:59:52 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c54c4bbaf374145c3304bfe33479e0b53e0047102ae2488c8190de918a16e3e1`  
		Last Modified: Wed, 05 Oct 2022 01:59:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bullseye` - linux; arm variant v7

```console
$ docker pull memcached@sha256:c809ce19f7998cea0a39f8a4d06573b6f886a9c98b5da65ebb6efb13e8886d5e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28095847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9ba6ef519428019c76007d4e4e34b0d8e293799d94f152576aeb3a23fca1d0a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Oct 2022 23:58:46 GMT
ADD file:ca1bf27f17594a91224a252bd446f97c3b898210c571f2f26fa2e723d2bf521e in / 
# Tue, 04 Oct 2022 23:58:46 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 05:07:01 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 05:07:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 05:07:05 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 05:07:05 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 05:12:39 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 05:12:39 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 05:12:39 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 05:12:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 05:12:39 GMT
USER memcache
# Wed, 05 Oct 2022 05:12:39 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 05:12:40 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2bc64aeac2e429577e497affc8a416d2fc59158aa967f07aced793368e19455f`  
		Last Modified: Wed, 05 Oct 2022 00:05:09 GMT  
		Size: 26.6 MB (26579199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7e548f4109245b4d3d68767b83de82ac836ac9d5cc1bc081a219d32dbbeda54`  
		Last Modified: Wed, 05 Oct 2022 08:13:34 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:697369682782d1b2dbc043f43ca3316b0db3fa9ea73f7db3dbc467bac02eb162`  
		Last Modified: Wed, 05 Oct 2022 08:13:34 GMT  
		Size: 312.1 KB (312059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dfb70795c00f40a530881bffe5c831e6db14159082a026ea6998712e348984a`  
		Last Modified: Wed, 05 Oct 2022 08:13:35 GMT  
		Size: 1.2 MB (1199286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:476c14bf2670ef65dcc686dfa808de6890eff3c4910ef826bb7faf2291852c8e`  
		Last Modified: Wed, 05 Oct 2022 08:13:34 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d568980c19cf77318fcb8d77bacb59d6693b433e7181df0f3caef176b52a3191`  
		Last Modified: Wed, 05 Oct 2022 08:13:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bullseye` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:d3f458555a9a339d16f76ef8013aa925929005de7217194985f7efa465554cad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31445121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6406224fb2a1c7a535f7f3e81b89efa7325ae81d6b21d9d6bc5d27f41395d88a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:05:55 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 03:05:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:05:59 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 03:06:00 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 03:08:31 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 03:08:33 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 03:08:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 03:08:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 03:08:35 GMT
USER memcache
# Wed, 05 Oct 2022 03:08:36 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 03:08:37 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d51bfc33abb0dd79aa4c51b1f9c4cfd1190791ddeea14d61e1b8e5f5d996da7`  
		Last Modified: Wed, 05 Oct 2022 03:09:28 GMT  
		Size: 4.9 KB (4907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e37070a0cb39b1adff15bff570c77cd0bbe4459d214fc5722701da4f7c5b402`  
		Last Modified: Wed, 05 Oct 2022 03:09:29 GMT  
		Size: 119.3 KB (119254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078e83a26c52c9ff73f62179ba3a9b4b9cdbe0d927d4245a2f3c14d96d909d11`  
		Last Modified: Wed, 05 Oct 2022 03:09:29 GMT  
		Size: 1.3 MB (1256157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f353bbcc7b933af6761691a3ba35fb1b80b182162960769306c81729487de9cf`  
		Last Modified: Wed, 05 Oct 2022 03:09:29 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78a605409bcc6452727b4f53d4b26811dcdc8b176a88c568b56302f9e39ff85`  
		Last Modified: Wed, 05 Oct 2022 03:09:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bullseye` - linux; 386

```console
$ docker pull memcached@sha256:95ab1613d2fcc9c5a7eba541a7dfb13495fa99b5d77d4656da4630b78bf74c5a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33785263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93de9a3d72d17c99080504de246a0b51465565d26793ad487cd2908476723333`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Oct 2022 23:39:40 GMT
ADD file:a66b7a182260a23fdb8b219600a8b48a5079997715006d9a5324dda11f9d0a7f in / 
# Tue, 04 Oct 2022 23:39:41 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:12:48 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 13:12:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:12:53 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 13:12:54 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 13:15:47 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 13:15:48 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 13:15:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 13:15:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 13:15:50 GMT
USER memcache
# Wed, 05 Oct 2022 13:15:51 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 13:15:52 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:711839e532aa3f129f9cfaa5125d0e379ddefd47f3da44d0674372663dfc6a9b`  
		Last Modified: Tue, 04 Oct 2022 23:45:35 GMT  
		Size: 32.4 MB (32396290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5161f80d1df63217fef9b1a73e067a92d04f472d1a4ba002103da6e1689201d2`  
		Last Modified: Wed, 05 Oct 2022 13:16:41 GMT  
		Size: 4.8 KB (4775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b8ca938e3262650de875a82b51d5429ed32858924ed01f31e08823a0110f78`  
		Last Modified: Wed, 05 Oct 2022 13:16:41 GMT  
		Size: 130.1 KB (130128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d56431e1a0c892213dfd9a453e3575db72680db48a6aed437295e181498ae6c7`  
		Last Modified: Wed, 05 Oct 2022 13:16:42 GMT  
		Size: 1.3 MB (1253663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47362ecff01e4b5783c28f0a1024c21cbacf2f17b789860e4ebf99773898229a`  
		Last Modified: Wed, 05 Oct 2022 13:16:41 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f86c83c1049b01f43ae03975626a66ecb9eae0281599db499528892e30e0269f`  
		Last Modified: Wed, 05 Oct 2022 13:16:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bullseye` - linux; mips64le

```console
$ docker pull memcached@sha256:922b5312101767b2b3fc81590e722b5e79a729452b4f0edd17a5d792aa90e1b2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31015160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ec29f9e0c7858b09669119d800f2569a6a8e381808abe1a3989aa060c7a64ea`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 05 Oct 2022 00:10:26 GMT
ADD file:48da6b2f4e0315e4f502001a00e4b2abb58d553de11a41901ba859a461052bea in / 
# Wed, 05 Oct 2022 00:10:29 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:59:00 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 03:59:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:59:18 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 03:59:21 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 04:06:17 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 04:06:19 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 04:06:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 04:06:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 04:06:29 GMT
USER memcache
# Wed, 05 Oct 2022 04:06:31 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 04:06:34 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3288c6e2e7130a1e313203f049bde0e57a05237441a3cab92c27f9ada139315b`  
		Last Modified: Wed, 05 Oct 2022 00:18:36 GMT  
		Size: 29.6 MB (29640851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaef4f8453620b9cc82968e1dbf1ed98c0e4c5e897da9cd2e4d5bc26601ef1d0`  
		Last Modified: Wed, 05 Oct 2022 04:06:52 GMT  
		Size: 4.9 KB (4864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcbc6cec97a2b18b7caa64c38f40669eb923898edf6757612abf69036cc94a9c`  
		Last Modified: Wed, 05 Oct 2022 04:06:52 GMT  
		Size: 117.2 KB (117176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b83a324f1ad5c2d5e153fcf42024969d9bbaea8df56221c47b2dcccade28696`  
		Last Modified: Wed, 05 Oct 2022 04:06:52 GMT  
		Size: 1.3 MB (1251861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f20f84bbdb83e24c72fda0fed4ef0cf58b3eee6e4f05b5f4c745e1dfb4779199`  
		Last Modified: Wed, 05 Oct 2022 04:06:52 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f4cdf4ad864d232b858c0042bc2537f61833806ddf7781642c27f0ba8c58fd`  
		Last Modified: Wed, 05 Oct 2022 04:06:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bullseye` - linux; ppc64le

```console
$ docker pull memcached@sha256:5843450835c3de77b73d275c84981ff40a8921d2fd8f63df29f20779afd4b011
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36977018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ac10fdcf830775d9abecef20325a6db9befca7259adb12da3754bd79025d14d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Oct 2022 23:18:04 GMT
ADD file:66a0f55a4b4dfbb5d64082ffdb24751f20c5773039277ba278fdb4ce4a538c33 in / 
# Tue, 04 Oct 2022 23:18:06 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 08:58:03 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 08:58:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 08:58:10 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 08:58:11 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 09:01:22 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 09:01:23 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 09:01:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 09:01:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 09:01:25 GMT
USER memcache
# Wed, 05 Oct 2022 09:01:25 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 09:01:25 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:4e001127162dd884a6f7bd2e6f74215816d325bebb3a374ae9fcee9f038f99b8`  
		Last Modified: Tue, 04 Oct 2022 23:24:13 GMT  
		Size: 35.3 MB (35290584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c333c30cea960d51a0fca6f30a61ffd7bc4ec7e6711905a2875c17661de45833`  
		Last Modified: Wed, 05 Oct 2022 09:02:24 GMT  
		Size: 5.0 KB (4981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de7f9617e3f96516ad14767e6645f8cccf14aabe76c9617293d3dbdb8d1d5013`  
		Last Modified: Wed, 05 Oct 2022 09:02:24 GMT  
		Size: 356.9 KB (356918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2668fc82899be9101fab61482fe66b640b92efae057ee88cfe0604cf0c08c270`  
		Last Modified: Wed, 05 Oct 2022 09:02:24 GMT  
		Size: 1.3 MB (1324127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617887de59cd713ef92f5af550338f216d62b3a52ff11d3db7437ae4a977677d`  
		Last Modified: Wed, 05 Oct 2022 09:02:24 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f391b42bfd5493f7f0a5e4702ef212bcbcd630dc98069b371f54008e52d555`  
		Last Modified: Wed, 05 Oct 2022 09:02:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bullseye` - linux; s390x

```console
$ docker pull memcached@sha256:a68d861d39d508e157bfec89650683c443e38e085c0bb686efd1c6f6fb771090
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31221752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f8e5591d33ad149aa1fcea8466745b9018322eb538b330f198f2a24b9b67325`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Oct 2022 23:42:42 GMT
ADD file:7acfe92be51da9cffeb5b063cc87926d1ce457729e3080de340603a38216a708 in / 
# Tue, 04 Oct 2022 23:42:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:21:53 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 01:21:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:21:56 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 01:21:56 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 01:25:31 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 01:25:31 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 01:25:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 01:25:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 01:25:32 GMT
USER memcache
# Wed, 05 Oct 2022 01:25:32 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 01:25:32 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:62990b94a520bfcf718ec711f8444f83c536af2c83c8e53fdfe1f89fdcb79826`  
		Last Modified: Tue, 04 Oct 2022 23:47:16 GMT  
		Size: 29.7 MB (29650719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e75be154924807ecff182be8b52f82593e3ac5c84f4834226f410139f250562`  
		Last Modified: Wed, 05 Oct 2022 01:26:23 GMT  
		Size: 5.0 KB (5027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c6fcd517c09d146d86a8ab0c84e0cb87c39b6d5aa6a5e4f7c2027005bc6c03`  
		Last Modified: Wed, 05 Oct 2022 01:26:23 GMT  
		Size: 324.2 KB (324212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c83fd7ffcf78cdd0c4e1cee3843ffea027ce70f87c997960ea0e14823194a62`  
		Last Modified: Wed, 05 Oct 2022 01:26:23 GMT  
		Size: 1.2 MB (1241387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b6ed6acfc224f832786cfe50858117e0ff11e69d4dfe846f50143f9479e37e`  
		Last Modified: Wed, 05 Oct 2022 01:26:23 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ebd5ba7dabf6f7077666fa277c434e6f23a6614e4dc4d5706bd30dbb2f3d80a`  
		Last Modified: Wed, 05 Oct 2022 01:26:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.17`

```console
$ docker pull memcached@sha256:32b63986179511a820e33f0335381897731f15c802aa1d2707e9891aca1403a5
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

### `memcached:1.6.17` - linux; amd64

```console
$ docker pull memcached@sha256:931b3d5a0c377a1ffba03d7692e157961e2802cd2fe528801182e80b099fcad8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (33009876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bdad48377094436fa7ba308ceb1b2bbce918630232e753085668b4e28281114`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:39 GMT
ADD file:b78b777208be08edd8f297035cdfbacddb45170ad778fd643c792ee045187e39 in / 
# Tue, 04 Oct 2022 23:26:39 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:17:54 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 04:17:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:17:57 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 04:17:57 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 04:20:39 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 04:20:39 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 04:20:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 04:20:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 04:20:40 GMT
USER memcache
# Wed, 05 Oct 2022 04:20:40 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 04:20:40 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:bd159e379b3b1bc0134341e4ffdeab5f966ec422ae04818bb69ecef08a823b05`  
		Last Modified: Tue, 04 Oct 2022 23:30:54 GMT  
		Size: 31.4 MB (31420102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ba15a7daa0d15e5ba45e9a9fdc332fce5b82c224ba42834aea059a6f245cf0`  
		Last Modified: Wed, 05 Oct 2022 04:21:07 GMT  
		Size: 5.0 KB (4983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7285127ceb5872fecb20531ce255b227f193cf0f6fceec79c876e4b8ebff29be`  
		Last Modified: Wed, 05 Oct 2022 04:21:08 GMT  
		Size: 328.1 KB (328117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e838e946498e1c28405bc1ae35d0fb6dafb97f0f47a462256719329c40afe865`  
		Last Modified: Wed, 05 Oct 2022 04:21:08 GMT  
		Size: 1.3 MB (1256265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd912af099a0b3bb0a430c2768ef0d784cab1d86924c157e945a751e12670e1d`  
		Last Modified: Wed, 05 Oct 2022 04:21:07 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60814b5c0f0d9e77d568f57890e62e11d94773423f772a3120117016d0de3294`  
		Last Modified: Wed, 05 Oct 2022 04:21:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.17` - linux; arm variant v5

```console
$ docker pull memcached@sha256:a84f9fc0812c5f2e6d4575b277b7421022c21829d34d89128c0058f22caf890e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30467657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:449c07e8773b5918abc8cf6d2542c0f1a102b52a38606808b8c1365296278cbc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Oct 2022 23:49:11 GMT
ADD file:effb9e2e2f8c7539e1a2200d069a2592e8ba20c9d034b5a73fbf173b6987193c in / 
# Tue, 04 Oct 2022 23:49:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:53:06 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 01:53:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:53:12 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 01:53:12 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 01:59:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 01:59:12 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 01:59:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 01:59:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 01:59:13 GMT
USER memcache
# Wed, 05 Oct 2022 01:59:13 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 01:59:13 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:7b9558bbfd8050a8e6af6e60560101c49bd53f81df6fa068419b44d028e465eb`  
		Last Modified: Tue, 04 Oct 2022 23:53:54 GMT  
		Size: 28.9 MB (28918381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f7663872748bf22ac651be2e08927fdd98e08f447cb7bcc3862ff485c6d5ddd`  
		Last Modified: Wed, 05 Oct 2022 01:59:52 GMT  
		Size: 4.9 KB (4897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b071b414257fa2a96433371bc4d51ce61fdac16c63b3f3c5e55c9818fa0529f`  
		Last Modified: Wed, 05 Oct 2022 01:59:52 GMT  
		Size: 316.6 KB (316627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f813defd9f0615e613628e02e7dadc2cbecc6b31ae8151aefb81d6a72922c9`  
		Last Modified: Wed, 05 Oct 2022 01:59:52 GMT  
		Size: 1.2 MB (1227346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb16c09a595afd6523b77641de3a45962bd09b125d8ba26b64c7ce6a17137a63`  
		Last Modified: Wed, 05 Oct 2022 01:59:52 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c54c4bbaf374145c3304bfe33479e0b53e0047102ae2488c8190de918a16e3e1`  
		Last Modified: Wed, 05 Oct 2022 01:59:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.17` - linux; arm variant v7

```console
$ docker pull memcached@sha256:c809ce19f7998cea0a39f8a4d06573b6f886a9c98b5da65ebb6efb13e8886d5e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28095847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9ba6ef519428019c76007d4e4e34b0d8e293799d94f152576aeb3a23fca1d0a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Oct 2022 23:58:46 GMT
ADD file:ca1bf27f17594a91224a252bd446f97c3b898210c571f2f26fa2e723d2bf521e in / 
# Tue, 04 Oct 2022 23:58:46 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 05:07:01 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 05:07:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 05:07:05 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 05:07:05 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 05:12:39 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 05:12:39 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 05:12:39 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 05:12:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 05:12:39 GMT
USER memcache
# Wed, 05 Oct 2022 05:12:39 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 05:12:40 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2bc64aeac2e429577e497affc8a416d2fc59158aa967f07aced793368e19455f`  
		Last Modified: Wed, 05 Oct 2022 00:05:09 GMT  
		Size: 26.6 MB (26579199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7e548f4109245b4d3d68767b83de82ac836ac9d5cc1bc081a219d32dbbeda54`  
		Last Modified: Wed, 05 Oct 2022 08:13:34 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:697369682782d1b2dbc043f43ca3316b0db3fa9ea73f7db3dbc467bac02eb162`  
		Last Modified: Wed, 05 Oct 2022 08:13:34 GMT  
		Size: 312.1 KB (312059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dfb70795c00f40a530881bffe5c831e6db14159082a026ea6998712e348984a`  
		Last Modified: Wed, 05 Oct 2022 08:13:35 GMT  
		Size: 1.2 MB (1199286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:476c14bf2670ef65dcc686dfa808de6890eff3c4910ef826bb7faf2291852c8e`  
		Last Modified: Wed, 05 Oct 2022 08:13:34 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d568980c19cf77318fcb8d77bacb59d6693b433e7181df0f3caef176b52a3191`  
		Last Modified: Wed, 05 Oct 2022 08:13:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.17` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:d3f458555a9a339d16f76ef8013aa925929005de7217194985f7efa465554cad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31445121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6406224fb2a1c7a535f7f3e81b89efa7325ae81d6b21d9d6bc5d27f41395d88a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:05:55 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 03:05:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:05:59 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 03:06:00 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 03:08:31 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 03:08:33 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 03:08:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 03:08:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 03:08:35 GMT
USER memcache
# Wed, 05 Oct 2022 03:08:36 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 03:08:37 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d51bfc33abb0dd79aa4c51b1f9c4cfd1190791ddeea14d61e1b8e5f5d996da7`  
		Last Modified: Wed, 05 Oct 2022 03:09:28 GMT  
		Size: 4.9 KB (4907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e37070a0cb39b1adff15bff570c77cd0bbe4459d214fc5722701da4f7c5b402`  
		Last Modified: Wed, 05 Oct 2022 03:09:29 GMT  
		Size: 119.3 KB (119254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078e83a26c52c9ff73f62179ba3a9b4b9cdbe0d927d4245a2f3c14d96d909d11`  
		Last Modified: Wed, 05 Oct 2022 03:09:29 GMT  
		Size: 1.3 MB (1256157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f353bbcc7b933af6761691a3ba35fb1b80b182162960769306c81729487de9cf`  
		Last Modified: Wed, 05 Oct 2022 03:09:29 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78a605409bcc6452727b4f53d4b26811dcdc8b176a88c568b56302f9e39ff85`  
		Last Modified: Wed, 05 Oct 2022 03:09:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.17` - linux; 386

```console
$ docker pull memcached@sha256:95ab1613d2fcc9c5a7eba541a7dfb13495fa99b5d77d4656da4630b78bf74c5a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33785263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93de9a3d72d17c99080504de246a0b51465565d26793ad487cd2908476723333`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Oct 2022 23:39:40 GMT
ADD file:a66b7a182260a23fdb8b219600a8b48a5079997715006d9a5324dda11f9d0a7f in / 
# Tue, 04 Oct 2022 23:39:41 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:12:48 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 13:12:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:12:53 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 13:12:54 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 13:15:47 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 13:15:48 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 13:15:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 13:15:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 13:15:50 GMT
USER memcache
# Wed, 05 Oct 2022 13:15:51 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 13:15:52 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:711839e532aa3f129f9cfaa5125d0e379ddefd47f3da44d0674372663dfc6a9b`  
		Last Modified: Tue, 04 Oct 2022 23:45:35 GMT  
		Size: 32.4 MB (32396290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5161f80d1df63217fef9b1a73e067a92d04f472d1a4ba002103da6e1689201d2`  
		Last Modified: Wed, 05 Oct 2022 13:16:41 GMT  
		Size: 4.8 KB (4775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b8ca938e3262650de875a82b51d5429ed32858924ed01f31e08823a0110f78`  
		Last Modified: Wed, 05 Oct 2022 13:16:41 GMT  
		Size: 130.1 KB (130128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d56431e1a0c892213dfd9a453e3575db72680db48a6aed437295e181498ae6c7`  
		Last Modified: Wed, 05 Oct 2022 13:16:42 GMT  
		Size: 1.3 MB (1253663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47362ecff01e4b5783c28f0a1024c21cbacf2f17b789860e4ebf99773898229a`  
		Last Modified: Wed, 05 Oct 2022 13:16:41 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f86c83c1049b01f43ae03975626a66ecb9eae0281599db499528892e30e0269f`  
		Last Modified: Wed, 05 Oct 2022 13:16:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.17` - linux; mips64le

```console
$ docker pull memcached@sha256:922b5312101767b2b3fc81590e722b5e79a729452b4f0edd17a5d792aa90e1b2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31015160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ec29f9e0c7858b09669119d800f2569a6a8e381808abe1a3989aa060c7a64ea`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 05 Oct 2022 00:10:26 GMT
ADD file:48da6b2f4e0315e4f502001a00e4b2abb58d553de11a41901ba859a461052bea in / 
# Wed, 05 Oct 2022 00:10:29 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:59:00 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 03:59:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:59:18 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 03:59:21 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 04:06:17 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 04:06:19 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 04:06:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 04:06:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 04:06:29 GMT
USER memcache
# Wed, 05 Oct 2022 04:06:31 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 04:06:34 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3288c6e2e7130a1e313203f049bde0e57a05237441a3cab92c27f9ada139315b`  
		Last Modified: Wed, 05 Oct 2022 00:18:36 GMT  
		Size: 29.6 MB (29640851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaef4f8453620b9cc82968e1dbf1ed98c0e4c5e897da9cd2e4d5bc26601ef1d0`  
		Last Modified: Wed, 05 Oct 2022 04:06:52 GMT  
		Size: 4.9 KB (4864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcbc6cec97a2b18b7caa64c38f40669eb923898edf6757612abf69036cc94a9c`  
		Last Modified: Wed, 05 Oct 2022 04:06:52 GMT  
		Size: 117.2 KB (117176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b83a324f1ad5c2d5e153fcf42024969d9bbaea8df56221c47b2dcccade28696`  
		Last Modified: Wed, 05 Oct 2022 04:06:52 GMT  
		Size: 1.3 MB (1251861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f20f84bbdb83e24c72fda0fed4ef0cf58b3eee6e4f05b5f4c745e1dfb4779199`  
		Last Modified: Wed, 05 Oct 2022 04:06:52 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f4cdf4ad864d232b858c0042bc2537f61833806ddf7781642c27f0ba8c58fd`  
		Last Modified: Wed, 05 Oct 2022 04:06:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.17` - linux; ppc64le

```console
$ docker pull memcached@sha256:5843450835c3de77b73d275c84981ff40a8921d2fd8f63df29f20779afd4b011
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36977018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ac10fdcf830775d9abecef20325a6db9befca7259adb12da3754bd79025d14d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Oct 2022 23:18:04 GMT
ADD file:66a0f55a4b4dfbb5d64082ffdb24751f20c5773039277ba278fdb4ce4a538c33 in / 
# Tue, 04 Oct 2022 23:18:06 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 08:58:03 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 08:58:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 08:58:10 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 08:58:11 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 09:01:22 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 09:01:23 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 09:01:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 09:01:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 09:01:25 GMT
USER memcache
# Wed, 05 Oct 2022 09:01:25 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 09:01:25 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:4e001127162dd884a6f7bd2e6f74215816d325bebb3a374ae9fcee9f038f99b8`  
		Last Modified: Tue, 04 Oct 2022 23:24:13 GMT  
		Size: 35.3 MB (35290584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c333c30cea960d51a0fca6f30a61ffd7bc4ec7e6711905a2875c17661de45833`  
		Last Modified: Wed, 05 Oct 2022 09:02:24 GMT  
		Size: 5.0 KB (4981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de7f9617e3f96516ad14767e6645f8cccf14aabe76c9617293d3dbdb8d1d5013`  
		Last Modified: Wed, 05 Oct 2022 09:02:24 GMT  
		Size: 356.9 KB (356918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2668fc82899be9101fab61482fe66b640b92efae057ee88cfe0604cf0c08c270`  
		Last Modified: Wed, 05 Oct 2022 09:02:24 GMT  
		Size: 1.3 MB (1324127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617887de59cd713ef92f5af550338f216d62b3a52ff11d3db7437ae4a977677d`  
		Last Modified: Wed, 05 Oct 2022 09:02:24 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f391b42bfd5493f7f0a5e4702ef212bcbcd630dc98069b371f54008e52d555`  
		Last Modified: Wed, 05 Oct 2022 09:02:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.17` - linux; s390x

```console
$ docker pull memcached@sha256:a68d861d39d508e157bfec89650683c443e38e085c0bb686efd1c6f6fb771090
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31221752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f8e5591d33ad149aa1fcea8466745b9018322eb538b330f198f2a24b9b67325`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Oct 2022 23:42:42 GMT
ADD file:7acfe92be51da9cffeb5b063cc87926d1ce457729e3080de340603a38216a708 in / 
# Tue, 04 Oct 2022 23:42:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:21:53 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 01:21:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:21:56 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 01:21:56 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 01:25:31 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 01:25:31 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 01:25:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 01:25:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 01:25:32 GMT
USER memcache
# Wed, 05 Oct 2022 01:25:32 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 01:25:32 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:62990b94a520bfcf718ec711f8444f83c536af2c83c8e53fdfe1f89fdcb79826`  
		Last Modified: Tue, 04 Oct 2022 23:47:16 GMT  
		Size: 29.7 MB (29650719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e75be154924807ecff182be8b52f82593e3ac5c84f4834226f410139f250562`  
		Last Modified: Wed, 05 Oct 2022 01:26:23 GMT  
		Size: 5.0 KB (5027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c6fcd517c09d146d86a8ab0c84e0cb87c39b6d5aa6a5e4f7c2027005bc6c03`  
		Last Modified: Wed, 05 Oct 2022 01:26:23 GMT  
		Size: 324.2 KB (324212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c83fd7ffcf78cdd0c4e1cee3843ffea027ce70f87c997960ea0e14823194a62`  
		Last Modified: Wed, 05 Oct 2022 01:26:23 GMT  
		Size: 1.2 MB (1241387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b6ed6acfc224f832786cfe50858117e0ff11e69d4dfe846f50143f9479e37e`  
		Last Modified: Wed, 05 Oct 2022 01:26:23 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ebd5ba7dabf6f7077666fa277c434e6f23a6614e4dc4d5706bd30dbb2f3d80a`  
		Last Modified: Wed, 05 Oct 2022 01:26:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.17-alpine`

```console
$ docker pull memcached@sha256:304980979f6f7d6e650ad82ab73d6b64a96c1b32800508b5c2afd9bb5341167c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1.6.17-alpine` - linux; amd64

```console
$ docker pull memcached@sha256:d7f1053070f1020a4fc773523705c1494bfb1edf25edf24459c81418bcddb2bf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3868456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98356558fb5c650e049187d5fbc075b7d1548df209aff29dedc7202e925ea665`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:53:39 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 09 Aug 2022 20:53:40 GMT
RUN apk add --no-cache libsasl
# Mon, 29 Aug 2022 19:59:54 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 19:59:54 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 20:02:37 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Mon, 29 Aug 2022 20:02:37 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 20:02:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 20:02:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 20:02:38 GMT
USER memcache
# Mon, 29 Aug 2022 20:02:38 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 20:02:38 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d572ef57cdf8eb58de4b4e89970c5e64c6a2f8470bbbe4746efd56927df10611`  
		Last Modified: Tue, 09 Aug 2022 20:57:08 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed8976416286665206f17c9c2ead879425c6c6c62051fa7af308abd8790c0bc`  
		Last Modified: Tue, 09 Aug 2022 20:57:08 GMT  
		Size: 108.3 KB (108322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb81a082d3307bee25bd754b44c17e3423ace86257a27e62b6492be54e6c04b3`  
		Last Modified: Mon, 29 Aug 2022 20:03:30 GMT  
		Size: 952.4 KB (952408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f0efad04b524c1b9e6115b5481dc72c9ee037e65e86b42ae61f40eb5c079b8`  
		Last Modified: Mon, 29 Aug 2022 20:03:30 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963603084de81044b37f07eb6489013949af1ab497be7ace91dd5087c64d70ce`  
		Last Modified: Mon, 29 Aug 2022 20:03:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.17-alpine` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:fe60e76484846f910192b2d5165415ba111c556789233c183ed18880187b5fed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3758619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc1d52e69bd83adcebc7479ed25934dbd29eb32cb68b338dd65aff944de86398`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:48:03 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 09 Aug 2022 20:48:05 GMT
RUN apk add --no-cache libsasl
# Mon, 29 Aug 2022 18:51:54 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 18:51:54 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 18:54:31 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Mon, 29 Aug 2022 18:54:33 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 18:54:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 18:54:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 18:54:35 GMT
USER memcache
# Mon, 29 Aug 2022 18:54:36 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 18:54:37 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d15db589ad12df2825238bc4f6832b2c6e3d991704c9b41db7865df5d402276`  
		Last Modified: Tue, 09 Aug 2022 20:51:50 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:103b4be7608736e9e24d225ccd97cc4dfad6bacbe7bcf2ca1cd716b45ee32855`  
		Last Modified: Tue, 09 Aug 2022 20:51:50 GMT  
		Size: 109.6 KB (109566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0212e668a84adeaf525aa82fe864ac8b57acb1950c67b38f17d4007d9f9bebbf`  
		Last Modified: Mon, 29 Aug 2022 18:55:51 GMT  
		Size: 939.7 KB (939742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8a69ef314b91110c98f842b3d141768e666cf4673f4414320521338faf28d6`  
		Last Modified: Mon, 29 Aug 2022 18:55:51 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d868394810ccf1649fee843c3a0588a6775265a67dec4936a32a8ee769205eb`  
		Last Modified: Mon, 29 Aug 2022 18:55:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.17-alpine` - linux; 386

```console
$ docker pull memcached@sha256:562b7a7602fbdc8c555c997346529640986f1a70c5310d0e7ac7ee5be5004134
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3891424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cf987911cc9f370d9a02fd24e09b38ac92f856013a58e52ae8e1e242e8f115d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:39 GMT
ADD file:b828bc14bc5ff03c8f7310fe0aed6ac5df19a393622d5d1d779a523234d07c0a in / 
# Tue, 09 Aug 2022 17:38:39 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:31:11 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 06 Oct 2022 20:31:12 GMT
RUN apk add --no-cache libsasl
# Thu, 06 Oct 2022 20:31:13 GMT
ENV MEMCACHED_VERSION=1.6.17
# Thu, 06 Oct 2022 20:31:14 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Thu, 06 Oct 2022 20:34:15 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 06 Oct 2022 20:34:17 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 06 Oct 2022 20:34:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 06 Oct 2022 20:34:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 20:34:19 GMT
USER memcache
# Thu, 06 Oct 2022 20:34:20 GMT
EXPOSE 11211
# Thu, 06 Oct 2022 20:34:21 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6c0d3b419d848ea31ca748254611d5d5ce3b76e3d7bba520fd87400fbb75f3b9`  
		Last Modified: Tue, 09 Aug 2022 17:39:33 GMT  
		Size: 2.8 MB (2807121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c5cf4da7d47a1675ec754c4abb2f8aed348ebb76a41a3feea34b6737965077`  
		Last Modified: Thu, 06 Oct 2022 20:35:16 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd19825385b793f75ea8e660e1a32ba82a67f889d2f0fa17286da02efcc7c82`  
		Last Modified: Thu, 06 Oct 2022 20:35:17 GMT  
		Size: 119.8 KB (119834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23144451377b23ee74c09325785c2d9979f0d546d9114753499726be49f0ac35`  
		Last Modified: Thu, 06 Oct 2022 20:35:17 GMT  
		Size: 962.8 KB (962822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9862d0ec769de46de1bc8c01602342b1bbb1d2b834cf3a1aeaaa013bfebbe42c`  
		Last Modified: Thu, 06 Oct 2022 20:35:16 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28aee3d7b7e60049b472288f76c206e4acab742797abacdae0d146f1b1c987be`  
		Last Modified: Thu, 06 Oct 2022 20:35:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.17-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:933ee3008de5fff45556eed8f813dbe28c638669e4f1fae22228f1d4ae97fa5d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3913068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c35abea284c9fdadf80277c4e589f260436f39426d12485ae9fd06c66e0cab6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:58:36 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 06 Oct 2022 20:58:39 GMT
RUN apk add --no-cache libsasl
# Thu, 06 Oct 2022 20:58:39 GMT
ENV MEMCACHED_VERSION=1.6.17
# Thu, 06 Oct 2022 20:58:40 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Thu, 06 Oct 2022 21:01:52 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 06 Oct 2022 21:01:52 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 06 Oct 2022 21:01:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 06 Oct 2022 21:01:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 21:01:54 GMT
USER memcache
# Thu, 06 Oct 2022 21:01:55 GMT
EXPOSE 11211
# Thu, 06 Oct 2022 21:01:55 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a4950a8cc87dd9e5ec07268592148771ee6a96b270c2ad0cd2de4ff7b00c1a`  
		Last Modified: Thu, 06 Oct 2022 21:02:46 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c992ad9a080419adb465c5ddd18a317cb7342af149a0deab2c2c7d15bd087442`  
		Last Modified: Thu, 06 Oct 2022 21:02:47 GMT  
		Size: 126.1 KB (126070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6091cffcf047d57d7b51ecc08c3dd0d176f21102199ec0e24ee40257b838287`  
		Last Modified: Thu, 06 Oct 2022 21:02:47 GMT  
		Size: 982.0 KB (982000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b1b52d56e86ac7b75aec7089c33a24d031a269242ee0fdc7a9929f955ecbecd`  
		Last Modified: Thu, 06 Oct 2022 21:02:46 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73885207a86618904bca9142334c74041f4658a7023f9a68e109a24a4dfbfae7`  
		Last Modified: Thu, 06 Oct 2022 21:02:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.17-alpine` - linux; s390x

```console
$ docker pull memcached@sha256:409d3e4b8b0de5fc4e5c9f070c5496a99e2d030c2772647bb04095fe6f0757f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3646992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b6a4697fa6b2f43f9e85db112952c4b5ff69b3c9bf3ebcdf7905a11785815b5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:45:36 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 06 Oct 2022 20:45:38 GMT
RUN apk add --no-cache libsasl
# Thu, 06 Oct 2022 20:45:39 GMT
ENV MEMCACHED_VERSION=1.6.17
# Thu, 06 Oct 2022 20:45:39 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Thu, 06 Oct 2022 20:49:59 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 06 Oct 2022 20:49:59 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 06 Oct 2022 20:50:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 06 Oct 2022 20:50:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 20:50:00 GMT
USER memcache
# Thu, 06 Oct 2022 20:50:00 GMT
EXPOSE 11211
# Thu, 06 Oct 2022 20:50:01 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb7a4b531f98c3a90954f542da5d7028ec87d1ee2a74467d087d237d1a5cb62`  
		Last Modified: Thu, 06 Oct 2022 20:50:54 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:248a438b0a1fd089205148ab101aaf2457c55967afad4e042339958b0c1b6b50`  
		Last Modified: Thu, 06 Oct 2022 20:50:54 GMT  
		Size: 112.5 KB (112508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:467a2ab9413d162f0d6b5e65207d0adc2e4d105f9d4a8c3ada6852bf1c5c7e35`  
		Last Modified: Thu, 06 Oct 2022 20:50:54 GMT  
		Size: 942.2 KB (942214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20d843cc1cc32f57f16bc13ab2c98e20dc0fa2b80303702cfce0cdd39a64e4d`  
		Last Modified: Thu, 06 Oct 2022 20:50:54 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b936f167ac6d6abd85c1ebe43c570c4ce1725b0cc4b912ac38a6164606562dc4`  
		Last Modified: Thu, 06 Oct 2022 20:50:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.17-alpine3.16`

```console
$ docker pull memcached@sha256:304980979f6f7d6e650ad82ab73d6b64a96c1b32800508b5c2afd9bb5341167c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1.6.17-alpine3.16` - linux; amd64

```console
$ docker pull memcached@sha256:d7f1053070f1020a4fc773523705c1494bfb1edf25edf24459c81418bcddb2bf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3868456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98356558fb5c650e049187d5fbc075b7d1548df209aff29dedc7202e925ea665`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:53:39 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 09 Aug 2022 20:53:40 GMT
RUN apk add --no-cache libsasl
# Mon, 29 Aug 2022 19:59:54 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 19:59:54 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 20:02:37 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Mon, 29 Aug 2022 20:02:37 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 20:02:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 20:02:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 20:02:38 GMT
USER memcache
# Mon, 29 Aug 2022 20:02:38 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 20:02:38 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d572ef57cdf8eb58de4b4e89970c5e64c6a2f8470bbbe4746efd56927df10611`  
		Last Modified: Tue, 09 Aug 2022 20:57:08 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed8976416286665206f17c9c2ead879425c6c6c62051fa7af308abd8790c0bc`  
		Last Modified: Tue, 09 Aug 2022 20:57:08 GMT  
		Size: 108.3 KB (108322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb81a082d3307bee25bd754b44c17e3423ace86257a27e62b6492be54e6c04b3`  
		Last Modified: Mon, 29 Aug 2022 20:03:30 GMT  
		Size: 952.4 KB (952408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f0efad04b524c1b9e6115b5481dc72c9ee037e65e86b42ae61f40eb5c079b8`  
		Last Modified: Mon, 29 Aug 2022 20:03:30 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963603084de81044b37f07eb6489013949af1ab497be7ace91dd5087c64d70ce`  
		Last Modified: Mon, 29 Aug 2022 20:03:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.17-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:fe60e76484846f910192b2d5165415ba111c556789233c183ed18880187b5fed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3758619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc1d52e69bd83adcebc7479ed25934dbd29eb32cb68b338dd65aff944de86398`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:48:03 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 09 Aug 2022 20:48:05 GMT
RUN apk add --no-cache libsasl
# Mon, 29 Aug 2022 18:51:54 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 18:51:54 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 18:54:31 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Mon, 29 Aug 2022 18:54:33 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 18:54:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 18:54:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 18:54:35 GMT
USER memcache
# Mon, 29 Aug 2022 18:54:36 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 18:54:37 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d15db589ad12df2825238bc4f6832b2c6e3d991704c9b41db7865df5d402276`  
		Last Modified: Tue, 09 Aug 2022 20:51:50 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:103b4be7608736e9e24d225ccd97cc4dfad6bacbe7bcf2ca1cd716b45ee32855`  
		Last Modified: Tue, 09 Aug 2022 20:51:50 GMT  
		Size: 109.6 KB (109566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0212e668a84adeaf525aa82fe864ac8b57acb1950c67b38f17d4007d9f9bebbf`  
		Last Modified: Mon, 29 Aug 2022 18:55:51 GMT  
		Size: 939.7 KB (939742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8a69ef314b91110c98f842b3d141768e666cf4673f4414320521338faf28d6`  
		Last Modified: Mon, 29 Aug 2022 18:55:51 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d868394810ccf1649fee843c3a0588a6775265a67dec4936a32a8ee769205eb`  
		Last Modified: Mon, 29 Aug 2022 18:55:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.17-alpine3.16` - linux; 386

```console
$ docker pull memcached@sha256:562b7a7602fbdc8c555c997346529640986f1a70c5310d0e7ac7ee5be5004134
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3891424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cf987911cc9f370d9a02fd24e09b38ac92f856013a58e52ae8e1e242e8f115d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:39 GMT
ADD file:b828bc14bc5ff03c8f7310fe0aed6ac5df19a393622d5d1d779a523234d07c0a in / 
# Tue, 09 Aug 2022 17:38:39 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:31:11 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 06 Oct 2022 20:31:12 GMT
RUN apk add --no-cache libsasl
# Thu, 06 Oct 2022 20:31:13 GMT
ENV MEMCACHED_VERSION=1.6.17
# Thu, 06 Oct 2022 20:31:14 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Thu, 06 Oct 2022 20:34:15 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 06 Oct 2022 20:34:17 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 06 Oct 2022 20:34:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 06 Oct 2022 20:34:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 20:34:19 GMT
USER memcache
# Thu, 06 Oct 2022 20:34:20 GMT
EXPOSE 11211
# Thu, 06 Oct 2022 20:34:21 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6c0d3b419d848ea31ca748254611d5d5ce3b76e3d7bba520fd87400fbb75f3b9`  
		Last Modified: Tue, 09 Aug 2022 17:39:33 GMT  
		Size: 2.8 MB (2807121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c5cf4da7d47a1675ec754c4abb2f8aed348ebb76a41a3feea34b6737965077`  
		Last Modified: Thu, 06 Oct 2022 20:35:16 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd19825385b793f75ea8e660e1a32ba82a67f889d2f0fa17286da02efcc7c82`  
		Last Modified: Thu, 06 Oct 2022 20:35:17 GMT  
		Size: 119.8 KB (119834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23144451377b23ee74c09325785c2d9979f0d546d9114753499726be49f0ac35`  
		Last Modified: Thu, 06 Oct 2022 20:35:17 GMT  
		Size: 962.8 KB (962822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9862d0ec769de46de1bc8c01602342b1bbb1d2b834cf3a1aeaaa013bfebbe42c`  
		Last Modified: Thu, 06 Oct 2022 20:35:16 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28aee3d7b7e60049b472288f76c206e4acab742797abacdae0d146f1b1c987be`  
		Last Modified: Thu, 06 Oct 2022 20:35:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.17-alpine3.16` - linux; ppc64le

```console
$ docker pull memcached@sha256:933ee3008de5fff45556eed8f813dbe28c638669e4f1fae22228f1d4ae97fa5d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3913068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c35abea284c9fdadf80277c4e589f260436f39426d12485ae9fd06c66e0cab6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:58:36 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 06 Oct 2022 20:58:39 GMT
RUN apk add --no-cache libsasl
# Thu, 06 Oct 2022 20:58:39 GMT
ENV MEMCACHED_VERSION=1.6.17
# Thu, 06 Oct 2022 20:58:40 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Thu, 06 Oct 2022 21:01:52 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 06 Oct 2022 21:01:52 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 06 Oct 2022 21:01:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 06 Oct 2022 21:01:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 21:01:54 GMT
USER memcache
# Thu, 06 Oct 2022 21:01:55 GMT
EXPOSE 11211
# Thu, 06 Oct 2022 21:01:55 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a4950a8cc87dd9e5ec07268592148771ee6a96b270c2ad0cd2de4ff7b00c1a`  
		Last Modified: Thu, 06 Oct 2022 21:02:46 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c992ad9a080419adb465c5ddd18a317cb7342af149a0deab2c2c7d15bd087442`  
		Last Modified: Thu, 06 Oct 2022 21:02:47 GMT  
		Size: 126.1 KB (126070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6091cffcf047d57d7b51ecc08c3dd0d176f21102199ec0e24ee40257b838287`  
		Last Modified: Thu, 06 Oct 2022 21:02:47 GMT  
		Size: 982.0 KB (982000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b1b52d56e86ac7b75aec7089c33a24d031a269242ee0fdc7a9929f955ecbecd`  
		Last Modified: Thu, 06 Oct 2022 21:02:46 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73885207a86618904bca9142334c74041f4658a7023f9a68e109a24a4dfbfae7`  
		Last Modified: Thu, 06 Oct 2022 21:02:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.17-alpine3.16` - linux; s390x

```console
$ docker pull memcached@sha256:409d3e4b8b0de5fc4e5c9f070c5496a99e2d030c2772647bb04095fe6f0757f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3646992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b6a4697fa6b2f43f9e85db112952c4b5ff69b3c9bf3ebcdf7905a11785815b5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:45:36 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 06 Oct 2022 20:45:38 GMT
RUN apk add --no-cache libsasl
# Thu, 06 Oct 2022 20:45:39 GMT
ENV MEMCACHED_VERSION=1.6.17
# Thu, 06 Oct 2022 20:45:39 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Thu, 06 Oct 2022 20:49:59 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 06 Oct 2022 20:49:59 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 06 Oct 2022 20:50:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 06 Oct 2022 20:50:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 20:50:00 GMT
USER memcache
# Thu, 06 Oct 2022 20:50:00 GMT
EXPOSE 11211
# Thu, 06 Oct 2022 20:50:01 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb7a4b531f98c3a90954f542da5d7028ec87d1ee2a74467d087d237d1a5cb62`  
		Last Modified: Thu, 06 Oct 2022 20:50:54 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:248a438b0a1fd089205148ab101aaf2457c55967afad4e042339958b0c1b6b50`  
		Last Modified: Thu, 06 Oct 2022 20:50:54 GMT  
		Size: 112.5 KB (112508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:467a2ab9413d162f0d6b5e65207d0adc2e4d105f9d4a8c3ada6852bf1c5c7e35`  
		Last Modified: Thu, 06 Oct 2022 20:50:54 GMT  
		Size: 942.2 KB (942214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20d843cc1cc32f57f16bc13ab2c98e20dc0fa2b80303702cfce0cdd39a64e4d`  
		Last Modified: Thu, 06 Oct 2022 20:50:54 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b936f167ac6d6abd85c1ebe43c570c4ce1725b0cc4b912ac38a6164606562dc4`  
		Last Modified: Thu, 06 Oct 2022 20:50:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.17-bullseye`

```console
$ docker pull memcached@sha256:32b63986179511a820e33f0335381897731f15c802aa1d2707e9891aca1403a5
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

### `memcached:1.6.17-bullseye` - linux; amd64

```console
$ docker pull memcached@sha256:931b3d5a0c377a1ffba03d7692e157961e2802cd2fe528801182e80b099fcad8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (33009876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bdad48377094436fa7ba308ceb1b2bbce918630232e753085668b4e28281114`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:39 GMT
ADD file:b78b777208be08edd8f297035cdfbacddb45170ad778fd643c792ee045187e39 in / 
# Tue, 04 Oct 2022 23:26:39 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:17:54 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 04:17:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:17:57 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 04:17:57 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 04:20:39 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 04:20:39 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 04:20:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 04:20:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 04:20:40 GMT
USER memcache
# Wed, 05 Oct 2022 04:20:40 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 04:20:40 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:bd159e379b3b1bc0134341e4ffdeab5f966ec422ae04818bb69ecef08a823b05`  
		Last Modified: Tue, 04 Oct 2022 23:30:54 GMT  
		Size: 31.4 MB (31420102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ba15a7daa0d15e5ba45e9a9fdc332fce5b82c224ba42834aea059a6f245cf0`  
		Last Modified: Wed, 05 Oct 2022 04:21:07 GMT  
		Size: 5.0 KB (4983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7285127ceb5872fecb20531ce255b227f193cf0f6fceec79c876e4b8ebff29be`  
		Last Modified: Wed, 05 Oct 2022 04:21:08 GMT  
		Size: 328.1 KB (328117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e838e946498e1c28405bc1ae35d0fb6dafb97f0f47a462256719329c40afe865`  
		Last Modified: Wed, 05 Oct 2022 04:21:08 GMT  
		Size: 1.3 MB (1256265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd912af099a0b3bb0a430c2768ef0d784cab1d86924c157e945a751e12670e1d`  
		Last Modified: Wed, 05 Oct 2022 04:21:07 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60814b5c0f0d9e77d568f57890e62e11d94773423f772a3120117016d0de3294`  
		Last Modified: Wed, 05 Oct 2022 04:21:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.17-bullseye` - linux; arm variant v5

```console
$ docker pull memcached@sha256:a84f9fc0812c5f2e6d4575b277b7421022c21829d34d89128c0058f22caf890e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30467657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:449c07e8773b5918abc8cf6d2542c0f1a102b52a38606808b8c1365296278cbc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Oct 2022 23:49:11 GMT
ADD file:effb9e2e2f8c7539e1a2200d069a2592e8ba20c9d034b5a73fbf173b6987193c in / 
# Tue, 04 Oct 2022 23:49:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:53:06 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 01:53:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:53:12 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 01:53:12 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 01:59:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 01:59:12 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 01:59:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 01:59:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 01:59:13 GMT
USER memcache
# Wed, 05 Oct 2022 01:59:13 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 01:59:13 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:7b9558bbfd8050a8e6af6e60560101c49bd53f81df6fa068419b44d028e465eb`  
		Last Modified: Tue, 04 Oct 2022 23:53:54 GMT  
		Size: 28.9 MB (28918381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f7663872748bf22ac651be2e08927fdd98e08f447cb7bcc3862ff485c6d5ddd`  
		Last Modified: Wed, 05 Oct 2022 01:59:52 GMT  
		Size: 4.9 KB (4897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b071b414257fa2a96433371bc4d51ce61fdac16c63b3f3c5e55c9818fa0529f`  
		Last Modified: Wed, 05 Oct 2022 01:59:52 GMT  
		Size: 316.6 KB (316627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f813defd9f0615e613628e02e7dadc2cbecc6b31ae8151aefb81d6a72922c9`  
		Last Modified: Wed, 05 Oct 2022 01:59:52 GMT  
		Size: 1.2 MB (1227346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb16c09a595afd6523b77641de3a45962bd09b125d8ba26b64c7ce6a17137a63`  
		Last Modified: Wed, 05 Oct 2022 01:59:52 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c54c4bbaf374145c3304bfe33479e0b53e0047102ae2488c8190de918a16e3e1`  
		Last Modified: Wed, 05 Oct 2022 01:59:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.17-bullseye` - linux; arm variant v7

```console
$ docker pull memcached@sha256:c809ce19f7998cea0a39f8a4d06573b6f886a9c98b5da65ebb6efb13e8886d5e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28095847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9ba6ef519428019c76007d4e4e34b0d8e293799d94f152576aeb3a23fca1d0a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Oct 2022 23:58:46 GMT
ADD file:ca1bf27f17594a91224a252bd446f97c3b898210c571f2f26fa2e723d2bf521e in / 
# Tue, 04 Oct 2022 23:58:46 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 05:07:01 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 05:07:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 05:07:05 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 05:07:05 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 05:12:39 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 05:12:39 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 05:12:39 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 05:12:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 05:12:39 GMT
USER memcache
# Wed, 05 Oct 2022 05:12:39 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 05:12:40 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2bc64aeac2e429577e497affc8a416d2fc59158aa967f07aced793368e19455f`  
		Last Modified: Wed, 05 Oct 2022 00:05:09 GMT  
		Size: 26.6 MB (26579199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7e548f4109245b4d3d68767b83de82ac836ac9d5cc1bc081a219d32dbbeda54`  
		Last Modified: Wed, 05 Oct 2022 08:13:34 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:697369682782d1b2dbc043f43ca3316b0db3fa9ea73f7db3dbc467bac02eb162`  
		Last Modified: Wed, 05 Oct 2022 08:13:34 GMT  
		Size: 312.1 KB (312059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dfb70795c00f40a530881bffe5c831e6db14159082a026ea6998712e348984a`  
		Last Modified: Wed, 05 Oct 2022 08:13:35 GMT  
		Size: 1.2 MB (1199286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:476c14bf2670ef65dcc686dfa808de6890eff3c4910ef826bb7faf2291852c8e`  
		Last Modified: Wed, 05 Oct 2022 08:13:34 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d568980c19cf77318fcb8d77bacb59d6693b433e7181df0f3caef176b52a3191`  
		Last Modified: Wed, 05 Oct 2022 08:13:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.17-bullseye` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:d3f458555a9a339d16f76ef8013aa925929005de7217194985f7efa465554cad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31445121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6406224fb2a1c7a535f7f3e81b89efa7325ae81d6b21d9d6bc5d27f41395d88a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:05:55 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 03:05:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:05:59 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 03:06:00 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 03:08:31 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 03:08:33 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 03:08:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 03:08:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 03:08:35 GMT
USER memcache
# Wed, 05 Oct 2022 03:08:36 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 03:08:37 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d51bfc33abb0dd79aa4c51b1f9c4cfd1190791ddeea14d61e1b8e5f5d996da7`  
		Last Modified: Wed, 05 Oct 2022 03:09:28 GMT  
		Size: 4.9 KB (4907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e37070a0cb39b1adff15bff570c77cd0bbe4459d214fc5722701da4f7c5b402`  
		Last Modified: Wed, 05 Oct 2022 03:09:29 GMT  
		Size: 119.3 KB (119254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078e83a26c52c9ff73f62179ba3a9b4b9cdbe0d927d4245a2f3c14d96d909d11`  
		Last Modified: Wed, 05 Oct 2022 03:09:29 GMT  
		Size: 1.3 MB (1256157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f353bbcc7b933af6761691a3ba35fb1b80b182162960769306c81729487de9cf`  
		Last Modified: Wed, 05 Oct 2022 03:09:29 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78a605409bcc6452727b4f53d4b26811dcdc8b176a88c568b56302f9e39ff85`  
		Last Modified: Wed, 05 Oct 2022 03:09:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.17-bullseye` - linux; 386

```console
$ docker pull memcached@sha256:95ab1613d2fcc9c5a7eba541a7dfb13495fa99b5d77d4656da4630b78bf74c5a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33785263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93de9a3d72d17c99080504de246a0b51465565d26793ad487cd2908476723333`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Oct 2022 23:39:40 GMT
ADD file:a66b7a182260a23fdb8b219600a8b48a5079997715006d9a5324dda11f9d0a7f in / 
# Tue, 04 Oct 2022 23:39:41 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:12:48 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 13:12:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:12:53 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 13:12:54 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 13:15:47 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 13:15:48 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 13:15:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 13:15:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 13:15:50 GMT
USER memcache
# Wed, 05 Oct 2022 13:15:51 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 13:15:52 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:711839e532aa3f129f9cfaa5125d0e379ddefd47f3da44d0674372663dfc6a9b`  
		Last Modified: Tue, 04 Oct 2022 23:45:35 GMT  
		Size: 32.4 MB (32396290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5161f80d1df63217fef9b1a73e067a92d04f472d1a4ba002103da6e1689201d2`  
		Last Modified: Wed, 05 Oct 2022 13:16:41 GMT  
		Size: 4.8 KB (4775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b8ca938e3262650de875a82b51d5429ed32858924ed01f31e08823a0110f78`  
		Last Modified: Wed, 05 Oct 2022 13:16:41 GMT  
		Size: 130.1 KB (130128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d56431e1a0c892213dfd9a453e3575db72680db48a6aed437295e181498ae6c7`  
		Last Modified: Wed, 05 Oct 2022 13:16:42 GMT  
		Size: 1.3 MB (1253663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47362ecff01e4b5783c28f0a1024c21cbacf2f17b789860e4ebf99773898229a`  
		Last Modified: Wed, 05 Oct 2022 13:16:41 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f86c83c1049b01f43ae03975626a66ecb9eae0281599db499528892e30e0269f`  
		Last Modified: Wed, 05 Oct 2022 13:16:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.17-bullseye` - linux; mips64le

```console
$ docker pull memcached@sha256:922b5312101767b2b3fc81590e722b5e79a729452b4f0edd17a5d792aa90e1b2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31015160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ec29f9e0c7858b09669119d800f2569a6a8e381808abe1a3989aa060c7a64ea`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 05 Oct 2022 00:10:26 GMT
ADD file:48da6b2f4e0315e4f502001a00e4b2abb58d553de11a41901ba859a461052bea in / 
# Wed, 05 Oct 2022 00:10:29 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:59:00 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 03:59:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:59:18 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 03:59:21 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 04:06:17 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 04:06:19 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 04:06:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 04:06:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 04:06:29 GMT
USER memcache
# Wed, 05 Oct 2022 04:06:31 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 04:06:34 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3288c6e2e7130a1e313203f049bde0e57a05237441a3cab92c27f9ada139315b`  
		Last Modified: Wed, 05 Oct 2022 00:18:36 GMT  
		Size: 29.6 MB (29640851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaef4f8453620b9cc82968e1dbf1ed98c0e4c5e897da9cd2e4d5bc26601ef1d0`  
		Last Modified: Wed, 05 Oct 2022 04:06:52 GMT  
		Size: 4.9 KB (4864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcbc6cec97a2b18b7caa64c38f40669eb923898edf6757612abf69036cc94a9c`  
		Last Modified: Wed, 05 Oct 2022 04:06:52 GMT  
		Size: 117.2 KB (117176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b83a324f1ad5c2d5e153fcf42024969d9bbaea8df56221c47b2dcccade28696`  
		Last Modified: Wed, 05 Oct 2022 04:06:52 GMT  
		Size: 1.3 MB (1251861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f20f84bbdb83e24c72fda0fed4ef0cf58b3eee6e4f05b5f4c745e1dfb4779199`  
		Last Modified: Wed, 05 Oct 2022 04:06:52 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f4cdf4ad864d232b858c0042bc2537f61833806ddf7781642c27f0ba8c58fd`  
		Last Modified: Wed, 05 Oct 2022 04:06:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.17-bullseye` - linux; ppc64le

```console
$ docker pull memcached@sha256:5843450835c3de77b73d275c84981ff40a8921d2fd8f63df29f20779afd4b011
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36977018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ac10fdcf830775d9abecef20325a6db9befca7259adb12da3754bd79025d14d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Oct 2022 23:18:04 GMT
ADD file:66a0f55a4b4dfbb5d64082ffdb24751f20c5773039277ba278fdb4ce4a538c33 in / 
# Tue, 04 Oct 2022 23:18:06 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 08:58:03 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 08:58:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 08:58:10 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 08:58:11 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 09:01:22 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 09:01:23 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 09:01:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 09:01:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 09:01:25 GMT
USER memcache
# Wed, 05 Oct 2022 09:01:25 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 09:01:25 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:4e001127162dd884a6f7bd2e6f74215816d325bebb3a374ae9fcee9f038f99b8`  
		Last Modified: Tue, 04 Oct 2022 23:24:13 GMT  
		Size: 35.3 MB (35290584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c333c30cea960d51a0fca6f30a61ffd7bc4ec7e6711905a2875c17661de45833`  
		Last Modified: Wed, 05 Oct 2022 09:02:24 GMT  
		Size: 5.0 KB (4981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de7f9617e3f96516ad14767e6645f8cccf14aabe76c9617293d3dbdb8d1d5013`  
		Last Modified: Wed, 05 Oct 2022 09:02:24 GMT  
		Size: 356.9 KB (356918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2668fc82899be9101fab61482fe66b640b92efae057ee88cfe0604cf0c08c270`  
		Last Modified: Wed, 05 Oct 2022 09:02:24 GMT  
		Size: 1.3 MB (1324127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617887de59cd713ef92f5af550338f216d62b3a52ff11d3db7437ae4a977677d`  
		Last Modified: Wed, 05 Oct 2022 09:02:24 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f391b42bfd5493f7f0a5e4702ef212bcbcd630dc98069b371f54008e52d555`  
		Last Modified: Wed, 05 Oct 2022 09:02:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.17-bullseye` - linux; s390x

```console
$ docker pull memcached@sha256:a68d861d39d508e157bfec89650683c443e38e085c0bb686efd1c6f6fb771090
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31221752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f8e5591d33ad149aa1fcea8466745b9018322eb538b330f198f2a24b9b67325`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Oct 2022 23:42:42 GMT
ADD file:7acfe92be51da9cffeb5b063cc87926d1ce457729e3080de340603a38216a708 in / 
# Tue, 04 Oct 2022 23:42:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:21:53 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 01:21:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:21:56 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 01:21:56 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 01:25:31 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 01:25:31 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 01:25:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 01:25:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 01:25:32 GMT
USER memcache
# Wed, 05 Oct 2022 01:25:32 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 01:25:32 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:62990b94a520bfcf718ec711f8444f83c536af2c83c8e53fdfe1f89fdcb79826`  
		Last Modified: Tue, 04 Oct 2022 23:47:16 GMT  
		Size: 29.7 MB (29650719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e75be154924807ecff182be8b52f82593e3ac5c84f4834226f410139f250562`  
		Last Modified: Wed, 05 Oct 2022 01:26:23 GMT  
		Size: 5.0 KB (5027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c6fcd517c09d146d86a8ab0c84e0cb87c39b6d5aa6a5e4f7c2027005bc6c03`  
		Last Modified: Wed, 05 Oct 2022 01:26:23 GMT  
		Size: 324.2 KB (324212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c83fd7ffcf78cdd0c4e1cee3843ffea027ce70f87c997960ea0e14823194a62`  
		Last Modified: Wed, 05 Oct 2022 01:26:23 GMT  
		Size: 1.2 MB (1241387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b6ed6acfc224f832786cfe50858117e0ff11e69d4dfe846f50143f9479e37e`  
		Last Modified: Wed, 05 Oct 2022 01:26:23 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ebd5ba7dabf6f7077666fa277c434e6f23a6614e4dc4d5706bd30dbb2f3d80a`  
		Last Modified: Wed, 05 Oct 2022 01:26:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:alpine`

```console
$ docker pull memcached@sha256:d1d0f8424d9564a6d28b20d441b221294ab09e586d3666e7d3329c811ac3f322
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
$ docker pull memcached@sha256:d7f1053070f1020a4fc773523705c1494bfb1edf25edf24459c81418bcddb2bf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3868456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98356558fb5c650e049187d5fbc075b7d1548df209aff29dedc7202e925ea665`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:53:39 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 09 Aug 2022 20:53:40 GMT
RUN apk add --no-cache libsasl
# Mon, 29 Aug 2022 19:59:54 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 19:59:54 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 20:02:37 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Mon, 29 Aug 2022 20:02:37 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 20:02:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 20:02:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 20:02:38 GMT
USER memcache
# Mon, 29 Aug 2022 20:02:38 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 20:02:38 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d572ef57cdf8eb58de4b4e89970c5e64c6a2f8470bbbe4746efd56927df10611`  
		Last Modified: Tue, 09 Aug 2022 20:57:08 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed8976416286665206f17c9c2ead879425c6c6c62051fa7af308abd8790c0bc`  
		Last Modified: Tue, 09 Aug 2022 20:57:08 GMT  
		Size: 108.3 KB (108322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb81a082d3307bee25bd754b44c17e3423ace86257a27e62b6492be54e6c04b3`  
		Last Modified: Mon, 29 Aug 2022 20:03:30 GMT  
		Size: 952.4 KB (952408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f0efad04b524c1b9e6115b5481dc72c9ee037e65e86b42ae61f40eb5c079b8`  
		Last Modified: Mon, 29 Aug 2022 20:03:30 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963603084de81044b37f07eb6489013949af1ab497be7ace91dd5087c64d70ce`  
		Last Modified: Mon, 29 Aug 2022 20:03:29 GMT  
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
$ docker pull memcached@sha256:fe60e76484846f910192b2d5165415ba111c556789233c183ed18880187b5fed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3758619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc1d52e69bd83adcebc7479ed25934dbd29eb32cb68b338dd65aff944de86398`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:48:03 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 09 Aug 2022 20:48:05 GMT
RUN apk add --no-cache libsasl
# Mon, 29 Aug 2022 18:51:54 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 18:51:54 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 18:54:31 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Mon, 29 Aug 2022 18:54:33 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 18:54:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 18:54:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 18:54:35 GMT
USER memcache
# Mon, 29 Aug 2022 18:54:36 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 18:54:37 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d15db589ad12df2825238bc4f6832b2c6e3d991704c9b41db7865df5d402276`  
		Last Modified: Tue, 09 Aug 2022 20:51:50 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:103b4be7608736e9e24d225ccd97cc4dfad6bacbe7bcf2ca1cd716b45ee32855`  
		Last Modified: Tue, 09 Aug 2022 20:51:50 GMT  
		Size: 109.6 KB (109566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0212e668a84adeaf525aa82fe864ac8b57acb1950c67b38f17d4007d9f9bebbf`  
		Last Modified: Mon, 29 Aug 2022 18:55:51 GMT  
		Size: 939.7 KB (939742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8a69ef314b91110c98f842b3d141768e666cf4673f4414320521338faf28d6`  
		Last Modified: Mon, 29 Aug 2022 18:55:51 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d868394810ccf1649fee843c3a0588a6775265a67dec4936a32a8ee769205eb`  
		Last Modified: Mon, 29 Aug 2022 18:55:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; 386

```console
$ docker pull memcached@sha256:562b7a7602fbdc8c555c997346529640986f1a70c5310d0e7ac7ee5be5004134
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3891424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cf987911cc9f370d9a02fd24e09b38ac92f856013a58e52ae8e1e242e8f115d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:39 GMT
ADD file:b828bc14bc5ff03c8f7310fe0aed6ac5df19a393622d5d1d779a523234d07c0a in / 
# Tue, 09 Aug 2022 17:38:39 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:31:11 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 06 Oct 2022 20:31:12 GMT
RUN apk add --no-cache libsasl
# Thu, 06 Oct 2022 20:31:13 GMT
ENV MEMCACHED_VERSION=1.6.17
# Thu, 06 Oct 2022 20:31:14 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Thu, 06 Oct 2022 20:34:15 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 06 Oct 2022 20:34:17 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 06 Oct 2022 20:34:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 06 Oct 2022 20:34:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 20:34:19 GMT
USER memcache
# Thu, 06 Oct 2022 20:34:20 GMT
EXPOSE 11211
# Thu, 06 Oct 2022 20:34:21 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6c0d3b419d848ea31ca748254611d5d5ce3b76e3d7bba520fd87400fbb75f3b9`  
		Last Modified: Tue, 09 Aug 2022 17:39:33 GMT  
		Size: 2.8 MB (2807121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c5cf4da7d47a1675ec754c4abb2f8aed348ebb76a41a3feea34b6737965077`  
		Last Modified: Thu, 06 Oct 2022 20:35:16 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd19825385b793f75ea8e660e1a32ba82a67f889d2f0fa17286da02efcc7c82`  
		Last Modified: Thu, 06 Oct 2022 20:35:17 GMT  
		Size: 119.8 KB (119834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23144451377b23ee74c09325785c2d9979f0d546d9114753499726be49f0ac35`  
		Last Modified: Thu, 06 Oct 2022 20:35:17 GMT  
		Size: 962.8 KB (962822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9862d0ec769de46de1bc8c01602342b1bbb1d2b834cf3a1aeaaa013bfebbe42c`  
		Last Modified: Thu, 06 Oct 2022 20:35:16 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28aee3d7b7e60049b472288f76c206e4acab742797abacdae0d146f1b1c987be`  
		Last Modified: Thu, 06 Oct 2022 20:35:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:933ee3008de5fff45556eed8f813dbe28c638669e4f1fae22228f1d4ae97fa5d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3913068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c35abea284c9fdadf80277c4e589f260436f39426d12485ae9fd06c66e0cab6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:58:36 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 06 Oct 2022 20:58:39 GMT
RUN apk add --no-cache libsasl
# Thu, 06 Oct 2022 20:58:39 GMT
ENV MEMCACHED_VERSION=1.6.17
# Thu, 06 Oct 2022 20:58:40 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Thu, 06 Oct 2022 21:01:52 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 06 Oct 2022 21:01:52 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 06 Oct 2022 21:01:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 06 Oct 2022 21:01:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 21:01:54 GMT
USER memcache
# Thu, 06 Oct 2022 21:01:55 GMT
EXPOSE 11211
# Thu, 06 Oct 2022 21:01:55 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a4950a8cc87dd9e5ec07268592148771ee6a96b270c2ad0cd2de4ff7b00c1a`  
		Last Modified: Thu, 06 Oct 2022 21:02:46 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c992ad9a080419adb465c5ddd18a317cb7342af149a0deab2c2c7d15bd087442`  
		Last Modified: Thu, 06 Oct 2022 21:02:47 GMT  
		Size: 126.1 KB (126070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6091cffcf047d57d7b51ecc08c3dd0d176f21102199ec0e24ee40257b838287`  
		Last Modified: Thu, 06 Oct 2022 21:02:47 GMT  
		Size: 982.0 KB (982000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b1b52d56e86ac7b75aec7089c33a24d031a269242ee0fdc7a9929f955ecbecd`  
		Last Modified: Thu, 06 Oct 2022 21:02:46 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73885207a86618904bca9142334c74041f4658a7023f9a68e109a24a4dfbfae7`  
		Last Modified: Thu, 06 Oct 2022 21:02:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; s390x

```console
$ docker pull memcached@sha256:409d3e4b8b0de5fc4e5c9f070c5496a99e2d030c2772647bb04095fe6f0757f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3646992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b6a4697fa6b2f43f9e85db112952c4b5ff69b3c9bf3ebcdf7905a11785815b5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:45:36 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 06 Oct 2022 20:45:38 GMT
RUN apk add --no-cache libsasl
# Thu, 06 Oct 2022 20:45:39 GMT
ENV MEMCACHED_VERSION=1.6.17
# Thu, 06 Oct 2022 20:45:39 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Thu, 06 Oct 2022 20:49:59 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 06 Oct 2022 20:49:59 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 06 Oct 2022 20:50:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 06 Oct 2022 20:50:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 20:50:00 GMT
USER memcache
# Thu, 06 Oct 2022 20:50:00 GMT
EXPOSE 11211
# Thu, 06 Oct 2022 20:50:01 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb7a4b531f98c3a90954f542da5d7028ec87d1ee2a74467d087d237d1a5cb62`  
		Last Modified: Thu, 06 Oct 2022 20:50:54 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:248a438b0a1fd089205148ab101aaf2457c55967afad4e042339958b0c1b6b50`  
		Last Modified: Thu, 06 Oct 2022 20:50:54 GMT  
		Size: 112.5 KB (112508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:467a2ab9413d162f0d6b5e65207d0adc2e4d105f9d4a8c3ada6852bf1c5c7e35`  
		Last Modified: Thu, 06 Oct 2022 20:50:54 GMT  
		Size: 942.2 KB (942214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20d843cc1cc32f57f16bc13ab2c98e20dc0fa2b80303702cfce0cdd39a64e4d`  
		Last Modified: Thu, 06 Oct 2022 20:50:54 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b936f167ac6d6abd85c1ebe43c570c4ce1725b0cc4b912ac38a6164606562dc4`  
		Last Modified: Thu, 06 Oct 2022 20:50:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:alpine3.16`

```console
$ docker pull memcached@sha256:304980979f6f7d6e650ad82ab73d6b64a96c1b32800508b5c2afd9bb5341167c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `memcached:alpine3.16` - linux; amd64

```console
$ docker pull memcached@sha256:d7f1053070f1020a4fc773523705c1494bfb1edf25edf24459c81418bcddb2bf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3868456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98356558fb5c650e049187d5fbc075b7d1548df209aff29dedc7202e925ea665`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:53:39 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 09 Aug 2022 20:53:40 GMT
RUN apk add --no-cache libsasl
# Mon, 29 Aug 2022 19:59:54 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 19:59:54 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 20:02:37 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Mon, 29 Aug 2022 20:02:37 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 20:02:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 20:02:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 20:02:38 GMT
USER memcache
# Mon, 29 Aug 2022 20:02:38 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 20:02:38 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d572ef57cdf8eb58de4b4e89970c5e64c6a2f8470bbbe4746efd56927df10611`  
		Last Modified: Tue, 09 Aug 2022 20:57:08 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed8976416286665206f17c9c2ead879425c6c6c62051fa7af308abd8790c0bc`  
		Last Modified: Tue, 09 Aug 2022 20:57:08 GMT  
		Size: 108.3 KB (108322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb81a082d3307bee25bd754b44c17e3423ace86257a27e62b6492be54e6c04b3`  
		Last Modified: Mon, 29 Aug 2022 20:03:30 GMT  
		Size: 952.4 KB (952408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f0efad04b524c1b9e6115b5481dc72c9ee037e65e86b42ae61f40eb5c079b8`  
		Last Modified: Mon, 29 Aug 2022 20:03:30 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963603084de81044b37f07eb6489013949af1ab497be7ace91dd5087c64d70ce`  
		Last Modified: Mon, 29 Aug 2022 20:03:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine3.16` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:fe60e76484846f910192b2d5165415ba111c556789233c183ed18880187b5fed
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.8 MB (3758619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc1d52e69bd83adcebc7479ed25934dbd29eb32cb68b338dd65aff944de86398`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:48:03 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 09 Aug 2022 20:48:05 GMT
RUN apk add --no-cache libsasl
# Mon, 29 Aug 2022 18:51:54 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 18:51:54 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 18:54:31 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Mon, 29 Aug 2022 18:54:33 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 18:54:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 18:54:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 18:54:35 GMT
USER memcache
# Mon, 29 Aug 2022 18:54:36 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 18:54:37 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d15db589ad12df2825238bc4f6832b2c6e3d991704c9b41db7865df5d402276`  
		Last Modified: Tue, 09 Aug 2022 20:51:50 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:103b4be7608736e9e24d225ccd97cc4dfad6bacbe7bcf2ca1cd716b45ee32855`  
		Last Modified: Tue, 09 Aug 2022 20:51:50 GMT  
		Size: 109.6 KB (109566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0212e668a84adeaf525aa82fe864ac8b57acb1950c67b38f17d4007d9f9bebbf`  
		Last Modified: Mon, 29 Aug 2022 18:55:51 GMT  
		Size: 939.7 KB (939742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8a69ef314b91110c98f842b3d141768e666cf4673f4414320521338faf28d6`  
		Last Modified: Mon, 29 Aug 2022 18:55:51 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d868394810ccf1649fee843c3a0588a6775265a67dec4936a32a8ee769205eb`  
		Last Modified: Mon, 29 Aug 2022 18:55:51 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine3.16` - linux; 386

```console
$ docker pull memcached@sha256:562b7a7602fbdc8c555c997346529640986f1a70c5310d0e7ac7ee5be5004134
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3891424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cf987911cc9f370d9a02fd24e09b38ac92f856013a58e52ae8e1e242e8f115d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:39 GMT
ADD file:b828bc14bc5ff03c8f7310fe0aed6ac5df19a393622d5d1d779a523234d07c0a in / 
# Tue, 09 Aug 2022 17:38:39 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:31:11 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 06 Oct 2022 20:31:12 GMT
RUN apk add --no-cache libsasl
# Thu, 06 Oct 2022 20:31:13 GMT
ENV MEMCACHED_VERSION=1.6.17
# Thu, 06 Oct 2022 20:31:14 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Thu, 06 Oct 2022 20:34:15 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 06 Oct 2022 20:34:17 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 06 Oct 2022 20:34:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 06 Oct 2022 20:34:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 20:34:19 GMT
USER memcache
# Thu, 06 Oct 2022 20:34:20 GMT
EXPOSE 11211
# Thu, 06 Oct 2022 20:34:21 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6c0d3b419d848ea31ca748254611d5d5ce3b76e3d7bba520fd87400fbb75f3b9`  
		Last Modified: Tue, 09 Aug 2022 17:39:33 GMT  
		Size: 2.8 MB (2807121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c5cf4da7d47a1675ec754c4abb2f8aed348ebb76a41a3feea34b6737965077`  
		Last Modified: Thu, 06 Oct 2022 20:35:16 GMT  
		Size: 1.2 KB (1243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd19825385b793f75ea8e660e1a32ba82a67f889d2f0fa17286da02efcc7c82`  
		Last Modified: Thu, 06 Oct 2022 20:35:17 GMT  
		Size: 119.8 KB (119834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23144451377b23ee74c09325785c2d9979f0d546d9114753499726be49f0ac35`  
		Last Modified: Thu, 06 Oct 2022 20:35:17 GMT  
		Size: 962.8 KB (962822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9862d0ec769de46de1bc8c01602342b1bbb1d2b834cf3a1aeaaa013bfebbe42c`  
		Last Modified: Thu, 06 Oct 2022 20:35:16 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28aee3d7b7e60049b472288f76c206e4acab742797abacdae0d146f1b1c987be`  
		Last Modified: Thu, 06 Oct 2022 20:35:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine3.16` - linux; ppc64le

```console
$ docker pull memcached@sha256:933ee3008de5fff45556eed8f813dbe28c638669e4f1fae22228f1d4ae97fa5d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3913068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c35abea284c9fdadf80277c4e589f260436f39426d12485ae9fd06c66e0cab6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:58:36 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 06 Oct 2022 20:58:39 GMT
RUN apk add --no-cache libsasl
# Thu, 06 Oct 2022 20:58:39 GMT
ENV MEMCACHED_VERSION=1.6.17
# Thu, 06 Oct 2022 20:58:40 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Thu, 06 Oct 2022 21:01:52 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 06 Oct 2022 21:01:52 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 06 Oct 2022 21:01:54 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 06 Oct 2022 21:01:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 21:01:54 GMT
USER memcache
# Thu, 06 Oct 2022 21:01:55 GMT
EXPOSE 11211
# Thu, 06 Oct 2022 21:01:55 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a4950a8cc87dd9e5ec07268592148771ee6a96b270c2ad0cd2de4ff7b00c1a`  
		Last Modified: Thu, 06 Oct 2022 21:02:46 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c992ad9a080419adb465c5ddd18a317cb7342af149a0deab2c2c7d15bd087442`  
		Last Modified: Thu, 06 Oct 2022 21:02:47 GMT  
		Size: 126.1 KB (126070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6091cffcf047d57d7b51ecc08c3dd0d176f21102199ec0e24ee40257b838287`  
		Last Modified: Thu, 06 Oct 2022 21:02:47 GMT  
		Size: 982.0 KB (982000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b1b52d56e86ac7b75aec7089c33a24d031a269242ee0fdc7a9929f955ecbecd`  
		Last Modified: Thu, 06 Oct 2022 21:02:46 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73885207a86618904bca9142334c74041f4658a7023f9a68e109a24a4dfbfae7`  
		Last Modified: Thu, 06 Oct 2022 21:02:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine3.16` - linux; s390x

```console
$ docker pull memcached@sha256:409d3e4b8b0de5fc4e5c9f070c5496a99e2d030c2772647bb04095fe6f0757f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3646992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b6a4697fa6b2f43f9e85db112952c4b5ff69b3c9bf3ebcdf7905a11785815b5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:45:36 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 06 Oct 2022 20:45:38 GMT
RUN apk add --no-cache libsasl
# Thu, 06 Oct 2022 20:45:39 GMT
ENV MEMCACHED_VERSION=1.6.17
# Thu, 06 Oct 2022 20:45:39 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Thu, 06 Oct 2022 20:49:59 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Thu, 06 Oct 2022 20:49:59 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Thu, 06 Oct 2022 20:50:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Thu, 06 Oct 2022 20:50:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 20:50:00 GMT
USER memcache
# Thu, 06 Oct 2022 20:50:00 GMT
EXPOSE 11211
# Thu, 06 Oct 2022 20:50:01 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb7a4b531f98c3a90954f542da5d7028ec87d1ee2a74467d087d237d1a5cb62`  
		Last Modified: Thu, 06 Oct 2022 20:50:54 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:248a438b0a1fd089205148ab101aaf2457c55967afad4e042339958b0c1b6b50`  
		Last Modified: Thu, 06 Oct 2022 20:50:54 GMT  
		Size: 112.5 KB (112508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:467a2ab9413d162f0d6b5e65207d0adc2e4d105f9d4a8c3ada6852bf1c5c7e35`  
		Last Modified: Thu, 06 Oct 2022 20:50:54 GMT  
		Size: 942.2 KB (942214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20d843cc1cc32f57f16bc13ab2c98e20dc0fa2b80303702cfce0cdd39a64e4d`  
		Last Modified: Thu, 06 Oct 2022 20:50:54 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b936f167ac6d6abd85c1ebe43c570c4ce1725b0cc4b912ac38a6164606562dc4`  
		Last Modified: Thu, 06 Oct 2022 20:50:54 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:bullseye`

```console
$ docker pull memcached@sha256:32b63986179511a820e33f0335381897731f15c802aa1d2707e9891aca1403a5
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
$ docker pull memcached@sha256:931b3d5a0c377a1ffba03d7692e157961e2802cd2fe528801182e80b099fcad8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (33009876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bdad48377094436fa7ba308ceb1b2bbce918630232e753085668b4e28281114`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:39 GMT
ADD file:b78b777208be08edd8f297035cdfbacddb45170ad778fd643c792ee045187e39 in / 
# Tue, 04 Oct 2022 23:26:39 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:17:54 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 04:17:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:17:57 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 04:17:57 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 04:20:39 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 04:20:39 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 04:20:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 04:20:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 04:20:40 GMT
USER memcache
# Wed, 05 Oct 2022 04:20:40 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 04:20:40 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:bd159e379b3b1bc0134341e4ffdeab5f966ec422ae04818bb69ecef08a823b05`  
		Last Modified: Tue, 04 Oct 2022 23:30:54 GMT  
		Size: 31.4 MB (31420102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ba15a7daa0d15e5ba45e9a9fdc332fce5b82c224ba42834aea059a6f245cf0`  
		Last Modified: Wed, 05 Oct 2022 04:21:07 GMT  
		Size: 5.0 KB (4983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7285127ceb5872fecb20531ce255b227f193cf0f6fceec79c876e4b8ebff29be`  
		Last Modified: Wed, 05 Oct 2022 04:21:08 GMT  
		Size: 328.1 KB (328117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e838e946498e1c28405bc1ae35d0fb6dafb97f0f47a462256719329c40afe865`  
		Last Modified: Wed, 05 Oct 2022 04:21:08 GMT  
		Size: 1.3 MB (1256265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd912af099a0b3bb0a430c2768ef0d784cab1d86924c157e945a751e12670e1d`  
		Last Modified: Wed, 05 Oct 2022 04:21:07 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60814b5c0f0d9e77d568f57890e62e11d94773423f772a3120117016d0de3294`  
		Last Modified: Wed, 05 Oct 2022 04:21:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; arm variant v5

```console
$ docker pull memcached@sha256:a84f9fc0812c5f2e6d4575b277b7421022c21829d34d89128c0058f22caf890e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30467657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:449c07e8773b5918abc8cf6d2542c0f1a102b52a38606808b8c1365296278cbc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Oct 2022 23:49:11 GMT
ADD file:effb9e2e2f8c7539e1a2200d069a2592e8ba20c9d034b5a73fbf173b6987193c in / 
# Tue, 04 Oct 2022 23:49:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:53:06 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 01:53:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:53:12 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 01:53:12 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 01:59:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 01:59:12 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 01:59:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 01:59:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 01:59:13 GMT
USER memcache
# Wed, 05 Oct 2022 01:59:13 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 01:59:13 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:7b9558bbfd8050a8e6af6e60560101c49bd53f81df6fa068419b44d028e465eb`  
		Last Modified: Tue, 04 Oct 2022 23:53:54 GMT  
		Size: 28.9 MB (28918381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f7663872748bf22ac651be2e08927fdd98e08f447cb7bcc3862ff485c6d5ddd`  
		Last Modified: Wed, 05 Oct 2022 01:59:52 GMT  
		Size: 4.9 KB (4897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b071b414257fa2a96433371bc4d51ce61fdac16c63b3f3c5e55c9818fa0529f`  
		Last Modified: Wed, 05 Oct 2022 01:59:52 GMT  
		Size: 316.6 KB (316627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f813defd9f0615e613628e02e7dadc2cbecc6b31ae8151aefb81d6a72922c9`  
		Last Modified: Wed, 05 Oct 2022 01:59:52 GMT  
		Size: 1.2 MB (1227346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb16c09a595afd6523b77641de3a45962bd09b125d8ba26b64c7ce6a17137a63`  
		Last Modified: Wed, 05 Oct 2022 01:59:52 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c54c4bbaf374145c3304bfe33479e0b53e0047102ae2488c8190de918a16e3e1`  
		Last Modified: Wed, 05 Oct 2022 01:59:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; arm variant v7

```console
$ docker pull memcached@sha256:c809ce19f7998cea0a39f8a4d06573b6f886a9c98b5da65ebb6efb13e8886d5e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28095847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9ba6ef519428019c76007d4e4e34b0d8e293799d94f152576aeb3a23fca1d0a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Oct 2022 23:58:46 GMT
ADD file:ca1bf27f17594a91224a252bd446f97c3b898210c571f2f26fa2e723d2bf521e in / 
# Tue, 04 Oct 2022 23:58:46 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 05:07:01 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 05:07:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 05:07:05 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 05:07:05 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 05:12:39 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 05:12:39 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 05:12:39 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 05:12:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 05:12:39 GMT
USER memcache
# Wed, 05 Oct 2022 05:12:39 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 05:12:40 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2bc64aeac2e429577e497affc8a416d2fc59158aa967f07aced793368e19455f`  
		Last Modified: Wed, 05 Oct 2022 00:05:09 GMT  
		Size: 26.6 MB (26579199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7e548f4109245b4d3d68767b83de82ac836ac9d5cc1bc081a219d32dbbeda54`  
		Last Modified: Wed, 05 Oct 2022 08:13:34 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:697369682782d1b2dbc043f43ca3316b0db3fa9ea73f7db3dbc467bac02eb162`  
		Last Modified: Wed, 05 Oct 2022 08:13:34 GMT  
		Size: 312.1 KB (312059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dfb70795c00f40a530881bffe5c831e6db14159082a026ea6998712e348984a`  
		Last Modified: Wed, 05 Oct 2022 08:13:35 GMT  
		Size: 1.2 MB (1199286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:476c14bf2670ef65dcc686dfa808de6890eff3c4910ef826bb7faf2291852c8e`  
		Last Modified: Wed, 05 Oct 2022 08:13:34 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d568980c19cf77318fcb8d77bacb59d6693b433e7181df0f3caef176b52a3191`  
		Last Modified: Wed, 05 Oct 2022 08:13:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:d3f458555a9a339d16f76ef8013aa925929005de7217194985f7efa465554cad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31445121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6406224fb2a1c7a535f7f3e81b89efa7325ae81d6b21d9d6bc5d27f41395d88a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:05:55 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 03:05:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:05:59 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 03:06:00 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 03:08:31 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 03:08:33 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 03:08:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 03:08:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 03:08:35 GMT
USER memcache
# Wed, 05 Oct 2022 03:08:36 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 03:08:37 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d51bfc33abb0dd79aa4c51b1f9c4cfd1190791ddeea14d61e1b8e5f5d996da7`  
		Last Modified: Wed, 05 Oct 2022 03:09:28 GMT  
		Size: 4.9 KB (4907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e37070a0cb39b1adff15bff570c77cd0bbe4459d214fc5722701da4f7c5b402`  
		Last Modified: Wed, 05 Oct 2022 03:09:29 GMT  
		Size: 119.3 KB (119254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078e83a26c52c9ff73f62179ba3a9b4b9cdbe0d927d4245a2f3c14d96d909d11`  
		Last Modified: Wed, 05 Oct 2022 03:09:29 GMT  
		Size: 1.3 MB (1256157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f353bbcc7b933af6761691a3ba35fb1b80b182162960769306c81729487de9cf`  
		Last Modified: Wed, 05 Oct 2022 03:09:29 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78a605409bcc6452727b4f53d4b26811dcdc8b176a88c568b56302f9e39ff85`  
		Last Modified: Wed, 05 Oct 2022 03:09:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; 386

```console
$ docker pull memcached@sha256:95ab1613d2fcc9c5a7eba541a7dfb13495fa99b5d77d4656da4630b78bf74c5a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33785263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93de9a3d72d17c99080504de246a0b51465565d26793ad487cd2908476723333`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Oct 2022 23:39:40 GMT
ADD file:a66b7a182260a23fdb8b219600a8b48a5079997715006d9a5324dda11f9d0a7f in / 
# Tue, 04 Oct 2022 23:39:41 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:12:48 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 13:12:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:12:53 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 13:12:54 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 13:15:47 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 13:15:48 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 13:15:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 13:15:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 13:15:50 GMT
USER memcache
# Wed, 05 Oct 2022 13:15:51 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 13:15:52 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:711839e532aa3f129f9cfaa5125d0e379ddefd47f3da44d0674372663dfc6a9b`  
		Last Modified: Tue, 04 Oct 2022 23:45:35 GMT  
		Size: 32.4 MB (32396290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5161f80d1df63217fef9b1a73e067a92d04f472d1a4ba002103da6e1689201d2`  
		Last Modified: Wed, 05 Oct 2022 13:16:41 GMT  
		Size: 4.8 KB (4775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b8ca938e3262650de875a82b51d5429ed32858924ed01f31e08823a0110f78`  
		Last Modified: Wed, 05 Oct 2022 13:16:41 GMT  
		Size: 130.1 KB (130128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d56431e1a0c892213dfd9a453e3575db72680db48a6aed437295e181498ae6c7`  
		Last Modified: Wed, 05 Oct 2022 13:16:42 GMT  
		Size: 1.3 MB (1253663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47362ecff01e4b5783c28f0a1024c21cbacf2f17b789860e4ebf99773898229a`  
		Last Modified: Wed, 05 Oct 2022 13:16:41 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f86c83c1049b01f43ae03975626a66ecb9eae0281599db499528892e30e0269f`  
		Last Modified: Wed, 05 Oct 2022 13:16:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; mips64le

```console
$ docker pull memcached@sha256:922b5312101767b2b3fc81590e722b5e79a729452b4f0edd17a5d792aa90e1b2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31015160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ec29f9e0c7858b09669119d800f2569a6a8e381808abe1a3989aa060c7a64ea`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 05 Oct 2022 00:10:26 GMT
ADD file:48da6b2f4e0315e4f502001a00e4b2abb58d553de11a41901ba859a461052bea in / 
# Wed, 05 Oct 2022 00:10:29 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:59:00 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 03:59:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:59:18 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 03:59:21 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 04:06:17 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 04:06:19 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 04:06:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 04:06:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 04:06:29 GMT
USER memcache
# Wed, 05 Oct 2022 04:06:31 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 04:06:34 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3288c6e2e7130a1e313203f049bde0e57a05237441a3cab92c27f9ada139315b`  
		Last Modified: Wed, 05 Oct 2022 00:18:36 GMT  
		Size: 29.6 MB (29640851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaef4f8453620b9cc82968e1dbf1ed98c0e4c5e897da9cd2e4d5bc26601ef1d0`  
		Last Modified: Wed, 05 Oct 2022 04:06:52 GMT  
		Size: 4.9 KB (4864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcbc6cec97a2b18b7caa64c38f40669eb923898edf6757612abf69036cc94a9c`  
		Last Modified: Wed, 05 Oct 2022 04:06:52 GMT  
		Size: 117.2 KB (117176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b83a324f1ad5c2d5e153fcf42024969d9bbaea8df56221c47b2dcccade28696`  
		Last Modified: Wed, 05 Oct 2022 04:06:52 GMT  
		Size: 1.3 MB (1251861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f20f84bbdb83e24c72fda0fed4ef0cf58b3eee6e4f05b5f4c745e1dfb4779199`  
		Last Modified: Wed, 05 Oct 2022 04:06:52 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f4cdf4ad864d232b858c0042bc2537f61833806ddf7781642c27f0ba8c58fd`  
		Last Modified: Wed, 05 Oct 2022 04:06:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; ppc64le

```console
$ docker pull memcached@sha256:5843450835c3de77b73d275c84981ff40a8921d2fd8f63df29f20779afd4b011
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36977018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ac10fdcf830775d9abecef20325a6db9befca7259adb12da3754bd79025d14d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Oct 2022 23:18:04 GMT
ADD file:66a0f55a4b4dfbb5d64082ffdb24751f20c5773039277ba278fdb4ce4a538c33 in / 
# Tue, 04 Oct 2022 23:18:06 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 08:58:03 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 08:58:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 08:58:10 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 08:58:11 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 09:01:22 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 09:01:23 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 09:01:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 09:01:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 09:01:25 GMT
USER memcache
# Wed, 05 Oct 2022 09:01:25 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 09:01:25 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:4e001127162dd884a6f7bd2e6f74215816d325bebb3a374ae9fcee9f038f99b8`  
		Last Modified: Tue, 04 Oct 2022 23:24:13 GMT  
		Size: 35.3 MB (35290584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c333c30cea960d51a0fca6f30a61ffd7bc4ec7e6711905a2875c17661de45833`  
		Last Modified: Wed, 05 Oct 2022 09:02:24 GMT  
		Size: 5.0 KB (4981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de7f9617e3f96516ad14767e6645f8cccf14aabe76c9617293d3dbdb8d1d5013`  
		Last Modified: Wed, 05 Oct 2022 09:02:24 GMT  
		Size: 356.9 KB (356918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2668fc82899be9101fab61482fe66b640b92efae057ee88cfe0604cf0c08c270`  
		Last Modified: Wed, 05 Oct 2022 09:02:24 GMT  
		Size: 1.3 MB (1324127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617887de59cd713ef92f5af550338f216d62b3a52ff11d3db7437ae4a977677d`  
		Last Modified: Wed, 05 Oct 2022 09:02:24 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f391b42bfd5493f7f0a5e4702ef212bcbcd630dc98069b371f54008e52d555`  
		Last Modified: Wed, 05 Oct 2022 09:02:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; s390x

```console
$ docker pull memcached@sha256:a68d861d39d508e157bfec89650683c443e38e085c0bb686efd1c6f6fb771090
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31221752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f8e5591d33ad149aa1fcea8466745b9018322eb538b330f198f2a24b9b67325`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Oct 2022 23:42:42 GMT
ADD file:7acfe92be51da9cffeb5b063cc87926d1ce457729e3080de340603a38216a708 in / 
# Tue, 04 Oct 2022 23:42:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:21:53 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 01:21:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:21:56 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 01:21:56 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 01:25:31 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 01:25:31 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 01:25:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 01:25:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 01:25:32 GMT
USER memcache
# Wed, 05 Oct 2022 01:25:32 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 01:25:32 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:62990b94a520bfcf718ec711f8444f83c536af2c83c8e53fdfe1f89fdcb79826`  
		Last Modified: Tue, 04 Oct 2022 23:47:16 GMT  
		Size: 29.7 MB (29650719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e75be154924807ecff182be8b52f82593e3ac5c84f4834226f410139f250562`  
		Last Modified: Wed, 05 Oct 2022 01:26:23 GMT  
		Size: 5.0 KB (5027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c6fcd517c09d146d86a8ab0c84e0cb87c39b6d5aa6a5e4f7c2027005bc6c03`  
		Last Modified: Wed, 05 Oct 2022 01:26:23 GMT  
		Size: 324.2 KB (324212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c83fd7ffcf78cdd0c4e1cee3843ffea027ce70f87c997960ea0e14823194a62`  
		Last Modified: Wed, 05 Oct 2022 01:26:23 GMT  
		Size: 1.2 MB (1241387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b6ed6acfc224f832786cfe50858117e0ff11e69d4dfe846f50143f9479e37e`  
		Last Modified: Wed, 05 Oct 2022 01:26:23 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ebd5ba7dabf6f7077666fa277c434e6f23a6614e4dc4d5706bd30dbb2f3d80a`  
		Last Modified: Wed, 05 Oct 2022 01:26:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:latest`

```console
$ docker pull memcached@sha256:32b63986179511a820e33f0335381897731f15c802aa1d2707e9891aca1403a5
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
$ docker pull memcached@sha256:931b3d5a0c377a1ffba03d7692e157961e2802cd2fe528801182e80b099fcad8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (33009876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bdad48377094436fa7ba308ceb1b2bbce918630232e753085668b4e28281114`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:39 GMT
ADD file:b78b777208be08edd8f297035cdfbacddb45170ad778fd643c792ee045187e39 in / 
# Tue, 04 Oct 2022 23:26:39 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 04:17:54 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 04:17:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 04:17:57 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 04:17:57 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 04:20:39 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 04:20:39 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 04:20:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 04:20:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 04:20:40 GMT
USER memcache
# Wed, 05 Oct 2022 04:20:40 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 04:20:40 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:bd159e379b3b1bc0134341e4ffdeab5f966ec422ae04818bb69ecef08a823b05`  
		Last Modified: Tue, 04 Oct 2022 23:30:54 GMT  
		Size: 31.4 MB (31420102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ba15a7daa0d15e5ba45e9a9fdc332fce5b82c224ba42834aea059a6f245cf0`  
		Last Modified: Wed, 05 Oct 2022 04:21:07 GMT  
		Size: 5.0 KB (4983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7285127ceb5872fecb20531ce255b227f193cf0f6fceec79c876e4b8ebff29be`  
		Last Modified: Wed, 05 Oct 2022 04:21:08 GMT  
		Size: 328.1 KB (328117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e838e946498e1c28405bc1ae35d0fb6dafb97f0f47a462256719329c40afe865`  
		Last Modified: Wed, 05 Oct 2022 04:21:08 GMT  
		Size: 1.3 MB (1256265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd912af099a0b3bb0a430c2768ef0d784cab1d86924c157e945a751e12670e1d`  
		Last Modified: Wed, 05 Oct 2022 04:21:07 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60814b5c0f0d9e77d568f57890e62e11d94773423f772a3120117016d0de3294`  
		Last Modified: Wed, 05 Oct 2022 04:21:07 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm variant v5

```console
$ docker pull memcached@sha256:a84f9fc0812c5f2e6d4575b277b7421022c21829d34d89128c0058f22caf890e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30467657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:449c07e8773b5918abc8cf6d2542c0f1a102b52a38606808b8c1365296278cbc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Oct 2022 23:49:11 GMT
ADD file:effb9e2e2f8c7539e1a2200d069a2592e8ba20c9d034b5a73fbf173b6987193c in / 
# Tue, 04 Oct 2022 23:49:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:53:06 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 01:53:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:53:12 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 01:53:12 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 01:59:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 01:59:12 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 01:59:13 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 01:59:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 01:59:13 GMT
USER memcache
# Wed, 05 Oct 2022 01:59:13 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 01:59:13 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:7b9558bbfd8050a8e6af6e60560101c49bd53f81df6fa068419b44d028e465eb`  
		Last Modified: Tue, 04 Oct 2022 23:53:54 GMT  
		Size: 28.9 MB (28918381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f7663872748bf22ac651be2e08927fdd98e08f447cb7bcc3862ff485c6d5ddd`  
		Last Modified: Wed, 05 Oct 2022 01:59:52 GMT  
		Size: 4.9 KB (4897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b071b414257fa2a96433371bc4d51ce61fdac16c63b3f3c5e55c9818fa0529f`  
		Last Modified: Wed, 05 Oct 2022 01:59:52 GMT  
		Size: 316.6 KB (316627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f813defd9f0615e613628e02e7dadc2cbecc6b31ae8151aefb81d6a72922c9`  
		Last Modified: Wed, 05 Oct 2022 01:59:52 GMT  
		Size: 1.2 MB (1227346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb16c09a595afd6523b77641de3a45962bd09b125d8ba26b64c7ce6a17137a63`  
		Last Modified: Wed, 05 Oct 2022 01:59:52 GMT  
		Size: 285.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c54c4bbaf374145c3304bfe33479e0b53e0047102ae2488c8190de918a16e3e1`  
		Last Modified: Wed, 05 Oct 2022 01:59:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm variant v7

```console
$ docker pull memcached@sha256:c809ce19f7998cea0a39f8a4d06573b6f886a9c98b5da65ebb6efb13e8886d5e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28095847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9ba6ef519428019c76007d4e4e34b0d8e293799d94f152576aeb3a23fca1d0a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Oct 2022 23:58:46 GMT
ADD file:ca1bf27f17594a91224a252bd446f97c3b898210c571f2f26fa2e723d2bf521e in / 
# Tue, 04 Oct 2022 23:58:46 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 05:07:01 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 05:07:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 05:07:05 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 05:07:05 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 05:12:39 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 05:12:39 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 05:12:39 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 05:12:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 05:12:39 GMT
USER memcache
# Wed, 05 Oct 2022 05:12:39 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 05:12:40 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2bc64aeac2e429577e497affc8a416d2fc59158aa967f07aced793368e19455f`  
		Last Modified: Wed, 05 Oct 2022 00:05:09 GMT  
		Size: 26.6 MB (26579199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7e548f4109245b4d3d68767b83de82ac836ac9d5cc1bc081a219d32dbbeda54`  
		Last Modified: Wed, 05 Oct 2022 08:13:34 GMT  
		Size: 4.9 KB (4895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:697369682782d1b2dbc043f43ca3316b0db3fa9ea73f7db3dbc467bac02eb162`  
		Last Modified: Wed, 05 Oct 2022 08:13:34 GMT  
		Size: 312.1 KB (312059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dfb70795c00f40a530881bffe5c831e6db14159082a026ea6998712e348984a`  
		Last Modified: Wed, 05 Oct 2022 08:13:35 GMT  
		Size: 1.2 MB (1199286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:476c14bf2670ef65dcc686dfa808de6890eff3c4910ef826bb7faf2291852c8e`  
		Last Modified: Wed, 05 Oct 2022 08:13:34 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d568980c19cf77318fcb8d77bacb59d6693b433e7181df0f3caef176b52a3191`  
		Last Modified: Wed, 05 Oct 2022 08:13:34 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:d3f458555a9a339d16f76ef8013aa925929005de7217194985f7efa465554cad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31445121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6406224fb2a1c7a535f7f3e81b89efa7325ae81d6b21d9d6bc5d27f41395d88a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:05:55 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 03:05:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:05:59 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 03:06:00 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 03:08:31 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 03:08:33 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 03:08:33 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 03:08:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 03:08:35 GMT
USER memcache
# Wed, 05 Oct 2022 03:08:36 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 03:08:37 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d51bfc33abb0dd79aa4c51b1f9c4cfd1190791ddeea14d61e1b8e5f5d996da7`  
		Last Modified: Wed, 05 Oct 2022 03:09:28 GMT  
		Size: 4.9 KB (4907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e37070a0cb39b1adff15bff570c77cd0bbe4459d214fc5722701da4f7c5b402`  
		Last Modified: Wed, 05 Oct 2022 03:09:29 GMT  
		Size: 119.3 KB (119254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078e83a26c52c9ff73f62179ba3a9b4b9cdbe0d927d4245a2f3c14d96d909d11`  
		Last Modified: Wed, 05 Oct 2022 03:09:29 GMT  
		Size: 1.3 MB (1256157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f353bbcc7b933af6761691a3ba35fb1b80b182162960769306c81729487de9cf`  
		Last Modified: Wed, 05 Oct 2022 03:09:29 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78a605409bcc6452727b4f53d4b26811dcdc8b176a88c568b56302f9e39ff85`  
		Last Modified: Wed, 05 Oct 2022 03:09:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; 386

```console
$ docker pull memcached@sha256:95ab1613d2fcc9c5a7eba541a7dfb13495fa99b5d77d4656da4630b78bf74c5a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33785263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93de9a3d72d17c99080504de246a0b51465565d26793ad487cd2908476723333`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Oct 2022 23:39:40 GMT
ADD file:a66b7a182260a23fdb8b219600a8b48a5079997715006d9a5324dda11f9d0a7f in / 
# Tue, 04 Oct 2022 23:39:41 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 13:12:48 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 13:12:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 13:12:53 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 13:12:54 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 13:15:47 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 13:15:48 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 13:15:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 13:15:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 13:15:50 GMT
USER memcache
# Wed, 05 Oct 2022 13:15:51 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 13:15:52 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:711839e532aa3f129f9cfaa5125d0e379ddefd47f3da44d0674372663dfc6a9b`  
		Last Modified: Tue, 04 Oct 2022 23:45:35 GMT  
		Size: 32.4 MB (32396290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5161f80d1df63217fef9b1a73e067a92d04f472d1a4ba002103da6e1689201d2`  
		Last Modified: Wed, 05 Oct 2022 13:16:41 GMT  
		Size: 4.8 KB (4775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b8ca938e3262650de875a82b51d5429ed32858924ed01f31e08823a0110f78`  
		Last Modified: Wed, 05 Oct 2022 13:16:41 GMT  
		Size: 130.1 KB (130128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d56431e1a0c892213dfd9a453e3575db72680db48a6aed437295e181498ae6c7`  
		Last Modified: Wed, 05 Oct 2022 13:16:42 GMT  
		Size: 1.3 MB (1253663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47362ecff01e4b5783c28f0a1024c21cbacf2f17b789860e4ebf99773898229a`  
		Last Modified: Wed, 05 Oct 2022 13:16:41 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f86c83c1049b01f43ae03975626a66ecb9eae0281599db499528892e30e0269f`  
		Last Modified: Wed, 05 Oct 2022 13:16:41 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; mips64le

```console
$ docker pull memcached@sha256:922b5312101767b2b3fc81590e722b5e79a729452b4f0edd17a5d792aa90e1b2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31015160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ec29f9e0c7858b09669119d800f2569a6a8e381808abe1a3989aa060c7a64ea`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 05 Oct 2022 00:10:26 GMT
ADD file:48da6b2f4e0315e4f502001a00e4b2abb58d553de11a41901ba859a461052bea in / 
# Wed, 05 Oct 2022 00:10:29 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:59:00 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 03:59:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:59:18 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 03:59:21 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 04:06:17 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 04:06:19 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 04:06:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 04:06:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 04:06:29 GMT
USER memcache
# Wed, 05 Oct 2022 04:06:31 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 04:06:34 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3288c6e2e7130a1e313203f049bde0e57a05237441a3cab92c27f9ada139315b`  
		Last Modified: Wed, 05 Oct 2022 00:18:36 GMT  
		Size: 29.6 MB (29640851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaef4f8453620b9cc82968e1dbf1ed98c0e4c5e897da9cd2e4d5bc26601ef1d0`  
		Last Modified: Wed, 05 Oct 2022 04:06:52 GMT  
		Size: 4.9 KB (4864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcbc6cec97a2b18b7caa64c38f40669eb923898edf6757612abf69036cc94a9c`  
		Last Modified: Wed, 05 Oct 2022 04:06:52 GMT  
		Size: 117.2 KB (117176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b83a324f1ad5c2d5e153fcf42024969d9bbaea8df56221c47b2dcccade28696`  
		Last Modified: Wed, 05 Oct 2022 04:06:52 GMT  
		Size: 1.3 MB (1251861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f20f84bbdb83e24c72fda0fed4ef0cf58b3eee6e4f05b5f4c745e1dfb4779199`  
		Last Modified: Wed, 05 Oct 2022 04:06:52 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81f4cdf4ad864d232b858c0042bc2537f61833806ddf7781642c27f0ba8c58fd`  
		Last Modified: Wed, 05 Oct 2022 04:06:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; ppc64le

```console
$ docker pull memcached@sha256:5843450835c3de77b73d275c84981ff40a8921d2fd8f63df29f20779afd4b011
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36977018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ac10fdcf830775d9abecef20325a6db9befca7259adb12da3754bd79025d14d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Oct 2022 23:18:04 GMT
ADD file:66a0f55a4b4dfbb5d64082ffdb24751f20c5773039277ba278fdb4ce4a538c33 in / 
# Tue, 04 Oct 2022 23:18:06 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 08:58:03 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 08:58:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 08:58:10 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 08:58:11 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 09:01:22 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 09:01:23 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 09:01:24 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 09:01:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 09:01:25 GMT
USER memcache
# Wed, 05 Oct 2022 09:01:25 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 09:01:25 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:4e001127162dd884a6f7bd2e6f74215816d325bebb3a374ae9fcee9f038f99b8`  
		Last Modified: Tue, 04 Oct 2022 23:24:13 GMT  
		Size: 35.3 MB (35290584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c333c30cea960d51a0fca6f30a61ffd7bc4ec7e6711905a2875c17661de45833`  
		Last Modified: Wed, 05 Oct 2022 09:02:24 GMT  
		Size: 5.0 KB (4981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de7f9617e3f96516ad14767e6645f8cccf14aabe76c9617293d3dbdb8d1d5013`  
		Last Modified: Wed, 05 Oct 2022 09:02:24 GMT  
		Size: 356.9 KB (356918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2668fc82899be9101fab61482fe66b640b92efae057ee88cfe0604cf0c08c270`  
		Last Modified: Wed, 05 Oct 2022 09:02:24 GMT  
		Size: 1.3 MB (1324127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617887de59cd713ef92f5af550338f216d62b3a52ff11d3db7437ae4a977677d`  
		Last Modified: Wed, 05 Oct 2022 09:02:24 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f391b42bfd5493f7f0a5e4702ef212bcbcd630dc98069b371f54008e52d555`  
		Last Modified: Wed, 05 Oct 2022 09:02:24 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; s390x

```console
$ docker pull memcached@sha256:a68d861d39d508e157bfec89650683c443e38e085c0bb686efd1c6f6fb771090
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31221752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f8e5591d33ad149aa1fcea8466745b9018322eb538b330f198f2a24b9b67325`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 04 Oct 2022 23:42:42 GMT
ADD file:7acfe92be51da9cffeb5b063cc87926d1ce457729e3080de340603a38216a708 in / 
# Tue, 04 Oct 2022 23:42:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:21:53 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 05 Oct 2022 01:21:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:21:56 GMT
ENV MEMCACHED_VERSION=1.6.17
# Wed, 05 Oct 2022 01:21:56 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Wed, 05 Oct 2022 01:25:31 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 05 Oct 2022 01:25:31 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 05 Oct 2022 01:25:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 05 Oct 2022 01:25:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Oct 2022 01:25:32 GMT
USER memcache
# Wed, 05 Oct 2022 01:25:32 GMT
EXPOSE 11211
# Wed, 05 Oct 2022 01:25:32 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:62990b94a520bfcf718ec711f8444f83c536af2c83c8e53fdfe1f89fdcb79826`  
		Last Modified: Tue, 04 Oct 2022 23:47:16 GMT  
		Size: 29.7 MB (29650719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e75be154924807ecff182be8b52f82593e3ac5c84f4834226f410139f250562`  
		Last Modified: Wed, 05 Oct 2022 01:26:23 GMT  
		Size: 5.0 KB (5027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c6fcd517c09d146d86a8ab0c84e0cb87c39b6d5aa6a5e4f7c2027005bc6c03`  
		Last Modified: Wed, 05 Oct 2022 01:26:23 GMT  
		Size: 324.2 KB (324212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c83fd7ffcf78cdd0c4e1cee3843ffea027ce70f87c997960ea0e14823194a62`  
		Last Modified: Wed, 05 Oct 2022 01:26:23 GMT  
		Size: 1.2 MB (1241387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b6ed6acfc224f832786cfe50858117e0ff11e69d4dfe846f50143f9479e37e`  
		Last Modified: Wed, 05 Oct 2022 01:26:23 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ebd5ba7dabf6f7077666fa277c434e6f23a6614e4dc4d5706bd30dbb2f3d80a`  
		Last Modified: Wed, 05 Oct 2022 01:26:23 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
