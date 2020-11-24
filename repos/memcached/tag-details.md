<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `memcached`

-	[`memcached:1`](#memcached1)
-	[`memcached:1.6`](#memcached16)
-	[`memcached:1.6.9`](#memcached169)
-	[`memcached:1.6.9-alpine`](#memcached169-alpine)
-	[`memcached:1.6-alpine`](#memcached16-alpine)
-	[`memcached:1-alpine`](#memcached1-alpine)
-	[`memcached:alpine`](#memcachedalpine)
-	[`memcached:latest`](#memcachedlatest)

## `memcached:1`

```console
$ docker pull memcached@sha256:a373b18f6ecc77c728c1b387b7c52fe331293319d37d4314ccbf283a726efb10
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
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
$ docker pull memcached@sha256:efe79d6cb73884b4cdc639183c3bdd27692034e92bd97a6972347db1f3f9940b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30513603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08ea1a3256c49616070a12b913da5051d159b2e7dc913e8a62ce0538f7a8a02a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:17 GMT
ADD file:d2abb0e4e7ac1773741f51f57d3a0b8ffc7907348842d773f8c341ba17f856d5 in / 
# Tue, 17 Nov 2020 20:21:17 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 23:59:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 17 Nov 2020 23:59:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 24 Nov 2020 00:40:08 GMT
ENV MEMCACHED_VERSION=1.6.9
# Tue, 24 Nov 2020 00:40:08 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Tue, 24 Nov 2020 00:44:14 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 24 Nov 2020 00:44:15 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 Nov 2020 00:44:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 Nov 2020 00:44:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Nov 2020 00:44:16 GMT
USER memcache
# Tue, 24 Nov 2020 00:44:16 GMT
EXPOSE 11211
# Tue, 24 Nov 2020 00:44:16 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:852e50cd189dfeb54d97680d9fa6bed21a6d7d18cfb56d6abfe2de9d7f173795`  
		Last Modified: Tue, 17 Nov 2020 20:27:25 GMT  
		Size: 27.1 MB (27105484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba259e022fc04d1e3da7b6650e0a253d23ade0fc8efd7f96e9146dd9337e7d74`  
		Last Modified: Wed, 18 Nov 2020 00:04:25 GMT  
		Size: 5.0 KB (4977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baff9e329932a3fa2a84550d57f41fa83ebd732b2079111e74f62ccbcaaeb084`  
		Last Modified: Wed, 18 Nov 2020 00:04:25 GMT  
		Size: 2.2 MB (2196434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f513b04a1f26d0f649ac982e308a03bcfa2cc147aa2654d57beca1d3c0ddfe2`  
		Last Modified: Tue, 24 Nov 2020 00:49:06 GMT  
		Size: 1.2 MB (1206301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb255edcd3e1c523644c575b9a937eab78cd4bb1b719a8e5030f81dab71bb9c3`  
		Last Modified: Tue, 24 Nov 2020 00:49:06 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee1dea1b4991d10177d54c728588378dfc740149e2dab0a2bb461f8e1ceb2d06`  
		Last Modified: Tue, 24 Nov 2020 00:49:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm variant v5

```console
$ docker pull memcached@sha256:b506cd917be5e584884f6bd23ab1c33563d1202186141d018e0b1efdb6d44536
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27931449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c96be237e7151156f8f06cc8123c1bdd31017cfc47efb0fbe0100317d3659424`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 17 Nov 2020 20:20:37 GMT
ADD file:d75cebdc79385debd2d6d1c8c34855d2bd4779b13ee47f76e34c6d8fca037531 in / 
# Tue, 17 Nov 2020 20:20:45 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 05:58:29 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 18 Nov 2020 05:58:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 23 Nov 2020 23:52:57 GMT
ENV MEMCACHED_VERSION=1.6.9
# Mon, 23 Nov 2020 23:52:59 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Mon, 23 Nov 2020 23:56:36 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Mon, 23 Nov 2020 23:56:37 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 23 Nov 2020 23:56:39 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 23 Nov 2020 23:56:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 Nov 2020 23:56:40 GMT
USER memcache
# Mon, 23 Nov 2020 23:56:41 GMT
EXPOSE 11211
# Mon, 23 Nov 2020 23:56:42 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1b8dd2ec17ab788b6ea03a9b6cf68afada9a8692681d29e9795db0abf6554404`  
		Last Modified: Tue, 17 Nov 2020 20:30:33 GMT  
		Size: 24.9 MB (24850311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eab7493baf19e0692ceefecef0ac524fdb4ba00028370800b97c2f0fdb2a840`  
		Last Modified: Wed, 18 Nov 2020 06:02:40 GMT  
		Size: 4.9 KB (4898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b096e22e759388a2bd7f3d04ba63e0b2fbbe300fe4093e3699e0ead554d3026`  
		Last Modified: Wed, 18 Nov 2020 06:02:40 GMT  
		Size: 1.9 MB (1896787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed956595633e1910b74834c64a03cbfa6fb9b0dd7c712ab74e05abaa2325aae`  
		Last Modified: Mon, 23 Nov 2020 23:56:53 GMT  
		Size: 1.2 MB (1179045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08931b56db74dd19b895412f1f1cc01c3416ff07a9b06d5db052cdb685d7975f`  
		Last Modified: Mon, 23 Nov 2020 23:56:52 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d581c95c1973377e4b69f2ee972d2e88141b440606f04bb7cf035a987ccc412`  
		Last Modified: Mon, 23 Nov 2020 23:56:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm variant v7

```console
$ docker pull memcached@sha256:23bfdefe9cc175f1d85d34f46637c56c49f675daac226d2ef27875d88f1d634a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25680615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83cc6416458d599f47ab03ce627dc26358df5d4d8e352bc0ed0e2e1e8bc9e031`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:06 GMT
ADD file:2035658a8d20545ee7b2ab3ee791a371925fca7968ac29435303da24a1378f34 in / 
# Tue, 17 Nov 2020 20:21:10 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 22:43:01 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 17 Nov 2020 22:43:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 24 Nov 2020 00:22:17 GMT
ENV MEMCACHED_VERSION=1.6.9
# Tue, 24 Nov 2020 00:22:18 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Tue, 24 Nov 2020 00:25:37 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 24 Nov 2020 00:25:38 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 Nov 2020 00:25:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 Nov 2020 00:25:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Nov 2020 00:25:42 GMT
USER memcache
# Tue, 24 Nov 2020 00:25:43 GMT
EXPOSE 11211
# Tue, 24 Nov 2020 00:25:48 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d5029e4b387017f20ad9f77baf3b81dd41f851d6340363b842a8a1d9786a60a0`  
		Last Modified: Tue, 17 Nov 2020 20:31:46 GMT  
		Size: 22.7 MB (22714186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dcb178bde3efeefaad9cde6e23e198ace47cd12278a903916a98fe226425c63`  
		Last Modified: Tue, 17 Nov 2020 22:47:04 GMT  
		Size: 4.9 KB (4888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:849c9255e9336e765f5fe8a15ddde316c5b6f9a38454be317f5b88d23490d4e9`  
		Last Modified: Tue, 17 Nov 2020 22:47:04 GMT  
		Size: 1.8 MB (1811529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee4f7e83b65d682e21adba125e9b5a00b62239a5f2a45a02a8ee980c77c033ed`  
		Last Modified: Tue, 24 Nov 2020 00:29:37 GMT  
		Size: 1.1 MB (1149604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae88eab2c47891856beb68524c3b63058f3c28a17b0cc5f9a2b7a310f0b23245`  
		Last Modified: Tue, 24 Nov 2020 00:29:37 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d745615f6bde6bb77f0f3c84750b88a63812b46e1972b2d40a987307300373f`  
		Last Modified: Tue, 24 Nov 2020 00:29:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:bca7dce6878924796ed4e59749a20a99b8b21095a6622de36e1669854f3995e7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29121866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b4113f866ef34853e089e9828737b4a19cfd3e9b7ab4673fb6b314a94105e1a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 17 Nov 2020 20:23:31 GMT
ADD file:a70d8c01f8f04f36038968567af779883f3b5ba3147b662b7d170d80418bc23c in / 
# Tue, 17 Nov 2020 20:23:32 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 01:22:43 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 18 Nov 2020 01:22:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 24 Nov 2020 00:47:00 GMT
ENV MEMCACHED_VERSION=1.6.9
# Tue, 24 Nov 2020 00:47:01 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Tue, 24 Nov 2020 00:54:18 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 24 Nov 2020 00:54:19 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 Nov 2020 00:54:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 Nov 2020 00:54:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Nov 2020 00:54:23 GMT
USER memcache
# Tue, 24 Nov 2020 00:54:24 GMT
EXPOSE 11211
# Tue, 24 Nov 2020 00:54:24 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:29ade854e0dcedde295dd89890d45271e9df839e42124558eb5283508ca70f5c`  
		Last Modified: Tue, 17 Nov 2020 20:32:02 GMT  
		Size: 25.9 MB (25862532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b138bddb332a0f874407cfaec3014ec6614883be703b52ff29808980118a91`  
		Last Modified: Wed, 18 Nov 2020 01:26:58 GMT  
		Size: 5.0 KB (5024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5452540f15530cb8fe9343e88516c0b3050b9bb0596613026fe0f84b13c30d6c`  
		Last Modified: Wed, 18 Nov 2020 01:26:59 GMT  
		Size: 2.1 MB (2074952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:373464c46512a6172ca94cdb2aaf1427f0710ce8289bf2a4a73b3a8eac65e689`  
		Last Modified: Tue, 24 Nov 2020 00:58:10 GMT  
		Size: 1.2 MB (1178950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d995428ce6fac044c4080e2e653157b5d2c86c8940d16d85d20ff3094d47d4`  
		Last Modified: Tue, 24 Nov 2020 00:58:09 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac3fb0a8b0191b0f3b130c75bc5d77bdecc4c5f041e4f0c0c8820cf189c5e785`  
		Last Modified: Tue, 24 Nov 2020 00:58:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; 386

```console
$ docker pull memcached@sha256:04f9bb7564b8ef32c9b16f7a84a06aa6ce963cd7341fb47580b22b5240e84ffb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31183406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2a87dfef3d28a151095f6d0a0d6cda6fa63975bd76e0221a8a04bfe82dea0e6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 17 Nov 2020 20:19:58 GMT
ADD file:b17dfa607fcb298beb9c58bfbb8b9b0743ceb385875776c56269db2506840edf in / 
# Tue, 17 Nov 2020 20:19:58 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 06:51:09 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 18 Nov 2020 06:51:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 24 Nov 2020 00:38:23 GMT
ENV MEMCACHED_VERSION=1.6.9
# Tue, 24 Nov 2020 00:38:23 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Tue, 24 Nov 2020 00:42:38 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 24 Nov 2020 00:42:39 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 Nov 2020 00:42:39 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 Nov 2020 00:42:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Nov 2020 00:42:40 GMT
USER memcache
# Tue, 24 Nov 2020 00:42:40 GMT
EXPOSE 11211
# Tue, 24 Nov 2020 00:42:40 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:e8e82c9fb36b8f3a9b8f18fe1d88e4d425d5c45968e3f2e94cdbb1255feb4878`  
		Last Modified: Tue, 17 Nov 2020 20:26:45 GMT  
		Size: 27.8 MB (27766186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:321cbeb51acb785f1b1c182cedb4064f03df6af524b61820be6dcd5b1cb2f8a2`  
		Last Modified: Wed, 18 Nov 2020 07:00:37 GMT  
		Size: 4.9 KB (4893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9992095793664bbd90982439c87351ec23b212e9622d90a144faa60a7acbe6d`  
		Last Modified: Wed, 18 Nov 2020 07:00:38 GMT  
		Size: 2.2 MB (2208086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7345a22027cf324340c6fe54efa2e573f790817c593fc990c4eb41f1d731061`  
		Last Modified: Tue, 24 Nov 2020 00:47:51 GMT  
		Size: 1.2 MB (1203835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94d7cbd4098036b6b2a3ddba5fd780fb6875c10dc8df39a054bcd89187a62bcd`  
		Last Modified: Tue, 24 Nov 2020 00:47:50 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53794b9614d9d66687bd0c4938c508a6dcd7e7970d8ba3c2078635fe95d6c856`  
		Last Modified: Tue, 24 Nov 2020 00:47:50 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; mips64le

```console
$ docker pull memcached@sha256:8bc36ac7c7accfbf668832c1f44aa9b8a72eea77027dd1cda17b12353928fc03
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.8 MB (28757547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23d47b7544c777f79de3b1b39c9d4702573764e302f83401ec54210ebc22c514`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 17 Nov 2020 20:19:24 GMT
ADD file:98a1b26b3eefd56b2867344c8c58f4bc3ef9a19c28e35c41df77ab80598d41bc in / 
# Tue, 17 Nov 2020 20:19:24 GMT
CMD ["bash"]
# Mon, 23 Nov 2020 23:07:26 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Mon, 23 Nov 2020 23:07:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 23 Nov 2020 23:07:39 GMT
ENV MEMCACHED_VERSION=1.6.9
# Mon, 23 Nov 2020 23:07:39 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Mon, 23 Nov 2020 23:13:24 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Mon, 23 Nov 2020 23:13:24 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 23 Nov 2020 23:13:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 23 Nov 2020 23:13:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 Nov 2020 23:13:26 GMT
USER memcache
# Mon, 23 Nov 2020 23:13:27 GMT
EXPOSE 11211
# Mon, 23 Nov 2020 23:13:27 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:071bb0a152ef32db0e7d172bcc4722a6a275885249ddb72bee023e268e82fc16`  
		Last Modified: Tue, 17 Nov 2020 20:26:34 GMT  
		Size: 25.8 MB (25777477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:664f5d146d813d299af77e5fc0e344f8a75bd40824a60c99a04bdb1ff4b13b43`  
		Last Modified: Mon, 23 Nov 2020 23:13:45 GMT  
		Size: 5.0 KB (4982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9431da82e8f3642d3474b3944f281ce0d9d5f81e50a7d814cc06bc4db3a55ff6`  
		Last Modified: Mon, 23 Nov 2020 23:13:46 GMT  
		Size: 1.8 MB (1776012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72e10c1044bcc0ce9b31d6c01d3f1b6be4c9a227a8d757cd5fbb803190e0372c`  
		Last Modified: Mon, 23 Nov 2020 23:13:46 GMT  
		Size: 1.2 MB (1198668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0d2b229dc61a9fd2afe3edd3cdf4354d3153027b44b22fec64257ac3e07c4e`  
		Last Modified: Mon, 23 Nov 2020 23:13:45 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ae54e7810b124e108a6331526af87033a40abd56d009854ad078554273f41b`  
		Last Modified: Mon, 23 Nov 2020 23:13:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; ppc64le

```console
$ docker pull memcached@sha256:5233f7be9d0b23aa88bf7fc2e75310bdb632ec93aa2db03c39ef676fbd2c111f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34085325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ed1158f0082c5bd5c24e244191a1a7c8dc37a0db0a0f27a9a61d238a6f45b60`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 17 Nov 2020 23:23:06 GMT
ADD file:49cd8b08964980901349e1f3d6cb34abd8145dea6e6d9ab83502452281ac73ca in / 
# Tue, 17 Nov 2020 23:23:11 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 02:08:02 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 18 Nov 2020 02:08:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 02:08:53 GMT
ENV MEMCACHED_VERSION=1.6.8
# Wed, 18 Nov 2020 02:09:05 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Wed, 18 Nov 2020 02:21:00 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 18 Nov 2020 02:21:04 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 18 Nov 2020 02:21:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 18 Nov 2020 02:21:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Nov 2020 02:21:20 GMT
USER memcache
# Wed, 18 Nov 2020 02:21:23 GMT
EXPOSE 11211
# Wed, 18 Nov 2020 02:21:29 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d79345c10f03543bff3982aedb35a18ba18626c0074014387ff5e1dc14474e2b`  
		Last Modified: Tue, 17 Nov 2020 23:32:54 GMT  
		Size: 30.5 MB (30531702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c81cd83e42b497f0cba94fa5211dd383d0d43fb3fefb1c49d84df1ec1bb8706`  
		Last Modified: Wed, 18 Nov 2020 02:21:58 GMT  
		Size: 5.0 KB (4990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2755aa03159fc35fb59a7fc785b128fa60a5940abb4d5777fea087d0a61c07a`  
		Last Modified: Wed, 18 Nov 2020 02:21:59 GMT  
		Size: 2.3 MB (2322767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f132d007583b65a7dae9876fd53c3ceb86e63cf51c9ac01c83d0c1ad73925ad`  
		Last Modified: Wed, 18 Nov 2020 02:21:58 GMT  
		Size: 1.2 MB (1225459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac54fbbfdd63057bf31b8403a24213cfb6c131e9e6e691bb90e9d35d8deb479`  
		Last Modified: Wed, 18 Nov 2020 02:21:58 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1fc8692195395ae28bbb8eadfb2c8e2cd572559f1b92bf620013f723f52303c`  
		Last Modified: Wed, 18 Nov 2020 02:21:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; s390x

```console
$ docker pull memcached@sha256:d4f378fbb763346873fb016770ad2e202370f526d24ccbeffc2f3a1247b9b3d5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.8 MB (28811191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ff2b9ce713317a592f1208e112eec5e2b257bd5b8a46984c37d8b8e63c010d3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 17 Nov 2020 20:18:29 GMT
ADD file:4a3215d1c9b4afb58053c4fff8d121547890c2a71bc027992f7f960551c6acb1 in / 
# Tue, 17 Nov 2020 20:18:34 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 01:46:32 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 18 Nov 2020 01:46:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 24 Nov 2020 01:29:39 GMT
ENV MEMCACHED_VERSION=1.6.9
# Tue, 24 Nov 2020 01:29:40 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Tue, 24 Nov 2020 01:38:32 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 24 Nov 2020 01:38:33 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 Nov 2020 01:38:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 Nov 2020 01:38:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Nov 2020 01:38:36 GMT
USER memcache
# Tue, 24 Nov 2020 01:38:36 GMT
EXPOSE 11211
# Tue, 24 Nov 2020 01:38:37 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c0d5e3cc51c0b20d3f68226f5332c9a9c2b17cce2f362ec742d4ed325ff7b530`  
		Last Modified: Tue, 17 Nov 2020 20:23:43 GMT  
		Size: 25.7 MB (25721143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b189bf5a9f20baf2f6e6ec9230535bdc36fc750196dd1e3f5eb5e17ee36a31`  
		Last Modified: Wed, 18 Nov 2020 01:53:06 GMT  
		Size: 5.0 KB (5027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1372a3dddcc126d1aad6887514b61ad9ac946b00f50834efdd6c376cc6cfcf65`  
		Last Modified: Wed, 18 Nov 2020 01:53:06 GMT  
		Size: 1.9 MB (1886092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d6c632cdb2f59084328d009bb036821bfe895d1bc1d1512150931d115ea0b40`  
		Last Modified: Tue, 24 Nov 2020 01:43:04 GMT  
		Size: 1.2 MB (1198521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247f0621f757137d4d49d296cd294fef8816daca0331d8406990d31eab886d2e`  
		Last Modified: Tue, 24 Nov 2020 01:43:03 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b13354fbc1d862e30d1c831d85eb9a4e24ba519cc341b6097aa6209cfd530e99`  
		Last Modified: Tue, 24 Nov 2020 01:43:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6`

```console
$ docker pull memcached@sha256:a373b18f6ecc77c728c1b387b7c52fe331293319d37d4314ccbf283a726efb10
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
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
$ docker pull memcached@sha256:efe79d6cb73884b4cdc639183c3bdd27692034e92bd97a6972347db1f3f9940b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30513603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08ea1a3256c49616070a12b913da5051d159b2e7dc913e8a62ce0538f7a8a02a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:17 GMT
ADD file:d2abb0e4e7ac1773741f51f57d3a0b8ffc7907348842d773f8c341ba17f856d5 in / 
# Tue, 17 Nov 2020 20:21:17 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 23:59:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 17 Nov 2020 23:59:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 24 Nov 2020 00:40:08 GMT
ENV MEMCACHED_VERSION=1.6.9
# Tue, 24 Nov 2020 00:40:08 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Tue, 24 Nov 2020 00:44:14 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 24 Nov 2020 00:44:15 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 Nov 2020 00:44:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 Nov 2020 00:44:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Nov 2020 00:44:16 GMT
USER memcache
# Tue, 24 Nov 2020 00:44:16 GMT
EXPOSE 11211
# Tue, 24 Nov 2020 00:44:16 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:852e50cd189dfeb54d97680d9fa6bed21a6d7d18cfb56d6abfe2de9d7f173795`  
		Last Modified: Tue, 17 Nov 2020 20:27:25 GMT  
		Size: 27.1 MB (27105484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba259e022fc04d1e3da7b6650e0a253d23ade0fc8efd7f96e9146dd9337e7d74`  
		Last Modified: Wed, 18 Nov 2020 00:04:25 GMT  
		Size: 5.0 KB (4977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baff9e329932a3fa2a84550d57f41fa83ebd732b2079111e74f62ccbcaaeb084`  
		Last Modified: Wed, 18 Nov 2020 00:04:25 GMT  
		Size: 2.2 MB (2196434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f513b04a1f26d0f649ac982e308a03bcfa2cc147aa2654d57beca1d3c0ddfe2`  
		Last Modified: Tue, 24 Nov 2020 00:49:06 GMT  
		Size: 1.2 MB (1206301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb255edcd3e1c523644c575b9a937eab78cd4bb1b719a8e5030f81dab71bb9c3`  
		Last Modified: Tue, 24 Nov 2020 00:49:06 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee1dea1b4991d10177d54c728588378dfc740149e2dab0a2bb461f8e1ceb2d06`  
		Last Modified: Tue, 24 Nov 2020 00:49:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm variant v5

```console
$ docker pull memcached@sha256:b506cd917be5e584884f6bd23ab1c33563d1202186141d018e0b1efdb6d44536
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27931449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c96be237e7151156f8f06cc8123c1bdd31017cfc47efb0fbe0100317d3659424`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 17 Nov 2020 20:20:37 GMT
ADD file:d75cebdc79385debd2d6d1c8c34855d2bd4779b13ee47f76e34c6d8fca037531 in / 
# Tue, 17 Nov 2020 20:20:45 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 05:58:29 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 18 Nov 2020 05:58:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 23 Nov 2020 23:52:57 GMT
ENV MEMCACHED_VERSION=1.6.9
# Mon, 23 Nov 2020 23:52:59 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Mon, 23 Nov 2020 23:56:36 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Mon, 23 Nov 2020 23:56:37 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 23 Nov 2020 23:56:39 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 23 Nov 2020 23:56:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 Nov 2020 23:56:40 GMT
USER memcache
# Mon, 23 Nov 2020 23:56:41 GMT
EXPOSE 11211
# Mon, 23 Nov 2020 23:56:42 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1b8dd2ec17ab788b6ea03a9b6cf68afada9a8692681d29e9795db0abf6554404`  
		Last Modified: Tue, 17 Nov 2020 20:30:33 GMT  
		Size: 24.9 MB (24850311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eab7493baf19e0692ceefecef0ac524fdb4ba00028370800b97c2f0fdb2a840`  
		Last Modified: Wed, 18 Nov 2020 06:02:40 GMT  
		Size: 4.9 KB (4898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b096e22e759388a2bd7f3d04ba63e0b2fbbe300fe4093e3699e0ead554d3026`  
		Last Modified: Wed, 18 Nov 2020 06:02:40 GMT  
		Size: 1.9 MB (1896787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed956595633e1910b74834c64a03cbfa6fb9b0dd7c712ab74e05abaa2325aae`  
		Last Modified: Mon, 23 Nov 2020 23:56:53 GMT  
		Size: 1.2 MB (1179045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08931b56db74dd19b895412f1f1cc01c3416ff07a9b06d5db052cdb685d7975f`  
		Last Modified: Mon, 23 Nov 2020 23:56:52 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d581c95c1973377e4b69f2ee972d2e88141b440606f04bb7cf035a987ccc412`  
		Last Modified: Mon, 23 Nov 2020 23:56:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm variant v7

```console
$ docker pull memcached@sha256:23bfdefe9cc175f1d85d34f46637c56c49f675daac226d2ef27875d88f1d634a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25680615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83cc6416458d599f47ab03ce627dc26358df5d4d8e352bc0ed0e2e1e8bc9e031`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:06 GMT
ADD file:2035658a8d20545ee7b2ab3ee791a371925fca7968ac29435303da24a1378f34 in / 
# Tue, 17 Nov 2020 20:21:10 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 22:43:01 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 17 Nov 2020 22:43:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 24 Nov 2020 00:22:17 GMT
ENV MEMCACHED_VERSION=1.6.9
# Tue, 24 Nov 2020 00:22:18 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Tue, 24 Nov 2020 00:25:37 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 24 Nov 2020 00:25:38 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 Nov 2020 00:25:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 Nov 2020 00:25:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Nov 2020 00:25:42 GMT
USER memcache
# Tue, 24 Nov 2020 00:25:43 GMT
EXPOSE 11211
# Tue, 24 Nov 2020 00:25:48 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d5029e4b387017f20ad9f77baf3b81dd41f851d6340363b842a8a1d9786a60a0`  
		Last Modified: Tue, 17 Nov 2020 20:31:46 GMT  
		Size: 22.7 MB (22714186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dcb178bde3efeefaad9cde6e23e198ace47cd12278a903916a98fe226425c63`  
		Last Modified: Tue, 17 Nov 2020 22:47:04 GMT  
		Size: 4.9 KB (4888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:849c9255e9336e765f5fe8a15ddde316c5b6f9a38454be317f5b88d23490d4e9`  
		Last Modified: Tue, 17 Nov 2020 22:47:04 GMT  
		Size: 1.8 MB (1811529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee4f7e83b65d682e21adba125e9b5a00b62239a5f2a45a02a8ee980c77c033ed`  
		Last Modified: Tue, 24 Nov 2020 00:29:37 GMT  
		Size: 1.1 MB (1149604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae88eab2c47891856beb68524c3b63058f3c28a17b0cc5f9a2b7a310f0b23245`  
		Last Modified: Tue, 24 Nov 2020 00:29:37 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d745615f6bde6bb77f0f3c84750b88a63812b46e1972b2d40a987307300373f`  
		Last Modified: Tue, 24 Nov 2020 00:29:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:bca7dce6878924796ed4e59749a20a99b8b21095a6622de36e1669854f3995e7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29121866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b4113f866ef34853e089e9828737b4a19cfd3e9b7ab4673fb6b314a94105e1a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 17 Nov 2020 20:23:31 GMT
ADD file:a70d8c01f8f04f36038968567af779883f3b5ba3147b662b7d170d80418bc23c in / 
# Tue, 17 Nov 2020 20:23:32 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 01:22:43 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 18 Nov 2020 01:22:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 24 Nov 2020 00:47:00 GMT
ENV MEMCACHED_VERSION=1.6.9
# Tue, 24 Nov 2020 00:47:01 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Tue, 24 Nov 2020 00:54:18 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 24 Nov 2020 00:54:19 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 Nov 2020 00:54:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 Nov 2020 00:54:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Nov 2020 00:54:23 GMT
USER memcache
# Tue, 24 Nov 2020 00:54:24 GMT
EXPOSE 11211
# Tue, 24 Nov 2020 00:54:24 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:29ade854e0dcedde295dd89890d45271e9df839e42124558eb5283508ca70f5c`  
		Last Modified: Tue, 17 Nov 2020 20:32:02 GMT  
		Size: 25.9 MB (25862532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b138bddb332a0f874407cfaec3014ec6614883be703b52ff29808980118a91`  
		Last Modified: Wed, 18 Nov 2020 01:26:58 GMT  
		Size: 5.0 KB (5024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5452540f15530cb8fe9343e88516c0b3050b9bb0596613026fe0f84b13c30d6c`  
		Last Modified: Wed, 18 Nov 2020 01:26:59 GMT  
		Size: 2.1 MB (2074952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:373464c46512a6172ca94cdb2aaf1427f0710ce8289bf2a4a73b3a8eac65e689`  
		Last Modified: Tue, 24 Nov 2020 00:58:10 GMT  
		Size: 1.2 MB (1178950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d995428ce6fac044c4080e2e653157b5d2c86c8940d16d85d20ff3094d47d4`  
		Last Modified: Tue, 24 Nov 2020 00:58:09 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac3fb0a8b0191b0f3b130c75bc5d77bdecc4c5f041e4f0c0c8820cf189c5e785`  
		Last Modified: Tue, 24 Nov 2020 00:58:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; 386

```console
$ docker pull memcached@sha256:04f9bb7564b8ef32c9b16f7a84a06aa6ce963cd7341fb47580b22b5240e84ffb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31183406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2a87dfef3d28a151095f6d0a0d6cda6fa63975bd76e0221a8a04bfe82dea0e6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 17 Nov 2020 20:19:58 GMT
ADD file:b17dfa607fcb298beb9c58bfbb8b9b0743ceb385875776c56269db2506840edf in / 
# Tue, 17 Nov 2020 20:19:58 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 06:51:09 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 18 Nov 2020 06:51:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 24 Nov 2020 00:38:23 GMT
ENV MEMCACHED_VERSION=1.6.9
# Tue, 24 Nov 2020 00:38:23 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Tue, 24 Nov 2020 00:42:38 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 24 Nov 2020 00:42:39 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 Nov 2020 00:42:39 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 Nov 2020 00:42:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Nov 2020 00:42:40 GMT
USER memcache
# Tue, 24 Nov 2020 00:42:40 GMT
EXPOSE 11211
# Tue, 24 Nov 2020 00:42:40 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:e8e82c9fb36b8f3a9b8f18fe1d88e4d425d5c45968e3f2e94cdbb1255feb4878`  
		Last Modified: Tue, 17 Nov 2020 20:26:45 GMT  
		Size: 27.8 MB (27766186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:321cbeb51acb785f1b1c182cedb4064f03df6af524b61820be6dcd5b1cb2f8a2`  
		Last Modified: Wed, 18 Nov 2020 07:00:37 GMT  
		Size: 4.9 KB (4893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9992095793664bbd90982439c87351ec23b212e9622d90a144faa60a7acbe6d`  
		Last Modified: Wed, 18 Nov 2020 07:00:38 GMT  
		Size: 2.2 MB (2208086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7345a22027cf324340c6fe54efa2e573f790817c593fc990c4eb41f1d731061`  
		Last Modified: Tue, 24 Nov 2020 00:47:51 GMT  
		Size: 1.2 MB (1203835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94d7cbd4098036b6b2a3ddba5fd780fb6875c10dc8df39a054bcd89187a62bcd`  
		Last Modified: Tue, 24 Nov 2020 00:47:50 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53794b9614d9d66687bd0c4938c508a6dcd7e7970d8ba3c2078635fe95d6c856`  
		Last Modified: Tue, 24 Nov 2020 00:47:50 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; mips64le

```console
$ docker pull memcached@sha256:8bc36ac7c7accfbf668832c1f44aa9b8a72eea77027dd1cda17b12353928fc03
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.8 MB (28757547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23d47b7544c777f79de3b1b39c9d4702573764e302f83401ec54210ebc22c514`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 17 Nov 2020 20:19:24 GMT
ADD file:98a1b26b3eefd56b2867344c8c58f4bc3ef9a19c28e35c41df77ab80598d41bc in / 
# Tue, 17 Nov 2020 20:19:24 GMT
CMD ["bash"]
# Mon, 23 Nov 2020 23:07:26 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Mon, 23 Nov 2020 23:07:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 23 Nov 2020 23:07:39 GMT
ENV MEMCACHED_VERSION=1.6.9
# Mon, 23 Nov 2020 23:07:39 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Mon, 23 Nov 2020 23:13:24 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Mon, 23 Nov 2020 23:13:24 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 23 Nov 2020 23:13:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 23 Nov 2020 23:13:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 Nov 2020 23:13:26 GMT
USER memcache
# Mon, 23 Nov 2020 23:13:27 GMT
EXPOSE 11211
# Mon, 23 Nov 2020 23:13:27 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:071bb0a152ef32db0e7d172bcc4722a6a275885249ddb72bee023e268e82fc16`  
		Last Modified: Tue, 17 Nov 2020 20:26:34 GMT  
		Size: 25.8 MB (25777477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:664f5d146d813d299af77e5fc0e344f8a75bd40824a60c99a04bdb1ff4b13b43`  
		Last Modified: Mon, 23 Nov 2020 23:13:45 GMT  
		Size: 5.0 KB (4982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9431da82e8f3642d3474b3944f281ce0d9d5f81e50a7d814cc06bc4db3a55ff6`  
		Last Modified: Mon, 23 Nov 2020 23:13:46 GMT  
		Size: 1.8 MB (1776012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72e10c1044bcc0ce9b31d6c01d3f1b6be4c9a227a8d757cd5fbb803190e0372c`  
		Last Modified: Mon, 23 Nov 2020 23:13:46 GMT  
		Size: 1.2 MB (1198668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0d2b229dc61a9fd2afe3edd3cdf4354d3153027b44b22fec64257ac3e07c4e`  
		Last Modified: Mon, 23 Nov 2020 23:13:45 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ae54e7810b124e108a6331526af87033a40abd56d009854ad078554273f41b`  
		Last Modified: Mon, 23 Nov 2020 23:13:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; ppc64le

```console
$ docker pull memcached@sha256:5233f7be9d0b23aa88bf7fc2e75310bdb632ec93aa2db03c39ef676fbd2c111f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34085325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ed1158f0082c5bd5c24e244191a1a7c8dc37a0db0a0f27a9a61d238a6f45b60`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 17 Nov 2020 23:23:06 GMT
ADD file:49cd8b08964980901349e1f3d6cb34abd8145dea6e6d9ab83502452281ac73ca in / 
# Tue, 17 Nov 2020 23:23:11 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 02:08:02 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 18 Nov 2020 02:08:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 02:08:53 GMT
ENV MEMCACHED_VERSION=1.6.8
# Wed, 18 Nov 2020 02:09:05 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Wed, 18 Nov 2020 02:21:00 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 18 Nov 2020 02:21:04 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 18 Nov 2020 02:21:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 18 Nov 2020 02:21:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Nov 2020 02:21:20 GMT
USER memcache
# Wed, 18 Nov 2020 02:21:23 GMT
EXPOSE 11211
# Wed, 18 Nov 2020 02:21:29 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d79345c10f03543bff3982aedb35a18ba18626c0074014387ff5e1dc14474e2b`  
		Last Modified: Tue, 17 Nov 2020 23:32:54 GMT  
		Size: 30.5 MB (30531702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c81cd83e42b497f0cba94fa5211dd383d0d43fb3fefb1c49d84df1ec1bb8706`  
		Last Modified: Wed, 18 Nov 2020 02:21:58 GMT  
		Size: 5.0 KB (4990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2755aa03159fc35fb59a7fc785b128fa60a5940abb4d5777fea087d0a61c07a`  
		Last Modified: Wed, 18 Nov 2020 02:21:59 GMT  
		Size: 2.3 MB (2322767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f132d007583b65a7dae9876fd53c3ceb86e63cf51c9ac01c83d0c1ad73925ad`  
		Last Modified: Wed, 18 Nov 2020 02:21:58 GMT  
		Size: 1.2 MB (1225459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac54fbbfdd63057bf31b8403a24213cfb6c131e9e6e691bb90e9d35d8deb479`  
		Last Modified: Wed, 18 Nov 2020 02:21:58 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1fc8692195395ae28bbb8eadfb2c8e2cd572559f1b92bf620013f723f52303c`  
		Last Modified: Wed, 18 Nov 2020 02:21:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; s390x

```console
$ docker pull memcached@sha256:d4f378fbb763346873fb016770ad2e202370f526d24ccbeffc2f3a1247b9b3d5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.8 MB (28811191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ff2b9ce713317a592f1208e112eec5e2b257bd5b8a46984c37d8b8e63c010d3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 17 Nov 2020 20:18:29 GMT
ADD file:4a3215d1c9b4afb58053c4fff8d121547890c2a71bc027992f7f960551c6acb1 in / 
# Tue, 17 Nov 2020 20:18:34 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 01:46:32 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 18 Nov 2020 01:46:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 24 Nov 2020 01:29:39 GMT
ENV MEMCACHED_VERSION=1.6.9
# Tue, 24 Nov 2020 01:29:40 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Tue, 24 Nov 2020 01:38:32 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 24 Nov 2020 01:38:33 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 Nov 2020 01:38:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 Nov 2020 01:38:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Nov 2020 01:38:36 GMT
USER memcache
# Tue, 24 Nov 2020 01:38:36 GMT
EXPOSE 11211
# Tue, 24 Nov 2020 01:38:37 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c0d5e3cc51c0b20d3f68226f5332c9a9c2b17cce2f362ec742d4ed325ff7b530`  
		Last Modified: Tue, 17 Nov 2020 20:23:43 GMT  
		Size: 25.7 MB (25721143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b189bf5a9f20baf2f6e6ec9230535bdc36fc750196dd1e3f5eb5e17ee36a31`  
		Last Modified: Wed, 18 Nov 2020 01:53:06 GMT  
		Size: 5.0 KB (5027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1372a3dddcc126d1aad6887514b61ad9ac946b00f50834efdd6c376cc6cfcf65`  
		Last Modified: Wed, 18 Nov 2020 01:53:06 GMT  
		Size: 1.9 MB (1886092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d6c632cdb2f59084328d009bb036821bfe895d1bc1d1512150931d115ea0b40`  
		Last Modified: Tue, 24 Nov 2020 01:43:04 GMT  
		Size: 1.2 MB (1198521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247f0621f757137d4d49d296cd294fef8816daca0331d8406990d31eab886d2e`  
		Last Modified: Tue, 24 Nov 2020 01:43:03 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b13354fbc1d862e30d1c831d85eb9a4e24ba519cc341b6097aa6209cfd530e99`  
		Last Modified: Tue, 24 Nov 2020 01:43:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.9`

```console
$ docker pull memcached@sha256:a5aaa8082ed5d24dd3c4b6a4f044634deaaa61cbba53accb5d295157e86d058e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; s390x

### `memcached:1.6.9` - linux; amd64

```console
$ docker pull memcached@sha256:efe79d6cb73884b4cdc639183c3bdd27692034e92bd97a6972347db1f3f9940b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30513603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08ea1a3256c49616070a12b913da5051d159b2e7dc913e8a62ce0538f7a8a02a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:17 GMT
ADD file:d2abb0e4e7ac1773741f51f57d3a0b8ffc7907348842d773f8c341ba17f856d5 in / 
# Tue, 17 Nov 2020 20:21:17 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 23:59:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 17 Nov 2020 23:59:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 24 Nov 2020 00:40:08 GMT
ENV MEMCACHED_VERSION=1.6.9
# Tue, 24 Nov 2020 00:40:08 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Tue, 24 Nov 2020 00:44:14 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 24 Nov 2020 00:44:15 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 Nov 2020 00:44:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 Nov 2020 00:44:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Nov 2020 00:44:16 GMT
USER memcache
# Tue, 24 Nov 2020 00:44:16 GMT
EXPOSE 11211
# Tue, 24 Nov 2020 00:44:16 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:852e50cd189dfeb54d97680d9fa6bed21a6d7d18cfb56d6abfe2de9d7f173795`  
		Last Modified: Tue, 17 Nov 2020 20:27:25 GMT  
		Size: 27.1 MB (27105484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba259e022fc04d1e3da7b6650e0a253d23ade0fc8efd7f96e9146dd9337e7d74`  
		Last Modified: Wed, 18 Nov 2020 00:04:25 GMT  
		Size: 5.0 KB (4977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baff9e329932a3fa2a84550d57f41fa83ebd732b2079111e74f62ccbcaaeb084`  
		Last Modified: Wed, 18 Nov 2020 00:04:25 GMT  
		Size: 2.2 MB (2196434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f513b04a1f26d0f649ac982e308a03bcfa2cc147aa2654d57beca1d3c0ddfe2`  
		Last Modified: Tue, 24 Nov 2020 00:49:06 GMT  
		Size: 1.2 MB (1206301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb255edcd3e1c523644c575b9a937eab78cd4bb1b719a8e5030f81dab71bb9c3`  
		Last Modified: Tue, 24 Nov 2020 00:49:06 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee1dea1b4991d10177d54c728588378dfc740149e2dab0a2bb461f8e1ceb2d06`  
		Last Modified: Tue, 24 Nov 2020 00:49:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.9` - linux; arm variant v5

```console
$ docker pull memcached@sha256:b506cd917be5e584884f6bd23ab1c33563d1202186141d018e0b1efdb6d44536
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27931449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c96be237e7151156f8f06cc8123c1bdd31017cfc47efb0fbe0100317d3659424`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 17 Nov 2020 20:20:37 GMT
ADD file:d75cebdc79385debd2d6d1c8c34855d2bd4779b13ee47f76e34c6d8fca037531 in / 
# Tue, 17 Nov 2020 20:20:45 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 05:58:29 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 18 Nov 2020 05:58:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 23 Nov 2020 23:52:57 GMT
ENV MEMCACHED_VERSION=1.6.9
# Mon, 23 Nov 2020 23:52:59 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Mon, 23 Nov 2020 23:56:36 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Mon, 23 Nov 2020 23:56:37 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 23 Nov 2020 23:56:39 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 23 Nov 2020 23:56:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 Nov 2020 23:56:40 GMT
USER memcache
# Mon, 23 Nov 2020 23:56:41 GMT
EXPOSE 11211
# Mon, 23 Nov 2020 23:56:42 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1b8dd2ec17ab788b6ea03a9b6cf68afada9a8692681d29e9795db0abf6554404`  
		Last Modified: Tue, 17 Nov 2020 20:30:33 GMT  
		Size: 24.9 MB (24850311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eab7493baf19e0692ceefecef0ac524fdb4ba00028370800b97c2f0fdb2a840`  
		Last Modified: Wed, 18 Nov 2020 06:02:40 GMT  
		Size: 4.9 KB (4898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b096e22e759388a2bd7f3d04ba63e0b2fbbe300fe4093e3699e0ead554d3026`  
		Last Modified: Wed, 18 Nov 2020 06:02:40 GMT  
		Size: 1.9 MB (1896787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed956595633e1910b74834c64a03cbfa6fb9b0dd7c712ab74e05abaa2325aae`  
		Last Modified: Mon, 23 Nov 2020 23:56:53 GMT  
		Size: 1.2 MB (1179045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08931b56db74dd19b895412f1f1cc01c3416ff07a9b06d5db052cdb685d7975f`  
		Last Modified: Mon, 23 Nov 2020 23:56:52 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d581c95c1973377e4b69f2ee972d2e88141b440606f04bb7cf035a987ccc412`  
		Last Modified: Mon, 23 Nov 2020 23:56:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.9` - linux; arm variant v7

```console
$ docker pull memcached@sha256:23bfdefe9cc175f1d85d34f46637c56c49f675daac226d2ef27875d88f1d634a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25680615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83cc6416458d599f47ab03ce627dc26358df5d4d8e352bc0ed0e2e1e8bc9e031`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:06 GMT
ADD file:2035658a8d20545ee7b2ab3ee791a371925fca7968ac29435303da24a1378f34 in / 
# Tue, 17 Nov 2020 20:21:10 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 22:43:01 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 17 Nov 2020 22:43:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 24 Nov 2020 00:22:17 GMT
ENV MEMCACHED_VERSION=1.6.9
# Tue, 24 Nov 2020 00:22:18 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Tue, 24 Nov 2020 00:25:37 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 24 Nov 2020 00:25:38 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 Nov 2020 00:25:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 Nov 2020 00:25:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Nov 2020 00:25:42 GMT
USER memcache
# Tue, 24 Nov 2020 00:25:43 GMT
EXPOSE 11211
# Tue, 24 Nov 2020 00:25:48 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d5029e4b387017f20ad9f77baf3b81dd41f851d6340363b842a8a1d9786a60a0`  
		Last Modified: Tue, 17 Nov 2020 20:31:46 GMT  
		Size: 22.7 MB (22714186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dcb178bde3efeefaad9cde6e23e198ace47cd12278a903916a98fe226425c63`  
		Last Modified: Tue, 17 Nov 2020 22:47:04 GMT  
		Size: 4.9 KB (4888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:849c9255e9336e765f5fe8a15ddde316c5b6f9a38454be317f5b88d23490d4e9`  
		Last Modified: Tue, 17 Nov 2020 22:47:04 GMT  
		Size: 1.8 MB (1811529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee4f7e83b65d682e21adba125e9b5a00b62239a5f2a45a02a8ee980c77c033ed`  
		Last Modified: Tue, 24 Nov 2020 00:29:37 GMT  
		Size: 1.1 MB (1149604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae88eab2c47891856beb68524c3b63058f3c28a17b0cc5f9a2b7a310f0b23245`  
		Last Modified: Tue, 24 Nov 2020 00:29:37 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d745615f6bde6bb77f0f3c84750b88a63812b46e1972b2d40a987307300373f`  
		Last Modified: Tue, 24 Nov 2020 00:29:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.9` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:bca7dce6878924796ed4e59749a20a99b8b21095a6622de36e1669854f3995e7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29121866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b4113f866ef34853e089e9828737b4a19cfd3e9b7ab4673fb6b314a94105e1a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 17 Nov 2020 20:23:31 GMT
ADD file:a70d8c01f8f04f36038968567af779883f3b5ba3147b662b7d170d80418bc23c in / 
# Tue, 17 Nov 2020 20:23:32 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 01:22:43 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 18 Nov 2020 01:22:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 24 Nov 2020 00:47:00 GMT
ENV MEMCACHED_VERSION=1.6.9
# Tue, 24 Nov 2020 00:47:01 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Tue, 24 Nov 2020 00:54:18 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 24 Nov 2020 00:54:19 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 Nov 2020 00:54:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 Nov 2020 00:54:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Nov 2020 00:54:23 GMT
USER memcache
# Tue, 24 Nov 2020 00:54:24 GMT
EXPOSE 11211
# Tue, 24 Nov 2020 00:54:24 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:29ade854e0dcedde295dd89890d45271e9df839e42124558eb5283508ca70f5c`  
		Last Modified: Tue, 17 Nov 2020 20:32:02 GMT  
		Size: 25.9 MB (25862532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b138bddb332a0f874407cfaec3014ec6614883be703b52ff29808980118a91`  
		Last Modified: Wed, 18 Nov 2020 01:26:58 GMT  
		Size: 5.0 KB (5024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5452540f15530cb8fe9343e88516c0b3050b9bb0596613026fe0f84b13c30d6c`  
		Last Modified: Wed, 18 Nov 2020 01:26:59 GMT  
		Size: 2.1 MB (2074952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:373464c46512a6172ca94cdb2aaf1427f0710ce8289bf2a4a73b3a8eac65e689`  
		Last Modified: Tue, 24 Nov 2020 00:58:10 GMT  
		Size: 1.2 MB (1178950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d995428ce6fac044c4080e2e653157b5d2c86c8940d16d85d20ff3094d47d4`  
		Last Modified: Tue, 24 Nov 2020 00:58:09 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac3fb0a8b0191b0f3b130c75bc5d77bdecc4c5f041e4f0c0c8820cf189c5e785`  
		Last Modified: Tue, 24 Nov 2020 00:58:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.9` - linux; 386

```console
$ docker pull memcached@sha256:04f9bb7564b8ef32c9b16f7a84a06aa6ce963cd7341fb47580b22b5240e84ffb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31183406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2a87dfef3d28a151095f6d0a0d6cda6fa63975bd76e0221a8a04bfe82dea0e6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 17 Nov 2020 20:19:58 GMT
ADD file:b17dfa607fcb298beb9c58bfbb8b9b0743ceb385875776c56269db2506840edf in / 
# Tue, 17 Nov 2020 20:19:58 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 06:51:09 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 18 Nov 2020 06:51:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 24 Nov 2020 00:38:23 GMT
ENV MEMCACHED_VERSION=1.6.9
# Tue, 24 Nov 2020 00:38:23 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Tue, 24 Nov 2020 00:42:38 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 24 Nov 2020 00:42:39 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 Nov 2020 00:42:39 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 Nov 2020 00:42:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Nov 2020 00:42:40 GMT
USER memcache
# Tue, 24 Nov 2020 00:42:40 GMT
EXPOSE 11211
# Tue, 24 Nov 2020 00:42:40 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:e8e82c9fb36b8f3a9b8f18fe1d88e4d425d5c45968e3f2e94cdbb1255feb4878`  
		Last Modified: Tue, 17 Nov 2020 20:26:45 GMT  
		Size: 27.8 MB (27766186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:321cbeb51acb785f1b1c182cedb4064f03df6af524b61820be6dcd5b1cb2f8a2`  
		Last Modified: Wed, 18 Nov 2020 07:00:37 GMT  
		Size: 4.9 KB (4893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9992095793664bbd90982439c87351ec23b212e9622d90a144faa60a7acbe6d`  
		Last Modified: Wed, 18 Nov 2020 07:00:38 GMT  
		Size: 2.2 MB (2208086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7345a22027cf324340c6fe54efa2e573f790817c593fc990c4eb41f1d731061`  
		Last Modified: Tue, 24 Nov 2020 00:47:51 GMT  
		Size: 1.2 MB (1203835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94d7cbd4098036b6b2a3ddba5fd780fb6875c10dc8df39a054bcd89187a62bcd`  
		Last Modified: Tue, 24 Nov 2020 00:47:50 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53794b9614d9d66687bd0c4938c508a6dcd7e7970d8ba3c2078635fe95d6c856`  
		Last Modified: Tue, 24 Nov 2020 00:47:50 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.9` - linux; mips64le

```console
$ docker pull memcached@sha256:8bc36ac7c7accfbf668832c1f44aa9b8a72eea77027dd1cda17b12353928fc03
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.8 MB (28757547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23d47b7544c777f79de3b1b39c9d4702573764e302f83401ec54210ebc22c514`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 17 Nov 2020 20:19:24 GMT
ADD file:98a1b26b3eefd56b2867344c8c58f4bc3ef9a19c28e35c41df77ab80598d41bc in / 
# Tue, 17 Nov 2020 20:19:24 GMT
CMD ["bash"]
# Mon, 23 Nov 2020 23:07:26 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Mon, 23 Nov 2020 23:07:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 23 Nov 2020 23:07:39 GMT
ENV MEMCACHED_VERSION=1.6.9
# Mon, 23 Nov 2020 23:07:39 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Mon, 23 Nov 2020 23:13:24 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Mon, 23 Nov 2020 23:13:24 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 23 Nov 2020 23:13:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 23 Nov 2020 23:13:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 Nov 2020 23:13:26 GMT
USER memcache
# Mon, 23 Nov 2020 23:13:27 GMT
EXPOSE 11211
# Mon, 23 Nov 2020 23:13:27 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:071bb0a152ef32db0e7d172bcc4722a6a275885249ddb72bee023e268e82fc16`  
		Last Modified: Tue, 17 Nov 2020 20:26:34 GMT  
		Size: 25.8 MB (25777477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:664f5d146d813d299af77e5fc0e344f8a75bd40824a60c99a04bdb1ff4b13b43`  
		Last Modified: Mon, 23 Nov 2020 23:13:45 GMT  
		Size: 5.0 KB (4982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9431da82e8f3642d3474b3944f281ce0d9d5f81e50a7d814cc06bc4db3a55ff6`  
		Last Modified: Mon, 23 Nov 2020 23:13:46 GMT  
		Size: 1.8 MB (1776012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72e10c1044bcc0ce9b31d6c01d3f1b6be4c9a227a8d757cd5fbb803190e0372c`  
		Last Modified: Mon, 23 Nov 2020 23:13:46 GMT  
		Size: 1.2 MB (1198668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0d2b229dc61a9fd2afe3edd3cdf4354d3153027b44b22fec64257ac3e07c4e`  
		Last Modified: Mon, 23 Nov 2020 23:13:45 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ae54e7810b124e108a6331526af87033a40abd56d009854ad078554273f41b`  
		Last Modified: Mon, 23 Nov 2020 23:13:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.9` - linux; s390x

```console
$ docker pull memcached@sha256:d4f378fbb763346873fb016770ad2e202370f526d24ccbeffc2f3a1247b9b3d5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.8 MB (28811191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ff2b9ce713317a592f1208e112eec5e2b257bd5b8a46984c37d8b8e63c010d3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 17 Nov 2020 20:18:29 GMT
ADD file:4a3215d1c9b4afb58053c4fff8d121547890c2a71bc027992f7f960551c6acb1 in / 
# Tue, 17 Nov 2020 20:18:34 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 01:46:32 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 18 Nov 2020 01:46:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 24 Nov 2020 01:29:39 GMT
ENV MEMCACHED_VERSION=1.6.9
# Tue, 24 Nov 2020 01:29:40 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Tue, 24 Nov 2020 01:38:32 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 24 Nov 2020 01:38:33 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 Nov 2020 01:38:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 Nov 2020 01:38:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Nov 2020 01:38:36 GMT
USER memcache
# Tue, 24 Nov 2020 01:38:36 GMT
EXPOSE 11211
# Tue, 24 Nov 2020 01:38:37 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c0d5e3cc51c0b20d3f68226f5332c9a9c2b17cce2f362ec742d4ed325ff7b530`  
		Last Modified: Tue, 17 Nov 2020 20:23:43 GMT  
		Size: 25.7 MB (25721143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b189bf5a9f20baf2f6e6ec9230535bdc36fc750196dd1e3f5eb5e17ee36a31`  
		Last Modified: Wed, 18 Nov 2020 01:53:06 GMT  
		Size: 5.0 KB (5027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1372a3dddcc126d1aad6887514b61ad9ac946b00f50834efdd6c376cc6cfcf65`  
		Last Modified: Wed, 18 Nov 2020 01:53:06 GMT  
		Size: 1.9 MB (1886092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d6c632cdb2f59084328d009bb036821bfe895d1bc1d1512150931d115ea0b40`  
		Last Modified: Tue, 24 Nov 2020 01:43:04 GMT  
		Size: 1.2 MB (1198521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247f0621f757137d4d49d296cd294fef8816daca0331d8406990d31eab886d2e`  
		Last Modified: Tue, 24 Nov 2020 01:43:03 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b13354fbc1d862e30d1c831d85eb9a4e24ba519cc341b6097aa6209cfd530e99`  
		Last Modified: Tue, 24 Nov 2020 01:43:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.9-alpine`

```console
$ docker pull memcached@sha256:9a9a6195edfc684d4861d6093856ad5bf612fcbbbedc65d0abe661a75c3af07f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; s390x

### `memcached:1.6.9-alpine` - linux; amd64

```console
$ docker pull memcached@sha256:e1928aafa8833a2470b47fcc89754c26403ba3cda2ecbb4c4266072279e22576
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4886255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff697670a954aa7c8407c1f4391c129aea5e6c94f3728513631fed5f7756e164`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 06:13:10 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 22 Oct 2020 06:13:11 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 24 Nov 2020 00:44:26 GMT
ENV MEMCACHED_VERSION=1.6.9
# Tue, 24 Nov 2020 00:44:26 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Tue, 24 Nov 2020 00:48:41 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 Nov 2020 00:48:42 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 Nov 2020 00:48:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 Nov 2020 00:48:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Nov 2020 00:48:43 GMT
USER memcache
# Tue, 24 Nov 2020 00:48:43 GMT
EXPOSE 11211
# Tue, 24 Nov 2020 00:48:44 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d1b6a787fe50693a51ebeff9bc428c161df9b2e970c32316dd2ae2b5c527dba`  
		Last Modified: Thu, 22 Oct 2020 06:23:41 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0ca5f2b599ba9318ceb754cff704386c2105eef5536b716bea76ed53c872ae4`  
		Last Modified: Thu, 22 Oct 2020 06:23:41 GMT  
		Size: 15.3 KB (15299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b822756c8bfaf1bc207adc2de3741e339a2693e9ee8e311a149808db14b5208`  
		Last Modified: Tue, 24 Nov 2020 00:49:13 GMT  
		Size: 2.1 MB (2072463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af2d6b4d764b9c213154f1680d12d1ccf7241e76e6064dda66d5d3c3031f0e2b`  
		Last Modified: Tue, 24 Nov 2020 00:49:13 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e55816799a4db3ab4e13a264038fa0de836f4301b050cca3324eb8290e423e62`  
		Last Modified: Tue, 24 Nov 2020 00:49:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.9-alpine` - linux; arm variant v6

```console
$ docker pull memcached@sha256:84a8ab8b2c2ae46bba6afd02619cb1d0a180fd46d11749f1cb624b952ab8c9f1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4647852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c1779891a9245caed80bbadedd3187997a4cd109651441cbf70107bc5045c55`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 05:51:39 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 22 Oct 2020 05:53:12 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 24 Nov 2020 00:04:10 GMT
ENV MEMCACHED_VERSION=1.6.9
# Tue, 24 Nov 2020 00:04:10 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Tue, 24 Nov 2020 00:07:15 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 Nov 2020 00:07:16 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 Nov 2020 00:07:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 Nov 2020 00:07:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Nov 2020 00:07:19 GMT
USER memcache
# Tue, 24 Nov 2020 00:07:19 GMT
EXPOSE 11211
# Tue, 24 Nov 2020 00:07:20 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74cfe72068d6a66c0b7a1abfb1e0f80970db6ef63759ceea1ce866e61e85c16a`  
		Last Modified: Thu, 22 Oct 2020 06:07:10 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e57387f8f435122e3cbbe902349b156804991be332f5bfaaa9472102703b0e8c`  
		Last Modified: Thu, 22 Oct 2020 06:07:11 GMT  
		Size: 14.9 KB (14901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d3cdccf3fbd7cd515e5b74a671cda38dd9df4bcbbd570db901bf84e5003914`  
		Last Modified: Tue, 24 Nov 2020 00:07:32 GMT  
		Size: 2.0 MB (2029372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27ab5b24072ce098cf121983637ecc7320b3b99a6596ee6f3233b82854182fe2`  
		Last Modified: Tue, 24 Nov 2020 00:07:31 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fec87d28784f49a987a725efbd26639511b95005578516f18eb091f70680a17`  
		Last Modified: Tue, 24 Nov 2020 00:07:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.9-alpine` - linux; arm variant v7

```console
$ docker pull memcached@sha256:bbdb2d34f35910a55efd127f93a3b084b4210359d3ba3e04d492a70beea0320e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4313145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7520fc1477e6051f5415fbdf6960a7f9c528353aeb867c7069aa259916176ad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 08:40:04 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 22 Oct 2020 08:40:07 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 24 Nov 2020 00:26:09 GMT
ENV MEMCACHED_VERSION=1.6.9
# Tue, 24 Nov 2020 00:26:10 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Tue, 24 Nov 2020 00:29:05 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 Nov 2020 00:29:06 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 Nov 2020 00:29:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 Nov 2020 00:29:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Nov 2020 00:29:11 GMT
USER memcache
# Tue, 24 Nov 2020 00:29:13 GMT
EXPOSE 11211
# Tue, 24 Nov 2020 00:29:14 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1674e7ddc5cb335deefc31c3d2b6c4b434d04890456bfaae72e3e62b205cd0b6`  
		Last Modified: Thu, 22 Oct 2020 08:50:29 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f08b455b568b076a4ef19ed5615ed2352792bbed759c525ecae331db901df04`  
		Last Modified: Thu, 22 Oct 2020 08:50:30 GMT  
		Size: 13.8 KB (13827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:510b94932fc56e01e3a03af48c5bcaabec2bb336f8f787734bf846feb7de347f`  
		Last Modified: Tue, 24 Nov 2020 00:29:48 GMT  
		Size: 1.9 MB (1891978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88faa5219b31e7f196605b6c2b273fae85f47d56c7fb5d5b320dd544e35414ba`  
		Last Modified: Tue, 24 Nov 2020 00:29:47 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92e34d046a66b160935550f49396501447c4ddb5001f0ec2c33e25b1c3c5059`  
		Last Modified: Tue, 24 Nov 2020 00:29:48 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.9-alpine` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:a869ac02f75f64470176cf16c595e4e58bae5d5d3f442227581808e68763ace4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4811465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fd84a91919653be4583fcf329fccb126128ca56a60319c8f9c28adc05682650`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 04:33:47 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 22 Oct 2020 04:34:20 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 24 Nov 2020 00:54:44 GMT
ENV MEMCACHED_VERSION=1.6.9
# Tue, 24 Nov 2020 00:54:45 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Tue, 24 Nov 2020 00:57:40 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 Nov 2020 00:57:40 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 Nov 2020 00:57:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 Nov 2020 00:57:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Nov 2020 00:57:45 GMT
USER memcache
# Tue, 24 Nov 2020 00:57:45 GMT
EXPOSE 11211
# Tue, 24 Nov 2020 00:57:46 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d21e501aba9ea61896a99eee3b86890f5e2420e0061883d06bb780661eb6dbae`  
		Last Modified: Thu, 22 Oct 2020 04:49:24 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e607140b86f07aa95f3be67e136183ec1def37d74e27ae1141ff257e6960ad1`  
		Last Modified: Thu, 22 Oct 2020 04:49:24 GMT  
		Size: 15.7 KB (15683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed9de8619e85f52cd0657870aadd42de21c84ce68ca3412f496fd6fcd4a22bd`  
		Last Modified: Tue, 24 Nov 2020 00:58:20 GMT  
		Size: 2.1 MB (2087563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1adb1280ccf1abb19444686be75fa42aaf40a41c2c1d972d78188844c921175`  
		Last Modified: Tue, 24 Nov 2020 00:58:21 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78dc9a71b866039ff5461d91fc16d477e864471680f8066f56f37ed996019d83`  
		Last Modified: Tue, 24 Nov 2020 00:58:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.9-alpine` - linux; 386

```console
$ docker pull memcached@sha256:8fe6ce4813127db9eda50ca3d2c739e1ee4e19e6b2604c42857a084f2cee7f20
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4962966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fde562f92d407d755937a5fd62e36ad4e6c11e614f0b1efe15b3c365a5919be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:11:28 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 22 Oct 2020 03:11:30 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 24 Nov 2020 00:42:56 GMT
ENV MEMCACHED_VERSION=1.6.9
# Tue, 24 Nov 2020 00:42:56 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Tue, 24 Nov 2020 00:47:29 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 Nov 2020 00:47:30 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 Nov 2020 00:47:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 Nov 2020 00:47:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Nov 2020 00:47:31 GMT
USER memcache
# Tue, 24 Nov 2020 00:47:31 GMT
EXPOSE 11211
# Tue, 24 Nov 2020 00:47:31 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f331a13b680b3ab05286a77980f705e8f4ab788d6ed224e10e80d9e2ab6a09a4`  
		Last Modified: Thu, 22 Oct 2020 03:21:50 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b40ae29247453a11c0bbfb92db01b919397d035232e9ef9fbc9e526af9e132`  
		Last Modified: Thu, 22 Oct 2020 03:21:50 GMT  
		Size: 16.3 KB (16323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a7eca4f7b1391c2d397e86710de5666847f1cb0acef37165d31b41883f22895`  
		Last Modified: Tue, 24 Nov 2020 00:47:58 GMT  
		Size: 2.2 MB (2153599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9fe46f7c3454fca381ef88344cfa1726d58a48fd7ddcbe6677de774e70c4c3`  
		Last Modified: Tue, 24 Nov 2020 00:47:57 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c645f1cec0c95903a4212ca1390af1c4ff8c0a4219b7a7ac4bedd631da2d447`  
		Last Modified: Tue, 24 Nov 2020 00:47:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.9-alpine` - linux; s390x

```console
$ docker pull memcached@sha256:a54e2e0ee91bb55a0d8521a4ab8f30649588d259e6b18320f292e51025dc35b8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4676494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e05224f43fe277aeda8f17fc8ded12da4a0d81a153a08e34d8ddf961d5c2d7e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 22 Oct 2020 01:59:08 GMT
ADD file:e07d6f40b1afc3d3eff230bc89e84704eb762706a373a60c6bea6a45b2287464 in / 
# Thu, 22 Oct 2020 01:59:09 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:10:18 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 22 Oct 2020 03:10:20 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 24 Nov 2020 01:38:51 GMT
ENV MEMCACHED_VERSION=1.6.9
# Tue, 24 Nov 2020 01:38:52 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Tue, 24 Nov 2020 01:42:39 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 Nov 2020 01:42:39 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 Nov 2020 01:42:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 Nov 2020 01:42:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Nov 2020 01:42:43 GMT
USER memcache
# Tue, 24 Nov 2020 01:42:43 GMT
EXPOSE 11211
# Tue, 24 Nov 2020 01:42:44 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a4c84ece3d2b98927d25f13a4f367bfd96cbfae272f6ff1117d74c84b92d11d3`  
		Last Modified: Thu, 22 Oct 2020 01:59:37 GMT  
		Size: 2.6 MB (2565829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e98aa9130fa92579b5c432ac74178649f4fd0284da983980df01d2d851561f`  
		Last Modified: Thu, 22 Oct 2020 03:20:27 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d6f60d4914d39284ba2d65ad8bb43b4421039cbfdf061f9c0bcb187e3790b4`  
		Last Modified: Thu, 22 Oct 2020 03:20:26 GMT  
		Size: 15.6 KB (15570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18bd0358bc33c61ca0847dc0ae52053ab05c8491609929457c3e5195a035ce1b`  
		Last Modified: Tue, 24 Nov 2020 01:43:20 GMT  
		Size: 2.1 MB (2093430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2eea37208f09cfee5b7632f5f78f5cf51df5b2b248d14d585ba256baad4914f`  
		Last Modified: Tue, 24 Nov 2020 01:43:19 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09896b451609b7d0e69a6af517cff8a599cf66df743696a3b53b57bd13d89582`  
		Last Modified: Tue, 24 Nov 2020 01:43:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6-alpine`

```console
$ docker pull memcached@sha256:32a6ff0c8679603a3977c810419511d6137db92c4f01d0d8282aa397e5cf71c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1.6-alpine` - linux; amd64

```console
$ docker pull memcached@sha256:e1928aafa8833a2470b47fcc89754c26403ba3cda2ecbb4c4266072279e22576
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4886255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff697670a954aa7c8407c1f4391c129aea5e6c94f3728513631fed5f7756e164`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 06:13:10 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 22 Oct 2020 06:13:11 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 24 Nov 2020 00:44:26 GMT
ENV MEMCACHED_VERSION=1.6.9
# Tue, 24 Nov 2020 00:44:26 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Tue, 24 Nov 2020 00:48:41 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 Nov 2020 00:48:42 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 Nov 2020 00:48:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 Nov 2020 00:48:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Nov 2020 00:48:43 GMT
USER memcache
# Tue, 24 Nov 2020 00:48:43 GMT
EXPOSE 11211
# Tue, 24 Nov 2020 00:48:44 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d1b6a787fe50693a51ebeff9bc428c161df9b2e970c32316dd2ae2b5c527dba`  
		Last Modified: Thu, 22 Oct 2020 06:23:41 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0ca5f2b599ba9318ceb754cff704386c2105eef5536b716bea76ed53c872ae4`  
		Last Modified: Thu, 22 Oct 2020 06:23:41 GMT  
		Size: 15.3 KB (15299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b822756c8bfaf1bc207adc2de3741e339a2693e9ee8e311a149808db14b5208`  
		Last Modified: Tue, 24 Nov 2020 00:49:13 GMT  
		Size: 2.1 MB (2072463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af2d6b4d764b9c213154f1680d12d1ccf7241e76e6064dda66d5d3c3031f0e2b`  
		Last Modified: Tue, 24 Nov 2020 00:49:13 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e55816799a4db3ab4e13a264038fa0de836f4301b050cca3324eb8290e423e62`  
		Last Modified: Tue, 24 Nov 2020 00:49:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; arm variant v6

```console
$ docker pull memcached@sha256:84a8ab8b2c2ae46bba6afd02619cb1d0a180fd46d11749f1cb624b952ab8c9f1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4647852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c1779891a9245caed80bbadedd3187997a4cd109651441cbf70107bc5045c55`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 05:51:39 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 22 Oct 2020 05:53:12 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 24 Nov 2020 00:04:10 GMT
ENV MEMCACHED_VERSION=1.6.9
# Tue, 24 Nov 2020 00:04:10 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Tue, 24 Nov 2020 00:07:15 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 Nov 2020 00:07:16 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 Nov 2020 00:07:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 Nov 2020 00:07:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Nov 2020 00:07:19 GMT
USER memcache
# Tue, 24 Nov 2020 00:07:19 GMT
EXPOSE 11211
# Tue, 24 Nov 2020 00:07:20 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74cfe72068d6a66c0b7a1abfb1e0f80970db6ef63759ceea1ce866e61e85c16a`  
		Last Modified: Thu, 22 Oct 2020 06:07:10 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e57387f8f435122e3cbbe902349b156804991be332f5bfaaa9472102703b0e8c`  
		Last Modified: Thu, 22 Oct 2020 06:07:11 GMT  
		Size: 14.9 KB (14901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d3cdccf3fbd7cd515e5b74a671cda38dd9df4bcbbd570db901bf84e5003914`  
		Last Modified: Tue, 24 Nov 2020 00:07:32 GMT  
		Size: 2.0 MB (2029372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27ab5b24072ce098cf121983637ecc7320b3b99a6596ee6f3233b82854182fe2`  
		Last Modified: Tue, 24 Nov 2020 00:07:31 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fec87d28784f49a987a725efbd26639511b95005578516f18eb091f70680a17`  
		Last Modified: Tue, 24 Nov 2020 00:07:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; arm variant v7

```console
$ docker pull memcached@sha256:bbdb2d34f35910a55efd127f93a3b084b4210359d3ba3e04d492a70beea0320e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4313145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7520fc1477e6051f5415fbdf6960a7f9c528353aeb867c7069aa259916176ad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 08:40:04 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 22 Oct 2020 08:40:07 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 24 Nov 2020 00:26:09 GMT
ENV MEMCACHED_VERSION=1.6.9
# Tue, 24 Nov 2020 00:26:10 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Tue, 24 Nov 2020 00:29:05 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 Nov 2020 00:29:06 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 Nov 2020 00:29:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 Nov 2020 00:29:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Nov 2020 00:29:11 GMT
USER memcache
# Tue, 24 Nov 2020 00:29:13 GMT
EXPOSE 11211
# Tue, 24 Nov 2020 00:29:14 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1674e7ddc5cb335deefc31c3d2b6c4b434d04890456bfaae72e3e62b205cd0b6`  
		Last Modified: Thu, 22 Oct 2020 08:50:29 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f08b455b568b076a4ef19ed5615ed2352792bbed759c525ecae331db901df04`  
		Last Modified: Thu, 22 Oct 2020 08:50:30 GMT  
		Size: 13.8 KB (13827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:510b94932fc56e01e3a03af48c5bcaabec2bb336f8f787734bf846feb7de347f`  
		Last Modified: Tue, 24 Nov 2020 00:29:48 GMT  
		Size: 1.9 MB (1891978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88faa5219b31e7f196605b6c2b273fae85f47d56c7fb5d5b320dd544e35414ba`  
		Last Modified: Tue, 24 Nov 2020 00:29:47 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92e34d046a66b160935550f49396501447c4ddb5001f0ec2c33e25b1c3c5059`  
		Last Modified: Tue, 24 Nov 2020 00:29:48 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:a869ac02f75f64470176cf16c595e4e58bae5d5d3f442227581808e68763ace4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4811465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fd84a91919653be4583fcf329fccb126128ca56a60319c8f9c28adc05682650`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 04:33:47 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 22 Oct 2020 04:34:20 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 24 Nov 2020 00:54:44 GMT
ENV MEMCACHED_VERSION=1.6.9
# Tue, 24 Nov 2020 00:54:45 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Tue, 24 Nov 2020 00:57:40 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 Nov 2020 00:57:40 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 Nov 2020 00:57:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 Nov 2020 00:57:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Nov 2020 00:57:45 GMT
USER memcache
# Tue, 24 Nov 2020 00:57:45 GMT
EXPOSE 11211
# Tue, 24 Nov 2020 00:57:46 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d21e501aba9ea61896a99eee3b86890f5e2420e0061883d06bb780661eb6dbae`  
		Last Modified: Thu, 22 Oct 2020 04:49:24 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e607140b86f07aa95f3be67e136183ec1def37d74e27ae1141ff257e6960ad1`  
		Last Modified: Thu, 22 Oct 2020 04:49:24 GMT  
		Size: 15.7 KB (15683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed9de8619e85f52cd0657870aadd42de21c84ce68ca3412f496fd6fcd4a22bd`  
		Last Modified: Tue, 24 Nov 2020 00:58:20 GMT  
		Size: 2.1 MB (2087563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1adb1280ccf1abb19444686be75fa42aaf40a41c2c1d972d78188844c921175`  
		Last Modified: Tue, 24 Nov 2020 00:58:21 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78dc9a71b866039ff5461d91fc16d477e864471680f8066f56f37ed996019d83`  
		Last Modified: Tue, 24 Nov 2020 00:58:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; 386

```console
$ docker pull memcached@sha256:8fe6ce4813127db9eda50ca3d2c739e1ee4e19e6b2604c42857a084f2cee7f20
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4962966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fde562f92d407d755937a5fd62e36ad4e6c11e614f0b1efe15b3c365a5919be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:11:28 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 22 Oct 2020 03:11:30 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 24 Nov 2020 00:42:56 GMT
ENV MEMCACHED_VERSION=1.6.9
# Tue, 24 Nov 2020 00:42:56 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Tue, 24 Nov 2020 00:47:29 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 Nov 2020 00:47:30 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 Nov 2020 00:47:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 Nov 2020 00:47:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Nov 2020 00:47:31 GMT
USER memcache
# Tue, 24 Nov 2020 00:47:31 GMT
EXPOSE 11211
# Tue, 24 Nov 2020 00:47:31 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f331a13b680b3ab05286a77980f705e8f4ab788d6ed224e10e80d9e2ab6a09a4`  
		Last Modified: Thu, 22 Oct 2020 03:21:50 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b40ae29247453a11c0bbfb92db01b919397d035232e9ef9fbc9e526af9e132`  
		Last Modified: Thu, 22 Oct 2020 03:21:50 GMT  
		Size: 16.3 KB (16323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a7eca4f7b1391c2d397e86710de5666847f1cb0acef37165d31b41883f22895`  
		Last Modified: Tue, 24 Nov 2020 00:47:58 GMT  
		Size: 2.2 MB (2153599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9fe46f7c3454fca381ef88344cfa1726d58a48fd7ddcbe6677de774e70c4c3`  
		Last Modified: Tue, 24 Nov 2020 00:47:57 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c645f1cec0c95903a4212ca1390af1c4ff8c0a4219b7a7ac4bedd631da2d447`  
		Last Modified: Tue, 24 Nov 2020 00:47:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:7d76bf4416ce1df4bd72710970fa497307b515895f95e2adc44fc0d927e2e3b8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4563787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7de761a79ff461eb8e54e9cd0cc6ceda36e3be45699b7a128f2cbb2b396ff5ad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 22 Oct 2020 11:00:06 GMT
ADD file:176e047fab2c1828575bffa6b14773efa297b7ecf312d86103c5dd4f78ec8027 in / 
# Thu, 22 Oct 2020 11:00:17 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 17:23:41 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 22 Oct 2020 17:23:57 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 27 Oct 2020 18:07:34 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 27 Oct 2020 18:07:36 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Fri, 30 Oct 2020 11:59:46 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 30 Oct 2020 11:59:48 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 30 Oct 2020 11:59:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 30 Oct 2020 11:59:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Oct 2020 11:59:56 GMT
USER memcache
# Fri, 30 Oct 2020 11:59:58 GMT
EXPOSE 11211
# Fri, 30 Oct 2020 12:00:00 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:692a9d763e196c85d79fc3e45b316b1bb557c93ba88a3c8ebf679a585d1efe73`  
		Last Modified: Thu, 22 Oct 2020 11:02:06 GMT  
		Size: 2.8 MB (2803218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c7c711d8b199bfca8f4578f6b934cf1694db2abd446c20fc40d2d8e94dee030`  
		Last Modified: Thu, 22 Oct 2020 17:36:41 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b24a99444366f41bd77307dbe956c7cd7b1fec53557510e9a1c28ca86a6fe90a`  
		Last Modified: Thu, 22 Oct 2020 17:36:40 GMT  
		Size: 16.3 KB (16318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603341c5c367a00c556b1cef2a45967f54bc3c608aeb15b041e6aaeaf5c278ef`  
		Last Modified: Fri, 30 Oct 2020 12:00:22 GMT  
		Size: 1.7 MB (1742583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8baf174d0a545732e56f7b659d48b19270ad1bcab34fb578b58254810b8966`  
		Last Modified: Fri, 30 Oct 2020 12:00:23 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:def13b85f243d3c6d7c04b72d6ec6736627101e18a3f1d3bfff329fac514f188`  
		Last Modified: Fri, 30 Oct 2020 12:00:22 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; s390x

```console
$ docker pull memcached@sha256:a54e2e0ee91bb55a0d8521a4ab8f30649588d259e6b18320f292e51025dc35b8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4676494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e05224f43fe277aeda8f17fc8ded12da4a0d81a153a08e34d8ddf961d5c2d7e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 22 Oct 2020 01:59:08 GMT
ADD file:e07d6f40b1afc3d3eff230bc89e84704eb762706a373a60c6bea6a45b2287464 in / 
# Thu, 22 Oct 2020 01:59:09 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:10:18 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 22 Oct 2020 03:10:20 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 24 Nov 2020 01:38:51 GMT
ENV MEMCACHED_VERSION=1.6.9
# Tue, 24 Nov 2020 01:38:52 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Tue, 24 Nov 2020 01:42:39 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 Nov 2020 01:42:39 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 Nov 2020 01:42:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 Nov 2020 01:42:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Nov 2020 01:42:43 GMT
USER memcache
# Tue, 24 Nov 2020 01:42:43 GMT
EXPOSE 11211
# Tue, 24 Nov 2020 01:42:44 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a4c84ece3d2b98927d25f13a4f367bfd96cbfae272f6ff1117d74c84b92d11d3`  
		Last Modified: Thu, 22 Oct 2020 01:59:37 GMT  
		Size: 2.6 MB (2565829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e98aa9130fa92579b5c432ac74178649f4fd0284da983980df01d2d851561f`  
		Last Modified: Thu, 22 Oct 2020 03:20:27 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d6f60d4914d39284ba2d65ad8bb43b4421039cbfdf061f9c0bcb187e3790b4`  
		Last Modified: Thu, 22 Oct 2020 03:20:26 GMT  
		Size: 15.6 KB (15570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18bd0358bc33c61ca0847dc0ae52053ab05c8491609929457c3e5195a035ce1b`  
		Last Modified: Tue, 24 Nov 2020 01:43:20 GMT  
		Size: 2.1 MB (2093430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2eea37208f09cfee5b7632f5f78f5cf51df5b2b248d14d585ba256baad4914f`  
		Last Modified: Tue, 24 Nov 2020 01:43:19 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09896b451609b7d0e69a6af517cff8a599cf66df743696a3b53b57bd13d89582`  
		Last Modified: Tue, 24 Nov 2020 01:43:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1-alpine`

```console
$ docker pull memcached@sha256:32a6ff0c8679603a3977c810419511d6137db92c4f01d0d8282aa397e5cf71c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1-alpine` - linux; amd64

```console
$ docker pull memcached@sha256:e1928aafa8833a2470b47fcc89754c26403ba3cda2ecbb4c4266072279e22576
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4886255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff697670a954aa7c8407c1f4391c129aea5e6c94f3728513631fed5f7756e164`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 06:13:10 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 22 Oct 2020 06:13:11 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 24 Nov 2020 00:44:26 GMT
ENV MEMCACHED_VERSION=1.6.9
# Tue, 24 Nov 2020 00:44:26 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Tue, 24 Nov 2020 00:48:41 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 Nov 2020 00:48:42 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 Nov 2020 00:48:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 Nov 2020 00:48:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Nov 2020 00:48:43 GMT
USER memcache
# Tue, 24 Nov 2020 00:48:43 GMT
EXPOSE 11211
# Tue, 24 Nov 2020 00:48:44 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d1b6a787fe50693a51ebeff9bc428c161df9b2e970c32316dd2ae2b5c527dba`  
		Last Modified: Thu, 22 Oct 2020 06:23:41 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0ca5f2b599ba9318ceb754cff704386c2105eef5536b716bea76ed53c872ae4`  
		Last Modified: Thu, 22 Oct 2020 06:23:41 GMT  
		Size: 15.3 KB (15299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b822756c8bfaf1bc207adc2de3741e339a2693e9ee8e311a149808db14b5208`  
		Last Modified: Tue, 24 Nov 2020 00:49:13 GMT  
		Size: 2.1 MB (2072463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af2d6b4d764b9c213154f1680d12d1ccf7241e76e6064dda66d5d3c3031f0e2b`  
		Last Modified: Tue, 24 Nov 2020 00:49:13 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e55816799a4db3ab4e13a264038fa0de836f4301b050cca3324eb8290e423e62`  
		Last Modified: Tue, 24 Nov 2020 00:49:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; arm variant v6

```console
$ docker pull memcached@sha256:84a8ab8b2c2ae46bba6afd02619cb1d0a180fd46d11749f1cb624b952ab8c9f1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4647852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c1779891a9245caed80bbadedd3187997a4cd109651441cbf70107bc5045c55`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 05:51:39 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 22 Oct 2020 05:53:12 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 24 Nov 2020 00:04:10 GMT
ENV MEMCACHED_VERSION=1.6.9
# Tue, 24 Nov 2020 00:04:10 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Tue, 24 Nov 2020 00:07:15 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 Nov 2020 00:07:16 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 Nov 2020 00:07:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 Nov 2020 00:07:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Nov 2020 00:07:19 GMT
USER memcache
# Tue, 24 Nov 2020 00:07:19 GMT
EXPOSE 11211
# Tue, 24 Nov 2020 00:07:20 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74cfe72068d6a66c0b7a1abfb1e0f80970db6ef63759ceea1ce866e61e85c16a`  
		Last Modified: Thu, 22 Oct 2020 06:07:10 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e57387f8f435122e3cbbe902349b156804991be332f5bfaaa9472102703b0e8c`  
		Last Modified: Thu, 22 Oct 2020 06:07:11 GMT  
		Size: 14.9 KB (14901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d3cdccf3fbd7cd515e5b74a671cda38dd9df4bcbbd570db901bf84e5003914`  
		Last Modified: Tue, 24 Nov 2020 00:07:32 GMT  
		Size: 2.0 MB (2029372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27ab5b24072ce098cf121983637ecc7320b3b99a6596ee6f3233b82854182fe2`  
		Last Modified: Tue, 24 Nov 2020 00:07:31 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fec87d28784f49a987a725efbd26639511b95005578516f18eb091f70680a17`  
		Last Modified: Tue, 24 Nov 2020 00:07:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; arm variant v7

```console
$ docker pull memcached@sha256:bbdb2d34f35910a55efd127f93a3b084b4210359d3ba3e04d492a70beea0320e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4313145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7520fc1477e6051f5415fbdf6960a7f9c528353aeb867c7069aa259916176ad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 08:40:04 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 22 Oct 2020 08:40:07 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 24 Nov 2020 00:26:09 GMT
ENV MEMCACHED_VERSION=1.6.9
# Tue, 24 Nov 2020 00:26:10 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Tue, 24 Nov 2020 00:29:05 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 Nov 2020 00:29:06 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 Nov 2020 00:29:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 Nov 2020 00:29:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Nov 2020 00:29:11 GMT
USER memcache
# Tue, 24 Nov 2020 00:29:13 GMT
EXPOSE 11211
# Tue, 24 Nov 2020 00:29:14 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1674e7ddc5cb335deefc31c3d2b6c4b434d04890456bfaae72e3e62b205cd0b6`  
		Last Modified: Thu, 22 Oct 2020 08:50:29 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f08b455b568b076a4ef19ed5615ed2352792bbed759c525ecae331db901df04`  
		Last Modified: Thu, 22 Oct 2020 08:50:30 GMT  
		Size: 13.8 KB (13827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:510b94932fc56e01e3a03af48c5bcaabec2bb336f8f787734bf846feb7de347f`  
		Last Modified: Tue, 24 Nov 2020 00:29:48 GMT  
		Size: 1.9 MB (1891978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88faa5219b31e7f196605b6c2b273fae85f47d56c7fb5d5b320dd544e35414ba`  
		Last Modified: Tue, 24 Nov 2020 00:29:47 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92e34d046a66b160935550f49396501447c4ddb5001f0ec2c33e25b1c3c5059`  
		Last Modified: Tue, 24 Nov 2020 00:29:48 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:a869ac02f75f64470176cf16c595e4e58bae5d5d3f442227581808e68763ace4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4811465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fd84a91919653be4583fcf329fccb126128ca56a60319c8f9c28adc05682650`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 04:33:47 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 22 Oct 2020 04:34:20 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 24 Nov 2020 00:54:44 GMT
ENV MEMCACHED_VERSION=1.6.9
# Tue, 24 Nov 2020 00:54:45 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Tue, 24 Nov 2020 00:57:40 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 Nov 2020 00:57:40 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 Nov 2020 00:57:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 Nov 2020 00:57:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Nov 2020 00:57:45 GMT
USER memcache
# Tue, 24 Nov 2020 00:57:45 GMT
EXPOSE 11211
# Tue, 24 Nov 2020 00:57:46 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d21e501aba9ea61896a99eee3b86890f5e2420e0061883d06bb780661eb6dbae`  
		Last Modified: Thu, 22 Oct 2020 04:49:24 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e607140b86f07aa95f3be67e136183ec1def37d74e27ae1141ff257e6960ad1`  
		Last Modified: Thu, 22 Oct 2020 04:49:24 GMT  
		Size: 15.7 KB (15683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed9de8619e85f52cd0657870aadd42de21c84ce68ca3412f496fd6fcd4a22bd`  
		Last Modified: Tue, 24 Nov 2020 00:58:20 GMT  
		Size: 2.1 MB (2087563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1adb1280ccf1abb19444686be75fa42aaf40a41c2c1d972d78188844c921175`  
		Last Modified: Tue, 24 Nov 2020 00:58:21 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78dc9a71b866039ff5461d91fc16d477e864471680f8066f56f37ed996019d83`  
		Last Modified: Tue, 24 Nov 2020 00:58:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; 386

```console
$ docker pull memcached@sha256:8fe6ce4813127db9eda50ca3d2c739e1ee4e19e6b2604c42857a084f2cee7f20
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4962966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fde562f92d407d755937a5fd62e36ad4e6c11e614f0b1efe15b3c365a5919be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:11:28 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 22 Oct 2020 03:11:30 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 24 Nov 2020 00:42:56 GMT
ENV MEMCACHED_VERSION=1.6.9
# Tue, 24 Nov 2020 00:42:56 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Tue, 24 Nov 2020 00:47:29 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 Nov 2020 00:47:30 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 Nov 2020 00:47:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 Nov 2020 00:47:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Nov 2020 00:47:31 GMT
USER memcache
# Tue, 24 Nov 2020 00:47:31 GMT
EXPOSE 11211
# Tue, 24 Nov 2020 00:47:31 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f331a13b680b3ab05286a77980f705e8f4ab788d6ed224e10e80d9e2ab6a09a4`  
		Last Modified: Thu, 22 Oct 2020 03:21:50 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b40ae29247453a11c0bbfb92db01b919397d035232e9ef9fbc9e526af9e132`  
		Last Modified: Thu, 22 Oct 2020 03:21:50 GMT  
		Size: 16.3 KB (16323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a7eca4f7b1391c2d397e86710de5666847f1cb0acef37165d31b41883f22895`  
		Last Modified: Tue, 24 Nov 2020 00:47:58 GMT  
		Size: 2.2 MB (2153599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9fe46f7c3454fca381ef88344cfa1726d58a48fd7ddcbe6677de774e70c4c3`  
		Last Modified: Tue, 24 Nov 2020 00:47:57 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c645f1cec0c95903a4212ca1390af1c4ff8c0a4219b7a7ac4bedd631da2d447`  
		Last Modified: Tue, 24 Nov 2020 00:47:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:7d76bf4416ce1df4bd72710970fa497307b515895f95e2adc44fc0d927e2e3b8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4563787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7de761a79ff461eb8e54e9cd0cc6ceda36e3be45699b7a128f2cbb2b396ff5ad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 22 Oct 2020 11:00:06 GMT
ADD file:176e047fab2c1828575bffa6b14773efa297b7ecf312d86103c5dd4f78ec8027 in / 
# Thu, 22 Oct 2020 11:00:17 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 17:23:41 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 22 Oct 2020 17:23:57 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 27 Oct 2020 18:07:34 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 27 Oct 2020 18:07:36 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Fri, 30 Oct 2020 11:59:46 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 30 Oct 2020 11:59:48 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 30 Oct 2020 11:59:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 30 Oct 2020 11:59:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Oct 2020 11:59:56 GMT
USER memcache
# Fri, 30 Oct 2020 11:59:58 GMT
EXPOSE 11211
# Fri, 30 Oct 2020 12:00:00 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:692a9d763e196c85d79fc3e45b316b1bb557c93ba88a3c8ebf679a585d1efe73`  
		Last Modified: Thu, 22 Oct 2020 11:02:06 GMT  
		Size: 2.8 MB (2803218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c7c711d8b199bfca8f4578f6b934cf1694db2abd446c20fc40d2d8e94dee030`  
		Last Modified: Thu, 22 Oct 2020 17:36:41 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b24a99444366f41bd77307dbe956c7cd7b1fec53557510e9a1c28ca86a6fe90a`  
		Last Modified: Thu, 22 Oct 2020 17:36:40 GMT  
		Size: 16.3 KB (16318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603341c5c367a00c556b1cef2a45967f54bc3c608aeb15b041e6aaeaf5c278ef`  
		Last Modified: Fri, 30 Oct 2020 12:00:22 GMT  
		Size: 1.7 MB (1742583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8baf174d0a545732e56f7b659d48b19270ad1bcab34fb578b58254810b8966`  
		Last Modified: Fri, 30 Oct 2020 12:00:23 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:def13b85f243d3c6d7c04b72d6ec6736627101e18a3f1d3bfff329fac514f188`  
		Last Modified: Fri, 30 Oct 2020 12:00:22 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; s390x

```console
$ docker pull memcached@sha256:a54e2e0ee91bb55a0d8521a4ab8f30649588d259e6b18320f292e51025dc35b8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4676494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e05224f43fe277aeda8f17fc8ded12da4a0d81a153a08e34d8ddf961d5c2d7e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 22 Oct 2020 01:59:08 GMT
ADD file:e07d6f40b1afc3d3eff230bc89e84704eb762706a373a60c6bea6a45b2287464 in / 
# Thu, 22 Oct 2020 01:59:09 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:10:18 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 22 Oct 2020 03:10:20 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 24 Nov 2020 01:38:51 GMT
ENV MEMCACHED_VERSION=1.6.9
# Tue, 24 Nov 2020 01:38:52 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Tue, 24 Nov 2020 01:42:39 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 Nov 2020 01:42:39 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 Nov 2020 01:42:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 Nov 2020 01:42:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Nov 2020 01:42:43 GMT
USER memcache
# Tue, 24 Nov 2020 01:42:43 GMT
EXPOSE 11211
# Tue, 24 Nov 2020 01:42:44 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a4c84ece3d2b98927d25f13a4f367bfd96cbfae272f6ff1117d74c84b92d11d3`  
		Last Modified: Thu, 22 Oct 2020 01:59:37 GMT  
		Size: 2.6 MB (2565829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e98aa9130fa92579b5c432ac74178649f4fd0284da983980df01d2d851561f`  
		Last Modified: Thu, 22 Oct 2020 03:20:27 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d6f60d4914d39284ba2d65ad8bb43b4421039cbfdf061f9c0bcb187e3790b4`  
		Last Modified: Thu, 22 Oct 2020 03:20:26 GMT  
		Size: 15.6 KB (15570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18bd0358bc33c61ca0847dc0ae52053ab05c8491609929457c3e5195a035ce1b`  
		Last Modified: Tue, 24 Nov 2020 01:43:20 GMT  
		Size: 2.1 MB (2093430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2eea37208f09cfee5b7632f5f78f5cf51df5b2b248d14d585ba256baad4914f`  
		Last Modified: Tue, 24 Nov 2020 01:43:19 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09896b451609b7d0e69a6af517cff8a599cf66df743696a3b53b57bd13d89582`  
		Last Modified: Tue, 24 Nov 2020 01:43:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:alpine`

```console
$ docker pull memcached@sha256:32a6ff0c8679603a3977c810419511d6137db92c4f01d0d8282aa397e5cf71c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `memcached:alpine` - linux; amd64

```console
$ docker pull memcached@sha256:e1928aafa8833a2470b47fcc89754c26403ba3cda2ecbb4c4266072279e22576
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4886255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff697670a954aa7c8407c1f4391c129aea5e6c94f3728513631fed5f7756e164`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 06:13:10 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 22 Oct 2020 06:13:11 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 24 Nov 2020 00:44:26 GMT
ENV MEMCACHED_VERSION=1.6.9
# Tue, 24 Nov 2020 00:44:26 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Tue, 24 Nov 2020 00:48:41 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 Nov 2020 00:48:42 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 Nov 2020 00:48:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 Nov 2020 00:48:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Nov 2020 00:48:43 GMT
USER memcache
# Tue, 24 Nov 2020 00:48:43 GMT
EXPOSE 11211
# Tue, 24 Nov 2020 00:48:44 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d1b6a787fe50693a51ebeff9bc428c161df9b2e970c32316dd2ae2b5c527dba`  
		Last Modified: Thu, 22 Oct 2020 06:23:41 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0ca5f2b599ba9318ceb754cff704386c2105eef5536b716bea76ed53c872ae4`  
		Last Modified: Thu, 22 Oct 2020 06:23:41 GMT  
		Size: 15.3 KB (15299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b822756c8bfaf1bc207adc2de3741e339a2693e9ee8e311a149808db14b5208`  
		Last Modified: Tue, 24 Nov 2020 00:49:13 GMT  
		Size: 2.1 MB (2072463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af2d6b4d764b9c213154f1680d12d1ccf7241e76e6064dda66d5d3c3031f0e2b`  
		Last Modified: Tue, 24 Nov 2020 00:49:13 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e55816799a4db3ab4e13a264038fa0de836f4301b050cca3324eb8290e423e62`  
		Last Modified: Tue, 24 Nov 2020 00:49:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; arm variant v6

```console
$ docker pull memcached@sha256:84a8ab8b2c2ae46bba6afd02619cb1d0a180fd46d11749f1cb624b952ab8c9f1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4647852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c1779891a9245caed80bbadedd3187997a4cd109651441cbf70107bc5045c55`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 05:51:39 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 22 Oct 2020 05:53:12 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 24 Nov 2020 00:04:10 GMT
ENV MEMCACHED_VERSION=1.6.9
# Tue, 24 Nov 2020 00:04:10 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Tue, 24 Nov 2020 00:07:15 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 Nov 2020 00:07:16 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 Nov 2020 00:07:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 Nov 2020 00:07:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Nov 2020 00:07:19 GMT
USER memcache
# Tue, 24 Nov 2020 00:07:19 GMT
EXPOSE 11211
# Tue, 24 Nov 2020 00:07:20 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74cfe72068d6a66c0b7a1abfb1e0f80970db6ef63759ceea1ce866e61e85c16a`  
		Last Modified: Thu, 22 Oct 2020 06:07:10 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e57387f8f435122e3cbbe902349b156804991be332f5bfaaa9472102703b0e8c`  
		Last Modified: Thu, 22 Oct 2020 06:07:11 GMT  
		Size: 14.9 KB (14901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d3cdccf3fbd7cd515e5b74a671cda38dd9df4bcbbd570db901bf84e5003914`  
		Last Modified: Tue, 24 Nov 2020 00:07:32 GMT  
		Size: 2.0 MB (2029372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27ab5b24072ce098cf121983637ecc7320b3b99a6596ee6f3233b82854182fe2`  
		Last Modified: Tue, 24 Nov 2020 00:07:31 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fec87d28784f49a987a725efbd26639511b95005578516f18eb091f70680a17`  
		Last Modified: Tue, 24 Nov 2020 00:07:32 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; arm variant v7

```console
$ docker pull memcached@sha256:bbdb2d34f35910a55efd127f93a3b084b4210359d3ba3e04d492a70beea0320e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4313145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7520fc1477e6051f5415fbdf6960a7f9c528353aeb867c7069aa259916176ad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 08:40:04 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 22 Oct 2020 08:40:07 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 24 Nov 2020 00:26:09 GMT
ENV MEMCACHED_VERSION=1.6.9
# Tue, 24 Nov 2020 00:26:10 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Tue, 24 Nov 2020 00:29:05 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 Nov 2020 00:29:06 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 Nov 2020 00:29:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 Nov 2020 00:29:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Nov 2020 00:29:11 GMT
USER memcache
# Tue, 24 Nov 2020 00:29:13 GMT
EXPOSE 11211
# Tue, 24 Nov 2020 00:29:14 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1674e7ddc5cb335deefc31c3d2b6c4b434d04890456bfaae72e3e62b205cd0b6`  
		Last Modified: Thu, 22 Oct 2020 08:50:29 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f08b455b568b076a4ef19ed5615ed2352792bbed759c525ecae331db901df04`  
		Last Modified: Thu, 22 Oct 2020 08:50:30 GMT  
		Size: 13.8 KB (13827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:510b94932fc56e01e3a03af48c5bcaabec2bb336f8f787734bf846feb7de347f`  
		Last Modified: Tue, 24 Nov 2020 00:29:48 GMT  
		Size: 1.9 MB (1891978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88faa5219b31e7f196605b6c2b273fae85f47d56c7fb5d5b320dd544e35414ba`  
		Last Modified: Tue, 24 Nov 2020 00:29:47 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92e34d046a66b160935550f49396501447c4ddb5001f0ec2c33e25b1c3c5059`  
		Last Modified: Tue, 24 Nov 2020 00:29:48 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:a869ac02f75f64470176cf16c595e4e58bae5d5d3f442227581808e68763ace4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4811465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fd84a91919653be4583fcf329fccb126128ca56a60319c8f9c28adc05682650`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 04:33:47 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 22 Oct 2020 04:34:20 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 24 Nov 2020 00:54:44 GMT
ENV MEMCACHED_VERSION=1.6.9
# Tue, 24 Nov 2020 00:54:45 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Tue, 24 Nov 2020 00:57:40 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 Nov 2020 00:57:40 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 Nov 2020 00:57:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 Nov 2020 00:57:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Nov 2020 00:57:45 GMT
USER memcache
# Tue, 24 Nov 2020 00:57:45 GMT
EXPOSE 11211
# Tue, 24 Nov 2020 00:57:46 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d21e501aba9ea61896a99eee3b86890f5e2420e0061883d06bb780661eb6dbae`  
		Last Modified: Thu, 22 Oct 2020 04:49:24 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e607140b86f07aa95f3be67e136183ec1def37d74e27ae1141ff257e6960ad1`  
		Last Modified: Thu, 22 Oct 2020 04:49:24 GMT  
		Size: 15.7 KB (15683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed9de8619e85f52cd0657870aadd42de21c84ce68ca3412f496fd6fcd4a22bd`  
		Last Modified: Tue, 24 Nov 2020 00:58:20 GMT  
		Size: 2.1 MB (2087563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1adb1280ccf1abb19444686be75fa42aaf40a41c2c1d972d78188844c921175`  
		Last Modified: Tue, 24 Nov 2020 00:58:21 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78dc9a71b866039ff5461d91fc16d477e864471680f8066f56f37ed996019d83`  
		Last Modified: Tue, 24 Nov 2020 00:58:20 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; 386

```console
$ docker pull memcached@sha256:8fe6ce4813127db9eda50ca3d2c739e1ee4e19e6b2604c42857a084f2cee7f20
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4962966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fde562f92d407d755937a5fd62e36ad4e6c11e614f0b1efe15b3c365a5919be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:11:28 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 22 Oct 2020 03:11:30 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 24 Nov 2020 00:42:56 GMT
ENV MEMCACHED_VERSION=1.6.9
# Tue, 24 Nov 2020 00:42:56 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Tue, 24 Nov 2020 00:47:29 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 Nov 2020 00:47:30 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 Nov 2020 00:47:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 Nov 2020 00:47:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Nov 2020 00:47:31 GMT
USER memcache
# Tue, 24 Nov 2020 00:47:31 GMT
EXPOSE 11211
# Tue, 24 Nov 2020 00:47:31 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f331a13b680b3ab05286a77980f705e8f4ab788d6ed224e10e80d9e2ab6a09a4`  
		Last Modified: Thu, 22 Oct 2020 03:21:50 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b40ae29247453a11c0bbfb92db01b919397d035232e9ef9fbc9e526af9e132`  
		Last Modified: Thu, 22 Oct 2020 03:21:50 GMT  
		Size: 16.3 KB (16323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a7eca4f7b1391c2d397e86710de5666847f1cb0acef37165d31b41883f22895`  
		Last Modified: Tue, 24 Nov 2020 00:47:58 GMT  
		Size: 2.2 MB (2153599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c9fe46f7c3454fca381ef88344cfa1726d58a48fd7ddcbe6677de774e70c4c3`  
		Last Modified: Tue, 24 Nov 2020 00:47:57 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c645f1cec0c95903a4212ca1390af1c4ff8c0a4219b7a7ac4bedd631da2d447`  
		Last Modified: Tue, 24 Nov 2020 00:47:57 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:7d76bf4416ce1df4bd72710970fa497307b515895f95e2adc44fc0d927e2e3b8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4563787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7de761a79ff461eb8e54e9cd0cc6ceda36e3be45699b7a128f2cbb2b396ff5ad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 22 Oct 2020 11:00:06 GMT
ADD file:176e047fab2c1828575bffa6b14773efa297b7ecf312d86103c5dd4f78ec8027 in / 
# Thu, 22 Oct 2020 11:00:17 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 17:23:41 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 22 Oct 2020 17:23:57 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 27 Oct 2020 18:07:34 GMT
ENV MEMCACHED_VERSION=1.6.8
# Tue, 27 Oct 2020 18:07:36 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Fri, 30 Oct 2020 11:59:46 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Fri, 30 Oct 2020 11:59:48 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 30 Oct 2020 11:59:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 30 Oct 2020 11:59:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 30 Oct 2020 11:59:56 GMT
USER memcache
# Fri, 30 Oct 2020 11:59:58 GMT
EXPOSE 11211
# Fri, 30 Oct 2020 12:00:00 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:692a9d763e196c85d79fc3e45b316b1bb557c93ba88a3c8ebf679a585d1efe73`  
		Last Modified: Thu, 22 Oct 2020 11:02:06 GMT  
		Size: 2.8 MB (2803218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c7c711d8b199bfca8f4578f6b934cf1694db2abd446c20fc40d2d8e94dee030`  
		Last Modified: Thu, 22 Oct 2020 17:36:41 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b24a99444366f41bd77307dbe956c7cd7b1fec53557510e9a1c28ca86a6fe90a`  
		Last Modified: Thu, 22 Oct 2020 17:36:40 GMT  
		Size: 16.3 KB (16318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603341c5c367a00c556b1cef2a45967f54bc3c608aeb15b041e6aaeaf5c278ef`  
		Last Modified: Fri, 30 Oct 2020 12:00:22 GMT  
		Size: 1.7 MB (1742583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8baf174d0a545732e56f7b659d48b19270ad1bcab34fb578b58254810b8966`  
		Last Modified: Fri, 30 Oct 2020 12:00:23 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:def13b85f243d3c6d7c04b72d6ec6736627101e18a3f1d3bfff329fac514f188`  
		Last Modified: Fri, 30 Oct 2020 12:00:22 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; s390x

```console
$ docker pull memcached@sha256:a54e2e0ee91bb55a0d8521a4ab8f30649588d259e6b18320f292e51025dc35b8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4676494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e05224f43fe277aeda8f17fc8ded12da4a0d81a153a08e34d8ddf961d5c2d7e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 22 Oct 2020 01:59:08 GMT
ADD file:e07d6f40b1afc3d3eff230bc89e84704eb762706a373a60c6bea6a45b2287464 in / 
# Thu, 22 Oct 2020 01:59:09 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:10:18 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 22 Oct 2020 03:10:20 GMT
RUN apk add --no-cache cyrus-sasl-plain
# Tue, 24 Nov 2020 01:38:51 GMT
ENV MEMCACHED_VERSION=1.6.9
# Tue, 24 Nov 2020 01:38:52 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Tue, 24 Nov 2020 01:42:39 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		dpkg-dev dpkg 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		tar 		wget 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 24 Nov 2020 01:42:39 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 Nov 2020 01:42:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 Nov 2020 01:42:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Nov 2020 01:42:43 GMT
USER memcache
# Tue, 24 Nov 2020 01:42:43 GMT
EXPOSE 11211
# Tue, 24 Nov 2020 01:42:44 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a4c84ece3d2b98927d25f13a4f367bfd96cbfae272f6ff1117d74c84b92d11d3`  
		Last Modified: Thu, 22 Oct 2020 01:59:37 GMT  
		Size: 2.6 MB (2565829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e98aa9130fa92579b5c432ac74178649f4fd0284da983980df01d2d851561f`  
		Last Modified: Thu, 22 Oct 2020 03:20:27 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d6f60d4914d39284ba2d65ad8bb43b4421039cbfdf061f9c0bcb187e3790b4`  
		Last Modified: Thu, 22 Oct 2020 03:20:26 GMT  
		Size: 15.6 KB (15570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18bd0358bc33c61ca0847dc0ae52053ab05c8491609929457c3e5195a035ce1b`  
		Last Modified: Tue, 24 Nov 2020 01:43:20 GMT  
		Size: 2.1 MB (2093430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2eea37208f09cfee5b7632f5f78f5cf51df5b2b248d14d585ba256baad4914f`  
		Last Modified: Tue, 24 Nov 2020 01:43:19 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09896b451609b7d0e69a6af517cff8a599cf66df743696a3b53b57bd13d89582`  
		Last Modified: Tue, 24 Nov 2020 01:43:19 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:latest`

```console
$ docker pull memcached@sha256:a373b18f6ecc77c728c1b387b7c52fe331293319d37d4314ccbf283a726efb10
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
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
$ docker pull memcached@sha256:efe79d6cb73884b4cdc639183c3bdd27692034e92bd97a6972347db1f3f9940b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30513603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08ea1a3256c49616070a12b913da5051d159b2e7dc913e8a62ce0538f7a8a02a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:17 GMT
ADD file:d2abb0e4e7ac1773741f51f57d3a0b8ffc7907348842d773f8c341ba17f856d5 in / 
# Tue, 17 Nov 2020 20:21:17 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 23:59:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 17 Nov 2020 23:59:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 24 Nov 2020 00:40:08 GMT
ENV MEMCACHED_VERSION=1.6.9
# Tue, 24 Nov 2020 00:40:08 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Tue, 24 Nov 2020 00:44:14 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 24 Nov 2020 00:44:15 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 Nov 2020 00:44:16 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 Nov 2020 00:44:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Nov 2020 00:44:16 GMT
USER memcache
# Tue, 24 Nov 2020 00:44:16 GMT
EXPOSE 11211
# Tue, 24 Nov 2020 00:44:16 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:852e50cd189dfeb54d97680d9fa6bed21a6d7d18cfb56d6abfe2de9d7f173795`  
		Last Modified: Tue, 17 Nov 2020 20:27:25 GMT  
		Size: 27.1 MB (27105484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba259e022fc04d1e3da7b6650e0a253d23ade0fc8efd7f96e9146dd9337e7d74`  
		Last Modified: Wed, 18 Nov 2020 00:04:25 GMT  
		Size: 5.0 KB (4977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baff9e329932a3fa2a84550d57f41fa83ebd732b2079111e74f62ccbcaaeb084`  
		Last Modified: Wed, 18 Nov 2020 00:04:25 GMT  
		Size: 2.2 MB (2196434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f513b04a1f26d0f649ac982e308a03bcfa2cc147aa2654d57beca1d3c0ddfe2`  
		Last Modified: Tue, 24 Nov 2020 00:49:06 GMT  
		Size: 1.2 MB (1206301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb255edcd3e1c523644c575b9a937eab78cd4bb1b719a8e5030f81dab71bb9c3`  
		Last Modified: Tue, 24 Nov 2020 00:49:06 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee1dea1b4991d10177d54c728588378dfc740149e2dab0a2bb461f8e1ceb2d06`  
		Last Modified: Tue, 24 Nov 2020 00:49:06 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm variant v5

```console
$ docker pull memcached@sha256:b506cd917be5e584884f6bd23ab1c33563d1202186141d018e0b1efdb6d44536
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27931449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c96be237e7151156f8f06cc8123c1bdd31017cfc47efb0fbe0100317d3659424`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 17 Nov 2020 20:20:37 GMT
ADD file:d75cebdc79385debd2d6d1c8c34855d2bd4779b13ee47f76e34c6d8fca037531 in / 
# Tue, 17 Nov 2020 20:20:45 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 05:58:29 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 18 Nov 2020 05:58:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 23 Nov 2020 23:52:57 GMT
ENV MEMCACHED_VERSION=1.6.9
# Mon, 23 Nov 2020 23:52:59 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Mon, 23 Nov 2020 23:56:36 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Mon, 23 Nov 2020 23:56:37 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 23 Nov 2020 23:56:39 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 23 Nov 2020 23:56:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 Nov 2020 23:56:40 GMT
USER memcache
# Mon, 23 Nov 2020 23:56:41 GMT
EXPOSE 11211
# Mon, 23 Nov 2020 23:56:42 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1b8dd2ec17ab788b6ea03a9b6cf68afada9a8692681d29e9795db0abf6554404`  
		Last Modified: Tue, 17 Nov 2020 20:30:33 GMT  
		Size: 24.9 MB (24850311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eab7493baf19e0692ceefecef0ac524fdb4ba00028370800b97c2f0fdb2a840`  
		Last Modified: Wed, 18 Nov 2020 06:02:40 GMT  
		Size: 4.9 KB (4898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b096e22e759388a2bd7f3d04ba63e0b2fbbe300fe4093e3699e0ead554d3026`  
		Last Modified: Wed, 18 Nov 2020 06:02:40 GMT  
		Size: 1.9 MB (1896787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed956595633e1910b74834c64a03cbfa6fb9b0dd7c712ab74e05abaa2325aae`  
		Last Modified: Mon, 23 Nov 2020 23:56:53 GMT  
		Size: 1.2 MB (1179045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08931b56db74dd19b895412f1f1cc01c3416ff07a9b06d5db052cdb685d7975f`  
		Last Modified: Mon, 23 Nov 2020 23:56:52 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d581c95c1973377e4b69f2ee972d2e88141b440606f04bb7cf035a987ccc412`  
		Last Modified: Mon, 23 Nov 2020 23:56:52 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm variant v7

```console
$ docker pull memcached@sha256:23bfdefe9cc175f1d85d34f46637c56c49f675daac226d2ef27875d88f1d634a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25680615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83cc6416458d599f47ab03ce627dc26358df5d4d8e352bc0ed0e2e1e8bc9e031`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:06 GMT
ADD file:2035658a8d20545ee7b2ab3ee791a371925fca7968ac29435303da24a1378f34 in / 
# Tue, 17 Nov 2020 20:21:10 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 22:43:01 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 17 Nov 2020 22:43:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 24 Nov 2020 00:22:17 GMT
ENV MEMCACHED_VERSION=1.6.9
# Tue, 24 Nov 2020 00:22:18 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Tue, 24 Nov 2020 00:25:37 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 24 Nov 2020 00:25:38 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 Nov 2020 00:25:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 Nov 2020 00:25:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Nov 2020 00:25:42 GMT
USER memcache
# Tue, 24 Nov 2020 00:25:43 GMT
EXPOSE 11211
# Tue, 24 Nov 2020 00:25:48 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d5029e4b387017f20ad9f77baf3b81dd41f851d6340363b842a8a1d9786a60a0`  
		Last Modified: Tue, 17 Nov 2020 20:31:46 GMT  
		Size: 22.7 MB (22714186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dcb178bde3efeefaad9cde6e23e198ace47cd12278a903916a98fe226425c63`  
		Last Modified: Tue, 17 Nov 2020 22:47:04 GMT  
		Size: 4.9 KB (4888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:849c9255e9336e765f5fe8a15ddde316c5b6f9a38454be317f5b88d23490d4e9`  
		Last Modified: Tue, 17 Nov 2020 22:47:04 GMT  
		Size: 1.8 MB (1811529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee4f7e83b65d682e21adba125e9b5a00b62239a5f2a45a02a8ee980c77c033ed`  
		Last Modified: Tue, 24 Nov 2020 00:29:37 GMT  
		Size: 1.1 MB (1149604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae88eab2c47891856beb68524c3b63058f3c28a17b0cc5f9a2b7a310f0b23245`  
		Last Modified: Tue, 24 Nov 2020 00:29:37 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d745615f6bde6bb77f0f3c84750b88a63812b46e1972b2d40a987307300373f`  
		Last Modified: Tue, 24 Nov 2020 00:29:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:bca7dce6878924796ed4e59749a20a99b8b21095a6622de36e1669854f3995e7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.1 MB (29121866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b4113f866ef34853e089e9828737b4a19cfd3e9b7ab4673fb6b314a94105e1a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 17 Nov 2020 20:23:31 GMT
ADD file:a70d8c01f8f04f36038968567af779883f3b5ba3147b662b7d170d80418bc23c in / 
# Tue, 17 Nov 2020 20:23:32 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 01:22:43 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 18 Nov 2020 01:22:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 24 Nov 2020 00:47:00 GMT
ENV MEMCACHED_VERSION=1.6.9
# Tue, 24 Nov 2020 00:47:01 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Tue, 24 Nov 2020 00:54:18 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 24 Nov 2020 00:54:19 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 Nov 2020 00:54:21 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 Nov 2020 00:54:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Nov 2020 00:54:23 GMT
USER memcache
# Tue, 24 Nov 2020 00:54:24 GMT
EXPOSE 11211
# Tue, 24 Nov 2020 00:54:24 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:29ade854e0dcedde295dd89890d45271e9df839e42124558eb5283508ca70f5c`  
		Last Modified: Tue, 17 Nov 2020 20:32:02 GMT  
		Size: 25.9 MB (25862532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b138bddb332a0f874407cfaec3014ec6614883be703b52ff29808980118a91`  
		Last Modified: Wed, 18 Nov 2020 01:26:58 GMT  
		Size: 5.0 KB (5024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5452540f15530cb8fe9343e88516c0b3050b9bb0596613026fe0f84b13c30d6c`  
		Last Modified: Wed, 18 Nov 2020 01:26:59 GMT  
		Size: 2.1 MB (2074952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:373464c46512a6172ca94cdb2aaf1427f0710ce8289bf2a4a73b3a8eac65e689`  
		Last Modified: Tue, 24 Nov 2020 00:58:10 GMT  
		Size: 1.2 MB (1178950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d995428ce6fac044c4080e2e653157b5d2c86c8940d16d85d20ff3094d47d4`  
		Last Modified: Tue, 24 Nov 2020 00:58:09 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac3fb0a8b0191b0f3b130c75bc5d77bdecc4c5f041e4f0c0c8820cf189c5e785`  
		Last Modified: Tue, 24 Nov 2020 00:58:10 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; 386

```console
$ docker pull memcached@sha256:04f9bb7564b8ef32c9b16f7a84a06aa6ce963cd7341fb47580b22b5240e84ffb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31183406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2a87dfef3d28a151095f6d0a0d6cda6fa63975bd76e0221a8a04bfe82dea0e6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 17 Nov 2020 20:19:58 GMT
ADD file:b17dfa607fcb298beb9c58bfbb8b9b0743ceb385875776c56269db2506840edf in / 
# Tue, 17 Nov 2020 20:19:58 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 06:51:09 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 18 Nov 2020 06:51:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 24 Nov 2020 00:38:23 GMT
ENV MEMCACHED_VERSION=1.6.9
# Tue, 24 Nov 2020 00:38:23 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Tue, 24 Nov 2020 00:42:38 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 24 Nov 2020 00:42:39 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 Nov 2020 00:42:39 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 Nov 2020 00:42:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Nov 2020 00:42:40 GMT
USER memcache
# Tue, 24 Nov 2020 00:42:40 GMT
EXPOSE 11211
# Tue, 24 Nov 2020 00:42:40 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:e8e82c9fb36b8f3a9b8f18fe1d88e4d425d5c45968e3f2e94cdbb1255feb4878`  
		Last Modified: Tue, 17 Nov 2020 20:26:45 GMT  
		Size: 27.8 MB (27766186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:321cbeb51acb785f1b1c182cedb4064f03df6af524b61820be6dcd5b1cb2f8a2`  
		Last Modified: Wed, 18 Nov 2020 07:00:37 GMT  
		Size: 4.9 KB (4893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9992095793664bbd90982439c87351ec23b212e9622d90a144faa60a7acbe6d`  
		Last Modified: Wed, 18 Nov 2020 07:00:38 GMT  
		Size: 2.2 MB (2208086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7345a22027cf324340c6fe54efa2e573f790817c593fc990c4eb41f1d731061`  
		Last Modified: Tue, 24 Nov 2020 00:47:51 GMT  
		Size: 1.2 MB (1203835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94d7cbd4098036b6b2a3ddba5fd780fb6875c10dc8df39a054bcd89187a62bcd`  
		Last Modified: Tue, 24 Nov 2020 00:47:50 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53794b9614d9d66687bd0c4938c508a6dcd7e7970d8ba3c2078635fe95d6c856`  
		Last Modified: Tue, 24 Nov 2020 00:47:50 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; mips64le

```console
$ docker pull memcached@sha256:8bc36ac7c7accfbf668832c1f44aa9b8a72eea77027dd1cda17b12353928fc03
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.8 MB (28757547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23d47b7544c777f79de3b1b39c9d4702573764e302f83401ec54210ebc22c514`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 17 Nov 2020 20:19:24 GMT
ADD file:98a1b26b3eefd56b2867344c8c58f4bc3ef9a19c28e35c41df77ab80598d41bc in / 
# Tue, 17 Nov 2020 20:19:24 GMT
CMD ["bash"]
# Mon, 23 Nov 2020 23:07:26 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Mon, 23 Nov 2020 23:07:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 23 Nov 2020 23:07:39 GMT
ENV MEMCACHED_VERSION=1.6.9
# Mon, 23 Nov 2020 23:07:39 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Mon, 23 Nov 2020 23:13:24 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Mon, 23 Nov 2020 23:13:24 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 23 Nov 2020 23:13:26 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 23 Nov 2020 23:13:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 Nov 2020 23:13:26 GMT
USER memcache
# Mon, 23 Nov 2020 23:13:27 GMT
EXPOSE 11211
# Mon, 23 Nov 2020 23:13:27 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:071bb0a152ef32db0e7d172bcc4722a6a275885249ddb72bee023e268e82fc16`  
		Last Modified: Tue, 17 Nov 2020 20:26:34 GMT  
		Size: 25.8 MB (25777477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:664f5d146d813d299af77e5fc0e344f8a75bd40824a60c99a04bdb1ff4b13b43`  
		Last Modified: Mon, 23 Nov 2020 23:13:45 GMT  
		Size: 5.0 KB (4982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9431da82e8f3642d3474b3944f281ce0d9d5f81e50a7d814cc06bc4db3a55ff6`  
		Last Modified: Mon, 23 Nov 2020 23:13:46 GMT  
		Size: 1.8 MB (1776012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72e10c1044bcc0ce9b31d6c01d3f1b6be4c9a227a8d757cd5fbb803190e0372c`  
		Last Modified: Mon, 23 Nov 2020 23:13:46 GMT  
		Size: 1.2 MB (1198668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0d2b229dc61a9fd2afe3edd3cdf4354d3153027b44b22fec64257ac3e07c4e`  
		Last Modified: Mon, 23 Nov 2020 23:13:45 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ae54e7810b124e108a6331526af87033a40abd56d009854ad078554273f41b`  
		Last Modified: Mon, 23 Nov 2020 23:13:44 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; ppc64le

```console
$ docker pull memcached@sha256:5233f7be9d0b23aa88bf7fc2e75310bdb632ec93aa2db03c39ef676fbd2c111f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34085325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ed1158f0082c5bd5c24e244191a1a7c8dc37a0db0a0f27a9a61d238a6f45b60`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 17 Nov 2020 23:23:06 GMT
ADD file:49cd8b08964980901349e1f3d6cb34abd8145dea6e6d9ab83502452281ac73ca in / 
# Tue, 17 Nov 2020 23:23:11 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 02:08:02 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 18 Nov 2020 02:08:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 02:08:53 GMT
ENV MEMCACHED_VERSION=1.6.8
# Wed, 18 Nov 2020 02:09:05 GMT
ENV MEMCACHED_SHA1=8f3efd851efc5b822bd991b93d06a271b2fac052
# Wed, 18 Nov 2020 02:21:00 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Wed, 18 Nov 2020 02:21:04 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 18 Nov 2020 02:21:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 18 Nov 2020 02:21:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 18 Nov 2020 02:21:20 GMT
USER memcache
# Wed, 18 Nov 2020 02:21:23 GMT
EXPOSE 11211
# Wed, 18 Nov 2020 02:21:29 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:d79345c10f03543bff3982aedb35a18ba18626c0074014387ff5e1dc14474e2b`  
		Last Modified: Tue, 17 Nov 2020 23:32:54 GMT  
		Size: 30.5 MB (30531702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c81cd83e42b497f0cba94fa5211dd383d0d43fb3fefb1c49d84df1ec1bb8706`  
		Last Modified: Wed, 18 Nov 2020 02:21:58 GMT  
		Size: 5.0 KB (4990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2755aa03159fc35fb59a7fc785b128fa60a5940abb4d5777fea087d0a61c07a`  
		Last Modified: Wed, 18 Nov 2020 02:21:59 GMT  
		Size: 2.3 MB (2322767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f132d007583b65a7dae9876fd53c3ceb86e63cf51c9ac01c83d0c1ad73925ad`  
		Last Modified: Wed, 18 Nov 2020 02:21:58 GMT  
		Size: 1.2 MB (1225459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac54fbbfdd63057bf31b8403a24213cfb6c131e9e6e691bb90e9d35d8deb479`  
		Last Modified: Wed, 18 Nov 2020 02:21:58 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1fc8692195395ae28bbb8eadfb2c8e2cd572559f1b92bf620013f723f52303c`  
		Last Modified: Wed, 18 Nov 2020 02:21:58 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; s390x

```console
$ docker pull memcached@sha256:d4f378fbb763346873fb016770ad2e202370f526d24ccbeffc2f3a1247b9b3d5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.8 MB (28811191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ff2b9ce713317a592f1208e112eec5e2b257bd5b8a46984c37d8b8e63c010d3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 17 Nov 2020 20:18:29 GMT
ADD file:4a3215d1c9b4afb58053c4fff8d121547890c2a71bc027992f7f960551c6acb1 in / 
# Tue, 17 Nov 2020 20:18:34 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 01:46:32 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Wed, 18 Nov 2020 01:46:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 24 Nov 2020 01:29:39 GMT
ENV MEMCACHED_VERSION=1.6.9
# Tue, 24 Nov 2020 01:29:40 GMT
ENV MEMCACHED_SHA1=42ae062094fdf083cfe7b21ff377c781011c2be1
# Tue, 24 Nov 2020 01:38:32 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 24 Nov 2020 01:38:33 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 24 Nov 2020 01:38:34 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 24 Nov 2020 01:38:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 24 Nov 2020 01:38:36 GMT
USER memcache
# Tue, 24 Nov 2020 01:38:36 GMT
EXPOSE 11211
# Tue, 24 Nov 2020 01:38:37 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c0d5e3cc51c0b20d3f68226f5332c9a9c2b17cce2f362ec742d4ed325ff7b530`  
		Last Modified: Tue, 17 Nov 2020 20:23:43 GMT  
		Size: 25.7 MB (25721143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b189bf5a9f20baf2f6e6ec9230535bdc36fc750196dd1e3f5eb5e17ee36a31`  
		Last Modified: Wed, 18 Nov 2020 01:53:06 GMT  
		Size: 5.0 KB (5027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1372a3dddcc126d1aad6887514b61ad9ac946b00f50834efdd6c376cc6cfcf65`  
		Last Modified: Wed, 18 Nov 2020 01:53:06 GMT  
		Size: 1.9 MB (1886092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d6c632cdb2f59084328d009bb036821bfe895d1bc1d1512150931d115ea0b40`  
		Last Modified: Tue, 24 Nov 2020 01:43:04 GMT  
		Size: 1.2 MB (1198521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247f0621f757137d4d49d296cd294fef8816daca0331d8406990d31eab886d2e`  
		Last Modified: Tue, 24 Nov 2020 01:43:03 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b13354fbc1d862e30d1c831d85eb9a4e24ba519cc341b6097aa6209cfd530e99`  
		Last Modified: Tue, 24 Nov 2020 01:43:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
