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
$ docker pull memcached@sha256:1917f1b4e48a69e5be80a57c321504338f9b65046386ea50ee679322413e26c7
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
$ docker pull memcached@sha256:2a9bf2539b24c553b92c876dfbe6dd48450a832f2b5395ec3217271018ad2ca0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32971284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92e1422c3edf80b790f0a601173b8e329b6619096d8cebb0b50b0f489ad1d971`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:54:26 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 23 Aug 2022 02:54:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 29 Aug 2022 19:57:00 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 19:57:01 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 19:59:41 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Mon, 29 Aug 2022 19:59:41 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 19:59:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 19:59:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 19:59:42 GMT
USER memcache
# Mon, 29 Aug 2022 19:59:42 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 19:59:42 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa73fb65ea8b12a2375459f0d656d3ad06e2863c906fcf962486eda3701f3fd6`  
		Last Modified: Tue, 23 Aug 2022 02:57:38 GMT  
		Size: 5.0 KB (4981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502b4e8803067b28098d0ea52281cfef66da1ee1e869241612b545d7e9ff12de`  
		Last Modified: Tue, 23 Aug 2022 02:57:38 GMT  
		Size: 328.1 KB (328108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b905db5d33a47882bd6cb4935bcc5d576d5cad5ba761b6b4004982c3aa7333`  
		Last Modified: Mon, 29 Aug 2022 20:03:05 GMT  
		Size: 1.3 MB (1256303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93643c661348540c2edcfc8a007b2c9aff33ac36cb9dcd910e0ddb51f50cd09e`  
		Last Modified: Mon, 29 Aug 2022 20:03:04 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc510e39dc783b83b00e5abd05d57df948435a0aaf45e87b131cc0fff83021e`  
		Last Modified: Mon, 29 Aug 2022 20:03:05 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm variant v5

```console
$ docker pull memcached@sha256:ef629e7153669e6100c98fba79336f87cc033d073c6219d6c7ec9360298a5d8e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30454536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84960478143b53154da0f3409e3f1141b62dabf4fe0c97c3661b5dd8a1c533ec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Sep 2022 00:53:30 GMT
ADD file:539e23f1c3a625a612a5a59b3939e9692c86c3cfa4956d30f4802c9f34ffa29c in / 
# Tue, 13 Sep 2022 00:53:31 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 03:18:14 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 13 Sep 2022 03:18:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 03:18:20 GMT
ENV MEMCACHED_VERSION=1.6.17
# Tue, 13 Sep 2022 03:18:20 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Tue, 13 Sep 2022 03:24:21 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 13 Sep 2022 03:24:22 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 13 Sep 2022 03:24:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Sep 2022 03:24:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Sep 2022 03:24:22 GMT
USER memcache
# Tue, 13 Sep 2022 03:24:22 GMT
EXPOSE 11211
# Tue, 13 Sep 2022 03:24:22 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:705abbab4fcb3a8dfe046a2ae6c450328aa11d93911abce66d3bba8bc693cbd4`  
		Last Modified: Tue, 13 Sep 2022 01:01:07 GMT  
		Size: 28.9 MB (28905288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eba43be24e48cc0796f0f5a17e6b674c0f07d5626f56ac8ed9f717cba0d0503`  
		Last Modified: Tue, 13 Sep 2022 03:24:59 GMT  
		Size: 4.9 KB (4894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c93e222cf0a02e2b4146a4d3ff6e5da33b929a10129fd88081a505e4011b9e`  
		Last Modified: Tue, 13 Sep 2022 03:25:00 GMT  
		Size: 316.6 KB (316638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b091f5c4cb7701e12cc29c82ee78e1704fdaaabcd851004efea8deb3acf7f2f`  
		Last Modified: Tue, 13 Sep 2022 03:25:00 GMT  
		Size: 1.2 MB (1227311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5e30653aa54ef905fcc6b97813278f8b54e56e889b1ffccf5101df4fa45882`  
		Last Modified: Tue, 13 Sep 2022 03:24:59 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471afe7d2cb0083a807b44b87fa581728a14e66fbada1f0ea0bcff34258f1cca`  
		Last Modified: Tue, 13 Sep 2022 03:24:59 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm variant v7

```console
$ docker pull memcached@sha256:960b71bacce5bbd2bf5c700ca3398d8ce00c1a9ebb35a5b690be486267128ef1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28088375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a54ccaf5bd1ba99327d598c288c19a655c2601e43aaf08c6429e99c287ab5b35`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 23 Aug 2022 01:43:01 GMT
ADD file:4cd1b4287674228db28402a76aa4f241740585448be48b5b15068d275ee9eb84 in / 
# Tue, 23 Aug 2022 01:43:01 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 18:03:50 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 23 Aug 2022 18:03:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 29 Aug 2022 19:04:31 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 19:04:31 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 19:09:39 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Mon, 29 Aug 2022 19:09:40 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 19:09:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 19:09:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 19:09:40 GMT
USER memcache
# Mon, 29 Aug 2022 19:09:40 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 19:09:40 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:051ba72559abd0cf65b34b75605580f58636ec3cb994f97de317632a85d82761`  
		Last Modified: Tue, 23 Aug 2022 01:50:05 GMT  
		Size: 26.6 MB (26571732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12dc4f2d8dca33e3850e55e4a2cd25a6dbf19afb27df3daef33de65ac91fd757`  
		Last Modified: Tue, 23 Aug 2022 21:10:42 GMT  
		Size: 4.9 KB (4893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:033f621bef4d3464e367d2c0ce45f3ec626c1c21f84ba7e84ece82bfbef4666e`  
		Last Modified: Tue, 23 Aug 2022 21:10:42 GMT  
		Size: 312.0 KB (312045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba873971d43c849095b8112993f9eb97b90c155f9f9f190da2bef761c9aa61a8`  
		Last Modified: Mon, 29 Aug 2022 19:26:29 GMT  
		Size: 1.2 MB (1199297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b256a2f081d1033d7ae503b0735b03640cd5b071e47fce65387238edf010a05c`  
		Last Modified: Mon, 29 Aug 2022 19:26:29 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a75e8764536efcd4e0fbd3d6c058eb6e05a0489f9e157f95e9e9ca0639c7d40b`  
		Last Modified: Mon, 29 Aug 2022 19:26:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:c67982406cd3e3fb90c50951d6a8cd766a4c0cc625ef035237913dfe56c0ae88
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31444531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02936ddd3c3f04b28ca0fbb9e803bfe5c3c1c0bda9ffe6ca0c6ea9954c351ab8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 13:12:07 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 23 Aug 2022 13:12:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 29 Aug 2022 18:48:57 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 18:48:58 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 18:51:30 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Mon, 29 Aug 2022 18:51:32 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 18:51:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 18:51:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 18:51:34 GMT
USER memcache
# Mon, 29 Aug 2022 18:51:35 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 18:51:36 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21794f0e498790afd69f2d317bbed8aa9cdbd3dddc56f7d52f1b806577e38a06`  
		Last Modified: Tue, 23 Aug 2022 13:15:43 GMT  
		Size: 4.9 KB (4904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:261db6d67ef285bdd84e6ae9e72182c4cd348b9f6c3c060c723764d03a12c2f6`  
		Last Modified: Tue, 23 Aug 2022 13:15:43 GMT  
		Size: 119.2 KB (119240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646e70d704c1f14afdd9de28cb4081703a4efc97e9c6a743ba80329c00705b37`  
		Last Modified: Mon, 29 Aug 2022 18:55:22 GMT  
		Size: 1.3 MB (1256190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db1c8f9c761c12c5c76962f55a2baff7f18d665a53fa76a2d3329fc2c0ccf313`  
		Last Modified: Mon, 29 Aug 2022 18:55:21 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4655eda4ba606249d810ba4d37deb1e82c106bcf3a2394f684a6ad8275d98950`  
		Last Modified: Mon, 29 Aug 2022 18:55:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; 386

```console
$ docker pull memcached@sha256:9a142ff1556091ea4d817d7ac5c26fcc6a0b2daa5bf99a56c64d19bb3e3cb866
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33776358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e0455947003534873a7c3f6d3bae27183601ae7c8b66f094e52d72450507327`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 23 Aug 2022 01:02:40 GMT
ADD file:5ca62c98116941aaa64ec72afb689a088c46f75a3e83d5b0d4e58d65ec905ccd in / 
# Tue, 23 Aug 2022 01:02:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:22:44 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 23 Aug 2022 03:22:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 29 Aug 2022 18:38:36 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 18:38:36 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 18:41:29 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Mon, 29 Aug 2022 18:41:31 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 18:41:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 18:41:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 18:41:33 GMT
USER memcache
# Mon, 29 Aug 2022 18:41:34 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 18:41:35 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6b3cb4a05a891d9d8a87a2bd7247b16f79832a9d4afbad3ff5068f6fc2ba1560`  
		Last Modified: Tue, 23 Aug 2022 01:08:25 GMT  
		Size: 32.4 MB (32387317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd24201e0b5e9a68a67bdc3b464a01aeb9a2e5a859a582cdaa80ab08a608337`  
		Last Modified: Tue, 23 Aug 2022 03:27:47 GMT  
		Size: 4.8 KB (4774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3070e5e3b1d98fa0b67b8390880b7596c4719b774864de21f36ed86873041793`  
		Last Modified: Tue, 23 Aug 2022 03:27:48 GMT  
		Size: 130.1 KB (130136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af8c1cee54f7ff86c820ca418aa3d2c05c5f200ca4d938ba76c8f8439b39cb04`  
		Last Modified: Mon, 29 Aug 2022 18:45:40 GMT  
		Size: 1.3 MB (1253721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94d7ae33ce7f8ea696d92c06ef6fd7c86c8228061b3b2485a78a9f59131a48aa`  
		Last Modified: Mon, 29 Aug 2022 18:45:43 GMT  
		Size: 289.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5348ed42ca0cf0c971fcaddc7677e8a3508548c0e3ca9e12b49cc06627f4657c`  
		Last Modified: Mon, 29 Aug 2022 18:45:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; mips64le

```console
$ docker pull memcached@sha256:e1403115858fda192fda48a365294d78dd1ea7fa6c9db3be737a883cb34fd9de
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31001916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ce2440650f197fcd6de50038d9a16d23be6db7efc79a8115173cc1ca5a769f5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Sep 2022 01:10:58 GMT
ADD file:91a8d8627a614ff3741d68216da46f13b393e52a70377b97ef317e4a00a3cac6 in / 
# Tue, 13 Sep 2022 01:11:02 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 04:50:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 13 Sep 2022 04:50:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 04:50:38 GMT
ENV MEMCACHED_VERSION=1.6.17
# Tue, 13 Sep 2022 04:50:40 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Tue, 13 Sep 2022 04:57:36 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 13 Sep 2022 04:57:38 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 13 Sep 2022 04:57:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Sep 2022 04:57:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Sep 2022 04:57:48 GMT
USER memcache
# Tue, 13 Sep 2022 04:57:50 GMT
EXPOSE 11211
# Tue, 13 Sep 2022 04:57:53 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:98abeb1446d0e9df6f48d5f72a70b36598cfc1091c9a5ca82690bedcf320e2b3`  
		Last Modified: Tue, 13 Sep 2022 01:18:50 GMT  
		Size: 29.6 MB (29627659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766602637141a485f59d0fc04aec4bfa1ac38583bba125b35c0b6809f1219ed9`  
		Last Modified: Tue, 13 Sep 2022 04:58:11 GMT  
		Size: 4.9 KB (4857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21b631e5bb3330fba3352d6332ae5cfa0b9a35dbc33b4d643b80f7b908c950f5`  
		Last Modified: Tue, 13 Sep 2022 04:58:11 GMT  
		Size: 117.2 KB (117159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee33141b788356ead96c93190f0008f455371a4562d92b27a20945aac60d1361`  
		Last Modified: Tue, 13 Sep 2022 04:58:12 GMT  
		Size: 1.3 MB (1251835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e488d322d0c180f442d31923e23e79064b584ac59e2cadf3be31cc702751460d`  
		Last Modified: Tue, 13 Sep 2022 04:58:11 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec80c89f379732f5466f55915bbad33a4b55dc651bf6346712c92cff64717b11`  
		Last Modified: Tue, 13 Sep 2022 04:58:11 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; ppc64le

```console
$ docker pull memcached@sha256:0176bec998e05785ddcaadb9c692b14571e10c2b71050a9988329f903660369b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36970738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7a0216731101d94583b08e4b42f59092a78019783e49a2ddb6401ea59c9d47d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 23 Aug 2022 01:24:52 GMT
ADD file:d35213360d726a18e220276d33f245115c3e94a321addaa4c9127488368b0203 in / 
# Tue, 23 Aug 2022 01:24:54 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:34:49 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 23 Aug 2022 02:34:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 29 Aug 2022 19:19:51 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 19:19:51 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 19:22:46 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Mon, 29 Aug 2022 19:22:47 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 19:22:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 19:22:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 19:22:48 GMT
USER memcache
# Mon, 29 Aug 2022 19:22:49 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 19:22:49 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:698954eda09d38dd1ccc9ce777b1f6bc7f7473fc6c4c3eb634acc8d035a42eae`  
		Last Modified: Tue, 23 Aug 2022 01:30:36 GMT  
		Size: 35.3 MB (35284280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffb080d920662043edc67113c0de4c68258ad19c0fffd9e3b79fa01800c6015`  
		Last Modified: Tue, 23 Aug 2022 02:39:09 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b1f66b68991d8f5ab064b3988db37a48b8f28b4ef0eb8e83efa4c419b630ff`  
		Last Modified: Tue, 23 Aug 2022 02:39:09 GMT  
		Size: 356.9 KB (356931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2256c5b8427744c7563d1151efbeb03c935fbb3e87d621903c9e7476a8db7494`  
		Last Modified: Mon, 29 Aug 2022 19:27:05 GMT  
		Size: 1.3 MB (1324139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee6919a18fb52b4b8259e2942d1d56ca42a4371f735bedd875c5eebdaee214a2`  
		Last Modified: Mon, 29 Aug 2022 19:27:04 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ac3c74fbd1e874bdc7163ccf1ba8bf496b085875b4165fcec2e4a771d9742f9`  
		Last Modified: Mon, 29 Aug 2022 19:27:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; s390x

```console
$ docker pull memcached@sha256:f063181874bf86b26f7e8d033e02792331b3282ef6614aa99d8d70c8b178aac0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31206151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c2827f7c0c4acdb1d09c90d24a8e27f37bd489dca825a2831b3f923831b1125`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Sep 2022 00:48:07 GMT
ADD file:e8a6c2e8be5d9d1f83c1e280419014489438391a9feb7c77b6c21adbf0ec062b in / 
# Tue, 13 Sep 2022 00:48:08 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 01:59:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 13 Sep 2022 01:59:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 01:59:22 GMT
ENV MEMCACHED_VERSION=1.6.17
# Tue, 13 Sep 2022 01:59:23 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Tue, 13 Sep 2022 02:02:36 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 13 Sep 2022 02:02:36 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 13 Sep 2022 02:02:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Sep 2022 02:02:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Sep 2022 02:02:37 GMT
USER memcache
# Tue, 13 Sep 2022 02:02:37 GMT
EXPOSE 11211
# Tue, 13 Sep 2022 02:02:37 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c64715e5ebd39975a39b5cf2535772544c27713cbed678b0a21e73680fffaf72`  
		Last Modified: Tue, 13 Sep 2022 00:52:39 GMT  
		Size: 29.6 MB (29635080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce5055aafbfbe726c8840111d8300b0c75f707a8ab517395bb8be985d2feb009`  
		Last Modified: Tue, 13 Sep 2022 02:03:36 GMT  
		Size: 5.0 KB (5021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9a227f323eed41d16b462d95503000badd5210aa179dd3065f4363fe3a1b9f`  
		Last Modified: Tue, 13 Sep 2022 02:03:36 GMT  
		Size: 324.2 KB (324172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36fb60d78f8bd69265b4c2d2246169797772da4584f6e063d49eab9c2f040c51`  
		Last Modified: Tue, 13 Sep 2022 02:03:36 GMT  
		Size: 1.2 MB (1241470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d23a9497c5fd3ec0d26f920c59f1f1628999ae546bd1b2f722b29fbf27e3402`  
		Last Modified: Tue, 13 Sep 2022 02:03:36 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009331f552a168c5b26209994b10c7684fc80fe6348a406878b2262037e82435`  
		Last Modified: Tue, 13 Sep 2022 02:03:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1-alpine`

```console
$ docker pull memcached@sha256:6eff5e1647ee867d3fac2bac716568ced7005b8044651f181988a1d0971d3fce
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
$ docker pull memcached@sha256:3b2a8f0dbcbb96b42edffa4959170c2486ddb2bef3de057f8ed71591348721c0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3891406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc6dc88eceeba2070ee6fe3c8c979afeaf5bf6d36e86d09d6457dd8432bb4c36`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:39 GMT
ADD file:b828bc14bc5ff03c8f7310fe0aed6ac5df19a393622d5d1d779a523234d07c0a in / 
# Tue, 09 Aug 2022 17:38:39 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:34:01 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 09 Aug 2022 18:34:02 GMT
RUN apk add --no-cache libsasl
# Mon, 29 Aug 2022 18:41:47 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 18:41:48 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 18:44:43 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Mon, 29 Aug 2022 18:44:45 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 18:44:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 18:44:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 18:44:47 GMT
USER memcache
# Mon, 29 Aug 2022 18:44:48 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 18:44:49 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6c0d3b419d848ea31ca748254611d5d5ce3b76e3d7bba520fd87400fbb75f3b9`  
		Last Modified: Tue, 09 Aug 2022 17:39:33 GMT  
		Size: 2.8 MB (2807121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240e236335200614c944d9ba79e2d7eda5cfa258a69e669b585cc28314d754f5`  
		Last Modified: Tue, 09 Aug 2022 18:38:05 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:844d1ba63a22190468423984b12b7d36f6c005e3316461b983f975f4b8dc9ee8`  
		Last Modified: Tue, 09 Aug 2022 18:38:05 GMT  
		Size: 119.8 KB (119826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2e7c344cfe47d96e7a9d170c9427c474246d16b76964c915cdd2f3d5e62698`  
		Last Modified: Mon, 29 Aug 2022 18:46:29 GMT  
		Size: 962.8 KB (962814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed467891e81f8057bb74046a7442a949b8f2ab27dc7099c321d77f2497584541`  
		Last Modified: Mon, 29 Aug 2022 18:46:29 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5326fe38fa94412c48f8bf0980206aed389413a089a646b582739edc31841a`  
		Last Modified: Mon, 29 Aug 2022 18:46:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:79f15ab95c7dc52c17fab8ebc50e1a380b3584fd2127402ba0486ca4311be7df
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3913056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d80b3f9d28d32be6c7fdc9e706c4555e3bc835f495aed408fe264c0a8ed3d6a7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:48:17 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 09 Aug 2022 18:48:19 GMT
RUN apk add --no-cache libsasl
# Mon, 29 Aug 2022 19:23:01 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 19:23:02 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 19:26:15 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Mon, 29 Aug 2022 19:26:16 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 19:26:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 19:26:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 19:26:17 GMT
USER memcache
# Mon, 29 Aug 2022 19:26:18 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 19:26:18 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:086c869249c97411ce380e3b76305e0b85731874d0ea57dfd0de74e1f387443d`  
		Last Modified: Tue, 09 Aug 2022 18:52:28 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75e55886182590f2e7eef7f1c21851fd9c322339484e8345afd12376d976ddbd`  
		Last Modified: Tue, 09 Aug 2022 18:52:28 GMT  
		Size: 126.1 KB (126064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:794c752514ed274efa4c408cc26745be991e45f3bdf327ec010ef5d614a12e81`  
		Last Modified: Mon, 29 Aug 2022 19:27:39 GMT  
		Size: 982.0 KB (981999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1872e17927a44c66bc7cc1ab89e743c7ce518c421ab7dbec3b77da2ed55f1191`  
		Last Modified: Mon, 29 Aug 2022 19:27:38 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671ee1b68e567ecbfd0d99f4331f15d70a320c05193a577228fa8b911be55513`  
		Last Modified: Mon, 29 Aug 2022 19:27:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; s390x

```console
$ docker pull memcached@sha256:1aca14af5e45939b3b68973e8c599cb648d30771513ce390a9f0eef85c4f17ea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3646984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d704b926b5f988e9db5404831fa6b7a4f8da14a0a3593e225669ff5e99aa2d56`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 19:11:19 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 09 Aug 2022 19:11:20 GMT
RUN apk add --no-cache libsasl
# Mon, 29 Aug 2022 18:51:35 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 18:51:35 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 18:55:03 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Mon, 29 Aug 2022 18:55:03 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 18:55:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 18:55:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 18:55:04 GMT
USER memcache
# Mon, 29 Aug 2022 18:55:04 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 18:55:04 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463a70f3df946e83a223bd55002470af1b7f8d483babe452e515a809b965d35c`  
		Last Modified: Tue, 09 Aug 2022 19:15:35 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df0b8be6e73cbbdde959ca7a21d3fd6c8e36e05bc9c7a46be4e5bfa5b664a50c`  
		Last Modified: Tue, 09 Aug 2022 19:15:35 GMT  
		Size: 112.5 KB (112508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54547b52522c89500f1653dc849604a8a264e93fd45501c6ecc53b9b32824c31`  
		Last Modified: Mon, 29 Aug 2022 18:56:03 GMT  
		Size: 942.2 KB (942207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d838190f94a4d872ed0e972e293eafdda311d2d029f93f8c9fcffe960c8bc74`  
		Last Modified: Mon, 29 Aug 2022 18:56:02 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b2bd5df4107bc3326be940291bf4aacb1a1de4760ca3315321bebf59195856`  
		Last Modified: Mon, 29 Aug 2022 18:56:03 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1-alpine3.16`

```console
$ docker pull memcached@sha256:c2f5df2c5099744a041132d1c11900d90f4b9e9c587a38ba8b12f9c03e82cfff
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
$ docker pull memcached@sha256:3b2a8f0dbcbb96b42edffa4959170c2486ddb2bef3de057f8ed71591348721c0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3891406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc6dc88eceeba2070ee6fe3c8c979afeaf5bf6d36e86d09d6457dd8432bb4c36`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:39 GMT
ADD file:b828bc14bc5ff03c8f7310fe0aed6ac5df19a393622d5d1d779a523234d07c0a in / 
# Tue, 09 Aug 2022 17:38:39 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:34:01 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 09 Aug 2022 18:34:02 GMT
RUN apk add --no-cache libsasl
# Mon, 29 Aug 2022 18:41:47 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 18:41:48 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 18:44:43 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Mon, 29 Aug 2022 18:44:45 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 18:44:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 18:44:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 18:44:47 GMT
USER memcache
# Mon, 29 Aug 2022 18:44:48 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 18:44:49 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6c0d3b419d848ea31ca748254611d5d5ce3b76e3d7bba520fd87400fbb75f3b9`  
		Last Modified: Tue, 09 Aug 2022 17:39:33 GMT  
		Size: 2.8 MB (2807121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240e236335200614c944d9ba79e2d7eda5cfa258a69e669b585cc28314d754f5`  
		Last Modified: Tue, 09 Aug 2022 18:38:05 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:844d1ba63a22190468423984b12b7d36f6c005e3316461b983f975f4b8dc9ee8`  
		Last Modified: Tue, 09 Aug 2022 18:38:05 GMT  
		Size: 119.8 KB (119826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2e7c344cfe47d96e7a9d170c9427c474246d16b76964c915cdd2f3d5e62698`  
		Last Modified: Mon, 29 Aug 2022 18:46:29 GMT  
		Size: 962.8 KB (962814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed467891e81f8057bb74046a7442a949b8f2ab27dc7099c321d77f2497584541`  
		Last Modified: Mon, 29 Aug 2022 18:46:29 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5326fe38fa94412c48f8bf0980206aed389413a089a646b582739edc31841a`  
		Last Modified: Mon, 29 Aug 2022 18:46:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.16` - linux; ppc64le

```console
$ docker pull memcached@sha256:79f15ab95c7dc52c17fab8ebc50e1a380b3584fd2127402ba0486ca4311be7df
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3913056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d80b3f9d28d32be6c7fdc9e706c4555e3bc835f495aed408fe264c0a8ed3d6a7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:48:17 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 09 Aug 2022 18:48:19 GMT
RUN apk add --no-cache libsasl
# Mon, 29 Aug 2022 19:23:01 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 19:23:02 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 19:26:15 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Mon, 29 Aug 2022 19:26:16 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 19:26:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 19:26:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 19:26:17 GMT
USER memcache
# Mon, 29 Aug 2022 19:26:18 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 19:26:18 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:086c869249c97411ce380e3b76305e0b85731874d0ea57dfd0de74e1f387443d`  
		Last Modified: Tue, 09 Aug 2022 18:52:28 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75e55886182590f2e7eef7f1c21851fd9c322339484e8345afd12376d976ddbd`  
		Last Modified: Tue, 09 Aug 2022 18:52:28 GMT  
		Size: 126.1 KB (126064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:794c752514ed274efa4c408cc26745be991e45f3bdf327ec010ef5d614a12e81`  
		Last Modified: Mon, 29 Aug 2022 19:27:39 GMT  
		Size: 982.0 KB (981999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1872e17927a44c66bc7cc1ab89e743c7ce518c421ab7dbec3b77da2ed55f1191`  
		Last Modified: Mon, 29 Aug 2022 19:27:38 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671ee1b68e567ecbfd0d99f4331f15d70a320c05193a577228fa8b911be55513`  
		Last Modified: Mon, 29 Aug 2022 19:27:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.16` - linux; s390x

```console
$ docker pull memcached@sha256:1aca14af5e45939b3b68973e8c599cb648d30771513ce390a9f0eef85c4f17ea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3646984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d704b926b5f988e9db5404831fa6b7a4f8da14a0a3593e225669ff5e99aa2d56`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 19:11:19 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 09 Aug 2022 19:11:20 GMT
RUN apk add --no-cache libsasl
# Mon, 29 Aug 2022 18:51:35 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 18:51:35 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 18:55:03 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Mon, 29 Aug 2022 18:55:03 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 18:55:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 18:55:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 18:55:04 GMT
USER memcache
# Mon, 29 Aug 2022 18:55:04 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 18:55:04 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463a70f3df946e83a223bd55002470af1b7f8d483babe452e515a809b965d35c`  
		Last Modified: Tue, 09 Aug 2022 19:15:35 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df0b8be6e73cbbdde959ca7a21d3fd6c8e36e05bc9c7a46be4e5bfa5b664a50c`  
		Last Modified: Tue, 09 Aug 2022 19:15:35 GMT  
		Size: 112.5 KB (112508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54547b52522c89500f1653dc849604a8a264e93fd45501c6ecc53b9b32824c31`  
		Last Modified: Mon, 29 Aug 2022 18:56:03 GMT  
		Size: 942.2 KB (942207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d838190f94a4d872ed0e972e293eafdda311d2d029f93f8c9fcffe960c8bc74`  
		Last Modified: Mon, 29 Aug 2022 18:56:02 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b2bd5df4107bc3326be940291bf4aacb1a1de4760ca3315321bebf59195856`  
		Last Modified: Mon, 29 Aug 2022 18:56:03 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1-bullseye`

```console
$ docker pull memcached@sha256:1917f1b4e48a69e5be80a57c321504338f9b65046386ea50ee679322413e26c7
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
$ docker pull memcached@sha256:2a9bf2539b24c553b92c876dfbe6dd48450a832f2b5395ec3217271018ad2ca0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32971284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92e1422c3edf80b790f0a601173b8e329b6619096d8cebb0b50b0f489ad1d971`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:54:26 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 23 Aug 2022 02:54:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 29 Aug 2022 19:57:00 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 19:57:01 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 19:59:41 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Mon, 29 Aug 2022 19:59:41 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 19:59:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 19:59:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 19:59:42 GMT
USER memcache
# Mon, 29 Aug 2022 19:59:42 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 19:59:42 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa73fb65ea8b12a2375459f0d656d3ad06e2863c906fcf962486eda3701f3fd6`  
		Last Modified: Tue, 23 Aug 2022 02:57:38 GMT  
		Size: 5.0 KB (4981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502b4e8803067b28098d0ea52281cfef66da1ee1e869241612b545d7e9ff12de`  
		Last Modified: Tue, 23 Aug 2022 02:57:38 GMT  
		Size: 328.1 KB (328108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b905db5d33a47882bd6cb4935bcc5d576d5cad5ba761b6b4004982c3aa7333`  
		Last Modified: Mon, 29 Aug 2022 20:03:05 GMT  
		Size: 1.3 MB (1256303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93643c661348540c2edcfc8a007b2c9aff33ac36cb9dcd910e0ddb51f50cd09e`  
		Last Modified: Mon, 29 Aug 2022 20:03:04 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc510e39dc783b83b00e5abd05d57df948435a0aaf45e87b131cc0fff83021e`  
		Last Modified: Mon, 29 Aug 2022 20:03:05 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; arm variant v5

```console
$ docker pull memcached@sha256:ef629e7153669e6100c98fba79336f87cc033d073c6219d6c7ec9360298a5d8e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30454536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84960478143b53154da0f3409e3f1141b62dabf4fe0c97c3661b5dd8a1c533ec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Sep 2022 00:53:30 GMT
ADD file:539e23f1c3a625a612a5a59b3939e9692c86c3cfa4956d30f4802c9f34ffa29c in / 
# Tue, 13 Sep 2022 00:53:31 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 03:18:14 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 13 Sep 2022 03:18:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 03:18:20 GMT
ENV MEMCACHED_VERSION=1.6.17
# Tue, 13 Sep 2022 03:18:20 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Tue, 13 Sep 2022 03:24:21 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 13 Sep 2022 03:24:22 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 13 Sep 2022 03:24:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Sep 2022 03:24:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Sep 2022 03:24:22 GMT
USER memcache
# Tue, 13 Sep 2022 03:24:22 GMT
EXPOSE 11211
# Tue, 13 Sep 2022 03:24:22 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:705abbab4fcb3a8dfe046a2ae6c450328aa11d93911abce66d3bba8bc693cbd4`  
		Last Modified: Tue, 13 Sep 2022 01:01:07 GMT  
		Size: 28.9 MB (28905288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eba43be24e48cc0796f0f5a17e6b674c0f07d5626f56ac8ed9f717cba0d0503`  
		Last Modified: Tue, 13 Sep 2022 03:24:59 GMT  
		Size: 4.9 KB (4894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c93e222cf0a02e2b4146a4d3ff6e5da33b929a10129fd88081a505e4011b9e`  
		Last Modified: Tue, 13 Sep 2022 03:25:00 GMT  
		Size: 316.6 KB (316638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b091f5c4cb7701e12cc29c82ee78e1704fdaaabcd851004efea8deb3acf7f2f`  
		Last Modified: Tue, 13 Sep 2022 03:25:00 GMT  
		Size: 1.2 MB (1227311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5e30653aa54ef905fcc6b97813278f8b54e56e889b1ffccf5101df4fa45882`  
		Last Modified: Tue, 13 Sep 2022 03:24:59 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471afe7d2cb0083a807b44b87fa581728a14e66fbada1f0ea0bcff34258f1cca`  
		Last Modified: Tue, 13 Sep 2022 03:24:59 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; arm variant v7

```console
$ docker pull memcached@sha256:960b71bacce5bbd2bf5c700ca3398d8ce00c1a9ebb35a5b690be486267128ef1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28088375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a54ccaf5bd1ba99327d598c288c19a655c2601e43aaf08c6429e99c287ab5b35`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 23 Aug 2022 01:43:01 GMT
ADD file:4cd1b4287674228db28402a76aa4f241740585448be48b5b15068d275ee9eb84 in / 
# Tue, 23 Aug 2022 01:43:01 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 18:03:50 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 23 Aug 2022 18:03:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 29 Aug 2022 19:04:31 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 19:04:31 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 19:09:39 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Mon, 29 Aug 2022 19:09:40 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 19:09:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 19:09:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 19:09:40 GMT
USER memcache
# Mon, 29 Aug 2022 19:09:40 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 19:09:40 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:051ba72559abd0cf65b34b75605580f58636ec3cb994f97de317632a85d82761`  
		Last Modified: Tue, 23 Aug 2022 01:50:05 GMT  
		Size: 26.6 MB (26571732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12dc4f2d8dca33e3850e55e4a2cd25a6dbf19afb27df3daef33de65ac91fd757`  
		Last Modified: Tue, 23 Aug 2022 21:10:42 GMT  
		Size: 4.9 KB (4893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:033f621bef4d3464e367d2c0ce45f3ec626c1c21f84ba7e84ece82bfbef4666e`  
		Last Modified: Tue, 23 Aug 2022 21:10:42 GMT  
		Size: 312.0 KB (312045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba873971d43c849095b8112993f9eb97b90c155f9f9f190da2bef761c9aa61a8`  
		Last Modified: Mon, 29 Aug 2022 19:26:29 GMT  
		Size: 1.2 MB (1199297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b256a2f081d1033d7ae503b0735b03640cd5b071e47fce65387238edf010a05c`  
		Last Modified: Mon, 29 Aug 2022 19:26:29 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a75e8764536efcd4e0fbd3d6c058eb6e05a0489f9e157f95e9e9ca0639c7d40b`  
		Last Modified: Mon, 29 Aug 2022 19:26:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:c67982406cd3e3fb90c50951d6a8cd766a4c0cc625ef035237913dfe56c0ae88
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31444531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02936ddd3c3f04b28ca0fbb9e803bfe5c3c1c0bda9ffe6ca0c6ea9954c351ab8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 13:12:07 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 23 Aug 2022 13:12:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 29 Aug 2022 18:48:57 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 18:48:58 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 18:51:30 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Mon, 29 Aug 2022 18:51:32 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 18:51:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 18:51:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 18:51:34 GMT
USER memcache
# Mon, 29 Aug 2022 18:51:35 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 18:51:36 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21794f0e498790afd69f2d317bbed8aa9cdbd3dddc56f7d52f1b806577e38a06`  
		Last Modified: Tue, 23 Aug 2022 13:15:43 GMT  
		Size: 4.9 KB (4904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:261db6d67ef285bdd84e6ae9e72182c4cd348b9f6c3c060c723764d03a12c2f6`  
		Last Modified: Tue, 23 Aug 2022 13:15:43 GMT  
		Size: 119.2 KB (119240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646e70d704c1f14afdd9de28cb4081703a4efc97e9c6a743ba80329c00705b37`  
		Last Modified: Mon, 29 Aug 2022 18:55:22 GMT  
		Size: 1.3 MB (1256190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db1c8f9c761c12c5c76962f55a2baff7f18d665a53fa76a2d3329fc2c0ccf313`  
		Last Modified: Mon, 29 Aug 2022 18:55:21 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4655eda4ba606249d810ba4d37deb1e82c106bcf3a2394f684a6ad8275d98950`  
		Last Modified: Mon, 29 Aug 2022 18:55:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; 386

```console
$ docker pull memcached@sha256:9a142ff1556091ea4d817d7ac5c26fcc6a0b2daa5bf99a56c64d19bb3e3cb866
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33776358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e0455947003534873a7c3f6d3bae27183601ae7c8b66f094e52d72450507327`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 23 Aug 2022 01:02:40 GMT
ADD file:5ca62c98116941aaa64ec72afb689a088c46f75a3e83d5b0d4e58d65ec905ccd in / 
# Tue, 23 Aug 2022 01:02:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:22:44 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 23 Aug 2022 03:22:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 29 Aug 2022 18:38:36 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 18:38:36 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 18:41:29 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Mon, 29 Aug 2022 18:41:31 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 18:41:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 18:41:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 18:41:33 GMT
USER memcache
# Mon, 29 Aug 2022 18:41:34 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 18:41:35 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6b3cb4a05a891d9d8a87a2bd7247b16f79832a9d4afbad3ff5068f6fc2ba1560`  
		Last Modified: Tue, 23 Aug 2022 01:08:25 GMT  
		Size: 32.4 MB (32387317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd24201e0b5e9a68a67bdc3b464a01aeb9a2e5a859a582cdaa80ab08a608337`  
		Last Modified: Tue, 23 Aug 2022 03:27:47 GMT  
		Size: 4.8 KB (4774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3070e5e3b1d98fa0b67b8390880b7596c4719b774864de21f36ed86873041793`  
		Last Modified: Tue, 23 Aug 2022 03:27:48 GMT  
		Size: 130.1 KB (130136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af8c1cee54f7ff86c820ca418aa3d2c05c5f200ca4d938ba76c8f8439b39cb04`  
		Last Modified: Mon, 29 Aug 2022 18:45:40 GMT  
		Size: 1.3 MB (1253721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94d7ae33ce7f8ea696d92c06ef6fd7c86c8228061b3b2485a78a9f59131a48aa`  
		Last Modified: Mon, 29 Aug 2022 18:45:43 GMT  
		Size: 289.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5348ed42ca0cf0c971fcaddc7677e8a3508548c0e3ca9e12b49cc06627f4657c`  
		Last Modified: Mon, 29 Aug 2022 18:45:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; mips64le

```console
$ docker pull memcached@sha256:e1403115858fda192fda48a365294d78dd1ea7fa6c9db3be737a883cb34fd9de
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31001916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ce2440650f197fcd6de50038d9a16d23be6db7efc79a8115173cc1ca5a769f5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Sep 2022 01:10:58 GMT
ADD file:91a8d8627a614ff3741d68216da46f13b393e52a70377b97ef317e4a00a3cac6 in / 
# Tue, 13 Sep 2022 01:11:02 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 04:50:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 13 Sep 2022 04:50:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 04:50:38 GMT
ENV MEMCACHED_VERSION=1.6.17
# Tue, 13 Sep 2022 04:50:40 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Tue, 13 Sep 2022 04:57:36 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 13 Sep 2022 04:57:38 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 13 Sep 2022 04:57:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Sep 2022 04:57:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Sep 2022 04:57:48 GMT
USER memcache
# Tue, 13 Sep 2022 04:57:50 GMT
EXPOSE 11211
# Tue, 13 Sep 2022 04:57:53 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:98abeb1446d0e9df6f48d5f72a70b36598cfc1091c9a5ca82690bedcf320e2b3`  
		Last Modified: Tue, 13 Sep 2022 01:18:50 GMT  
		Size: 29.6 MB (29627659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766602637141a485f59d0fc04aec4bfa1ac38583bba125b35c0b6809f1219ed9`  
		Last Modified: Tue, 13 Sep 2022 04:58:11 GMT  
		Size: 4.9 KB (4857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21b631e5bb3330fba3352d6332ae5cfa0b9a35dbc33b4d643b80f7b908c950f5`  
		Last Modified: Tue, 13 Sep 2022 04:58:11 GMT  
		Size: 117.2 KB (117159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee33141b788356ead96c93190f0008f455371a4562d92b27a20945aac60d1361`  
		Last Modified: Tue, 13 Sep 2022 04:58:12 GMT  
		Size: 1.3 MB (1251835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e488d322d0c180f442d31923e23e79064b584ac59e2cadf3be31cc702751460d`  
		Last Modified: Tue, 13 Sep 2022 04:58:11 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec80c89f379732f5466f55915bbad33a4b55dc651bf6346712c92cff64717b11`  
		Last Modified: Tue, 13 Sep 2022 04:58:11 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; ppc64le

```console
$ docker pull memcached@sha256:0176bec998e05785ddcaadb9c692b14571e10c2b71050a9988329f903660369b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36970738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7a0216731101d94583b08e4b42f59092a78019783e49a2ddb6401ea59c9d47d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 23 Aug 2022 01:24:52 GMT
ADD file:d35213360d726a18e220276d33f245115c3e94a321addaa4c9127488368b0203 in / 
# Tue, 23 Aug 2022 01:24:54 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:34:49 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 23 Aug 2022 02:34:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 29 Aug 2022 19:19:51 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 19:19:51 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 19:22:46 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Mon, 29 Aug 2022 19:22:47 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 19:22:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 19:22:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 19:22:48 GMT
USER memcache
# Mon, 29 Aug 2022 19:22:49 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 19:22:49 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:698954eda09d38dd1ccc9ce777b1f6bc7f7473fc6c4c3eb634acc8d035a42eae`  
		Last Modified: Tue, 23 Aug 2022 01:30:36 GMT  
		Size: 35.3 MB (35284280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffb080d920662043edc67113c0de4c68258ad19c0fffd9e3b79fa01800c6015`  
		Last Modified: Tue, 23 Aug 2022 02:39:09 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b1f66b68991d8f5ab064b3988db37a48b8f28b4ef0eb8e83efa4c419b630ff`  
		Last Modified: Tue, 23 Aug 2022 02:39:09 GMT  
		Size: 356.9 KB (356931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2256c5b8427744c7563d1151efbeb03c935fbb3e87d621903c9e7476a8db7494`  
		Last Modified: Mon, 29 Aug 2022 19:27:05 GMT  
		Size: 1.3 MB (1324139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee6919a18fb52b4b8259e2942d1d56ca42a4371f735bedd875c5eebdaee214a2`  
		Last Modified: Mon, 29 Aug 2022 19:27:04 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ac3c74fbd1e874bdc7163ccf1ba8bf496b085875b4165fcec2e4a771d9742f9`  
		Last Modified: Mon, 29 Aug 2022 19:27:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bullseye` - linux; s390x

```console
$ docker pull memcached@sha256:f063181874bf86b26f7e8d033e02792331b3282ef6614aa99d8d70c8b178aac0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31206151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c2827f7c0c4acdb1d09c90d24a8e27f37bd489dca825a2831b3f923831b1125`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Sep 2022 00:48:07 GMT
ADD file:e8a6c2e8be5d9d1f83c1e280419014489438391a9feb7c77b6c21adbf0ec062b in / 
# Tue, 13 Sep 2022 00:48:08 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 01:59:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 13 Sep 2022 01:59:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 01:59:22 GMT
ENV MEMCACHED_VERSION=1.6.17
# Tue, 13 Sep 2022 01:59:23 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Tue, 13 Sep 2022 02:02:36 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 13 Sep 2022 02:02:36 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 13 Sep 2022 02:02:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Sep 2022 02:02:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Sep 2022 02:02:37 GMT
USER memcache
# Tue, 13 Sep 2022 02:02:37 GMT
EXPOSE 11211
# Tue, 13 Sep 2022 02:02:37 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c64715e5ebd39975a39b5cf2535772544c27713cbed678b0a21e73680fffaf72`  
		Last Modified: Tue, 13 Sep 2022 00:52:39 GMT  
		Size: 29.6 MB (29635080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce5055aafbfbe726c8840111d8300b0c75f707a8ab517395bb8be985d2feb009`  
		Last Modified: Tue, 13 Sep 2022 02:03:36 GMT  
		Size: 5.0 KB (5021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9a227f323eed41d16b462d95503000badd5210aa179dd3065f4363fe3a1b9f`  
		Last Modified: Tue, 13 Sep 2022 02:03:36 GMT  
		Size: 324.2 KB (324172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36fb60d78f8bd69265b4c2d2246169797772da4584f6e063d49eab9c2f040c51`  
		Last Modified: Tue, 13 Sep 2022 02:03:36 GMT  
		Size: 1.2 MB (1241470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d23a9497c5fd3ec0d26f920c59f1f1628999ae546bd1b2f722b29fbf27e3402`  
		Last Modified: Tue, 13 Sep 2022 02:03:36 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009331f552a168c5b26209994b10c7684fc80fe6348a406878b2262037e82435`  
		Last Modified: Tue, 13 Sep 2022 02:03:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6`

```console
$ docker pull memcached@sha256:1917f1b4e48a69e5be80a57c321504338f9b65046386ea50ee679322413e26c7
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
$ docker pull memcached@sha256:2a9bf2539b24c553b92c876dfbe6dd48450a832f2b5395ec3217271018ad2ca0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32971284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92e1422c3edf80b790f0a601173b8e329b6619096d8cebb0b50b0f489ad1d971`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:54:26 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 23 Aug 2022 02:54:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 29 Aug 2022 19:57:00 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 19:57:01 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 19:59:41 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Mon, 29 Aug 2022 19:59:41 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 19:59:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 19:59:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 19:59:42 GMT
USER memcache
# Mon, 29 Aug 2022 19:59:42 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 19:59:42 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa73fb65ea8b12a2375459f0d656d3ad06e2863c906fcf962486eda3701f3fd6`  
		Last Modified: Tue, 23 Aug 2022 02:57:38 GMT  
		Size: 5.0 KB (4981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502b4e8803067b28098d0ea52281cfef66da1ee1e869241612b545d7e9ff12de`  
		Last Modified: Tue, 23 Aug 2022 02:57:38 GMT  
		Size: 328.1 KB (328108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b905db5d33a47882bd6cb4935bcc5d576d5cad5ba761b6b4004982c3aa7333`  
		Last Modified: Mon, 29 Aug 2022 20:03:05 GMT  
		Size: 1.3 MB (1256303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93643c661348540c2edcfc8a007b2c9aff33ac36cb9dcd910e0ddb51f50cd09e`  
		Last Modified: Mon, 29 Aug 2022 20:03:04 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc510e39dc783b83b00e5abd05d57df948435a0aaf45e87b131cc0fff83021e`  
		Last Modified: Mon, 29 Aug 2022 20:03:05 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm variant v5

```console
$ docker pull memcached@sha256:ef629e7153669e6100c98fba79336f87cc033d073c6219d6c7ec9360298a5d8e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30454536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84960478143b53154da0f3409e3f1141b62dabf4fe0c97c3661b5dd8a1c533ec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Sep 2022 00:53:30 GMT
ADD file:539e23f1c3a625a612a5a59b3939e9692c86c3cfa4956d30f4802c9f34ffa29c in / 
# Tue, 13 Sep 2022 00:53:31 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 03:18:14 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 13 Sep 2022 03:18:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 03:18:20 GMT
ENV MEMCACHED_VERSION=1.6.17
# Tue, 13 Sep 2022 03:18:20 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Tue, 13 Sep 2022 03:24:21 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 13 Sep 2022 03:24:22 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 13 Sep 2022 03:24:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Sep 2022 03:24:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Sep 2022 03:24:22 GMT
USER memcache
# Tue, 13 Sep 2022 03:24:22 GMT
EXPOSE 11211
# Tue, 13 Sep 2022 03:24:22 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:705abbab4fcb3a8dfe046a2ae6c450328aa11d93911abce66d3bba8bc693cbd4`  
		Last Modified: Tue, 13 Sep 2022 01:01:07 GMT  
		Size: 28.9 MB (28905288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eba43be24e48cc0796f0f5a17e6b674c0f07d5626f56ac8ed9f717cba0d0503`  
		Last Modified: Tue, 13 Sep 2022 03:24:59 GMT  
		Size: 4.9 KB (4894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c93e222cf0a02e2b4146a4d3ff6e5da33b929a10129fd88081a505e4011b9e`  
		Last Modified: Tue, 13 Sep 2022 03:25:00 GMT  
		Size: 316.6 KB (316638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b091f5c4cb7701e12cc29c82ee78e1704fdaaabcd851004efea8deb3acf7f2f`  
		Last Modified: Tue, 13 Sep 2022 03:25:00 GMT  
		Size: 1.2 MB (1227311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5e30653aa54ef905fcc6b97813278f8b54e56e889b1ffccf5101df4fa45882`  
		Last Modified: Tue, 13 Sep 2022 03:24:59 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471afe7d2cb0083a807b44b87fa581728a14e66fbada1f0ea0bcff34258f1cca`  
		Last Modified: Tue, 13 Sep 2022 03:24:59 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm variant v7

```console
$ docker pull memcached@sha256:960b71bacce5bbd2bf5c700ca3398d8ce00c1a9ebb35a5b690be486267128ef1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28088375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a54ccaf5bd1ba99327d598c288c19a655c2601e43aaf08c6429e99c287ab5b35`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 23 Aug 2022 01:43:01 GMT
ADD file:4cd1b4287674228db28402a76aa4f241740585448be48b5b15068d275ee9eb84 in / 
# Tue, 23 Aug 2022 01:43:01 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 18:03:50 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 23 Aug 2022 18:03:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 29 Aug 2022 19:04:31 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 19:04:31 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 19:09:39 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Mon, 29 Aug 2022 19:09:40 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 19:09:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 19:09:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 19:09:40 GMT
USER memcache
# Mon, 29 Aug 2022 19:09:40 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 19:09:40 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:051ba72559abd0cf65b34b75605580f58636ec3cb994f97de317632a85d82761`  
		Last Modified: Tue, 23 Aug 2022 01:50:05 GMT  
		Size: 26.6 MB (26571732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12dc4f2d8dca33e3850e55e4a2cd25a6dbf19afb27df3daef33de65ac91fd757`  
		Last Modified: Tue, 23 Aug 2022 21:10:42 GMT  
		Size: 4.9 KB (4893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:033f621bef4d3464e367d2c0ce45f3ec626c1c21f84ba7e84ece82bfbef4666e`  
		Last Modified: Tue, 23 Aug 2022 21:10:42 GMT  
		Size: 312.0 KB (312045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba873971d43c849095b8112993f9eb97b90c155f9f9f190da2bef761c9aa61a8`  
		Last Modified: Mon, 29 Aug 2022 19:26:29 GMT  
		Size: 1.2 MB (1199297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b256a2f081d1033d7ae503b0735b03640cd5b071e47fce65387238edf010a05c`  
		Last Modified: Mon, 29 Aug 2022 19:26:29 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a75e8764536efcd4e0fbd3d6c058eb6e05a0489f9e157f95e9e9ca0639c7d40b`  
		Last Modified: Mon, 29 Aug 2022 19:26:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:c67982406cd3e3fb90c50951d6a8cd766a4c0cc625ef035237913dfe56c0ae88
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31444531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02936ddd3c3f04b28ca0fbb9e803bfe5c3c1c0bda9ffe6ca0c6ea9954c351ab8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 13:12:07 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 23 Aug 2022 13:12:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 29 Aug 2022 18:48:57 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 18:48:58 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 18:51:30 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Mon, 29 Aug 2022 18:51:32 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 18:51:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 18:51:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 18:51:34 GMT
USER memcache
# Mon, 29 Aug 2022 18:51:35 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 18:51:36 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21794f0e498790afd69f2d317bbed8aa9cdbd3dddc56f7d52f1b806577e38a06`  
		Last Modified: Tue, 23 Aug 2022 13:15:43 GMT  
		Size: 4.9 KB (4904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:261db6d67ef285bdd84e6ae9e72182c4cd348b9f6c3c060c723764d03a12c2f6`  
		Last Modified: Tue, 23 Aug 2022 13:15:43 GMT  
		Size: 119.2 KB (119240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646e70d704c1f14afdd9de28cb4081703a4efc97e9c6a743ba80329c00705b37`  
		Last Modified: Mon, 29 Aug 2022 18:55:22 GMT  
		Size: 1.3 MB (1256190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db1c8f9c761c12c5c76962f55a2baff7f18d665a53fa76a2d3329fc2c0ccf313`  
		Last Modified: Mon, 29 Aug 2022 18:55:21 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4655eda4ba606249d810ba4d37deb1e82c106bcf3a2394f684a6ad8275d98950`  
		Last Modified: Mon, 29 Aug 2022 18:55:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; 386

```console
$ docker pull memcached@sha256:9a142ff1556091ea4d817d7ac5c26fcc6a0b2daa5bf99a56c64d19bb3e3cb866
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33776358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e0455947003534873a7c3f6d3bae27183601ae7c8b66f094e52d72450507327`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 23 Aug 2022 01:02:40 GMT
ADD file:5ca62c98116941aaa64ec72afb689a088c46f75a3e83d5b0d4e58d65ec905ccd in / 
# Tue, 23 Aug 2022 01:02:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:22:44 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 23 Aug 2022 03:22:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 29 Aug 2022 18:38:36 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 18:38:36 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 18:41:29 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Mon, 29 Aug 2022 18:41:31 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 18:41:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 18:41:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 18:41:33 GMT
USER memcache
# Mon, 29 Aug 2022 18:41:34 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 18:41:35 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6b3cb4a05a891d9d8a87a2bd7247b16f79832a9d4afbad3ff5068f6fc2ba1560`  
		Last Modified: Tue, 23 Aug 2022 01:08:25 GMT  
		Size: 32.4 MB (32387317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd24201e0b5e9a68a67bdc3b464a01aeb9a2e5a859a582cdaa80ab08a608337`  
		Last Modified: Tue, 23 Aug 2022 03:27:47 GMT  
		Size: 4.8 KB (4774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3070e5e3b1d98fa0b67b8390880b7596c4719b774864de21f36ed86873041793`  
		Last Modified: Tue, 23 Aug 2022 03:27:48 GMT  
		Size: 130.1 KB (130136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af8c1cee54f7ff86c820ca418aa3d2c05c5f200ca4d938ba76c8f8439b39cb04`  
		Last Modified: Mon, 29 Aug 2022 18:45:40 GMT  
		Size: 1.3 MB (1253721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94d7ae33ce7f8ea696d92c06ef6fd7c86c8228061b3b2485a78a9f59131a48aa`  
		Last Modified: Mon, 29 Aug 2022 18:45:43 GMT  
		Size: 289.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5348ed42ca0cf0c971fcaddc7677e8a3508548c0e3ca9e12b49cc06627f4657c`  
		Last Modified: Mon, 29 Aug 2022 18:45:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; mips64le

```console
$ docker pull memcached@sha256:e1403115858fda192fda48a365294d78dd1ea7fa6c9db3be737a883cb34fd9de
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31001916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ce2440650f197fcd6de50038d9a16d23be6db7efc79a8115173cc1ca5a769f5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Sep 2022 01:10:58 GMT
ADD file:91a8d8627a614ff3741d68216da46f13b393e52a70377b97ef317e4a00a3cac6 in / 
# Tue, 13 Sep 2022 01:11:02 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 04:50:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 13 Sep 2022 04:50:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 04:50:38 GMT
ENV MEMCACHED_VERSION=1.6.17
# Tue, 13 Sep 2022 04:50:40 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Tue, 13 Sep 2022 04:57:36 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 13 Sep 2022 04:57:38 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 13 Sep 2022 04:57:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Sep 2022 04:57:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Sep 2022 04:57:48 GMT
USER memcache
# Tue, 13 Sep 2022 04:57:50 GMT
EXPOSE 11211
# Tue, 13 Sep 2022 04:57:53 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:98abeb1446d0e9df6f48d5f72a70b36598cfc1091c9a5ca82690bedcf320e2b3`  
		Last Modified: Tue, 13 Sep 2022 01:18:50 GMT  
		Size: 29.6 MB (29627659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766602637141a485f59d0fc04aec4bfa1ac38583bba125b35c0b6809f1219ed9`  
		Last Modified: Tue, 13 Sep 2022 04:58:11 GMT  
		Size: 4.9 KB (4857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21b631e5bb3330fba3352d6332ae5cfa0b9a35dbc33b4d643b80f7b908c950f5`  
		Last Modified: Tue, 13 Sep 2022 04:58:11 GMT  
		Size: 117.2 KB (117159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee33141b788356ead96c93190f0008f455371a4562d92b27a20945aac60d1361`  
		Last Modified: Tue, 13 Sep 2022 04:58:12 GMT  
		Size: 1.3 MB (1251835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e488d322d0c180f442d31923e23e79064b584ac59e2cadf3be31cc702751460d`  
		Last Modified: Tue, 13 Sep 2022 04:58:11 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec80c89f379732f5466f55915bbad33a4b55dc651bf6346712c92cff64717b11`  
		Last Modified: Tue, 13 Sep 2022 04:58:11 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; ppc64le

```console
$ docker pull memcached@sha256:0176bec998e05785ddcaadb9c692b14571e10c2b71050a9988329f903660369b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36970738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7a0216731101d94583b08e4b42f59092a78019783e49a2ddb6401ea59c9d47d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 23 Aug 2022 01:24:52 GMT
ADD file:d35213360d726a18e220276d33f245115c3e94a321addaa4c9127488368b0203 in / 
# Tue, 23 Aug 2022 01:24:54 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:34:49 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 23 Aug 2022 02:34:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 29 Aug 2022 19:19:51 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 19:19:51 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 19:22:46 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Mon, 29 Aug 2022 19:22:47 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 19:22:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 19:22:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 19:22:48 GMT
USER memcache
# Mon, 29 Aug 2022 19:22:49 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 19:22:49 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:698954eda09d38dd1ccc9ce777b1f6bc7f7473fc6c4c3eb634acc8d035a42eae`  
		Last Modified: Tue, 23 Aug 2022 01:30:36 GMT  
		Size: 35.3 MB (35284280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffb080d920662043edc67113c0de4c68258ad19c0fffd9e3b79fa01800c6015`  
		Last Modified: Tue, 23 Aug 2022 02:39:09 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b1f66b68991d8f5ab064b3988db37a48b8f28b4ef0eb8e83efa4c419b630ff`  
		Last Modified: Tue, 23 Aug 2022 02:39:09 GMT  
		Size: 356.9 KB (356931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2256c5b8427744c7563d1151efbeb03c935fbb3e87d621903c9e7476a8db7494`  
		Last Modified: Mon, 29 Aug 2022 19:27:05 GMT  
		Size: 1.3 MB (1324139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee6919a18fb52b4b8259e2942d1d56ca42a4371f735bedd875c5eebdaee214a2`  
		Last Modified: Mon, 29 Aug 2022 19:27:04 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ac3c74fbd1e874bdc7163ccf1ba8bf496b085875b4165fcec2e4a771d9742f9`  
		Last Modified: Mon, 29 Aug 2022 19:27:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; s390x

```console
$ docker pull memcached@sha256:f063181874bf86b26f7e8d033e02792331b3282ef6614aa99d8d70c8b178aac0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31206151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c2827f7c0c4acdb1d09c90d24a8e27f37bd489dca825a2831b3f923831b1125`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Sep 2022 00:48:07 GMT
ADD file:e8a6c2e8be5d9d1f83c1e280419014489438391a9feb7c77b6c21adbf0ec062b in / 
# Tue, 13 Sep 2022 00:48:08 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 01:59:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 13 Sep 2022 01:59:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 01:59:22 GMT
ENV MEMCACHED_VERSION=1.6.17
# Tue, 13 Sep 2022 01:59:23 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Tue, 13 Sep 2022 02:02:36 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 13 Sep 2022 02:02:36 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 13 Sep 2022 02:02:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Sep 2022 02:02:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Sep 2022 02:02:37 GMT
USER memcache
# Tue, 13 Sep 2022 02:02:37 GMT
EXPOSE 11211
# Tue, 13 Sep 2022 02:02:37 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c64715e5ebd39975a39b5cf2535772544c27713cbed678b0a21e73680fffaf72`  
		Last Modified: Tue, 13 Sep 2022 00:52:39 GMT  
		Size: 29.6 MB (29635080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce5055aafbfbe726c8840111d8300b0c75f707a8ab517395bb8be985d2feb009`  
		Last Modified: Tue, 13 Sep 2022 02:03:36 GMT  
		Size: 5.0 KB (5021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9a227f323eed41d16b462d95503000badd5210aa179dd3065f4363fe3a1b9f`  
		Last Modified: Tue, 13 Sep 2022 02:03:36 GMT  
		Size: 324.2 KB (324172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36fb60d78f8bd69265b4c2d2246169797772da4584f6e063d49eab9c2f040c51`  
		Last Modified: Tue, 13 Sep 2022 02:03:36 GMT  
		Size: 1.2 MB (1241470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d23a9497c5fd3ec0d26f920c59f1f1628999ae546bd1b2f722b29fbf27e3402`  
		Last Modified: Tue, 13 Sep 2022 02:03:36 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009331f552a168c5b26209994b10c7684fc80fe6348a406878b2262037e82435`  
		Last Modified: Tue, 13 Sep 2022 02:03:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6-alpine`

```console
$ docker pull memcached@sha256:6eff5e1647ee867d3fac2bac716568ced7005b8044651f181988a1d0971d3fce
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
$ docker pull memcached@sha256:3b2a8f0dbcbb96b42edffa4959170c2486ddb2bef3de057f8ed71591348721c0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3891406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc6dc88eceeba2070ee6fe3c8c979afeaf5bf6d36e86d09d6457dd8432bb4c36`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:39 GMT
ADD file:b828bc14bc5ff03c8f7310fe0aed6ac5df19a393622d5d1d779a523234d07c0a in / 
# Tue, 09 Aug 2022 17:38:39 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:34:01 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 09 Aug 2022 18:34:02 GMT
RUN apk add --no-cache libsasl
# Mon, 29 Aug 2022 18:41:47 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 18:41:48 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 18:44:43 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Mon, 29 Aug 2022 18:44:45 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 18:44:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 18:44:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 18:44:47 GMT
USER memcache
# Mon, 29 Aug 2022 18:44:48 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 18:44:49 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6c0d3b419d848ea31ca748254611d5d5ce3b76e3d7bba520fd87400fbb75f3b9`  
		Last Modified: Tue, 09 Aug 2022 17:39:33 GMT  
		Size: 2.8 MB (2807121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240e236335200614c944d9ba79e2d7eda5cfa258a69e669b585cc28314d754f5`  
		Last Modified: Tue, 09 Aug 2022 18:38:05 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:844d1ba63a22190468423984b12b7d36f6c005e3316461b983f975f4b8dc9ee8`  
		Last Modified: Tue, 09 Aug 2022 18:38:05 GMT  
		Size: 119.8 KB (119826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2e7c344cfe47d96e7a9d170c9427c474246d16b76964c915cdd2f3d5e62698`  
		Last Modified: Mon, 29 Aug 2022 18:46:29 GMT  
		Size: 962.8 KB (962814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed467891e81f8057bb74046a7442a949b8f2ab27dc7099c321d77f2497584541`  
		Last Modified: Mon, 29 Aug 2022 18:46:29 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5326fe38fa94412c48f8bf0980206aed389413a089a646b582739edc31841a`  
		Last Modified: Mon, 29 Aug 2022 18:46:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:79f15ab95c7dc52c17fab8ebc50e1a380b3584fd2127402ba0486ca4311be7df
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3913056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d80b3f9d28d32be6c7fdc9e706c4555e3bc835f495aed408fe264c0a8ed3d6a7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:48:17 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 09 Aug 2022 18:48:19 GMT
RUN apk add --no-cache libsasl
# Mon, 29 Aug 2022 19:23:01 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 19:23:02 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 19:26:15 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Mon, 29 Aug 2022 19:26:16 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 19:26:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 19:26:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 19:26:17 GMT
USER memcache
# Mon, 29 Aug 2022 19:26:18 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 19:26:18 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:086c869249c97411ce380e3b76305e0b85731874d0ea57dfd0de74e1f387443d`  
		Last Modified: Tue, 09 Aug 2022 18:52:28 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75e55886182590f2e7eef7f1c21851fd9c322339484e8345afd12376d976ddbd`  
		Last Modified: Tue, 09 Aug 2022 18:52:28 GMT  
		Size: 126.1 KB (126064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:794c752514ed274efa4c408cc26745be991e45f3bdf327ec010ef5d614a12e81`  
		Last Modified: Mon, 29 Aug 2022 19:27:39 GMT  
		Size: 982.0 KB (981999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1872e17927a44c66bc7cc1ab89e743c7ce518c421ab7dbec3b77da2ed55f1191`  
		Last Modified: Mon, 29 Aug 2022 19:27:38 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671ee1b68e567ecbfd0d99f4331f15d70a320c05193a577228fa8b911be55513`  
		Last Modified: Mon, 29 Aug 2022 19:27:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; s390x

```console
$ docker pull memcached@sha256:1aca14af5e45939b3b68973e8c599cb648d30771513ce390a9f0eef85c4f17ea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3646984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d704b926b5f988e9db5404831fa6b7a4f8da14a0a3593e225669ff5e99aa2d56`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 19:11:19 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 09 Aug 2022 19:11:20 GMT
RUN apk add --no-cache libsasl
# Mon, 29 Aug 2022 18:51:35 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 18:51:35 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 18:55:03 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Mon, 29 Aug 2022 18:55:03 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 18:55:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 18:55:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 18:55:04 GMT
USER memcache
# Mon, 29 Aug 2022 18:55:04 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 18:55:04 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463a70f3df946e83a223bd55002470af1b7f8d483babe452e515a809b965d35c`  
		Last Modified: Tue, 09 Aug 2022 19:15:35 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df0b8be6e73cbbdde959ca7a21d3fd6c8e36e05bc9c7a46be4e5bfa5b664a50c`  
		Last Modified: Tue, 09 Aug 2022 19:15:35 GMT  
		Size: 112.5 KB (112508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54547b52522c89500f1653dc849604a8a264e93fd45501c6ecc53b9b32824c31`  
		Last Modified: Mon, 29 Aug 2022 18:56:03 GMT  
		Size: 942.2 KB (942207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d838190f94a4d872ed0e972e293eafdda311d2d029f93f8c9fcffe960c8bc74`  
		Last Modified: Mon, 29 Aug 2022 18:56:02 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b2bd5df4107bc3326be940291bf4aacb1a1de4760ca3315321bebf59195856`  
		Last Modified: Mon, 29 Aug 2022 18:56:03 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6-alpine3.16`

```console
$ docker pull memcached@sha256:c2f5df2c5099744a041132d1c11900d90f4b9e9c587a38ba8b12f9c03e82cfff
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
$ docker pull memcached@sha256:3b2a8f0dbcbb96b42edffa4959170c2486ddb2bef3de057f8ed71591348721c0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3891406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc6dc88eceeba2070ee6fe3c8c979afeaf5bf6d36e86d09d6457dd8432bb4c36`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:39 GMT
ADD file:b828bc14bc5ff03c8f7310fe0aed6ac5df19a393622d5d1d779a523234d07c0a in / 
# Tue, 09 Aug 2022 17:38:39 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:34:01 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 09 Aug 2022 18:34:02 GMT
RUN apk add --no-cache libsasl
# Mon, 29 Aug 2022 18:41:47 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 18:41:48 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 18:44:43 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Mon, 29 Aug 2022 18:44:45 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 18:44:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 18:44:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 18:44:47 GMT
USER memcache
# Mon, 29 Aug 2022 18:44:48 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 18:44:49 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6c0d3b419d848ea31ca748254611d5d5ce3b76e3d7bba520fd87400fbb75f3b9`  
		Last Modified: Tue, 09 Aug 2022 17:39:33 GMT  
		Size: 2.8 MB (2807121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240e236335200614c944d9ba79e2d7eda5cfa258a69e669b585cc28314d754f5`  
		Last Modified: Tue, 09 Aug 2022 18:38:05 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:844d1ba63a22190468423984b12b7d36f6c005e3316461b983f975f4b8dc9ee8`  
		Last Modified: Tue, 09 Aug 2022 18:38:05 GMT  
		Size: 119.8 KB (119826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2e7c344cfe47d96e7a9d170c9427c474246d16b76964c915cdd2f3d5e62698`  
		Last Modified: Mon, 29 Aug 2022 18:46:29 GMT  
		Size: 962.8 KB (962814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed467891e81f8057bb74046a7442a949b8f2ab27dc7099c321d77f2497584541`  
		Last Modified: Mon, 29 Aug 2022 18:46:29 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5326fe38fa94412c48f8bf0980206aed389413a089a646b582739edc31841a`  
		Last Modified: Mon, 29 Aug 2022 18:46:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine3.16` - linux; ppc64le

```console
$ docker pull memcached@sha256:79f15ab95c7dc52c17fab8ebc50e1a380b3584fd2127402ba0486ca4311be7df
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3913056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d80b3f9d28d32be6c7fdc9e706c4555e3bc835f495aed408fe264c0a8ed3d6a7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:48:17 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 09 Aug 2022 18:48:19 GMT
RUN apk add --no-cache libsasl
# Mon, 29 Aug 2022 19:23:01 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 19:23:02 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 19:26:15 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Mon, 29 Aug 2022 19:26:16 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 19:26:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 19:26:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 19:26:17 GMT
USER memcache
# Mon, 29 Aug 2022 19:26:18 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 19:26:18 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:086c869249c97411ce380e3b76305e0b85731874d0ea57dfd0de74e1f387443d`  
		Last Modified: Tue, 09 Aug 2022 18:52:28 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75e55886182590f2e7eef7f1c21851fd9c322339484e8345afd12376d976ddbd`  
		Last Modified: Tue, 09 Aug 2022 18:52:28 GMT  
		Size: 126.1 KB (126064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:794c752514ed274efa4c408cc26745be991e45f3bdf327ec010ef5d614a12e81`  
		Last Modified: Mon, 29 Aug 2022 19:27:39 GMT  
		Size: 982.0 KB (981999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1872e17927a44c66bc7cc1ab89e743c7ce518c421ab7dbec3b77da2ed55f1191`  
		Last Modified: Mon, 29 Aug 2022 19:27:38 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671ee1b68e567ecbfd0d99f4331f15d70a320c05193a577228fa8b911be55513`  
		Last Modified: Mon, 29 Aug 2022 19:27:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine3.16` - linux; s390x

```console
$ docker pull memcached@sha256:1aca14af5e45939b3b68973e8c599cb648d30771513ce390a9f0eef85c4f17ea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3646984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d704b926b5f988e9db5404831fa6b7a4f8da14a0a3593e225669ff5e99aa2d56`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 19:11:19 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 09 Aug 2022 19:11:20 GMT
RUN apk add --no-cache libsasl
# Mon, 29 Aug 2022 18:51:35 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 18:51:35 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 18:55:03 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Mon, 29 Aug 2022 18:55:03 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 18:55:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 18:55:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 18:55:04 GMT
USER memcache
# Mon, 29 Aug 2022 18:55:04 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 18:55:04 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463a70f3df946e83a223bd55002470af1b7f8d483babe452e515a809b965d35c`  
		Last Modified: Tue, 09 Aug 2022 19:15:35 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df0b8be6e73cbbdde959ca7a21d3fd6c8e36e05bc9c7a46be4e5bfa5b664a50c`  
		Last Modified: Tue, 09 Aug 2022 19:15:35 GMT  
		Size: 112.5 KB (112508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54547b52522c89500f1653dc849604a8a264e93fd45501c6ecc53b9b32824c31`  
		Last Modified: Mon, 29 Aug 2022 18:56:03 GMT  
		Size: 942.2 KB (942207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d838190f94a4d872ed0e972e293eafdda311d2d029f93f8c9fcffe960c8bc74`  
		Last Modified: Mon, 29 Aug 2022 18:56:02 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b2bd5df4107bc3326be940291bf4aacb1a1de4760ca3315321bebf59195856`  
		Last Modified: Mon, 29 Aug 2022 18:56:03 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6-bullseye`

```console
$ docker pull memcached@sha256:1917f1b4e48a69e5be80a57c321504338f9b65046386ea50ee679322413e26c7
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
$ docker pull memcached@sha256:2a9bf2539b24c553b92c876dfbe6dd48450a832f2b5395ec3217271018ad2ca0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32971284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92e1422c3edf80b790f0a601173b8e329b6619096d8cebb0b50b0f489ad1d971`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:54:26 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 23 Aug 2022 02:54:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 29 Aug 2022 19:57:00 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 19:57:01 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 19:59:41 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Mon, 29 Aug 2022 19:59:41 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 19:59:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 19:59:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 19:59:42 GMT
USER memcache
# Mon, 29 Aug 2022 19:59:42 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 19:59:42 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa73fb65ea8b12a2375459f0d656d3ad06e2863c906fcf962486eda3701f3fd6`  
		Last Modified: Tue, 23 Aug 2022 02:57:38 GMT  
		Size: 5.0 KB (4981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502b4e8803067b28098d0ea52281cfef66da1ee1e869241612b545d7e9ff12de`  
		Last Modified: Tue, 23 Aug 2022 02:57:38 GMT  
		Size: 328.1 KB (328108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b905db5d33a47882bd6cb4935bcc5d576d5cad5ba761b6b4004982c3aa7333`  
		Last Modified: Mon, 29 Aug 2022 20:03:05 GMT  
		Size: 1.3 MB (1256303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93643c661348540c2edcfc8a007b2c9aff33ac36cb9dcd910e0ddb51f50cd09e`  
		Last Modified: Mon, 29 Aug 2022 20:03:04 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc510e39dc783b83b00e5abd05d57df948435a0aaf45e87b131cc0fff83021e`  
		Last Modified: Mon, 29 Aug 2022 20:03:05 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bullseye` - linux; arm variant v5

```console
$ docker pull memcached@sha256:ef629e7153669e6100c98fba79336f87cc033d073c6219d6c7ec9360298a5d8e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30454536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84960478143b53154da0f3409e3f1141b62dabf4fe0c97c3661b5dd8a1c533ec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Sep 2022 00:53:30 GMT
ADD file:539e23f1c3a625a612a5a59b3939e9692c86c3cfa4956d30f4802c9f34ffa29c in / 
# Tue, 13 Sep 2022 00:53:31 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 03:18:14 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 13 Sep 2022 03:18:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 03:18:20 GMT
ENV MEMCACHED_VERSION=1.6.17
# Tue, 13 Sep 2022 03:18:20 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Tue, 13 Sep 2022 03:24:21 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 13 Sep 2022 03:24:22 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 13 Sep 2022 03:24:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Sep 2022 03:24:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Sep 2022 03:24:22 GMT
USER memcache
# Tue, 13 Sep 2022 03:24:22 GMT
EXPOSE 11211
# Tue, 13 Sep 2022 03:24:22 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:705abbab4fcb3a8dfe046a2ae6c450328aa11d93911abce66d3bba8bc693cbd4`  
		Last Modified: Tue, 13 Sep 2022 01:01:07 GMT  
		Size: 28.9 MB (28905288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eba43be24e48cc0796f0f5a17e6b674c0f07d5626f56ac8ed9f717cba0d0503`  
		Last Modified: Tue, 13 Sep 2022 03:24:59 GMT  
		Size: 4.9 KB (4894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c93e222cf0a02e2b4146a4d3ff6e5da33b929a10129fd88081a505e4011b9e`  
		Last Modified: Tue, 13 Sep 2022 03:25:00 GMT  
		Size: 316.6 KB (316638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b091f5c4cb7701e12cc29c82ee78e1704fdaaabcd851004efea8deb3acf7f2f`  
		Last Modified: Tue, 13 Sep 2022 03:25:00 GMT  
		Size: 1.2 MB (1227311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5e30653aa54ef905fcc6b97813278f8b54e56e889b1ffccf5101df4fa45882`  
		Last Modified: Tue, 13 Sep 2022 03:24:59 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471afe7d2cb0083a807b44b87fa581728a14e66fbada1f0ea0bcff34258f1cca`  
		Last Modified: Tue, 13 Sep 2022 03:24:59 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bullseye` - linux; arm variant v7

```console
$ docker pull memcached@sha256:960b71bacce5bbd2bf5c700ca3398d8ce00c1a9ebb35a5b690be486267128ef1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28088375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a54ccaf5bd1ba99327d598c288c19a655c2601e43aaf08c6429e99c287ab5b35`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 23 Aug 2022 01:43:01 GMT
ADD file:4cd1b4287674228db28402a76aa4f241740585448be48b5b15068d275ee9eb84 in / 
# Tue, 23 Aug 2022 01:43:01 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 18:03:50 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 23 Aug 2022 18:03:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 29 Aug 2022 19:04:31 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 19:04:31 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 19:09:39 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Mon, 29 Aug 2022 19:09:40 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 19:09:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 19:09:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 19:09:40 GMT
USER memcache
# Mon, 29 Aug 2022 19:09:40 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 19:09:40 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:051ba72559abd0cf65b34b75605580f58636ec3cb994f97de317632a85d82761`  
		Last Modified: Tue, 23 Aug 2022 01:50:05 GMT  
		Size: 26.6 MB (26571732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12dc4f2d8dca33e3850e55e4a2cd25a6dbf19afb27df3daef33de65ac91fd757`  
		Last Modified: Tue, 23 Aug 2022 21:10:42 GMT  
		Size: 4.9 KB (4893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:033f621bef4d3464e367d2c0ce45f3ec626c1c21f84ba7e84ece82bfbef4666e`  
		Last Modified: Tue, 23 Aug 2022 21:10:42 GMT  
		Size: 312.0 KB (312045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba873971d43c849095b8112993f9eb97b90c155f9f9f190da2bef761c9aa61a8`  
		Last Modified: Mon, 29 Aug 2022 19:26:29 GMT  
		Size: 1.2 MB (1199297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b256a2f081d1033d7ae503b0735b03640cd5b071e47fce65387238edf010a05c`  
		Last Modified: Mon, 29 Aug 2022 19:26:29 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a75e8764536efcd4e0fbd3d6c058eb6e05a0489f9e157f95e9e9ca0639c7d40b`  
		Last Modified: Mon, 29 Aug 2022 19:26:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bullseye` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:c67982406cd3e3fb90c50951d6a8cd766a4c0cc625ef035237913dfe56c0ae88
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31444531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02936ddd3c3f04b28ca0fbb9e803bfe5c3c1c0bda9ffe6ca0c6ea9954c351ab8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 13:12:07 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 23 Aug 2022 13:12:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 29 Aug 2022 18:48:57 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 18:48:58 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 18:51:30 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Mon, 29 Aug 2022 18:51:32 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 18:51:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 18:51:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 18:51:34 GMT
USER memcache
# Mon, 29 Aug 2022 18:51:35 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 18:51:36 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21794f0e498790afd69f2d317bbed8aa9cdbd3dddc56f7d52f1b806577e38a06`  
		Last Modified: Tue, 23 Aug 2022 13:15:43 GMT  
		Size: 4.9 KB (4904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:261db6d67ef285bdd84e6ae9e72182c4cd348b9f6c3c060c723764d03a12c2f6`  
		Last Modified: Tue, 23 Aug 2022 13:15:43 GMT  
		Size: 119.2 KB (119240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646e70d704c1f14afdd9de28cb4081703a4efc97e9c6a743ba80329c00705b37`  
		Last Modified: Mon, 29 Aug 2022 18:55:22 GMT  
		Size: 1.3 MB (1256190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db1c8f9c761c12c5c76962f55a2baff7f18d665a53fa76a2d3329fc2c0ccf313`  
		Last Modified: Mon, 29 Aug 2022 18:55:21 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4655eda4ba606249d810ba4d37deb1e82c106bcf3a2394f684a6ad8275d98950`  
		Last Modified: Mon, 29 Aug 2022 18:55:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bullseye` - linux; 386

```console
$ docker pull memcached@sha256:9a142ff1556091ea4d817d7ac5c26fcc6a0b2daa5bf99a56c64d19bb3e3cb866
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33776358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e0455947003534873a7c3f6d3bae27183601ae7c8b66f094e52d72450507327`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 23 Aug 2022 01:02:40 GMT
ADD file:5ca62c98116941aaa64ec72afb689a088c46f75a3e83d5b0d4e58d65ec905ccd in / 
# Tue, 23 Aug 2022 01:02:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:22:44 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 23 Aug 2022 03:22:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 29 Aug 2022 18:38:36 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 18:38:36 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 18:41:29 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Mon, 29 Aug 2022 18:41:31 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 18:41:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 18:41:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 18:41:33 GMT
USER memcache
# Mon, 29 Aug 2022 18:41:34 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 18:41:35 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6b3cb4a05a891d9d8a87a2bd7247b16f79832a9d4afbad3ff5068f6fc2ba1560`  
		Last Modified: Tue, 23 Aug 2022 01:08:25 GMT  
		Size: 32.4 MB (32387317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd24201e0b5e9a68a67bdc3b464a01aeb9a2e5a859a582cdaa80ab08a608337`  
		Last Modified: Tue, 23 Aug 2022 03:27:47 GMT  
		Size: 4.8 KB (4774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3070e5e3b1d98fa0b67b8390880b7596c4719b774864de21f36ed86873041793`  
		Last Modified: Tue, 23 Aug 2022 03:27:48 GMT  
		Size: 130.1 KB (130136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af8c1cee54f7ff86c820ca418aa3d2c05c5f200ca4d938ba76c8f8439b39cb04`  
		Last Modified: Mon, 29 Aug 2022 18:45:40 GMT  
		Size: 1.3 MB (1253721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94d7ae33ce7f8ea696d92c06ef6fd7c86c8228061b3b2485a78a9f59131a48aa`  
		Last Modified: Mon, 29 Aug 2022 18:45:43 GMT  
		Size: 289.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5348ed42ca0cf0c971fcaddc7677e8a3508548c0e3ca9e12b49cc06627f4657c`  
		Last Modified: Mon, 29 Aug 2022 18:45:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bullseye` - linux; mips64le

```console
$ docker pull memcached@sha256:e1403115858fda192fda48a365294d78dd1ea7fa6c9db3be737a883cb34fd9de
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31001916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ce2440650f197fcd6de50038d9a16d23be6db7efc79a8115173cc1ca5a769f5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Sep 2022 01:10:58 GMT
ADD file:91a8d8627a614ff3741d68216da46f13b393e52a70377b97ef317e4a00a3cac6 in / 
# Tue, 13 Sep 2022 01:11:02 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 04:50:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 13 Sep 2022 04:50:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 04:50:38 GMT
ENV MEMCACHED_VERSION=1.6.17
# Tue, 13 Sep 2022 04:50:40 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Tue, 13 Sep 2022 04:57:36 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 13 Sep 2022 04:57:38 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 13 Sep 2022 04:57:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Sep 2022 04:57:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Sep 2022 04:57:48 GMT
USER memcache
# Tue, 13 Sep 2022 04:57:50 GMT
EXPOSE 11211
# Tue, 13 Sep 2022 04:57:53 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:98abeb1446d0e9df6f48d5f72a70b36598cfc1091c9a5ca82690bedcf320e2b3`  
		Last Modified: Tue, 13 Sep 2022 01:18:50 GMT  
		Size: 29.6 MB (29627659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766602637141a485f59d0fc04aec4bfa1ac38583bba125b35c0b6809f1219ed9`  
		Last Modified: Tue, 13 Sep 2022 04:58:11 GMT  
		Size: 4.9 KB (4857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21b631e5bb3330fba3352d6332ae5cfa0b9a35dbc33b4d643b80f7b908c950f5`  
		Last Modified: Tue, 13 Sep 2022 04:58:11 GMT  
		Size: 117.2 KB (117159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee33141b788356ead96c93190f0008f455371a4562d92b27a20945aac60d1361`  
		Last Modified: Tue, 13 Sep 2022 04:58:12 GMT  
		Size: 1.3 MB (1251835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e488d322d0c180f442d31923e23e79064b584ac59e2cadf3be31cc702751460d`  
		Last Modified: Tue, 13 Sep 2022 04:58:11 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec80c89f379732f5466f55915bbad33a4b55dc651bf6346712c92cff64717b11`  
		Last Modified: Tue, 13 Sep 2022 04:58:11 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bullseye` - linux; ppc64le

```console
$ docker pull memcached@sha256:0176bec998e05785ddcaadb9c692b14571e10c2b71050a9988329f903660369b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36970738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7a0216731101d94583b08e4b42f59092a78019783e49a2ddb6401ea59c9d47d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 23 Aug 2022 01:24:52 GMT
ADD file:d35213360d726a18e220276d33f245115c3e94a321addaa4c9127488368b0203 in / 
# Tue, 23 Aug 2022 01:24:54 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:34:49 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 23 Aug 2022 02:34:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 29 Aug 2022 19:19:51 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 19:19:51 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 19:22:46 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Mon, 29 Aug 2022 19:22:47 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 19:22:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 19:22:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 19:22:48 GMT
USER memcache
# Mon, 29 Aug 2022 19:22:49 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 19:22:49 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:698954eda09d38dd1ccc9ce777b1f6bc7f7473fc6c4c3eb634acc8d035a42eae`  
		Last Modified: Tue, 23 Aug 2022 01:30:36 GMT  
		Size: 35.3 MB (35284280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffb080d920662043edc67113c0de4c68258ad19c0fffd9e3b79fa01800c6015`  
		Last Modified: Tue, 23 Aug 2022 02:39:09 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b1f66b68991d8f5ab064b3988db37a48b8f28b4ef0eb8e83efa4c419b630ff`  
		Last Modified: Tue, 23 Aug 2022 02:39:09 GMT  
		Size: 356.9 KB (356931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2256c5b8427744c7563d1151efbeb03c935fbb3e87d621903c9e7476a8db7494`  
		Last Modified: Mon, 29 Aug 2022 19:27:05 GMT  
		Size: 1.3 MB (1324139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee6919a18fb52b4b8259e2942d1d56ca42a4371f735bedd875c5eebdaee214a2`  
		Last Modified: Mon, 29 Aug 2022 19:27:04 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ac3c74fbd1e874bdc7163ccf1ba8bf496b085875b4165fcec2e4a771d9742f9`  
		Last Modified: Mon, 29 Aug 2022 19:27:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bullseye` - linux; s390x

```console
$ docker pull memcached@sha256:f063181874bf86b26f7e8d033e02792331b3282ef6614aa99d8d70c8b178aac0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31206151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c2827f7c0c4acdb1d09c90d24a8e27f37bd489dca825a2831b3f923831b1125`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Sep 2022 00:48:07 GMT
ADD file:e8a6c2e8be5d9d1f83c1e280419014489438391a9feb7c77b6c21adbf0ec062b in / 
# Tue, 13 Sep 2022 00:48:08 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 01:59:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 13 Sep 2022 01:59:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 01:59:22 GMT
ENV MEMCACHED_VERSION=1.6.17
# Tue, 13 Sep 2022 01:59:23 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Tue, 13 Sep 2022 02:02:36 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 13 Sep 2022 02:02:36 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 13 Sep 2022 02:02:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Sep 2022 02:02:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Sep 2022 02:02:37 GMT
USER memcache
# Tue, 13 Sep 2022 02:02:37 GMT
EXPOSE 11211
# Tue, 13 Sep 2022 02:02:37 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c64715e5ebd39975a39b5cf2535772544c27713cbed678b0a21e73680fffaf72`  
		Last Modified: Tue, 13 Sep 2022 00:52:39 GMT  
		Size: 29.6 MB (29635080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce5055aafbfbe726c8840111d8300b0c75f707a8ab517395bb8be985d2feb009`  
		Last Modified: Tue, 13 Sep 2022 02:03:36 GMT  
		Size: 5.0 KB (5021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9a227f323eed41d16b462d95503000badd5210aa179dd3065f4363fe3a1b9f`  
		Last Modified: Tue, 13 Sep 2022 02:03:36 GMT  
		Size: 324.2 KB (324172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36fb60d78f8bd69265b4c2d2246169797772da4584f6e063d49eab9c2f040c51`  
		Last Modified: Tue, 13 Sep 2022 02:03:36 GMT  
		Size: 1.2 MB (1241470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d23a9497c5fd3ec0d26f920c59f1f1628999ae546bd1b2f722b29fbf27e3402`  
		Last Modified: Tue, 13 Sep 2022 02:03:36 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009331f552a168c5b26209994b10c7684fc80fe6348a406878b2262037e82435`  
		Last Modified: Tue, 13 Sep 2022 02:03:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.17`

```console
$ docker pull memcached@sha256:1917f1b4e48a69e5be80a57c321504338f9b65046386ea50ee679322413e26c7
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
$ docker pull memcached@sha256:2a9bf2539b24c553b92c876dfbe6dd48450a832f2b5395ec3217271018ad2ca0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32971284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92e1422c3edf80b790f0a601173b8e329b6619096d8cebb0b50b0f489ad1d971`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:54:26 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 23 Aug 2022 02:54:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 29 Aug 2022 19:57:00 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 19:57:01 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 19:59:41 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Mon, 29 Aug 2022 19:59:41 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 19:59:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 19:59:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 19:59:42 GMT
USER memcache
# Mon, 29 Aug 2022 19:59:42 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 19:59:42 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa73fb65ea8b12a2375459f0d656d3ad06e2863c906fcf962486eda3701f3fd6`  
		Last Modified: Tue, 23 Aug 2022 02:57:38 GMT  
		Size: 5.0 KB (4981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502b4e8803067b28098d0ea52281cfef66da1ee1e869241612b545d7e9ff12de`  
		Last Modified: Tue, 23 Aug 2022 02:57:38 GMT  
		Size: 328.1 KB (328108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b905db5d33a47882bd6cb4935bcc5d576d5cad5ba761b6b4004982c3aa7333`  
		Last Modified: Mon, 29 Aug 2022 20:03:05 GMT  
		Size: 1.3 MB (1256303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93643c661348540c2edcfc8a007b2c9aff33ac36cb9dcd910e0ddb51f50cd09e`  
		Last Modified: Mon, 29 Aug 2022 20:03:04 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc510e39dc783b83b00e5abd05d57df948435a0aaf45e87b131cc0fff83021e`  
		Last Modified: Mon, 29 Aug 2022 20:03:05 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.17` - linux; arm variant v5

```console
$ docker pull memcached@sha256:ef629e7153669e6100c98fba79336f87cc033d073c6219d6c7ec9360298a5d8e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30454536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84960478143b53154da0f3409e3f1141b62dabf4fe0c97c3661b5dd8a1c533ec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Sep 2022 00:53:30 GMT
ADD file:539e23f1c3a625a612a5a59b3939e9692c86c3cfa4956d30f4802c9f34ffa29c in / 
# Tue, 13 Sep 2022 00:53:31 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 03:18:14 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 13 Sep 2022 03:18:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 03:18:20 GMT
ENV MEMCACHED_VERSION=1.6.17
# Tue, 13 Sep 2022 03:18:20 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Tue, 13 Sep 2022 03:24:21 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 13 Sep 2022 03:24:22 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 13 Sep 2022 03:24:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Sep 2022 03:24:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Sep 2022 03:24:22 GMT
USER memcache
# Tue, 13 Sep 2022 03:24:22 GMT
EXPOSE 11211
# Tue, 13 Sep 2022 03:24:22 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:705abbab4fcb3a8dfe046a2ae6c450328aa11d93911abce66d3bba8bc693cbd4`  
		Last Modified: Tue, 13 Sep 2022 01:01:07 GMT  
		Size: 28.9 MB (28905288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eba43be24e48cc0796f0f5a17e6b674c0f07d5626f56ac8ed9f717cba0d0503`  
		Last Modified: Tue, 13 Sep 2022 03:24:59 GMT  
		Size: 4.9 KB (4894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c93e222cf0a02e2b4146a4d3ff6e5da33b929a10129fd88081a505e4011b9e`  
		Last Modified: Tue, 13 Sep 2022 03:25:00 GMT  
		Size: 316.6 KB (316638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b091f5c4cb7701e12cc29c82ee78e1704fdaaabcd851004efea8deb3acf7f2f`  
		Last Modified: Tue, 13 Sep 2022 03:25:00 GMT  
		Size: 1.2 MB (1227311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5e30653aa54ef905fcc6b97813278f8b54e56e889b1ffccf5101df4fa45882`  
		Last Modified: Tue, 13 Sep 2022 03:24:59 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471afe7d2cb0083a807b44b87fa581728a14e66fbada1f0ea0bcff34258f1cca`  
		Last Modified: Tue, 13 Sep 2022 03:24:59 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.17` - linux; arm variant v7

```console
$ docker pull memcached@sha256:960b71bacce5bbd2bf5c700ca3398d8ce00c1a9ebb35a5b690be486267128ef1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28088375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a54ccaf5bd1ba99327d598c288c19a655c2601e43aaf08c6429e99c287ab5b35`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 23 Aug 2022 01:43:01 GMT
ADD file:4cd1b4287674228db28402a76aa4f241740585448be48b5b15068d275ee9eb84 in / 
# Tue, 23 Aug 2022 01:43:01 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 18:03:50 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 23 Aug 2022 18:03:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 29 Aug 2022 19:04:31 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 19:04:31 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 19:09:39 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Mon, 29 Aug 2022 19:09:40 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 19:09:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 19:09:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 19:09:40 GMT
USER memcache
# Mon, 29 Aug 2022 19:09:40 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 19:09:40 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:051ba72559abd0cf65b34b75605580f58636ec3cb994f97de317632a85d82761`  
		Last Modified: Tue, 23 Aug 2022 01:50:05 GMT  
		Size: 26.6 MB (26571732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12dc4f2d8dca33e3850e55e4a2cd25a6dbf19afb27df3daef33de65ac91fd757`  
		Last Modified: Tue, 23 Aug 2022 21:10:42 GMT  
		Size: 4.9 KB (4893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:033f621bef4d3464e367d2c0ce45f3ec626c1c21f84ba7e84ece82bfbef4666e`  
		Last Modified: Tue, 23 Aug 2022 21:10:42 GMT  
		Size: 312.0 KB (312045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba873971d43c849095b8112993f9eb97b90c155f9f9f190da2bef761c9aa61a8`  
		Last Modified: Mon, 29 Aug 2022 19:26:29 GMT  
		Size: 1.2 MB (1199297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b256a2f081d1033d7ae503b0735b03640cd5b071e47fce65387238edf010a05c`  
		Last Modified: Mon, 29 Aug 2022 19:26:29 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a75e8764536efcd4e0fbd3d6c058eb6e05a0489f9e157f95e9e9ca0639c7d40b`  
		Last Modified: Mon, 29 Aug 2022 19:26:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.17` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:c67982406cd3e3fb90c50951d6a8cd766a4c0cc625ef035237913dfe56c0ae88
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31444531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02936ddd3c3f04b28ca0fbb9e803bfe5c3c1c0bda9ffe6ca0c6ea9954c351ab8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 13:12:07 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 23 Aug 2022 13:12:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 29 Aug 2022 18:48:57 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 18:48:58 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 18:51:30 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Mon, 29 Aug 2022 18:51:32 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 18:51:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 18:51:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 18:51:34 GMT
USER memcache
# Mon, 29 Aug 2022 18:51:35 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 18:51:36 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21794f0e498790afd69f2d317bbed8aa9cdbd3dddc56f7d52f1b806577e38a06`  
		Last Modified: Tue, 23 Aug 2022 13:15:43 GMT  
		Size: 4.9 KB (4904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:261db6d67ef285bdd84e6ae9e72182c4cd348b9f6c3c060c723764d03a12c2f6`  
		Last Modified: Tue, 23 Aug 2022 13:15:43 GMT  
		Size: 119.2 KB (119240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646e70d704c1f14afdd9de28cb4081703a4efc97e9c6a743ba80329c00705b37`  
		Last Modified: Mon, 29 Aug 2022 18:55:22 GMT  
		Size: 1.3 MB (1256190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db1c8f9c761c12c5c76962f55a2baff7f18d665a53fa76a2d3329fc2c0ccf313`  
		Last Modified: Mon, 29 Aug 2022 18:55:21 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4655eda4ba606249d810ba4d37deb1e82c106bcf3a2394f684a6ad8275d98950`  
		Last Modified: Mon, 29 Aug 2022 18:55:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.17` - linux; 386

```console
$ docker pull memcached@sha256:9a142ff1556091ea4d817d7ac5c26fcc6a0b2daa5bf99a56c64d19bb3e3cb866
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33776358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e0455947003534873a7c3f6d3bae27183601ae7c8b66f094e52d72450507327`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 23 Aug 2022 01:02:40 GMT
ADD file:5ca62c98116941aaa64ec72afb689a088c46f75a3e83d5b0d4e58d65ec905ccd in / 
# Tue, 23 Aug 2022 01:02:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:22:44 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 23 Aug 2022 03:22:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 29 Aug 2022 18:38:36 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 18:38:36 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 18:41:29 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Mon, 29 Aug 2022 18:41:31 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 18:41:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 18:41:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 18:41:33 GMT
USER memcache
# Mon, 29 Aug 2022 18:41:34 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 18:41:35 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6b3cb4a05a891d9d8a87a2bd7247b16f79832a9d4afbad3ff5068f6fc2ba1560`  
		Last Modified: Tue, 23 Aug 2022 01:08:25 GMT  
		Size: 32.4 MB (32387317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd24201e0b5e9a68a67bdc3b464a01aeb9a2e5a859a582cdaa80ab08a608337`  
		Last Modified: Tue, 23 Aug 2022 03:27:47 GMT  
		Size: 4.8 KB (4774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3070e5e3b1d98fa0b67b8390880b7596c4719b774864de21f36ed86873041793`  
		Last Modified: Tue, 23 Aug 2022 03:27:48 GMT  
		Size: 130.1 KB (130136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af8c1cee54f7ff86c820ca418aa3d2c05c5f200ca4d938ba76c8f8439b39cb04`  
		Last Modified: Mon, 29 Aug 2022 18:45:40 GMT  
		Size: 1.3 MB (1253721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94d7ae33ce7f8ea696d92c06ef6fd7c86c8228061b3b2485a78a9f59131a48aa`  
		Last Modified: Mon, 29 Aug 2022 18:45:43 GMT  
		Size: 289.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5348ed42ca0cf0c971fcaddc7677e8a3508548c0e3ca9e12b49cc06627f4657c`  
		Last Modified: Mon, 29 Aug 2022 18:45:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.17` - linux; mips64le

```console
$ docker pull memcached@sha256:e1403115858fda192fda48a365294d78dd1ea7fa6c9db3be737a883cb34fd9de
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31001916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ce2440650f197fcd6de50038d9a16d23be6db7efc79a8115173cc1ca5a769f5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Sep 2022 01:10:58 GMT
ADD file:91a8d8627a614ff3741d68216da46f13b393e52a70377b97ef317e4a00a3cac6 in / 
# Tue, 13 Sep 2022 01:11:02 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 04:50:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 13 Sep 2022 04:50:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 04:50:38 GMT
ENV MEMCACHED_VERSION=1.6.17
# Tue, 13 Sep 2022 04:50:40 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Tue, 13 Sep 2022 04:57:36 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 13 Sep 2022 04:57:38 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 13 Sep 2022 04:57:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Sep 2022 04:57:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Sep 2022 04:57:48 GMT
USER memcache
# Tue, 13 Sep 2022 04:57:50 GMT
EXPOSE 11211
# Tue, 13 Sep 2022 04:57:53 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:98abeb1446d0e9df6f48d5f72a70b36598cfc1091c9a5ca82690bedcf320e2b3`  
		Last Modified: Tue, 13 Sep 2022 01:18:50 GMT  
		Size: 29.6 MB (29627659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766602637141a485f59d0fc04aec4bfa1ac38583bba125b35c0b6809f1219ed9`  
		Last Modified: Tue, 13 Sep 2022 04:58:11 GMT  
		Size: 4.9 KB (4857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21b631e5bb3330fba3352d6332ae5cfa0b9a35dbc33b4d643b80f7b908c950f5`  
		Last Modified: Tue, 13 Sep 2022 04:58:11 GMT  
		Size: 117.2 KB (117159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee33141b788356ead96c93190f0008f455371a4562d92b27a20945aac60d1361`  
		Last Modified: Tue, 13 Sep 2022 04:58:12 GMT  
		Size: 1.3 MB (1251835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e488d322d0c180f442d31923e23e79064b584ac59e2cadf3be31cc702751460d`  
		Last Modified: Tue, 13 Sep 2022 04:58:11 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec80c89f379732f5466f55915bbad33a4b55dc651bf6346712c92cff64717b11`  
		Last Modified: Tue, 13 Sep 2022 04:58:11 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.17` - linux; ppc64le

```console
$ docker pull memcached@sha256:0176bec998e05785ddcaadb9c692b14571e10c2b71050a9988329f903660369b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36970738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7a0216731101d94583b08e4b42f59092a78019783e49a2ddb6401ea59c9d47d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 23 Aug 2022 01:24:52 GMT
ADD file:d35213360d726a18e220276d33f245115c3e94a321addaa4c9127488368b0203 in / 
# Tue, 23 Aug 2022 01:24:54 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:34:49 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 23 Aug 2022 02:34:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 29 Aug 2022 19:19:51 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 19:19:51 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 19:22:46 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Mon, 29 Aug 2022 19:22:47 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 19:22:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 19:22:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 19:22:48 GMT
USER memcache
# Mon, 29 Aug 2022 19:22:49 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 19:22:49 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:698954eda09d38dd1ccc9ce777b1f6bc7f7473fc6c4c3eb634acc8d035a42eae`  
		Last Modified: Tue, 23 Aug 2022 01:30:36 GMT  
		Size: 35.3 MB (35284280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffb080d920662043edc67113c0de4c68258ad19c0fffd9e3b79fa01800c6015`  
		Last Modified: Tue, 23 Aug 2022 02:39:09 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b1f66b68991d8f5ab064b3988db37a48b8f28b4ef0eb8e83efa4c419b630ff`  
		Last Modified: Tue, 23 Aug 2022 02:39:09 GMT  
		Size: 356.9 KB (356931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2256c5b8427744c7563d1151efbeb03c935fbb3e87d621903c9e7476a8db7494`  
		Last Modified: Mon, 29 Aug 2022 19:27:05 GMT  
		Size: 1.3 MB (1324139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee6919a18fb52b4b8259e2942d1d56ca42a4371f735bedd875c5eebdaee214a2`  
		Last Modified: Mon, 29 Aug 2022 19:27:04 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ac3c74fbd1e874bdc7163ccf1ba8bf496b085875b4165fcec2e4a771d9742f9`  
		Last Modified: Mon, 29 Aug 2022 19:27:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.17` - linux; s390x

```console
$ docker pull memcached@sha256:f063181874bf86b26f7e8d033e02792331b3282ef6614aa99d8d70c8b178aac0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31206151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c2827f7c0c4acdb1d09c90d24a8e27f37bd489dca825a2831b3f923831b1125`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Sep 2022 00:48:07 GMT
ADD file:e8a6c2e8be5d9d1f83c1e280419014489438391a9feb7c77b6c21adbf0ec062b in / 
# Tue, 13 Sep 2022 00:48:08 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 01:59:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 13 Sep 2022 01:59:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 01:59:22 GMT
ENV MEMCACHED_VERSION=1.6.17
# Tue, 13 Sep 2022 01:59:23 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Tue, 13 Sep 2022 02:02:36 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 13 Sep 2022 02:02:36 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 13 Sep 2022 02:02:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Sep 2022 02:02:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Sep 2022 02:02:37 GMT
USER memcache
# Tue, 13 Sep 2022 02:02:37 GMT
EXPOSE 11211
# Tue, 13 Sep 2022 02:02:37 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c64715e5ebd39975a39b5cf2535772544c27713cbed678b0a21e73680fffaf72`  
		Last Modified: Tue, 13 Sep 2022 00:52:39 GMT  
		Size: 29.6 MB (29635080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce5055aafbfbe726c8840111d8300b0c75f707a8ab517395bb8be985d2feb009`  
		Last Modified: Tue, 13 Sep 2022 02:03:36 GMT  
		Size: 5.0 KB (5021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9a227f323eed41d16b462d95503000badd5210aa179dd3065f4363fe3a1b9f`  
		Last Modified: Tue, 13 Sep 2022 02:03:36 GMT  
		Size: 324.2 KB (324172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36fb60d78f8bd69265b4c2d2246169797772da4584f6e063d49eab9c2f040c51`  
		Last Modified: Tue, 13 Sep 2022 02:03:36 GMT  
		Size: 1.2 MB (1241470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d23a9497c5fd3ec0d26f920c59f1f1628999ae546bd1b2f722b29fbf27e3402`  
		Last Modified: Tue, 13 Sep 2022 02:03:36 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009331f552a168c5b26209994b10c7684fc80fe6348a406878b2262037e82435`  
		Last Modified: Tue, 13 Sep 2022 02:03:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.17-alpine`

```console
$ docker pull memcached@sha256:c2f5df2c5099744a041132d1c11900d90f4b9e9c587a38ba8b12f9c03e82cfff
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
$ docker pull memcached@sha256:3b2a8f0dbcbb96b42edffa4959170c2486ddb2bef3de057f8ed71591348721c0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3891406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc6dc88eceeba2070ee6fe3c8c979afeaf5bf6d36e86d09d6457dd8432bb4c36`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:39 GMT
ADD file:b828bc14bc5ff03c8f7310fe0aed6ac5df19a393622d5d1d779a523234d07c0a in / 
# Tue, 09 Aug 2022 17:38:39 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:34:01 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 09 Aug 2022 18:34:02 GMT
RUN apk add --no-cache libsasl
# Mon, 29 Aug 2022 18:41:47 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 18:41:48 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 18:44:43 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Mon, 29 Aug 2022 18:44:45 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 18:44:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 18:44:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 18:44:47 GMT
USER memcache
# Mon, 29 Aug 2022 18:44:48 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 18:44:49 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6c0d3b419d848ea31ca748254611d5d5ce3b76e3d7bba520fd87400fbb75f3b9`  
		Last Modified: Tue, 09 Aug 2022 17:39:33 GMT  
		Size: 2.8 MB (2807121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240e236335200614c944d9ba79e2d7eda5cfa258a69e669b585cc28314d754f5`  
		Last Modified: Tue, 09 Aug 2022 18:38:05 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:844d1ba63a22190468423984b12b7d36f6c005e3316461b983f975f4b8dc9ee8`  
		Last Modified: Tue, 09 Aug 2022 18:38:05 GMT  
		Size: 119.8 KB (119826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2e7c344cfe47d96e7a9d170c9427c474246d16b76964c915cdd2f3d5e62698`  
		Last Modified: Mon, 29 Aug 2022 18:46:29 GMT  
		Size: 962.8 KB (962814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed467891e81f8057bb74046a7442a949b8f2ab27dc7099c321d77f2497584541`  
		Last Modified: Mon, 29 Aug 2022 18:46:29 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5326fe38fa94412c48f8bf0980206aed389413a089a646b582739edc31841a`  
		Last Modified: Mon, 29 Aug 2022 18:46:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.17-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:79f15ab95c7dc52c17fab8ebc50e1a380b3584fd2127402ba0486ca4311be7df
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3913056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d80b3f9d28d32be6c7fdc9e706c4555e3bc835f495aed408fe264c0a8ed3d6a7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:48:17 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 09 Aug 2022 18:48:19 GMT
RUN apk add --no-cache libsasl
# Mon, 29 Aug 2022 19:23:01 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 19:23:02 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 19:26:15 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Mon, 29 Aug 2022 19:26:16 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 19:26:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 19:26:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 19:26:17 GMT
USER memcache
# Mon, 29 Aug 2022 19:26:18 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 19:26:18 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:086c869249c97411ce380e3b76305e0b85731874d0ea57dfd0de74e1f387443d`  
		Last Modified: Tue, 09 Aug 2022 18:52:28 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75e55886182590f2e7eef7f1c21851fd9c322339484e8345afd12376d976ddbd`  
		Last Modified: Tue, 09 Aug 2022 18:52:28 GMT  
		Size: 126.1 KB (126064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:794c752514ed274efa4c408cc26745be991e45f3bdf327ec010ef5d614a12e81`  
		Last Modified: Mon, 29 Aug 2022 19:27:39 GMT  
		Size: 982.0 KB (981999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1872e17927a44c66bc7cc1ab89e743c7ce518c421ab7dbec3b77da2ed55f1191`  
		Last Modified: Mon, 29 Aug 2022 19:27:38 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671ee1b68e567ecbfd0d99f4331f15d70a320c05193a577228fa8b911be55513`  
		Last Modified: Mon, 29 Aug 2022 19:27:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.17-alpine` - linux; s390x

```console
$ docker pull memcached@sha256:1aca14af5e45939b3b68973e8c599cb648d30771513ce390a9f0eef85c4f17ea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3646984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d704b926b5f988e9db5404831fa6b7a4f8da14a0a3593e225669ff5e99aa2d56`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 19:11:19 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 09 Aug 2022 19:11:20 GMT
RUN apk add --no-cache libsasl
# Mon, 29 Aug 2022 18:51:35 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 18:51:35 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 18:55:03 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Mon, 29 Aug 2022 18:55:03 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 18:55:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 18:55:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 18:55:04 GMT
USER memcache
# Mon, 29 Aug 2022 18:55:04 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 18:55:04 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463a70f3df946e83a223bd55002470af1b7f8d483babe452e515a809b965d35c`  
		Last Modified: Tue, 09 Aug 2022 19:15:35 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df0b8be6e73cbbdde959ca7a21d3fd6c8e36e05bc9c7a46be4e5bfa5b664a50c`  
		Last Modified: Tue, 09 Aug 2022 19:15:35 GMT  
		Size: 112.5 KB (112508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54547b52522c89500f1653dc849604a8a264e93fd45501c6ecc53b9b32824c31`  
		Last Modified: Mon, 29 Aug 2022 18:56:03 GMT  
		Size: 942.2 KB (942207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d838190f94a4d872ed0e972e293eafdda311d2d029f93f8c9fcffe960c8bc74`  
		Last Modified: Mon, 29 Aug 2022 18:56:02 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b2bd5df4107bc3326be940291bf4aacb1a1de4760ca3315321bebf59195856`  
		Last Modified: Mon, 29 Aug 2022 18:56:03 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.17-alpine3.16`

```console
$ docker pull memcached@sha256:c2f5df2c5099744a041132d1c11900d90f4b9e9c587a38ba8b12f9c03e82cfff
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
$ docker pull memcached@sha256:3b2a8f0dbcbb96b42edffa4959170c2486ddb2bef3de057f8ed71591348721c0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3891406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc6dc88eceeba2070ee6fe3c8c979afeaf5bf6d36e86d09d6457dd8432bb4c36`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:39 GMT
ADD file:b828bc14bc5ff03c8f7310fe0aed6ac5df19a393622d5d1d779a523234d07c0a in / 
# Tue, 09 Aug 2022 17:38:39 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:34:01 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 09 Aug 2022 18:34:02 GMT
RUN apk add --no-cache libsasl
# Mon, 29 Aug 2022 18:41:47 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 18:41:48 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 18:44:43 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Mon, 29 Aug 2022 18:44:45 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 18:44:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 18:44:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 18:44:47 GMT
USER memcache
# Mon, 29 Aug 2022 18:44:48 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 18:44:49 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6c0d3b419d848ea31ca748254611d5d5ce3b76e3d7bba520fd87400fbb75f3b9`  
		Last Modified: Tue, 09 Aug 2022 17:39:33 GMT  
		Size: 2.8 MB (2807121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240e236335200614c944d9ba79e2d7eda5cfa258a69e669b585cc28314d754f5`  
		Last Modified: Tue, 09 Aug 2022 18:38:05 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:844d1ba63a22190468423984b12b7d36f6c005e3316461b983f975f4b8dc9ee8`  
		Last Modified: Tue, 09 Aug 2022 18:38:05 GMT  
		Size: 119.8 KB (119826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2e7c344cfe47d96e7a9d170c9427c474246d16b76964c915cdd2f3d5e62698`  
		Last Modified: Mon, 29 Aug 2022 18:46:29 GMT  
		Size: 962.8 KB (962814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed467891e81f8057bb74046a7442a949b8f2ab27dc7099c321d77f2497584541`  
		Last Modified: Mon, 29 Aug 2022 18:46:29 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5326fe38fa94412c48f8bf0980206aed389413a089a646b582739edc31841a`  
		Last Modified: Mon, 29 Aug 2022 18:46:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.17-alpine3.16` - linux; ppc64le

```console
$ docker pull memcached@sha256:79f15ab95c7dc52c17fab8ebc50e1a380b3584fd2127402ba0486ca4311be7df
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3913056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d80b3f9d28d32be6c7fdc9e706c4555e3bc835f495aed408fe264c0a8ed3d6a7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:48:17 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 09 Aug 2022 18:48:19 GMT
RUN apk add --no-cache libsasl
# Mon, 29 Aug 2022 19:23:01 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 19:23:02 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 19:26:15 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Mon, 29 Aug 2022 19:26:16 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 19:26:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 19:26:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 19:26:17 GMT
USER memcache
# Mon, 29 Aug 2022 19:26:18 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 19:26:18 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:086c869249c97411ce380e3b76305e0b85731874d0ea57dfd0de74e1f387443d`  
		Last Modified: Tue, 09 Aug 2022 18:52:28 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75e55886182590f2e7eef7f1c21851fd9c322339484e8345afd12376d976ddbd`  
		Last Modified: Tue, 09 Aug 2022 18:52:28 GMT  
		Size: 126.1 KB (126064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:794c752514ed274efa4c408cc26745be991e45f3bdf327ec010ef5d614a12e81`  
		Last Modified: Mon, 29 Aug 2022 19:27:39 GMT  
		Size: 982.0 KB (981999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1872e17927a44c66bc7cc1ab89e743c7ce518c421ab7dbec3b77da2ed55f1191`  
		Last Modified: Mon, 29 Aug 2022 19:27:38 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671ee1b68e567ecbfd0d99f4331f15d70a320c05193a577228fa8b911be55513`  
		Last Modified: Mon, 29 Aug 2022 19:27:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.17-alpine3.16` - linux; s390x

```console
$ docker pull memcached@sha256:1aca14af5e45939b3b68973e8c599cb648d30771513ce390a9f0eef85c4f17ea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3646984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d704b926b5f988e9db5404831fa6b7a4f8da14a0a3593e225669ff5e99aa2d56`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 19:11:19 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 09 Aug 2022 19:11:20 GMT
RUN apk add --no-cache libsasl
# Mon, 29 Aug 2022 18:51:35 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 18:51:35 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 18:55:03 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Mon, 29 Aug 2022 18:55:03 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 18:55:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 18:55:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 18:55:04 GMT
USER memcache
# Mon, 29 Aug 2022 18:55:04 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 18:55:04 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463a70f3df946e83a223bd55002470af1b7f8d483babe452e515a809b965d35c`  
		Last Modified: Tue, 09 Aug 2022 19:15:35 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df0b8be6e73cbbdde959ca7a21d3fd6c8e36e05bc9c7a46be4e5bfa5b664a50c`  
		Last Modified: Tue, 09 Aug 2022 19:15:35 GMT  
		Size: 112.5 KB (112508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54547b52522c89500f1653dc849604a8a264e93fd45501c6ecc53b9b32824c31`  
		Last Modified: Mon, 29 Aug 2022 18:56:03 GMT  
		Size: 942.2 KB (942207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d838190f94a4d872ed0e972e293eafdda311d2d029f93f8c9fcffe960c8bc74`  
		Last Modified: Mon, 29 Aug 2022 18:56:02 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b2bd5df4107bc3326be940291bf4aacb1a1de4760ca3315321bebf59195856`  
		Last Modified: Mon, 29 Aug 2022 18:56:03 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.17-bullseye`

```console
$ docker pull memcached@sha256:1917f1b4e48a69e5be80a57c321504338f9b65046386ea50ee679322413e26c7
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
$ docker pull memcached@sha256:2a9bf2539b24c553b92c876dfbe6dd48450a832f2b5395ec3217271018ad2ca0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32971284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92e1422c3edf80b790f0a601173b8e329b6619096d8cebb0b50b0f489ad1d971`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:54:26 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 23 Aug 2022 02:54:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 29 Aug 2022 19:57:00 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 19:57:01 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 19:59:41 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Mon, 29 Aug 2022 19:59:41 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 19:59:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 19:59:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 19:59:42 GMT
USER memcache
# Mon, 29 Aug 2022 19:59:42 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 19:59:42 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa73fb65ea8b12a2375459f0d656d3ad06e2863c906fcf962486eda3701f3fd6`  
		Last Modified: Tue, 23 Aug 2022 02:57:38 GMT  
		Size: 5.0 KB (4981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502b4e8803067b28098d0ea52281cfef66da1ee1e869241612b545d7e9ff12de`  
		Last Modified: Tue, 23 Aug 2022 02:57:38 GMT  
		Size: 328.1 KB (328108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b905db5d33a47882bd6cb4935bcc5d576d5cad5ba761b6b4004982c3aa7333`  
		Last Modified: Mon, 29 Aug 2022 20:03:05 GMT  
		Size: 1.3 MB (1256303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93643c661348540c2edcfc8a007b2c9aff33ac36cb9dcd910e0ddb51f50cd09e`  
		Last Modified: Mon, 29 Aug 2022 20:03:04 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc510e39dc783b83b00e5abd05d57df948435a0aaf45e87b131cc0fff83021e`  
		Last Modified: Mon, 29 Aug 2022 20:03:05 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.17-bullseye` - linux; arm variant v5

```console
$ docker pull memcached@sha256:ef629e7153669e6100c98fba79336f87cc033d073c6219d6c7ec9360298a5d8e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30454536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84960478143b53154da0f3409e3f1141b62dabf4fe0c97c3661b5dd8a1c533ec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Sep 2022 00:53:30 GMT
ADD file:539e23f1c3a625a612a5a59b3939e9692c86c3cfa4956d30f4802c9f34ffa29c in / 
# Tue, 13 Sep 2022 00:53:31 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 03:18:14 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 13 Sep 2022 03:18:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 03:18:20 GMT
ENV MEMCACHED_VERSION=1.6.17
# Tue, 13 Sep 2022 03:18:20 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Tue, 13 Sep 2022 03:24:21 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 13 Sep 2022 03:24:22 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 13 Sep 2022 03:24:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Sep 2022 03:24:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Sep 2022 03:24:22 GMT
USER memcache
# Tue, 13 Sep 2022 03:24:22 GMT
EXPOSE 11211
# Tue, 13 Sep 2022 03:24:22 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:705abbab4fcb3a8dfe046a2ae6c450328aa11d93911abce66d3bba8bc693cbd4`  
		Last Modified: Tue, 13 Sep 2022 01:01:07 GMT  
		Size: 28.9 MB (28905288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eba43be24e48cc0796f0f5a17e6b674c0f07d5626f56ac8ed9f717cba0d0503`  
		Last Modified: Tue, 13 Sep 2022 03:24:59 GMT  
		Size: 4.9 KB (4894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c93e222cf0a02e2b4146a4d3ff6e5da33b929a10129fd88081a505e4011b9e`  
		Last Modified: Tue, 13 Sep 2022 03:25:00 GMT  
		Size: 316.6 KB (316638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b091f5c4cb7701e12cc29c82ee78e1704fdaaabcd851004efea8deb3acf7f2f`  
		Last Modified: Tue, 13 Sep 2022 03:25:00 GMT  
		Size: 1.2 MB (1227311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5e30653aa54ef905fcc6b97813278f8b54e56e889b1ffccf5101df4fa45882`  
		Last Modified: Tue, 13 Sep 2022 03:24:59 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471afe7d2cb0083a807b44b87fa581728a14e66fbada1f0ea0bcff34258f1cca`  
		Last Modified: Tue, 13 Sep 2022 03:24:59 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.17-bullseye` - linux; arm variant v7

```console
$ docker pull memcached@sha256:960b71bacce5bbd2bf5c700ca3398d8ce00c1a9ebb35a5b690be486267128ef1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28088375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a54ccaf5bd1ba99327d598c288c19a655c2601e43aaf08c6429e99c287ab5b35`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 23 Aug 2022 01:43:01 GMT
ADD file:4cd1b4287674228db28402a76aa4f241740585448be48b5b15068d275ee9eb84 in / 
# Tue, 23 Aug 2022 01:43:01 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 18:03:50 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 23 Aug 2022 18:03:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 29 Aug 2022 19:04:31 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 19:04:31 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 19:09:39 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Mon, 29 Aug 2022 19:09:40 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 19:09:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 19:09:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 19:09:40 GMT
USER memcache
# Mon, 29 Aug 2022 19:09:40 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 19:09:40 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:051ba72559abd0cf65b34b75605580f58636ec3cb994f97de317632a85d82761`  
		Last Modified: Tue, 23 Aug 2022 01:50:05 GMT  
		Size: 26.6 MB (26571732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12dc4f2d8dca33e3850e55e4a2cd25a6dbf19afb27df3daef33de65ac91fd757`  
		Last Modified: Tue, 23 Aug 2022 21:10:42 GMT  
		Size: 4.9 KB (4893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:033f621bef4d3464e367d2c0ce45f3ec626c1c21f84ba7e84ece82bfbef4666e`  
		Last Modified: Tue, 23 Aug 2022 21:10:42 GMT  
		Size: 312.0 KB (312045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba873971d43c849095b8112993f9eb97b90c155f9f9f190da2bef761c9aa61a8`  
		Last Modified: Mon, 29 Aug 2022 19:26:29 GMT  
		Size: 1.2 MB (1199297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b256a2f081d1033d7ae503b0735b03640cd5b071e47fce65387238edf010a05c`  
		Last Modified: Mon, 29 Aug 2022 19:26:29 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a75e8764536efcd4e0fbd3d6c058eb6e05a0489f9e157f95e9e9ca0639c7d40b`  
		Last Modified: Mon, 29 Aug 2022 19:26:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.17-bullseye` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:c67982406cd3e3fb90c50951d6a8cd766a4c0cc625ef035237913dfe56c0ae88
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31444531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02936ddd3c3f04b28ca0fbb9e803bfe5c3c1c0bda9ffe6ca0c6ea9954c351ab8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 13:12:07 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 23 Aug 2022 13:12:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 29 Aug 2022 18:48:57 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 18:48:58 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 18:51:30 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Mon, 29 Aug 2022 18:51:32 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 18:51:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 18:51:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 18:51:34 GMT
USER memcache
# Mon, 29 Aug 2022 18:51:35 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 18:51:36 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21794f0e498790afd69f2d317bbed8aa9cdbd3dddc56f7d52f1b806577e38a06`  
		Last Modified: Tue, 23 Aug 2022 13:15:43 GMT  
		Size: 4.9 KB (4904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:261db6d67ef285bdd84e6ae9e72182c4cd348b9f6c3c060c723764d03a12c2f6`  
		Last Modified: Tue, 23 Aug 2022 13:15:43 GMT  
		Size: 119.2 KB (119240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646e70d704c1f14afdd9de28cb4081703a4efc97e9c6a743ba80329c00705b37`  
		Last Modified: Mon, 29 Aug 2022 18:55:22 GMT  
		Size: 1.3 MB (1256190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db1c8f9c761c12c5c76962f55a2baff7f18d665a53fa76a2d3329fc2c0ccf313`  
		Last Modified: Mon, 29 Aug 2022 18:55:21 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4655eda4ba606249d810ba4d37deb1e82c106bcf3a2394f684a6ad8275d98950`  
		Last Modified: Mon, 29 Aug 2022 18:55:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.17-bullseye` - linux; 386

```console
$ docker pull memcached@sha256:9a142ff1556091ea4d817d7ac5c26fcc6a0b2daa5bf99a56c64d19bb3e3cb866
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33776358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e0455947003534873a7c3f6d3bae27183601ae7c8b66f094e52d72450507327`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 23 Aug 2022 01:02:40 GMT
ADD file:5ca62c98116941aaa64ec72afb689a088c46f75a3e83d5b0d4e58d65ec905ccd in / 
# Tue, 23 Aug 2022 01:02:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:22:44 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 23 Aug 2022 03:22:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 29 Aug 2022 18:38:36 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 18:38:36 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 18:41:29 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Mon, 29 Aug 2022 18:41:31 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 18:41:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 18:41:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 18:41:33 GMT
USER memcache
# Mon, 29 Aug 2022 18:41:34 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 18:41:35 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6b3cb4a05a891d9d8a87a2bd7247b16f79832a9d4afbad3ff5068f6fc2ba1560`  
		Last Modified: Tue, 23 Aug 2022 01:08:25 GMT  
		Size: 32.4 MB (32387317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd24201e0b5e9a68a67bdc3b464a01aeb9a2e5a859a582cdaa80ab08a608337`  
		Last Modified: Tue, 23 Aug 2022 03:27:47 GMT  
		Size: 4.8 KB (4774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3070e5e3b1d98fa0b67b8390880b7596c4719b774864de21f36ed86873041793`  
		Last Modified: Tue, 23 Aug 2022 03:27:48 GMT  
		Size: 130.1 KB (130136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af8c1cee54f7ff86c820ca418aa3d2c05c5f200ca4d938ba76c8f8439b39cb04`  
		Last Modified: Mon, 29 Aug 2022 18:45:40 GMT  
		Size: 1.3 MB (1253721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94d7ae33ce7f8ea696d92c06ef6fd7c86c8228061b3b2485a78a9f59131a48aa`  
		Last Modified: Mon, 29 Aug 2022 18:45:43 GMT  
		Size: 289.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5348ed42ca0cf0c971fcaddc7677e8a3508548c0e3ca9e12b49cc06627f4657c`  
		Last Modified: Mon, 29 Aug 2022 18:45:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.17-bullseye` - linux; mips64le

```console
$ docker pull memcached@sha256:e1403115858fda192fda48a365294d78dd1ea7fa6c9db3be737a883cb34fd9de
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31001916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ce2440650f197fcd6de50038d9a16d23be6db7efc79a8115173cc1ca5a769f5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Sep 2022 01:10:58 GMT
ADD file:91a8d8627a614ff3741d68216da46f13b393e52a70377b97ef317e4a00a3cac6 in / 
# Tue, 13 Sep 2022 01:11:02 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 04:50:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 13 Sep 2022 04:50:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 04:50:38 GMT
ENV MEMCACHED_VERSION=1.6.17
# Tue, 13 Sep 2022 04:50:40 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Tue, 13 Sep 2022 04:57:36 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 13 Sep 2022 04:57:38 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 13 Sep 2022 04:57:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Sep 2022 04:57:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Sep 2022 04:57:48 GMT
USER memcache
# Tue, 13 Sep 2022 04:57:50 GMT
EXPOSE 11211
# Tue, 13 Sep 2022 04:57:53 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:98abeb1446d0e9df6f48d5f72a70b36598cfc1091c9a5ca82690bedcf320e2b3`  
		Last Modified: Tue, 13 Sep 2022 01:18:50 GMT  
		Size: 29.6 MB (29627659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766602637141a485f59d0fc04aec4bfa1ac38583bba125b35c0b6809f1219ed9`  
		Last Modified: Tue, 13 Sep 2022 04:58:11 GMT  
		Size: 4.9 KB (4857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21b631e5bb3330fba3352d6332ae5cfa0b9a35dbc33b4d643b80f7b908c950f5`  
		Last Modified: Tue, 13 Sep 2022 04:58:11 GMT  
		Size: 117.2 KB (117159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee33141b788356ead96c93190f0008f455371a4562d92b27a20945aac60d1361`  
		Last Modified: Tue, 13 Sep 2022 04:58:12 GMT  
		Size: 1.3 MB (1251835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e488d322d0c180f442d31923e23e79064b584ac59e2cadf3be31cc702751460d`  
		Last Modified: Tue, 13 Sep 2022 04:58:11 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec80c89f379732f5466f55915bbad33a4b55dc651bf6346712c92cff64717b11`  
		Last Modified: Tue, 13 Sep 2022 04:58:11 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.17-bullseye` - linux; ppc64le

```console
$ docker pull memcached@sha256:0176bec998e05785ddcaadb9c692b14571e10c2b71050a9988329f903660369b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36970738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7a0216731101d94583b08e4b42f59092a78019783e49a2ddb6401ea59c9d47d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 23 Aug 2022 01:24:52 GMT
ADD file:d35213360d726a18e220276d33f245115c3e94a321addaa4c9127488368b0203 in / 
# Tue, 23 Aug 2022 01:24:54 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:34:49 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 23 Aug 2022 02:34:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 29 Aug 2022 19:19:51 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 19:19:51 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 19:22:46 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Mon, 29 Aug 2022 19:22:47 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 19:22:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 19:22:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 19:22:48 GMT
USER memcache
# Mon, 29 Aug 2022 19:22:49 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 19:22:49 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:698954eda09d38dd1ccc9ce777b1f6bc7f7473fc6c4c3eb634acc8d035a42eae`  
		Last Modified: Tue, 23 Aug 2022 01:30:36 GMT  
		Size: 35.3 MB (35284280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffb080d920662043edc67113c0de4c68258ad19c0fffd9e3b79fa01800c6015`  
		Last Modified: Tue, 23 Aug 2022 02:39:09 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b1f66b68991d8f5ab064b3988db37a48b8f28b4ef0eb8e83efa4c419b630ff`  
		Last Modified: Tue, 23 Aug 2022 02:39:09 GMT  
		Size: 356.9 KB (356931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2256c5b8427744c7563d1151efbeb03c935fbb3e87d621903c9e7476a8db7494`  
		Last Modified: Mon, 29 Aug 2022 19:27:05 GMT  
		Size: 1.3 MB (1324139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee6919a18fb52b4b8259e2942d1d56ca42a4371f735bedd875c5eebdaee214a2`  
		Last Modified: Mon, 29 Aug 2022 19:27:04 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ac3c74fbd1e874bdc7163ccf1ba8bf496b085875b4165fcec2e4a771d9742f9`  
		Last Modified: Mon, 29 Aug 2022 19:27:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.17-bullseye` - linux; s390x

```console
$ docker pull memcached@sha256:f063181874bf86b26f7e8d033e02792331b3282ef6614aa99d8d70c8b178aac0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31206151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c2827f7c0c4acdb1d09c90d24a8e27f37bd489dca825a2831b3f923831b1125`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Sep 2022 00:48:07 GMT
ADD file:e8a6c2e8be5d9d1f83c1e280419014489438391a9feb7c77b6c21adbf0ec062b in / 
# Tue, 13 Sep 2022 00:48:08 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 01:59:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 13 Sep 2022 01:59:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 01:59:22 GMT
ENV MEMCACHED_VERSION=1.6.17
# Tue, 13 Sep 2022 01:59:23 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Tue, 13 Sep 2022 02:02:36 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 13 Sep 2022 02:02:36 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 13 Sep 2022 02:02:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Sep 2022 02:02:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Sep 2022 02:02:37 GMT
USER memcache
# Tue, 13 Sep 2022 02:02:37 GMT
EXPOSE 11211
# Tue, 13 Sep 2022 02:02:37 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c64715e5ebd39975a39b5cf2535772544c27713cbed678b0a21e73680fffaf72`  
		Last Modified: Tue, 13 Sep 2022 00:52:39 GMT  
		Size: 29.6 MB (29635080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce5055aafbfbe726c8840111d8300b0c75f707a8ab517395bb8be985d2feb009`  
		Last Modified: Tue, 13 Sep 2022 02:03:36 GMT  
		Size: 5.0 KB (5021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9a227f323eed41d16b462d95503000badd5210aa179dd3065f4363fe3a1b9f`  
		Last Modified: Tue, 13 Sep 2022 02:03:36 GMT  
		Size: 324.2 KB (324172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36fb60d78f8bd69265b4c2d2246169797772da4584f6e063d49eab9c2f040c51`  
		Last Modified: Tue, 13 Sep 2022 02:03:36 GMT  
		Size: 1.2 MB (1241470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d23a9497c5fd3ec0d26f920c59f1f1628999ae546bd1b2f722b29fbf27e3402`  
		Last Modified: Tue, 13 Sep 2022 02:03:36 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009331f552a168c5b26209994b10c7684fc80fe6348a406878b2262037e82435`  
		Last Modified: Tue, 13 Sep 2022 02:03:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:alpine`

```console
$ docker pull memcached@sha256:6eff5e1647ee867d3fac2bac716568ced7005b8044651f181988a1d0971d3fce
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
$ docker pull memcached@sha256:3b2a8f0dbcbb96b42edffa4959170c2486ddb2bef3de057f8ed71591348721c0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3891406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc6dc88eceeba2070ee6fe3c8c979afeaf5bf6d36e86d09d6457dd8432bb4c36`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:39 GMT
ADD file:b828bc14bc5ff03c8f7310fe0aed6ac5df19a393622d5d1d779a523234d07c0a in / 
# Tue, 09 Aug 2022 17:38:39 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:34:01 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 09 Aug 2022 18:34:02 GMT
RUN apk add --no-cache libsasl
# Mon, 29 Aug 2022 18:41:47 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 18:41:48 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 18:44:43 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Mon, 29 Aug 2022 18:44:45 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 18:44:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 18:44:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 18:44:47 GMT
USER memcache
# Mon, 29 Aug 2022 18:44:48 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 18:44:49 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6c0d3b419d848ea31ca748254611d5d5ce3b76e3d7bba520fd87400fbb75f3b9`  
		Last Modified: Tue, 09 Aug 2022 17:39:33 GMT  
		Size: 2.8 MB (2807121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240e236335200614c944d9ba79e2d7eda5cfa258a69e669b585cc28314d754f5`  
		Last Modified: Tue, 09 Aug 2022 18:38:05 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:844d1ba63a22190468423984b12b7d36f6c005e3316461b983f975f4b8dc9ee8`  
		Last Modified: Tue, 09 Aug 2022 18:38:05 GMT  
		Size: 119.8 KB (119826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2e7c344cfe47d96e7a9d170c9427c474246d16b76964c915cdd2f3d5e62698`  
		Last Modified: Mon, 29 Aug 2022 18:46:29 GMT  
		Size: 962.8 KB (962814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed467891e81f8057bb74046a7442a949b8f2ab27dc7099c321d77f2497584541`  
		Last Modified: Mon, 29 Aug 2022 18:46:29 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5326fe38fa94412c48f8bf0980206aed389413a089a646b582739edc31841a`  
		Last Modified: Mon, 29 Aug 2022 18:46:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:79f15ab95c7dc52c17fab8ebc50e1a380b3584fd2127402ba0486ca4311be7df
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3913056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d80b3f9d28d32be6c7fdc9e706c4555e3bc835f495aed408fe264c0a8ed3d6a7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:48:17 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 09 Aug 2022 18:48:19 GMT
RUN apk add --no-cache libsasl
# Mon, 29 Aug 2022 19:23:01 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 19:23:02 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 19:26:15 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Mon, 29 Aug 2022 19:26:16 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 19:26:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 19:26:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 19:26:17 GMT
USER memcache
# Mon, 29 Aug 2022 19:26:18 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 19:26:18 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:086c869249c97411ce380e3b76305e0b85731874d0ea57dfd0de74e1f387443d`  
		Last Modified: Tue, 09 Aug 2022 18:52:28 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75e55886182590f2e7eef7f1c21851fd9c322339484e8345afd12376d976ddbd`  
		Last Modified: Tue, 09 Aug 2022 18:52:28 GMT  
		Size: 126.1 KB (126064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:794c752514ed274efa4c408cc26745be991e45f3bdf327ec010ef5d614a12e81`  
		Last Modified: Mon, 29 Aug 2022 19:27:39 GMT  
		Size: 982.0 KB (981999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1872e17927a44c66bc7cc1ab89e743c7ce518c421ab7dbec3b77da2ed55f1191`  
		Last Modified: Mon, 29 Aug 2022 19:27:38 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671ee1b68e567ecbfd0d99f4331f15d70a320c05193a577228fa8b911be55513`  
		Last Modified: Mon, 29 Aug 2022 19:27:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; s390x

```console
$ docker pull memcached@sha256:1aca14af5e45939b3b68973e8c599cb648d30771513ce390a9f0eef85c4f17ea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3646984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d704b926b5f988e9db5404831fa6b7a4f8da14a0a3593e225669ff5e99aa2d56`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 19:11:19 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 09 Aug 2022 19:11:20 GMT
RUN apk add --no-cache libsasl
# Mon, 29 Aug 2022 18:51:35 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 18:51:35 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 18:55:03 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Mon, 29 Aug 2022 18:55:03 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 18:55:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 18:55:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 18:55:04 GMT
USER memcache
# Mon, 29 Aug 2022 18:55:04 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 18:55:04 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463a70f3df946e83a223bd55002470af1b7f8d483babe452e515a809b965d35c`  
		Last Modified: Tue, 09 Aug 2022 19:15:35 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df0b8be6e73cbbdde959ca7a21d3fd6c8e36e05bc9c7a46be4e5bfa5b664a50c`  
		Last Modified: Tue, 09 Aug 2022 19:15:35 GMT  
		Size: 112.5 KB (112508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54547b52522c89500f1653dc849604a8a264e93fd45501c6ecc53b9b32824c31`  
		Last Modified: Mon, 29 Aug 2022 18:56:03 GMT  
		Size: 942.2 KB (942207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d838190f94a4d872ed0e972e293eafdda311d2d029f93f8c9fcffe960c8bc74`  
		Last Modified: Mon, 29 Aug 2022 18:56:02 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b2bd5df4107bc3326be940291bf4aacb1a1de4760ca3315321bebf59195856`  
		Last Modified: Mon, 29 Aug 2022 18:56:03 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:alpine3.16`

```console
$ docker pull memcached@sha256:c2f5df2c5099744a041132d1c11900d90f4b9e9c587a38ba8b12f9c03e82cfff
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
$ docker pull memcached@sha256:3b2a8f0dbcbb96b42edffa4959170c2486ddb2bef3de057f8ed71591348721c0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3891406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc6dc88eceeba2070ee6fe3c8c979afeaf5bf6d36e86d09d6457dd8432bb4c36`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:39 GMT
ADD file:b828bc14bc5ff03c8f7310fe0aed6ac5df19a393622d5d1d779a523234d07c0a in / 
# Tue, 09 Aug 2022 17:38:39 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:34:01 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 09 Aug 2022 18:34:02 GMT
RUN apk add --no-cache libsasl
# Mon, 29 Aug 2022 18:41:47 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 18:41:48 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 18:44:43 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Mon, 29 Aug 2022 18:44:45 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 18:44:45 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 18:44:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 18:44:47 GMT
USER memcache
# Mon, 29 Aug 2022 18:44:48 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 18:44:49 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6c0d3b419d848ea31ca748254611d5d5ce3b76e3d7bba520fd87400fbb75f3b9`  
		Last Modified: Tue, 09 Aug 2022 17:39:33 GMT  
		Size: 2.8 MB (2807121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240e236335200614c944d9ba79e2d7eda5cfa258a69e669b585cc28314d754f5`  
		Last Modified: Tue, 09 Aug 2022 18:38:05 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:844d1ba63a22190468423984b12b7d36f6c005e3316461b983f975f4b8dc9ee8`  
		Last Modified: Tue, 09 Aug 2022 18:38:05 GMT  
		Size: 119.8 KB (119826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2e7c344cfe47d96e7a9d170c9427c474246d16b76964c915cdd2f3d5e62698`  
		Last Modified: Mon, 29 Aug 2022 18:46:29 GMT  
		Size: 962.8 KB (962814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed467891e81f8057bb74046a7442a949b8f2ab27dc7099c321d77f2497584541`  
		Last Modified: Mon, 29 Aug 2022 18:46:29 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5326fe38fa94412c48f8bf0980206aed389413a089a646b582739edc31841a`  
		Last Modified: Mon, 29 Aug 2022 18:46:29 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine3.16` - linux; ppc64le

```console
$ docker pull memcached@sha256:79f15ab95c7dc52c17fab8ebc50e1a380b3584fd2127402ba0486ca4311be7df
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.9 MB (3913056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d80b3f9d28d32be6c7fdc9e706c4555e3bc835f495aed408fe264c0a8ed3d6a7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:48:17 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 09 Aug 2022 18:48:19 GMT
RUN apk add --no-cache libsasl
# Mon, 29 Aug 2022 19:23:01 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 19:23:02 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 19:26:15 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Mon, 29 Aug 2022 19:26:16 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 19:26:17 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 19:26:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 19:26:17 GMT
USER memcache
# Mon, 29 Aug 2022 19:26:18 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 19:26:18 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:086c869249c97411ce380e3b76305e0b85731874d0ea57dfd0de74e1f387443d`  
		Last Modified: Tue, 09 Aug 2022 18:52:28 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75e55886182590f2e7eef7f1c21851fd9c322339484e8345afd12376d976ddbd`  
		Last Modified: Tue, 09 Aug 2022 18:52:28 GMT  
		Size: 126.1 KB (126064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:794c752514ed274efa4c408cc26745be991e45f3bdf327ec010ef5d614a12e81`  
		Last Modified: Mon, 29 Aug 2022 19:27:39 GMT  
		Size: 982.0 KB (981999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1872e17927a44c66bc7cc1ab89e743c7ce518c421ab7dbec3b77da2ed55f1191`  
		Last Modified: Mon, 29 Aug 2022 19:27:38 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671ee1b68e567ecbfd0d99f4331f15d70a320c05193a577228fa8b911be55513`  
		Last Modified: Mon, 29 Aug 2022 19:27:38 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine3.16` - linux; s390x

```console
$ docker pull memcached@sha256:1aca14af5e45939b3b68973e8c599cb648d30771513ce390a9f0eef85c4f17ea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3646984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d704b926b5f988e9db5404831fa6b7a4f8da14a0a3593e225669ff5e99aa2d56`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 19:11:19 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 09 Aug 2022 19:11:20 GMT
RUN apk add --no-cache libsasl
# Mon, 29 Aug 2022 18:51:35 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 18:51:35 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 18:55:03 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Mon, 29 Aug 2022 18:55:03 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 18:55:04 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 18:55:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 18:55:04 GMT
USER memcache
# Mon, 29 Aug 2022 18:55:04 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 18:55:04 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463a70f3df946e83a223bd55002470af1b7f8d483babe452e515a809b965d35c`  
		Last Modified: Tue, 09 Aug 2022 19:15:35 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df0b8be6e73cbbdde959ca7a21d3fd6c8e36e05bc9c7a46be4e5bfa5b664a50c`  
		Last Modified: Tue, 09 Aug 2022 19:15:35 GMT  
		Size: 112.5 KB (112508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54547b52522c89500f1653dc849604a8a264e93fd45501c6ecc53b9b32824c31`  
		Last Modified: Mon, 29 Aug 2022 18:56:03 GMT  
		Size: 942.2 KB (942207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d838190f94a4d872ed0e972e293eafdda311d2d029f93f8c9fcffe960c8bc74`  
		Last Modified: Mon, 29 Aug 2022 18:56:02 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b2bd5df4107bc3326be940291bf4aacb1a1de4760ca3315321bebf59195856`  
		Last Modified: Mon, 29 Aug 2022 18:56:03 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:bullseye`

```console
$ docker pull memcached@sha256:1917f1b4e48a69e5be80a57c321504338f9b65046386ea50ee679322413e26c7
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
$ docker pull memcached@sha256:2a9bf2539b24c553b92c876dfbe6dd48450a832f2b5395ec3217271018ad2ca0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32971284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92e1422c3edf80b790f0a601173b8e329b6619096d8cebb0b50b0f489ad1d971`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:54:26 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 23 Aug 2022 02:54:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 29 Aug 2022 19:57:00 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 19:57:01 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 19:59:41 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Mon, 29 Aug 2022 19:59:41 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 19:59:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 19:59:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 19:59:42 GMT
USER memcache
# Mon, 29 Aug 2022 19:59:42 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 19:59:42 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa73fb65ea8b12a2375459f0d656d3ad06e2863c906fcf962486eda3701f3fd6`  
		Last Modified: Tue, 23 Aug 2022 02:57:38 GMT  
		Size: 5.0 KB (4981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502b4e8803067b28098d0ea52281cfef66da1ee1e869241612b545d7e9ff12de`  
		Last Modified: Tue, 23 Aug 2022 02:57:38 GMT  
		Size: 328.1 KB (328108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b905db5d33a47882bd6cb4935bcc5d576d5cad5ba761b6b4004982c3aa7333`  
		Last Modified: Mon, 29 Aug 2022 20:03:05 GMT  
		Size: 1.3 MB (1256303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93643c661348540c2edcfc8a007b2c9aff33ac36cb9dcd910e0ddb51f50cd09e`  
		Last Modified: Mon, 29 Aug 2022 20:03:04 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc510e39dc783b83b00e5abd05d57df948435a0aaf45e87b131cc0fff83021e`  
		Last Modified: Mon, 29 Aug 2022 20:03:05 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; arm variant v5

```console
$ docker pull memcached@sha256:ef629e7153669e6100c98fba79336f87cc033d073c6219d6c7ec9360298a5d8e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30454536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84960478143b53154da0f3409e3f1141b62dabf4fe0c97c3661b5dd8a1c533ec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Sep 2022 00:53:30 GMT
ADD file:539e23f1c3a625a612a5a59b3939e9692c86c3cfa4956d30f4802c9f34ffa29c in / 
# Tue, 13 Sep 2022 00:53:31 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 03:18:14 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 13 Sep 2022 03:18:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 03:18:20 GMT
ENV MEMCACHED_VERSION=1.6.17
# Tue, 13 Sep 2022 03:18:20 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Tue, 13 Sep 2022 03:24:21 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 13 Sep 2022 03:24:22 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 13 Sep 2022 03:24:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Sep 2022 03:24:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Sep 2022 03:24:22 GMT
USER memcache
# Tue, 13 Sep 2022 03:24:22 GMT
EXPOSE 11211
# Tue, 13 Sep 2022 03:24:22 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:705abbab4fcb3a8dfe046a2ae6c450328aa11d93911abce66d3bba8bc693cbd4`  
		Last Modified: Tue, 13 Sep 2022 01:01:07 GMT  
		Size: 28.9 MB (28905288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eba43be24e48cc0796f0f5a17e6b674c0f07d5626f56ac8ed9f717cba0d0503`  
		Last Modified: Tue, 13 Sep 2022 03:24:59 GMT  
		Size: 4.9 KB (4894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c93e222cf0a02e2b4146a4d3ff6e5da33b929a10129fd88081a505e4011b9e`  
		Last Modified: Tue, 13 Sep 2022 03:25:00 GMT  
		Size: 316.6 KB (316638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b091f5c4cb7701e12cc29c82ee78e1704fdaaabcd851004efea8deb3acf7f2f`  
		Last Modified: Tue, 13 Sep 2022 03:25:00 GMT  
		Size: 1.2 MB (1227311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5e30653aa54ef905fcc6b97813278f8b54e56e889b1ffccf5101df4fa45882`  
		Last Modified: Tue, 13 Sep 2022 03:24:59 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471afe7d2cb0083a807b44b87fa581728a14e66fbada1f0ea0bcff34258f1cca`  
		Last Modified: Tue, 13 Sep 2022 03:24:59 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; arm variant v7

```console
$ docker pull memcached@sha256:960b71bacce5bbd2bf5c700ca3398d8ce00c1a9ebb35a5b690be486267128ef1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28088375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a54ccaf5bd1ba99327d598c288c19a655c2601e43aaf08c6429e99c287ab5b35`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 23 Aug 2022 01:43:01 GMT
ADD file:4cd1b4287674228db28402a76aa4f241740585448be48b5b15068d275ee9eb84 in / 
# Tue, 23 Aug 2022 01:43:01 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 18:03:50 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 23 Aug 2022 18:03:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 29 Aug 2022 19:04:31 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 19:04:31 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 19:09:39 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Mon, 29 Aug 2022 19:09:40 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 19:09:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 19:09:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 19:09:40 GMT
USER memcache
# Mon, 29 Aug 2022 19:09:40 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 19:09:40 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:051ba72559abd0cf65b34b75605580f58636ec3cb994f97de317632a85d82761`  
		Last Modified: Tue, 23 Aug 2022 01:50:05 GMT  
		Size: 26.6 MB (26571732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12dc4f2d8dca33e3850e55e4a2cd25a6dbf19afb27df3daef33de65ac91fd757`  
		Last Modified: Tue, 23 Aug 2022 21:10:42 GMT  
		Size: 4.9 KB (4893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:033f621bef4d3464e367d2c0ce45f3ec626c1c21f84ba7e84ece82bfbef4666e`  
		Last Modified: Tue, 23 Aug 2022 21:10:42 GMT  
		Size: 312.0 KB (312045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba873971d43c849095b8112993f9eb97b90c155f9f9f190da2bef761c9aa61a8`  
		Last Modified: Mon, 29 Aug 2022 19:26:29 GMT  
		Size: 1.2 MB (1199297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b256a2f081d1033d7ae503b0735b03640cd5b071e47fce65387238edf010a05c`  
		Last Modified: Mon, 29 Aug 2022 19:26:29 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a75e8764536efcd4e0fbd3d6c058eb6e05a0489f9e157f95e9e9ca0639c7d40b`  
		Last Modified: Mon, 29 Aug 2022 19:26:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:c67982406cd3e3fb90c50951d6a8cd766a4c0cc625ef035237913dfe56c0ae88
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31444531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02936ddd3c3f04b28ca0fbb9e803bfe5c3c1c0bda9ffe6ca0c6ea9954c351ab8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 13:12:07 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 23 Aug 2022 13:12:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 29 Aug 2022 18:48:57 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 18:48:58 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 18:51:30 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Mon, 29 Aug 2022 18:51:32 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 18:51:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 18:51:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 18:51:34 GMT
USER memcache
# Mon, 29 Aug 2022 18:51:35 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 18:51:36 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21794f0e498790afd69f2d317bbed8aa9cdbd3dddc56f7d52f1b806577e38a06`  
		Last Modified: Tue, 23 Aug 2022 13:15:43 GMT  
		Size: 4.9 KB (4904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:261db6d67ef285bdd84e6ae9e72182c4cd348b9f6c3c060c723764d03a12c2f6`  
		Last Modified: Tue, 23 Aug 2022 13:15:43 GMT  
		Size: 119.2 KB (119240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646e70d704c1f14afdd9de28cb4081703a4efc97e9c6a743ba80329c00705b37`  
		Last Modified: Mon, 29 Aug 2022 18:55:22 GMT  
		Size: 1.3 MB (1256190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db1c8f9c761c12c5c76962f55a2baff7f18d665a53fa76a2d3329fc2c0ccf313`  
		Last Modified: Mon, 29 Aug 2022 18:55:21 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4655eda4ba606249d810ba4d37deb1e82c106bcf3a2394f684a6ad8275d98950`  
		Last Modified: Mon, 29 Aug 2022 18:55:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; 386

```console
$ docker pull memcached@sha256:9a142ff1556091ea4d817d7ac5c26fcc6a0b2daa5bf99a56c64d19bb3e3cb866
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33776358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e0455947003534873a7c3f6d3bae27183601ae7c8b66f094e52d72450507327`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 23 Aug 2022 01:02:40 GMT
ADD file:5ca62c98116941aaa64ec72afb689a088c46f75a3e83d5b0d4e58d65ec905ccd in / 
# Tue, 23 Aug 2022 01:02:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:22:44 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 23 Aug 2022 03:22:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 29 Aug 2022 18:38:36 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 18:38:36 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 18:41:29 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Mon, 29 Aug 2022 18:41:31 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 18:41:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 18:41:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 18:41:33 GMT
USER memcache
# Mon, 29 Aug 2022 18:41:34 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 18:41:35 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6b3cb4a05a891d9d8a87a2bd7247b16f79832a9d4afbad3ff5068f6fc2ba1560`  
		Last Modified: Tue, 23 Aug 2022 01:08:25 GMT  
		Size: 32.4 MB (32387317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd24201e0b5e9a68a67bdc3b464a01aeb9a2e5a859a582cdaa80ab08a608337`  
		Last Modified: Tue, 23 Aug 2022 03:27:47 GMT  
		Size: 4.8 KB (4774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3070e5e3b1d98fa0b67b8390880b7596c4719b774864de21f36ed86873041793`  
		Last Modified: Tue, 23 Aug 2022 03:27:48 GMT  
		Size: 130.1 KB (130136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af8c1cee54f7ff86c820ca418aa3d2c05c5f200ca4d938ba76c8f8439b39cb04`  
		Last Modified: Mon, 29 Aug 2022 18:45:40 GMT  
		Size: 1.3 MB (1253721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94d7ae33ce7f8ea696d92c06ef6fd7c86c8228061b3b2485a78a9f59131a48aa`  
		Last Modified: Mon, 29 Aug 2022 18:45:43 GMT  
		Size: 289.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5348ed42ca0cf0c971fcaddc7677e8a3508548c0e3ca9e12b49cc06627f4657c`  
		Last Modified: Mon, 29 Aug 2022 18:45:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; mips64le

```console
$ docker pull memcached@sha256:e1403115858fda192fda48a365294d78dd1ea7fa6c9db3be737a883cb34fd9de
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31001916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ce2440650f197fcd6de50038d9a16d23be6db7efc79a8115173cc1ca5a769f5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Sep 2022 01:10:58 GMT
ADD file:91a8d8627a614ff3741d68216da46f13b393e52a70377b97ef317e4a00a3cac6 in / 
# Tue, 13 Sep 2022 01:11:02 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 04:50:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 13 Sep 2022 04:50:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 04:50:38 GMT
ENV MEMCACHED_VERSION=1.6.17
# Tue, 13 Sep 2022 04:50:40 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Tue, 13 Sep 2022 04:57:36 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 13 Sep 2022 04:57:38 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 13 Sep 2022 04:57:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Sep 2022 04:57:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Sep 2022 04:57:48 GMT
USER memcache
# Tue, 13 Sep 2022 04:57:50 GMT
EXPOSE 11211
# Tue, 13 Sep 2022 04:57:53 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:98abeb1446d0e9df6f48d5f72a70b36598cfc1091c9a5ca82690bedcf320e2b3`  
		Last Modified: Tue, 13 Sep 2022 01:18:50 GMT  
		Size: 29.6 MB (29627659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766602637141a485f59d0fc04aec4bfa1ac38583bba125b35c0b6809f1219ed9`  
		Last Modified: Tue, 13 Sep 2022 04:58:11 GMT  
		Size: 4.9 KB (4857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21b631e5bb3330fba3352d6332ae5cfa0b9a35dbc33b4d643b80f7b908c950f5`  
		Last Modified: Tue, 13 Sep 2022 04:58:11 GMT  
		Size: 117.2 KB (117159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee33141b788356ead96c93190f0008f455371a4562d92b27a20945aac60d1361`  
		Last Modified: Tue, 13 Sep 2022 04:58:12 GMT  
		Size: 1.3 MB (1251835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e488d322d0c180f442d31923e23e79064b584ac59e2cadf3be31cc702751460d`  
		Last Modified: Tue, 13 Sep 2022 04:58:11 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec80c89f379732f5466f55915bbad33a4b55dc651bf6346712c92cff64717b11`  
		Last Modified: Tue, 13 Sep 2022 04:58:11 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; ppc64le

```console
$ docker pull memcached@sha256:0176bec998e05785ddcaadb9c692b14571e10c2b71050a9988329f903660369b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36970738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7a0216731101d94583b08e4b42f59092a78019783e49a2ddb6401ea59c9d47d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 23 Aug 2022 01:24:52 GMT
ADD file:d35213360d726a18e220276d33f245115c3e94a321addaa4c9127488368b0203 in / 
# Tue, 23 Aug 2022 01:24:54 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:34:49 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 23 Aug 2022 02:34:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 29 Aug 2022 19:19:51 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 19:19:51 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 19:22:46 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Mon, 29 Aug 2022 19:22:47 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 19:22:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 19:22:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 19:22:48 GMT
USER memcache
# Mon, 29 Aug 2022 19:22:49 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 19:22:49 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:698954eda09d38dd1ccc9ce777b1f6bc7f7473fc6c4c3eb634acc8d035a42eae`  
		Last Modified: Tue, 23 Aug 2022 01:30:36 GMT  
		Size: 35.3 MB (35284280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffb080d920662043edc67113c0de4c68258ad19c0fffd9e3b79fa01800c6015`  
		Last Modified: Tue, 23 Aug 2022 02:39:09 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b1f66b68991d8f5ab064b3988db37a48b8f28b4ef0eb8e83efa4c419b630ff`  
		Last Modified: Tue, 23 Aug 2022 02:39:09 GMT  
		Size: 356.9 KB (356931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2256c5b8427744c7563d1151efbeb03c935fbb3e87d621903c9e7476a8db7494`  
		Last Modified: Mon, 29 Aug 2022 19:27:05 GMT  
		Size: 1.3 MB (1324139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee6919a18fb52b4b8259e2942d1d56ca42a4371f735bedd875c5eebdaee214a2`  
		Last Modified: Mon, 29 Aug 2022 19:27:04 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ac3c74fbd1e874bdc7163ccf1ba8bf496b085875b4165fcec2e4a771d9742f9`  
		Last Modified: Mon, 29 Aug 2022 19:27:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bullseye` - linux; s390x

```console
$ docker pull memcached@sha256:f063181874bf86b26f7e8d033e02792331b3282ef6614aa99d8d70c8b178aac0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31206151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c2827f7c0c4acdb1d09c90d24a8e27f37bd489dca825a2831b3f923831b1125`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Sep 2022 00:48:07 GMT
ADD file:e8a6c2e8be5d9d1f83c1e280419014489438391a9feb7c77b6c21adbf0ec062b in / 
# Tue, 13 Sep 2022 00:48:08 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 01:59:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 13 Sep 2022 01:59:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 01:59:22 GMT
ENV MEMCACHED_VERSION=1.6.17
# Tue, 13 Sep 2022 01:59:23 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Tue, 13 Sep 2022 02:02:36 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 13 Sep 2022 02:02:36 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 13 Sep 2022 02:02:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Sep 2022 02:02:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Sep 2022 02:02:37 GMT
USER memcache
# Tue, 13 Sep 2022 02:02:37 GMT
EXPOSE 11211
# Tue, 13 Sep 2022 02:02:37 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c64715e5ebd39975a39b5cf2535772544c27713cbed678b0a21e73680fffaf72`  
		Last Modified: Tue, 13 Sep 2022 00:52:39 GMT  
		Size: 29.6 MB (29635080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce5055aafbfbe726c8840111d8300b0c75f707a8ab517395bb8be985d2feb009`  
		Last Modified: Tue, 13 Sep 2022 02:03:36 GMT  
		Size: 5.0 KB (5021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9a227f323eed41d16b462d95503000badd5210aa179dd3065f4363fe3a1b9f`  
		Last Modified: Tue, 13 Sep 2022 02:03:36 GMT  
		Size: 324.2 KB (324172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36fb60d78f8bd69265b4c2d2246169797772da4584f6e063d49eab9c2f040c51`  
		Last Modified: Tue, 13 Sep 2022 02:03:36 GMT  
		Size: 1.2 MB (1241470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d23a9497c5fd3ec0d26f920c59f1f1628999ae546bd1b2f722b29fbf27e3402`  
		Last Modified: Tue, 13 Sep 2022 02:03:36 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009331f552a168c5b26209994b10c7684fc80fe6348a406878b2262037e82435`  
		Last Modified: Tue, 13 Sep 2022 02:03:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:latest`

```console
$ docker pull memcached@sha256:1917f1b4e48a69e5be80a57c321504338f9b65046386ea50ee679322413e26c7
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
$ docker pull memcached@sha256:2a9bf2539b24c553b92c876dfbe6dd48450a832f2b5395ec3217271018ad2ca0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (32971284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92e1422c3edf80b790f0a601173b8e329b6619096d8cebb0b50b0f489ad1d971`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:54:26 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 23 Aug 2022 02:54:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 29 Aug 2022 19:57:00 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 19:57:01 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 19:59:41 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Mon, 29 Aug 2022 19:59:41 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 19:59:41 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 19:59:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 19:59:42 GMT
USER memcache
# Mon, 29 Aug 2022 19:59:42 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 19:59:42 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa73fb65ea8b12a2375459f0d656d3ad06e2863c906fcf962486eda3701f3fd6`  
		Last Modified: Tue, 23 Aug 2022 02:57:38 GMT  
		Size: 5.0 KB (4981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502b4e8803067b28098d0ea52281cfef66da1ee1e869241612b545d7e9ff12de`  
		Last Modified: Tue, 23 Aug 2022 02:57:38 GMT  
		Size: 328.1 KB (328108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b905db5d33a47882bd6cb4935bcc5d576d5cad5ba761b6b4004982c3aa7333`  
		Last Modified: Mon, 29 Aug 2022 20:03:05 GMT  
		Size: 1.3 MB (1256303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93643c661348540c2edcfc8a007b2c9aff33ac36cb9dcd910e0ddb51f50cd09e`  
		Last Modified: Mon, 29 Aug 2022 20:03:04 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc510e39dc783b83b00e5abd05d57df948435a0aaf45e87b131cc0fff83021e`  
		Last Modified: Mon, 29 Aug 2022 20:03:05 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm variant v5

```console
$ docker pull memcached@sha256:ef629e7153669e6100c98fba79336f87cc033d073c6219d6c7ec9360298a5d8e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30454536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84960478143b53154da0f3409e3f1141b62dabf4fe0c97c3661b5dd8a1c533ec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Sep 2022 00:53:30 GMT
ADD file:539e23f1c3a625a612a5a59b3939e9692c86c3cfa4956d30f4802c9f34ffa29c in / 
# Tue, 13 Sep 2022 00:53:31 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 03:18:14 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 13 Sep 2022 03:18:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 03:18:20 GMT
ENV MEMCACHED_VERSION=1.6.17
# Tue, 13 Sep 2022 03:18:20 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Tue, 13 Sep 2022 03:24:21 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 13 Sep 2022 03:24:22 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 13 Sep 2022 03:24:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Sep 2022 03:24:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Sep 2022 03:24:22 GMT
USER memcache
# Tue, 13 Sep 2022 03:24:22 GMT
EXPOSE 11211
# Tue, 13 Sep 2022 03:24:22 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:705abbab4fcb3a8dfe046a2ae6c450328aa11d93911abce66d3bba8bc693cbd4`  
		Last Modified: Tue, 13 Sep 2022 01:01:07 GMT  
		Size: 28.9 MB (28905288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eba43be24e48cc0796f0f5a17e6b674c0f07d5626f56ac8ed9f717cba0d0503`  
		Last Modified: Tue, 13 Sep 2022 03:24:59 GMT  
		Size: 4.9 KB (4894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c93e222cf0a02e2b4146a4d3ff6e5da33b929a10129fd88081a505e4011b9e`  
		Last Modified: Tue, 13 Sep 2022 03:25:00 GMT  
		Size: 316.6 KB (316638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b091f5c4cb7701e12cc29c82ee78e1704fdaaabcd851004efea8deb3acf7f2f`  
		Last Modified: Tue, 13 Sep 2022 03:25:00 GMT  
		Size: 1.2 MB (1227311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5e30653aa54ef905fcc6b97813278f8b54e56e889b1ffccf5101df4fa45882`  
		Last Modified: Tue, 13 Sep 2022 03:24:59 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471afe7d2cb0083a807b44b87fa581728a14e66fbada1f0ea0bcff34258f1cca`  
		Last Modified: Tue, 13 Sep 2022 03:24:59 GMT  
		Size: 119.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm variant v7

```console
$ docker pull memcached@sha256:960b71bacce5bbd2bf5c700ca3398d8ce00c1a9ebb35a5b690be486267128ef1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28088375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a54ccaf5bd1ba99327d598c288c19a655c2601e43aaf08c6429e99c287ab5b35`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 23 Aug 2022 01:43:01 GMT
ADD file:4cd1b4287674228db28402a76aa4f241740585448be48b5b15068d275ee9eb84 in / 
# Tue, 23 Aug 2022 01:43:01 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 18:03:50 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 23 Aug 2022 18:03:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 29 Aug 2022 19:04:31 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 19:04:31 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 19:09:39 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Mon, 29 Aug 2022 19:09:40 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 19:09:40 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 19:09:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 19:09:40 GMT
USER memcache
# Mon, 29 Aug 2022 19:09:40 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 19:09:40 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:051ba72559abd0cf65b34b75605580f58636ec3cb994f97de317632a85d82761`  
		Last Modified: Tue, 23 Aug 2022 01:50:05 GMT  
		Size: 26.6 MB (26571732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12dc4f2d8dca33e3850e55e4a2cd25a6dbf19afb27df3daef33de65ac91fd757`  
		Last Modified: Tue, 23 Aug 2022 21:10:42 GMT  
		Size: 4.9 KB (4893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:033f621bef4d3464e367d2c0ce45f3ec626c1c21f84ba7e84ece82bfbef4666e`  
		Last Modified: Tue, 23 Aug 2022 21:10:42 GMT  
		Size: 312.0 KB (312045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba873971d43c849095b8112993f9eb97b90c155f9f9f190da2bef761c9aa61a8`  
		Last Modified: Mon, 29 Aug 2022 19:26:29 GMT  
		Size: 1.2 MB (1199297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b256a2f081d1033d7ae503b0735b03640cd5b071e47fce65387238edf010a05c`  
		Last Modified: Mon, 29 Aug 2022 19:26:29 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a75e8764536efcd4e0fbd3d6c058eb6e05a0489f9e157f95e9e9ca0639c7d40b`  
		Last Modified: Mon, 29 Aug 2022 19:26:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:c67982406cd3e3fb90c50951d6a8cd766a4c0cc625ef035237913dfe56c0ae88
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31444531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02936ddd3c3f04b28ca0fbb9e803bfe5c3c1c0bda9ffe6ca0c6ea9954c351ab8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 13:12:07 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 23 Aug 2022 13:12:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 29 Aug 2022 18:48:57 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 18:48:58 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 18:51:30 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Mon, 29 Aug 2022 18:51:32 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 18:51:32 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 18:51:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 18:51:34 GMT
USER memcache
# Mon, 29 Aug 2022 18:51:35 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 18:51:36 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21794f0e498790afd69f2d317bbed8aa9cdbd3dddc56f7d52f1b806577e38a06`  
		Last Modified: Tue, 23 Aug 2022 13:15:43 GMT  
		Size: 4.9 KB (4904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:261db6d67ef285bdd84e6ae9e72182c4cd348b9f6c3c060c723764d03a12c2f6`  
		Last Modified: Tue, 23 Aug 2022 13:15:43 GMT  
		Size: 119.2 KB (119240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646e70d704c1f14afdd9de28cb4081703a4efc97e9c6a743ba80329c00705b37`  
		Last Modified: Mon, 29 Aug 2022 18:55:22 GMT  
		Size: 1.3 MB (1256190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db1c8f9c761c12c5c76962f55a2baff7f18d665a53fa76a2d3329fc2c0ccf313`  
		Last Modified: Mon, 29 Aug 2022 18:55:21 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4655eda4ba606249d810ba4d37deb1e82c106bcf3a2394f684a6ad8275d98950`  
		Last Modified: Mon, 29 Aug 2022 18:55:21 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; 386

```console
$ docker pull memcached@sha256:9a142ff1556091ea4d817d7ac5c26fcc6a0b2daa5bf99a56c64d19bb3e3cb866
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33776358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e0455947003534873a7c3f6d3bae27183601ae7c8b66f094e52d72450507327`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 23 Aug 2022 01:02:40 GMT
ADD file:5ca62c98116941aaa64ec72afb689a088c46f75a3e83d5b0d4e58d65ec905ccd in / 
# Tue, 23 Aug 2022 01:02:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 03:22:44 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 23 Aug 2022 03:22:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 29 Aug 2022 18:38:36 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 18:38:36 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 18:41:29 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Mon, 29 Aug 2022 18:41:31 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 18:41:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 18:41:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 18:41:33 GMT
USER memcache
# Mon, 29 Aug 2022 18:41:34 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 18:41:35 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6b3cb4a05a891d9d8a87a2bd7247b16f79832a9d4afbad3ff5068f6fc2ba1560`  
		Last Modified: Tue, 23 Aug 2022 01:08:25 GMT  
		Size: 32.4 MB (32387317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd24201e0b5e9a68a67bdc3b464a01aeb9a2e5a859a582cdaa80ab08a608337`  
		Last Modified: Tue, 23 Aug 2022 03:27:47 GMT  
		Size: 4.8 KB (4774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3070e5e3b1d98fa0b67b8390880b7596c4719b774864de21f36ed86873041793`  
		Last Modified: Tue, 23 Aug 2022 03:27:48 GMT  
		Size: 130.1 KB (130136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af8c1cee54f7ff86c820ca418aa3d2c05c5f200ca4d938ba76c8f8439b39cb04`  
		Last Modified: Mon, 29 Aug 2022 18:45:40 GMT  
		Size: 1.3 MB (1253721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94d7ae33ce7f8ea696d92c06ef6fd7c86c8228061b3b2485a78a9f59131a48aa`  
		Last Modified: Mon, 29 Aug 2022 18:45:43 GMT  
		Size: 289.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5348ed42ca0cf0c971fcaddc7677e8a3508548c0e3ca9e12b49cc06627f4657c`  
		Last Modified: Mon, 29 Aug 2022 18:45:39 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; mips64le

```console
$ docker pull memcached@sha256:e1403115858fda192fda48a365294d78dd1ea7fa6c9db3be737a883cb34fd9de
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31001916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ce2440650f197fcd6de50038d9a16d23be6db7efc79a8115173cc1ca5a769f5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Sep 2022 01:10:58 GMT
ADD file:91a8d8627a614ff3741d68216da46f13b393e52a70377b97ef317e4a00a3cac6 in / 
# Tue, 13 Sep 2022 01:11:02 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 04:50:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 13 Sep 2022 04:50:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 04:50:38 GMT
ENV MEMCACHED_VERSION=1.6.17
# Tue, 13 Sep 2022 04:50:40 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Tue, 13 Sep 2022 04:57:36 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 13 Sep 2022 04:57:38 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 13 Sep 2022 04:57:43 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Sep 2022 04:57:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Sep 2022 04:57:48 GMT
USER memcache
# Tue, 13 Sep 2022 04:57:50 GMT
EXPOSE 11211
# Tue, 13 Sep 2022 04:57:53 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:98abeb1446d0e9df6f48d5f72a70b36598cfc1091c9a5ca82690bedcf320e2b3`  
		Last Modified: Tue, 13 Sep 2022 01:18:50 GMT  
		Size: 29.6 MB (29627659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766602637141a485f59d0fc04aec4bfa1ac38583bba125b35c0b6809f1219ed9`  
		Last Modified: Tue, 13 Sep 2022 04:58:11 GMT  
		Size: 4.9 KB (4857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21b631e5bb3330fba3352d6332ae5cfa0b9a35dbc33b4d643b80f7b908c950f5`  
		Last Modified: Tue, 13 Sep 2022 04:58:11 GMT  
		Size: 117.2 KB (117159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee33141b788356ead96c93190f0008f455371a4562d92b27a20945aac60d1361`  
		Last Modified: Tue, 13 Sep 2022 04:58:12 GMT  
		Size: 1.3 MB (1251835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e488d322d0c180f442d31923e23e79064b584ac59e2cadf3be31cc702751460d`  
		Last Modified: Tue, 13 Sep 2022 04:58:11 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec80c89f379732f5466f55915bbad33a4b55dc651bf6346712c92cff64717b11`  
		Last Modified: Tue, 13 Sep 2022 04:58:11 GMT  
		Size: 120.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; ppc64le

```console
$ docker pull memcached@sha256:0176bec998e05785ddcaadb9c692b14571e10c2b71050a9988329f903660369b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36970738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7a0216731101d94583b08e4b42f59092a78019783e49a2ddb6401ea59c9d47d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 23 Aug 2022 01:24:52 GMT
ADD file:d35213360d726a18e220276d33f245115c3e94a321addaa4c9127488368b0203 in / 
# Tue, 23 Aug 2022 01:24:54 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:34:49 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 23 Aug 2022 02:34:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 29 Aug 2022 19:19:51 GMT
ENV MEMCACHED_VERSION=1.6.17
# Mon, 29 Aug 2022 19:19:51 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Mon, 29 Aug 2022 19:22:46 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Mon, 29 Aug 2022 19:22:47 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 29 Aug 2022 19:22:48 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 29 Aug 2022 19:22:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 29 Aug 2022 19:22:48 GMT
USER memcache
# Mon, 29 Aug 2022 19:22:49 GMT
EXPOSE 11211
# Mon, 29 Aug 2022 19:22:49 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:698954eda09d38dd1ccc9ce777b1f6bc7f7473fc6c4c3eb634acc8d035a42eae`  
		Last Modified: Tue, 23 Aug 2022 01:30:36 GMT  
		Size: 35.3 MB (35284280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffb080d920662043edc67113c0de4c68258ad19c0fffd9e3b79fa01800c6015`  
		Last Modified: Tue, 23 Aug 2022 02:39:09 GMT  
		Size: 5.0 KB (4980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b1f66b68991d8f5ab064b3988db37a48b8f28b4ef0eb8e83efa4c419b630ff`  
		Last Modified: Tue, 23 Aug 2022 02:39:09 GMT  
		Size: 356.9 KB (356931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2256c5b8427744c7563d1151efbeb03c935fbb3e87d621903c9e7476a8db7494`  
		Last Modified: Mon, 29 Aug 2022 19:27:05 GMT  
		Size: 1.3 MB (1324139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee6919a18fb52b4b8259e2942d1d56ca42a4371f735bedd875c5eebdaee214a2`  
		Last Modified: Mon, 29 Aug 2022 19:27:04 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ac3c74fbd1e874bdc7163ccf1ba8bf496b085875b4165fcec2e4a771d9742f9`  
		Last Modified: Mon, 29 Aug 2022 19:27:04 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; s390x

```console
$ docker pull memcached@sha256:f063181874bf86b26f7e8d033e02792331b3282ef6614aa99d8d70c8b178aac0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31206151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c2827f7c0c4acdb1d09c90d24a8e27f37bd489dca825a2831b3f923831b1125`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 13 Sep 2022 00:48:07 GMT
ADD file:e8a6c2e8be5d9d1f83c1e280419014489438391a9feb7c77b6c21adbf0ec062b in / 
# Tue, 13 Sep 2022 00:48:08 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 01:59:19 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Tue, 13 Sep 2022 01:59:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 01:59:22 GMT
ENV MEMCACHED_VERSION=1.6.17
# Tue, 13 Sep 2022 01:59:23 GMT
ENV MEMCACHED_SHA1=e25639473e15f1bd9516b915fb7e03ab8209030f
# Tue, 13 Sep 2022 02:02:36 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Tue, 13 Sep 2022 02:02:36 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 13 Sep 2022 02:02:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 13 Sep 2022 02:02:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 13 Sep 2022 02:02:37 GMT
USER memcache
# Tue, 13 Sep 2022 02:02:37 GMT
EXPOSE 11211
# Tue, 13 Sep 2022 02:02:37 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c64715e5ebd39975a39b5cf2535772544c27713cbed678b0a21e73680fffaf72`  
		Last Modified: Tue, 13 Sep 2022 00:52:39 GMT  
		Size: 29.6 MB (29635080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce5055aafbfbe726c8840111d8300b0c75f707a8ab517395bb8be985d2feb009`  
		Last Modified: Tue, 13 Sep 2022 02:03:36 GMT  
		Size: 5.0 KB (5021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9a227f323eed41d16b462d95503000badd5210aa179dd3065f4363fe3a1b9f`  
		Last Modified: Tue, 13 Sep 2022 02:03:36 GMT  
		Size: 324.2 KB (324172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36fb60d78f8bd69265b4c2d2246169797772da4584f6e063d49eab9c2f040c51`  
		Last Modified: Tue, 13 Sep 2022 02:03:36 GMT  
		Size: 1.2 MB (1241470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d23a9497c5fd3ec0d26f920c59f1f1628999ae546bd1b2f722b29fbf27e3402`  
		Last Modified: Tue, 13 Sep 2022 02:03:36 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009331f552a168c5b26209994b10c7684fc80fe6348a406878b2262037e82435`  
		Last Modified: Tue, 13 Sep 2022 02:03:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
