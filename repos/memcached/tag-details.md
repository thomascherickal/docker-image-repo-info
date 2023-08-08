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
$ docker pull memcached@sha256:daa7eae2d45bc644f697eed288cff1460c73a7b44c291770014eb16c2ef6ff99
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
$ docker pull memcached@sha256:0c8398104f83351267e51ec72b34de06b734f2eca6637c10d246702afff814b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.0 MB (38974916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:354b899e400fa323ffaea769644cc66778676b4f4eeca0e3e1523100e8803d97`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:44 GMT
ADD file:209589a8bdb5a3788ee42ecdbccbbb561835dab96b0d8286bb5a2229d2f41be7 in / 
# Thu, 27 Jul 2023 23:24:45 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 04:03:18 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 28 Jul 2023 04:03:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 04:03:22 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 28 Jul 2023 04:03:22 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 28 Jul 2023 04:05:37 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 28 Jul 2023 04:05:37 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 28 Jul 2023 04:05:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 04:05:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 04:05:38 GMT
USER memcache
# Fri, 28 Jul 2023 04:05:38 GMT
EXPOSE 11211
# Fri, 28 Jul 2023 04:05:38 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:648e0aadf75ac2ef63c5390adc6dc14fde37a5ad88c2870ea604df0a9c0eb4e5`  
		Last Modified: Thu, 27 Jul 2023 23:29:26 GMT  
		Size: 29.1 MB (29124532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baaf8e9cef6b92919a723712ed912794373f6fc1d8dac9d5ed1d320378f657ba`  
		Last Modified: Fri, 28 Jul 2023 04:05:56 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52dca4bf886a56187b224e812b7a65f7825798dc8d536db9bb9344cb112b98e0`  
		Last Modified: Fri, 28 Jul 2023 04:05:56 GMT  
		Size: 2.7 MB (2677283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6861252b28dd75ed1a4f9accdcef6f35366a5dd59d3d7921945a20ec3f64661`  
		Last Modified: Fri, 28 Jul 2023 04:05:57 GMT  
		Size: 7.2 MB (7171562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49870ab6c52b8db6c693e18bd63b718827cd451bde693287ca70314a991cbfb6`  
		Last Modified: Fri, 28 Jul 2023 04:05:56 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da541564580ce27d2c3710f1420b22d4bc544196f1bf6536a5c58150854283d`  
		Last Modified: Fri, 28 Jul 2023 04:05:56 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; arm variant v5

```console
$ docker pull memcached@sha256:ec7dc6727737267a059c047a43864e1c5bdda0a6b8d3cdd0b49110523acfe7f7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35098422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8ce1a3d6a1d0c9162fa735664905dded291bfaa1a0398a381448950a7b9ee91`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 27 Jul 2023 23:48:29 GMT
ADD file:53cf36eb7b72a7e970f4b18af1589402b2900f12e30820cdeccc8bb0c166df80 in / 
# Thu, 27 Jul 2023 23:48:30 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 11:05:31 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 28 Jul 2023 11:05:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 11:05:37 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 28 Jul 2023 11:05:37 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 28 Jul 2023 11:08:31 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 28 Jul 2023 11:08:31 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 28 Jul 2023 11:08:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 11:08:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 11:08:31 GMT
USER memcache
# Fri, 28 Jul 2023 11:08:31 GMT
EXPOSE 11211
# Fri, 28 Jul 2023 11:08:32 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2bd6dfc5281e13a0ca9fb8d9238ac9f14a0de04489913030c8e33b9398b4a4af`  
		Last Modified: Thu, 27 Jul 2023 23:51:28 GMT  
		Size: 27.0 MB (26983508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5936d9d99182ef30677e20dad76c0549b2b7612ca100ef6c0f03c87027cee0b`  
		Last Modified: Fri, 28 Jul 2023 11:08:45 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7717a35af981145073f1343f8447ffd5b5c52de46680b1e75e4c0c11ba64bf`  
		Last Modified: Fri, 28 Jul 2023 11:08:46 GMT  
		Size: 2.3 MB (2281851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56b5203e649ffe900465b0cf521d6be756bd5dd83b5905d7ccc6aced143610b`  
		Last Modified: Fri, 28 Jul 2023 11:08:47 GMT  
		Size: 5.8 MB (5831523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6dee9c51b3b15c0179684c9c61eebfc3091a8f40afd9714ddae2728364aee4f`  
		Last Modified: Fri, 28 Jul 2023 11:08:45 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51b980bae702ef385ef2cbe3eb556c8377334b4c31c97e39cced7ed58375bc55`  
		Last Modified: Fri, 28 Jul 2023 11:08:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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
$ docker pull memcached@sha256:4b2d19d8c0d48b44b1f24b2ea0e8a62749f05db1bedbe481ff6112db44c703cc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.9 MB (37878121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c74af541d05a0758cbf5f13d5d190f1ab10b86ef5fd75112aa98b0638def7d9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 27 Jul 2023 23:43:00 GMT
ADD file:1de2ba0dc88aa343332814e19adc6b850d08e62c31589fe902b8eb2cb465934e in / 
# Thu, 27 Jul 2023 23:43:00 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 06:38:57 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 28 Jul 2023 06:39:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 06:39:01 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 28 Jul 2023 06:39:01 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 28 Jul 2023 06:41:36 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 28 Jul 2023 06:41:36 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 28 Jul 2023 06:41:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 06:41:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 06:41:37 GMT
USER memcache
# Fri, 28 Jul 2023 06:41:37 GMT
EXPOSE 11211
# Fri, 28 Jul 2023 06:41:37 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:90524f7dc01b4ce9b387992acc6cbdbcc2a9ee8c6addfd632429ca06ea18751e`  
		Last Modified: Thu, 27 Jul 2023 23:46:17 GMT  
		Size: 29.2 MB (29157226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6146d0684a3303f06ef62333440ab9aba6cab719b5762ddaee7f7b7a3a62e9ee`  
		Last Modified: Fri, 28 Jul 2023 06:42:01 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b513dbaa02d89264c8df677c8871ec60a8cba234a96d77165fc06157ed2ec1f`  
		Last Modified: Fri, 28 Jul 2023 06:42:01 GMT  
		Size: 2.5 MB (2539192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe211375d2d86acd694c377eeaf6fe900e6f57dadd07e6bd6f21809eab75c53a`  
		Last Modified: Fri, 28 Jul 2023 06:42:02 GMT  
		Size: 6.2 MB (6180162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1b4b070b2921c7d9f5349e7b258c1400ac5d0a1154df0028e634899e86fbda`  
		Last Modified: Fri, 28 Jul 2023 06:42:01 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d40396358d46edf0c2615a77e13da10249786f2546d4a9623e18ec0ce9d6aa91`  
		Last Modified: Fri, 28 Jul 2023 06:42:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; 386

```console
$ docker pull memcached@sha256:d3e70a847a7f720a3a129c6e060b3f9b3428add5e0458c1974a6a895783073e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39459484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fe4fee0ccc34611e17f9be47d4048890aa66e445397fb679f2f27edcb5de08a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 27 Jul 2023 23:38:56 GMT
ADD file:3d6e6f3e900e480a7e060fcaf57313c0f954bf906967a7fa0317567c387cf5aa in / 
# Thu, 27 Jul 2023 23:38:57 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 00:12:30 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 28 Jul 2023 00:12:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 00:12:35 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 28 Jul 2023 00:12:35 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 28 Jul 2023 00:16:17 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 28 Jul 2023 00:16:17 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 28 Jul 2023 00:16:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 00:16:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 00:16:18 GMT
USER memcache
# Fri, 28 Jul 2023 00:16:18 GMT
EXPOSE 11211
# Fri, 28 Jul 2023 00:16:18 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3a8b0c4b1a83609d978d576be6174f951ff27084d7c9aef91892b60b223a5104`  
		Last Modified: Thu, 27 Jul 2023 23:43:26 GMT  
		Size: 30.1 MB (30141788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:700ff590600873a2721ed53371f8797b79c09c48cf32c7190640b4a1d4f5755d`  
		Last Modified: Fri, 28 Jul 2023 00:16:36 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f15bfc1eebf505da6ff5a5b1b1810ad762b79725e742a9b354c57fbabd31f01a`  
		Last Modified: Fri, 28 Jul 2023 00:16:37 GMT  
		Size: 2.7 MB (2685093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80fdef0976acae3ce13d23a176fc9e9ce15eeb2ac874a0915725bbaa3108059b`  
		Last Modified: Fri, 28 Jul 2023 00:16:38 GMT  
		Size: 6.6 MB (6631063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3442227f7348458fb36b2e0d739658a8fb589ed322fd578df8e39e59fc32000d`  
		Last Modified: Fri, 28 Jul 2023 00:16:36 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5501a93139182f8a01992f6de5a5e4eaebdebaaec5a10506a07f59b936d266e6`  
		Last Modified: Fri, 28 Jul 2023 00:16:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; mips64le

```console
$ docker pull memcached@sha256:fbc5c08e8c901f9b6c9cab47733639d29f3ff1167ab861aa26fe0bb751a308d9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.6 MB (37558667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f390b2a92aa8ce938675a24263c1e7f6b619c4c584343f3dd7a0e9d6615051d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 27 Jul 2023 23:11:23 GMT
ADD file:90cbcf9a2aaf48a433b00118dd0821eeb291092da7b7f67ce6a525ce2cba1e3f in / 
# Thu, 27 Jul 2023 23:11:27 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:45:56 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 28 Jul 2023 01:46:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:46:17 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 28 Jul 2023 01:46:19 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 28 Jul 2023 01:53:01 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 28 Jul 2023 01:53:03 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 28 Jul 2023 01:53:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 01:53:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 01:53:14 GMT
USER memcache
# Fri, 28 Jul 2023 01:53:16 GMT
EXPOSE 11211
# Fri, 28 Jul 2023 01:53:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3252778e08fa8eb67ab052ad63281284b5ef1afdc40a36021228133487ab5d52`  
		Last Modified: Thu, 27 Jul 2023 23:22:26 GMT  
		Size: 29.1 MB (29121405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63e55e013f2ab63ff93eaaf154b0debea8de9ffc8fbadaf67d3bc03851f57910`  
		Last Modified: Fri, 28 Jul 2023 01:53:46 GMT  
		Size: 1.1 KB (1082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d9a9f24853cb0188d2273603847b46ed81bd544b868ae314d609c1d9e7db7c`  
		Last Modified: Fri, 28 Jul 2023 01:53:48 GMT  
		Size: 1.9 MB (1934904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4467025968ec633fd090be17fe8c5f61d7ee738a0b34a10db006d35397e27cc`  
		Last Modified: Fri, 28 Jul 2023 01:53:51 GMT  
		Size: 6.5 MB (6500867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07da0cd083ab7d3e91ac9e7ae33d316bd7affeb2852262ff2d687be0e5c273b6`  
		Last Modified: Fri, 28 Jul 2023 01:53:46 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57f5929847506e0cf79067f8348bd883548c83f0c23defbaccf512eb17d65758`  
		Last Modified: Fri, 28 Jul 2023 01:53:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; ppc64le

```console
$ docker pull memcached@sha256:a32969620e95d4b08d5711678e6bcbd313e3bc3511d1b96cf5d08e675a90d0fb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43196803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d6a8d8d3e6746723698507be3f910bb02f0a22617da462f56031004e606edf6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 27 Jul 2023 23:23:01 GMT
ADD file:774a99e5c40757d27c981eb5ad6e03eb72970bb0c54f799eab1442624238ea3e in / 
# Thu, 27 Jul 2023 23:23:03 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:38:39 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 28 Jul 2023 03:38:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:38:51 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 28 Jul 2023 03:38:52 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 28 Jul 2023 03:42:57 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 28 Jul 2023 03:42:58 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 28 Jul 2023 03:43:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 03:43:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 03:43:01 GMT
USER memcache
# Fri, 28 Jul 2023 03:43:02 GMT
EXPOSE 11211
# Fri, 28 Jul 2023 03:43:03 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:ad974e0ada84177d519dec70d0d7d9ff6a4f468bc7306425feb8429bc276bd8a`  
		Last Modified: Thu, 27 Jul 2023 23:29:24 GMT  
		Size: 33.1 MB (33119211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ed68aff2ca1a6e8c25d8462f4b2ebbb3866c768911785569560ede6a2f053d`  
		Last Modified: Fri, 28 Jul 2023 03:43:33 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d519acbf803e11e9a1e21f396dd4e021495fa7b97a4c9df3e6f7639d8c050790`  
		Last Modified: Fri, 28 Jul 2023 03:43:33 GMT  
		Size: 2.9 MB (2891351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:097534b38ed1845470192cab29ec2d22d4e0c7a9d5f01c9948ebc1273dfe809c`  
		Last Modified: Fri, 28 Jul 2023 03:43:35 GMT  
		Size: 7.2 MB (7184700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2f9c6ce8e611c611c0bfdb7cb8ec798950618d80a9be8db98c59fdd0654825`  
		Last Modified: Fri, 28 Jul 2023 03:43:33 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d974aa6a849abcd290ae3bbfbc44f776e3928269bfa1bdbc65e2a1f11c368afe`  
		Last Modified: Fri, 28 Jul 2023 03:43:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1` - linux; s390x

```console
$ docker pull memcached@sha256:1ab909233ee99a6798929725205b93abb2bd9a8c78ab048d925dffd359fe8cf2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35910248 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:845b0ff32d8c04c5820146361e7a2e8c8579ad2a96318fdbc7e6c669bfc27569`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 27 Jul 2023 23:47:11 GMT
ADD file:0a5e1e86b375d60637d0829f77a12085777cf2ca07495b0f6249d8efea84e958 in / 
# Thu, 27 Jul 2023 23:47:13 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 02:58:10 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 28 Jul 2023 02:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 02:58:13 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 28 Jul 2023 02:58:13 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 28 Jul 2023 03:01:19 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 28 Jul 2023 03:01:20 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 28 Jul 2023 03:01:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 03:01:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 03:01:20 GMT
USER memcache
# Fri, 28 Jul 2023 03:01:20 GMT
EXPOSE 11211
# Fri, 28 Jul 2023 03:01:21 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f4301d25bb1bea85fcc5b364aec84ff58274f714cea191ab22d9b1b1e4f78527`  
		Last Modified: Thu, 27 Jul 2023 23:52:17 GMT  
		Size: 27.5 MB (27489697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8055eb96c9dacdcc9c91194a8d4504ab82a88a0fa9f927413c1dde2e493a815`  
		Last Modified: Fri, 28 Jul 2023 03:01:51 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:040e9d91e418b36f9ea07fcd1d9db85ae7713bd99a0a17f31f41a7ef410c3423`  
		Last Modified: Fri, 28 Jul 2023 03:01:54 GMT  
		Size: 2.3 MB (2345395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a638c5b62a02bc60b52234e1556bcf148e66b74e50a0bd02d2b5f23ea2ee136d`  
		Last Modified: Fri, 28 Jul 2023 03:01:52 GMT  
		Size: 6.1 MB (6073620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c41c8e1cb6d4df65052cc47729124edceae5af653ff6a3555cf6e69a57f6de1`  
		Last Modified: Fri, 28 Jul 2023 03:01:51 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2516714a4b2b11720bd2fcf5338749e05ae2dff40f716814b7531fcbe356fdce`  
		Last Modified: Fri, 28 Jul 2023 03:01:51 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1-alpine`

```console
$ docker pull memcached@sha256:bb610e3fb1dcd27fa39cf120269b71ab32f1202deb4b517a2b80f17fe90beb5f
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
$ docker pull memcached@sha256:574ef430513a38925cc52ae5954677a12e0a57205fed96be5707196a180e5159
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4462428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f7da63106561ab1f7284992dad2396b234096070b4269971b23c53f2f8498ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:50:58 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Wed, 14 Jun 2023 20:50:59 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 01:07:13 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 01:07:13 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:09:21 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 01:09:21 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:09:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:09:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:09:22 GMT
USER memcache
# Wed, 21 Jun 2023 01:09:22 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:09:22 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b2b2df106c5026cd33ea4ac655b77f25410ec9f4b8a6756ebc1ceeb79fca3c7`  
		Last Modified: Wed, 14 Jun 2023 20:53:58 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed63668528d3e2159f55909c66dc48a6f746ce24c2e2f6d963b992aefaa457ce`  
		Last Modified: Wed, 14 Jun 2023 20:53:58 GMT  
		Size: 108.1 KB (108080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05536f2f26c904a5aa1b07720957a37e8b57a223725d76f8d1473dcab297a233`  
		Last Modified: Wed, 21 Jun 2023 01:10:14 GMT  
		Size: 954.8 KB (954811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e448b573a98adc8bd0a4805cb0e1b451aea0d1582f0462aa0b147799a97fad7`  
		Last Modified: Wed, 21 Jun 2023 01:10:13 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3029a709b7be20aeff1e9cebe5c6112cd1df5a0ea3efb58e61380cc75b9296e`  
		Last Modified: Wed, 21 Jun 2023 01:10:13 GMT  
		Size: 117.0 B  
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
$ docker pull memcached@sha256:eb4b801b9c9e9af6565ac003b21af39b06d55943bbc4e59a02d465fdf7f07776
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4399342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4aa99dd98a2fa001241d907951530f4afebadfd4895545c5d73f31e29b7a35fa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:57:26 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Wed, 14 Jun 2023 20:57:27 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 01:08:09 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 01:08:09 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:10:35 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 01:10:35 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:10:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:10:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:10:36 GMT
USER memcache
# Wed, 21 Jun 2023 01:10:36 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:10:36 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666588188768f19b27fb821e02d084406af8fd867cc4595b896b9eed50b2105e`  
		Last Modified: Wed, 14 Jun 2023 21:00:51 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d958a137d671266f063c0af4d7b0b6d44d9018b77fdbddb8fd412d3c0b1be3`  
		Last Modified: Wed, 14 Jun 2023 21:00:51 GMT  
		Size: 124.1 KB (124137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66841dcfe05dcef1af82648941fa1ea0e10dbdf022326916d1d74afc99885c6`  
		Last Modified: Wed, 21 Jun 2023 01:11:21 GMT  
		Size: 944.3 KB (944292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b46fdc76bcbc8fa94ae23177ac32b97a4d370a630ec7d3f52bd8aae174e75982`  
		Last Modified: Wed, 21 Jun 2023 01:11:20 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea70db1a59f508c629aef54fb39ac3ada5cfcc3aac7aa1d6ed6cde22e97d3e3b`  
		Last Modified: Wed, 21 Jun 2023 01:11:20 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; 386

```console
$ docker pull memcached@sha256:1468666da56924eda85c3bbc484ce7835f472fd27dd171a5bb32b2c929ef52b7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4283458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7cc593f180f84bb7bdbcb9e4b50cbc7d3c3bc0f5a83d2b6b9abce4758814bb0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 07 Aug 2023 19:38:26 GMT
ADD file:4b33c52e11b19fde30197c62ead0b77bde28d34edaa08346a5302cd892d3cebe in / 
# Mon, 07 Aug 2023 19:38:27 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 21:40:23 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Mon, 07 Aug 2023 21:40:25 GMT
RUN apk add --no-cache libsasl
# Mon, 07 Aug 2023 21:40:25 GMT
ENV MEMCACHED_VERSION=1.6.21
# Mon, 07 Aug 2023 21:40:25 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Mon, 07 Aug 2023 21:43:52 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Mon, 07 Aug 2023 21:43:52 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 07 Aug 2023 21:43:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 07 Aug 2023 21:43:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 21:43:53 GMT
USER memcache
# Mon, 07 Aug 2023 21:43:53 GMT
EXPOSE 11211
# Mon, 07 Aug 2023 21:43:53 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:95dc695758361a4038a2d9026959d72e1f531114edb0341be7ce47d912ef069e`  
		Last Modified: Mon, 07 Aug 2023 19:38:56 GMT  
		Size: 3.2 MB (3235144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:038b25459839e567ceb29349d695abf1d64f7664699e6ac0f4ea807603c54220`  
		Last Modified: Mon, 07 Aug 2023 21:44:17 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ed277dfdfb7162fb18aa73173b2a45185a326869f4ad568557b667d337b8b1`  
		Last Modified: Mon, 07 Aug 2023 21:44:17 GMT  
		Size: 109.5 KB (109531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e1b11e58caccee0d368106698c71335d98063d4ed22c19c716d2da506ddef4`  
		Last Modified: Mon, 07 Aug 2023 21:44:17 GMT  
		Size: 937.1 KB (937114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5f84ab2372dcf436661f4f50a1a95ec0e21e7bdb30ebb567b68f7c443dae44`  
		Last Modified: Mon, 07 Aug 2023 21:44:17 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa27df056ec91886a0dd6eb3b95024a3d02bb1b20b887da0525621d78d880a2`  
		Last Modified: Mon, 07 Aug 2023 21:44:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:ed70e3e81930652804f6d430c71ed014f9daff26aa4ad302cd37c04a8ef038de
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4454755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ddfb07c34bdda47806fc2cec7489bef9f20f0e4d6d47f4c99dbf139dbd4700d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:25 GMT
ADD file:b8cf7516cdf9487d9347da0b5b5e3a6f65f24ebcdcadf81f430adb2b2664f2d1 in / 
# Mon, 07 Aug 2023 20:16:26 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 00:46:29 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 08 Aug 2023 00:46:31 GMT
RUN apk add --no-cache libsasl
# Tue, 08 Aug 2023 00:46:32 GMT
ENV MEMCACHED_VERSION=1.6.21
# Tue, 08 Aug 2023 00:46:32 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Tue, 08 Aug 2023 00:49:28 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 08 Aug 2023 00:49:28 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Aug 2023 00:49:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Aug 2023 00:49:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Aug 2023 00:49:39 GMT
USER memcache
# Tue, 08 Aug 2023 00:49:41 GMT
EXPOSE 11211
# Tue, 08 Aug 2023 00:49:43 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:55353ca330e9474ce7b858eca6842bb540ef4a70b2981c2ed47eefb9ef4253ad`  
		Last Modified: Mon, 07 Aug 2023 20:17:20 GMT  
		Size: 3.3 MB (3346251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05163a2a65d29a4d5c99749b9902892698d3b79714d37728f6a9e2f7a2c58441`  
		Last Modified: Tue, 08 Aug 2023 00:50:16 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823f7ceea96296f95c9085f083e8083413bcc70fcd4cf20b04543ab718b3419c`  
		Last Modified: Tue, 08 Aug 2023 00:50:16 GMT  
		Size: 123.9 KB (123936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a31a6f6c857bb6d5975504a61cbdfd4142af5d54776b833e03644c98433f216e`  
		Last Modified: Tue, 08 Aug 2023 00:50:18 GMT  
		Size: 982.9 KB (982892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721f4e8ef111056d9b345692fa8573c6486de7e886c2d2333e068e0bfc6e24c2`  
		Last Modified: Tue, 08 Aug 2023 00:50:16 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c144e3114e36623a8cdb3fd49d5b274689ac0d8ac00d9e1e10c402670090de1c`  
		Last Modified: Tue, 08 Aug 2023 00:50:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine` - linux; s390x

```console
$ docker pull memcached@sha256:cd97d93e79c2345a0c10f20a912f29a0ccf5590e15c00df81596397b9567233f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4278263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f56d14fce8cfd200c86bd00cd28c95574b6bf2863bd203e7644d44a08db84ab`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 15 Jun 2023 05:18:38 GMT
ADD file:a59beca78118ebf4f86cc1685237dc3a29a519401a70668da520beaa3d29eb7a in / 
# Thu, 15 Jun 2023 05:18:38 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:27:47 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 15 Jun 2023 06:27:49 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 00:58:01 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 00:58:01 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:01:08 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 01:01:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:01:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:01:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:01:09 GMT
USER memcache
# Wed, 21 Jun 2023 01:01:10 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:01:10 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:998cc98447b44e5f0fe799dce691412796ba586ab22eb7c99aebf9d45f34833b`  
		Last Modified: Thu, 15 Jun 2023 05:29:38 GMT  
		Size: 3.2 MB (3213497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156deb87465a2c5629e5ae28c2a7251d5684baea5a930cf65ff6b478de321202`  
		Last Modified: Thu, 15 Jun 2023 06:36:33 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19020c60d58f4724218660e819b1b33b5d1428c3c5027492a2ee3c44228231df`  
		Last Modified: Thu, 15 Jun 2023 06:36:33 GMT  
		Size: 112.8 KB (112849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e76f938f015ccb0b5d2915145432efbc0af21a2f4964e0c9a67bfbbe6a577e`  
		Last Modified: Wed, 21 Jun 2023 01:01:46 GMT  
		Size: 950.3 KB (950254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b613e0a69ced3425a5949c15688d493ef10d80eb28c7bb626f0c092223fe1302`  
		Last Modified: Wed, 21 Jun 2023 01:01:46 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db4c30d38bb65cd11068e1892913b2fa04add8f27abe601485cc3b09754eb50`  
		Last Modified: Wed, 21 Jun 2023 01:01:46 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1-alpine3.18`

```console
$ docker pull memcached@sha256:8ac412315105d6fa923db09279b93ee601a4c2348b9f3fd1ccb9aa6f1562d612
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1-alpine3.18` - linux; amd64

```console
$ docker pull memcached@sha256:574ef430513a38925cc52ae5954677a12e0a57205fed96be5707196a180e5159
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4462428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f7da63106561ab1f7284992dad2396b234096070b4269971b23c53f2f8498ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:50:58 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Wed, 14 Jun 2023 20:50:59 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 01:07:13 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 01:07:13 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:09:21 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 01:09:21 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:09:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:09:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:09:22 GMT
USER memcache
# Wed, 21 Jun 2023 01:09:22 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:09:22 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b2b2df106c5026cd33ea4ac655b77f25410ec9f4b8a6756ebc1ceeb79fca3c7`  
		Last Modified: Wed, 14 Jun 2023 20:53:58 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed63668528d3e2159f55909c66dc48a6f746ce24c2e2f6d963b992aefaa457ce`  
		Last Modified: Wed, 14 Jun 2023 20:53:58 GMT  
		Size: 108.1 KB (108080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05536f2f26c904a5aa1b07720957a37e8b57a223725d76f8d1473dcab297a233`  
		Last Modified: Wed, 21 Jun 2023 01:10:14 GMT  
		Size: 954.8 KB (954811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e448b573a98adc8bd0a4805cb0e1b451aea0d1582f0462aa0b147799a97fad7`  
		Last Modified: Wed, 21 Jun 2023 01:10:13 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3029a709b7be20aeff1e9cebe5c6112cd1df5a0ea3efb58e61380cc75b9296e`  
		Last Modified: Wed, 21 Jun 2023 01:10:13 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:eb4b801b9c9e9af6565ac003b21af39b06d55943bbc4e59a02d465fdf7f07776
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4399342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4aa99dd98a2fa001241d907951530f4afebadfd4895545c5d73f31e29b7a35fa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:57:26 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Wed, 14 Jun 2023 20:57:27 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 01:08:09 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 01:08:09 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:10:35 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 01:10:35 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:10:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:10:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:10:36 GMT
USER memcache
# Wed, 21 Jun 2023 01:10:36 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:10:36 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666588188768f19b27fb821e02d084406af8fd867cc4595b896b9eed50b2105e`  
		Last Modified: Wed, 14 Jun 2023 21:00:51 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d958a137d671266f063c0af4d7b0b6d44d9018b77fdbddb8fd412d3c0b1be3`  
		Last Modified: Wed, 14 Jun 2023 21:00:51 GMT  
		Size: 124.1 KB (124137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66841dcfe05dcef1af82648941fa1ea0e10dbdf022326916d1d74afc99885c6`  
		Last Modified: Wed, 21 Jun 2023 01:11:21 GMT  
		Size: 944.3 KB (944292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b46fdc76bcbc8fa94ae23177ac32b97a4d370a630ec7d3f52bd8aae174e75982`  
		Last Modified: Wed, 21 Jun 2023 01:11:20 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea70db1a59f508c629aef54fb39ac3ada5cfcc3aac7aa1d6ed6cde22e97d3e3b`  
		Last Modified: Wed, 21 Jun 2023 01:11:20 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.18` - linux; 386

```console
$ docker pull memcached@sha256:1468666da56924eda85c3bbc484ce7835f472fd27dd171a5bb32b2c929ef52b7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4283458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7cc593f180f84bb7bdbcb9e4b50cbc7d3c3bc0f5a83d2b6b9abce4758814bb0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 07 Aug 2023 19:38:26 GMT
ADD file:4b33c52e11b19fde30197c62ead0b77bde28d34edaa08346a5302cd892d3cebe in / 
# Mon, 07 Aug 2023 19:38:27 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 21:40:23 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Mon, 07 Aug 2023 21:40:25 GMT
RUN apk add --no-cache libsasl
# Mon, 07 Aug 2023 21:40:25 GMT
ENV MEMCACHED_VERSION=1.6.21
# Mon, 07 Aug 2023 21:40:25 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Mon, 07 Aug 2023 21:43:52 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Mon, 07 Aug 2023 21:43:52 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 07 Aug 2023 21:43:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 07 Aug 2023 21:43:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 21:43:53 GMT
USER memcache
# Mon, 07 Aug 2023 21:43:53 GMT
EXPOSE 11211
# Mon, 07 Aug 2023 21:43:53 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:95dc695758361a4038a2d9026959d72e1f531114edb0341be7ce47d912ef069e`  
		Last Modified: Mon, 07 Aug 2023 19:38:56 GMT  
		Size: 3.2 MB (3235144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:038b25459839e567ceb29349d695abf1d64f7664699e6ac0f4ea807603c54220`  
		Last Modified: Mon, 07 Aug 2023 21:44:17 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ed277dfdfb7162fb18aa73173b2a45185a326869f4ad568557b667d337b8b1`  
		Last Modified: Mon, 07 Aug 2023 21:44:17 GMT  
		Size: 109.5 KB (109531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e1b11e58caccee0d368106698c71335d98063d4ed22c19c716d2da506ddef4`  
		Last Modified: Mon, 07 Aug 2023 21:44:17 GMT  
		Size: 937.1 KB (937114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5f84ab2372dcf436661f4f50a1a95ec0e21e7bdb30ebb567b68f7c443dae44`  
		Last Modified: Mon, 07 Aug 2023 21:44:17 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa27df056ec91886a0dd6eb3b95024a3d02bb1b20b887da0525621d78d880a2`  
		Last Modified: Mon, 07 Aug 2023 21:44:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.18` - linux; ppc64le

```console
$ docker pull memcached@sha256:ed70e3e81930652804f6d430c71ed014f9daff26aa4ad302cd37c04a8ef038de
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4454755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ddfb07c34bdda47806fc2cec7489bef9f20f0e4d6d47f4c99dbf139dbd4700d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:25 GMT
ADD file:b8cf7516cdf9487d9347da0b5b5e3a6f65f24ebcdcadf81f430adb2b2664f2d1 in / 
# Mon, 07 Aug 2023 20:16:26 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 00:46:29 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 08 Aug 2023 00:46:31 GMT
RUN apk add --no-cache libsasl
# Tue, 08 Aug 2023 00:46:32 GMT
ENV MEMCACHED_VERSION=1.6.21
# Tue, 08 Aug 2023 00:46:32 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Tue, 08 Aug 2023 00:49:28 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 08 Aug 2023 00:49:28 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Aug 2023 00:49:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Aug 2023 00:49:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Aug 2023 00:49:39 GMT
USER memcache
# Tue, 08 Aug 2023 00:49:41 GMT
EXPOSE 11211
# Tue, 08 Aug 2023 00:49:43 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:55353ca330e9474ce7b858eca6842bb540ef4a70b2981c2ed47eefb9ef4253ad`  
		Last Modified: Mon, 07 Aug 2023 20:17:20 GMT  
		Size: 3.3 MB (3346251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05163a2a65d29a4d5c99749b9902892698d3b79714d37728f6a9e2f7a2c58441`  
		Last Modified: Tue, 08 Aug 2023 00:50:16 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823f7ceea96296f95c9085f083e8083413bcc70fcd4cf20b04543ab718b3419c`  
		Last Modified: Tue, 08 Aug 2023 00:50:16 GMT  
		Size: 123.9 KB (123936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a31a6f6c857bb6d5975504a61cbdfd4142af5d54776b833e03644c98433f216e`  
		Last Modified: Tue, 08 Aug 2023 00:50:18 GMT  
		Size: 982.9 KB (982892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721f4e8ef111056d9b345692fa8573c6486de7e886c2d2333e068e0bfc6e24c2`  
		Last Modified: Tue, 08 Aug 2023 00:50:16 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c144e3114e36623a8cdb3fd49d5b274689ac0d8ac00d9e1e10c402670090de1c`  
		Last Modified: Tue, 08 Aug 2023 00:50:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-alpine3.18` - linux; s390x

```console
$ docker pull memcached@sha256:cd97d93e79c2345a0c10f20a912f29a0ccf5590e15c00df81596397b9567233f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4278263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f56d14fce8cfd200c86bd00cd28c95574b6bf2863bd203e7644d44a08db84ab`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 15 Jun 2023 05:18:38 GMT
ADD file:a59beca78118ebf4f86cc1685237dc3a29a519401a70668da520beaa3d29eb7a in / 
# Thu, 15 Jun 2023 05:18:38 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:27:47 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 15 Jun 2023 06:27:49 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 00:58:01 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 00:58:01 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:01:08 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 01:01:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:01:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:01:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:01:09 GMT
USER memcache
# Wed, 21 Jun 2023 01:01:10 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:01:10 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:998cc98447b44e5f0fe799dce691412796ba586ab22eb7c99aebf9d45f34833b`  
		Last Modified: Thu, 15 Jun 2023 05:29:38 GMT  
		Size: 3.2 MB (3213497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156deb87465a2c5629e5ae28c2a7251d5684baea5a930cf65ff6b478de321202`  
		Last Modified: Thu, 15 Jun 2023 06:36:33 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19020c60d58f4724218660e819b1b33b5d1428c3c5027492a2ee3c44228231df`  
		Last Modified: Thu, 15 Jun 2023 06:36:33 GMT  
		Size: 112.8 KB (112849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e76f938f015ccb0b5d2915145432efbc0af21a2f4964e0c9a67bfbbe6a577e`  
		Last Modified: Wed, 21 Jun 2023 01:01:46 GMT  
		Size: 950.3 KB (950254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b613e0a69ced3425a5949c15688d493ef10d80eb28c7bb626f0c092223fe1302`  
		Last Modified: Wed, 21 Jun 2023 01:01:46 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db4c30d38bb65cd11068e1892913b2fa04add8f27abe601485cc3b09754eb50`  
		Last Modified: Wed, 21 Jun 2023 01:01:46 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1-bookworm`

```console
$ docker pull memcached@sha256:a917777975a7039b6ed70ef2faab453b1e5ea7aa741899aba952d744546cc781
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1-bookworm` - linux; amd64

```console
$ docker pull memcached@sha256:0c8398104f83351267e51ec72b34de06b734f2eca6637c10d246702afff814b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.0 MB (38974916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:354b899e400fa323ffaea769644cc66778676b4f4eeca0e3e1523100e8803d97`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:44 GMT
ADD file:209589a8bdb5a3788ee42ecdbccbbb561835dab96b0d8286bb5a2229d2f41be7 in / 
# Thu, 27 Jul 2023 23:24:45 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 04:03:18 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 28 Jul 2023 04:03:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 04:03:22 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 28 Jul 2023 04:03:22 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 28 Jul 2023 04:05:37 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 28 Jul 2023 04:05:37 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 28 Jul 2023 04:05:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 04:05:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 04:05:38 GMT
USER memcache
# Fri, 28 Jul 2023 04:05:38 GMT
EXPOSE 11211
# Fri, 28 Jul 2023 04:05:38 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:648e0aadf75ac2ef63c5390adc6dc14fde37a5ad88c2870ea604df0a9c0eb4e5`  
		Last Modified: Thu, 27 Jul 2023 23:29:26 GMT  
		Size: 29.1 MB (29124532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baaf8e9cef6b92919a723712ed912794373f6fc1d8dac9d5ed1d320378f657ba`  
		Last Modified: Fri, 28 Jul 2023 04:05:56 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52dca4bf886a56187b224e812b7a65f7825798dc8d536db9bb9344cb112b98e0`  
		Last Modified: Fri, 28 Jul 2023 04:05:56 GMT  
		Size: 2.7 MB (2677283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6861252b28dd75ed1a4f9accdcef6f35366a5dd59d3d7921945a20ec3f64661`  
		Last Modified: Fri, 28 Jul 2023 04:05:57 GMT  
		Size: 7.2 MB (7171562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49870ab6c52b8db6c693e18bd63b718827cd451bde693287ca70314a991cbfb6`  
		Last Modified: Fri, 28 Jul 2023 04:05:56 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da541564580ce27d2c3710f1420b22d4bc544196f1bf6536a5c58150854283d`  
		Last Modified: Fri, 28 Jul 2023 04:05:56 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bookworm` - linux; arm variant v5

```console
$ docker pull memcached@sha256:ec7dc6727737267a059c047a43864e1c5bdda0a6b8d3cdd0b49110523acfe7f7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35098422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8ce1a3d6a1d0c9162fa735664905dded291bfaa1a0398a381448950a7b9ee91`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 27 Jul 2023 23:48:29 GMT
ADD file:53cf36eb7b72a7e970f4b18af1589402b2900f12e30820cdeccc8bb0c166df80 in / 
# Thu, 27 Jul 2023 23:48:30 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 11:05:31 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 28 Jul 2023 11:05:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 11:05:37 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 28 Jul 2023 11:05:37 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 28 Jul 2023 11:08:31 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 28 Jul 2023 11:08:31 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 28 Jul 2023 11:08:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 11:08:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 11:08:31 GMT
USER memcache
# Fri, 28 Jul 2023 11:08:31 GMT
EXPOSE 11211
# Fri, 28 Jul 2023 11:08:32 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2bd6dfc5281e13a0ca9fb8d9238ac9f14a0de04489913030c8e33b9398b4a4af`  
		Last Modified: Thu, 27 Jul 2023 23:51:28 GMT  
		Size: 27.0 MB (26983508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5936d9d99182ef30677e20dad76c0549b2b7612ca100ef6c0f03c87027cee0b`  
		Last Modified: Fri, 28 Jul 2023 11:08:45 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7717a35af981145073f1343f8447ffd5b5c52de46680b1e75e4c0c11ba64bf`  
		Last Modified: Fri, 28 Jul 2023 11:08:46 GMT  
		Size: 2.3 MB (2281851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56b5203e649ffe900465b0cf521d6be756bd5dd83b5905d7ccc6aced143610b`  
		Last Modified: Fri, 28 Jul 2023 11:08:47 GMT  
		Size: 5.8 MB (5831523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6dee9c51b3b15c0179684c9c61eebfc3091a8f40afd9714ddae2728364aee4f`  
		Last Modified: Fri, 28 Jul 2023 11:08:45 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51b980bae702ef385ef2cbe3eb556c8377334b4c31c97e39cced7ed58375bc55`  
		Last Modified: Fri, 28 Jul 2023 11:08:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bookworm` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:4b2d19d8c0d48b44b1f24b2ea0e8a62749f05db1bedbe481ff6112db44c703cc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.9 MB (37878121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c74af541d05a0758cbf5f13d5d190f1ab10b86ef5fd75112aa98b0638def7d9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 27 Jul 2023 23:43:00 GMT
ADD file:1de2ba0dc88aa343332814e19adc6b850d08e62c31589fe902b8eb2cb465934e in / 
# Thu, 27 Jul 2023 23:43:00 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 06:38:57 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 28 Jul 2023 06:39:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 06:39:01 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 28 Jul 2023 06:39:01 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 28 Jul 2023 06:41:36 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 28 Jul 2023 06:41:36 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 28 Jul 2023 06:41:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 06:41:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 06:41:37 GMT
USER memcache
# Fri, 28 Jul 2023 06:41:37 GMT
EXPOSE 11211
# Fri, 28 Jul 2023 06:41:37 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:90524f7dc01b4ce9b387992acc6cbdbcc2a9ee8c6addfd632429ca06ea18751e`  
		Last Modified: Thu, 27 Jul 2023 23:46:17 GMT  
		Size: 29.2 MB (29157226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6146d0684a3303f06ef62333440ab9aba6cab719b5762ddaee7f7b7a3a62e9ee`  
		Last Modified: Fri, 28 Jul 2023 06:42:01 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b513dbaa02d89264c8df677c8871ec60a8cba234a96d77165fc06157ed2ec1f`  
		Last Modified: Fri, 28 Jul 2023 06:42:01 GMT  
		Size: 2.5 MB (2539192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe211375d2d86acd694c377eeaf6fe900e6f57dadd07e6bd6f21809eab75c53a`  
		Last Modified: Fri, 28 Jul 2023 06:42:02 GMT  
		Size: 6.2 MB (6180162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1b4b070b2921c7d9f5349e7b258c1400ac5d0a1154df0028e634899e86fbda`  
		Last Modified: Fri, 28 Jul 2023 06:42:01 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d40396358d46edf0c2615a77e13da10249786f2546d4a9623e18ec0ce9d6aa91`  
		Last Modified: Fri, 28 Jul 2023 06:42:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bookworm` - linux; 386

```console
$ docker pull memcached@sha256:d3e70a847a7f720a3a129c6e060b3f9b3428add5e0458c1974a6a895783073e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39459484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fe4fee0ccc34611e17f9be47d4048890aa66e445397fb679f2f27edcb5de08a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 27 Jul 2023 23:38:56 GMT
ADD file:3d6e6f3e900e480a7e060fcaf57313c0f954bf906967a7fa0317567c387cf5aa in / 
# Thu, 27 Jul 2023 23:38:57 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 00:12:30 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 28 Jul 2023 00:12:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 00:12:35 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 28 Jul 2023 00:12:35 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 28 Jul 2023 00:16:17 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 28 Jul 2023 00:16:17 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 28 Jul 2023 00:16:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 00:16:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 00:16:18 GMT
USER memcache
# Fri, 28 Jul 2023 00:16:18 GMT
EXPOSE 11211
# Fri, 28 Jul 2023 00:16:18 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3a8b0c4b1a83609d978d576be6174f951ff27084d7c9aef91892b60b223a5104`  
		Last Modified: Thu, 27 Jul 2023 23:43:26 GMT  
		Size: 30.1 MB (30141788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:700ff590600873a2721ed53371f8797b79c09c48cf32c7190640b4a1d4f5755d`  
		Last Modified: Fri, 28 Jul 2023 00:16:36 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f15bfc1eebf505da6ff5a5b1b1810ad762b79725e742a9b354c57fbabd31f01a`  
		Last Modified: Fri, 28 Jul 2023 00:16:37 GMT  
		Size: 2.7 MB (2685093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80fdef0976acae3ce13d23a176fc9e9ce15eeb2ac874a0915725bbaa3108059b`  
		Last Modified: Fri, 28 Jul 2023 00:16:38 GMT  
		Size: 6.6 MB (6631063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3442227f7348458fb36b2e0d739658a8fb589ed322fd578df8e39e59fc32000d`  
		Last Modified: Fri, 28 Jul 2023 00:16:36 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5501a93139182f8a01992f6de5a5e4eaebdebaaec5a10506a07f59b936d266e6`  
		Last Modified: Fri, 28 Jul 2023 00:16:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bookworm` - linux; mips64le

```console
$ docker pull memcached@sha256:fbc5c08e8c901f9b6c9cab47733639d29f3ff1167ab861aa26fe0bb751a308d9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.6 MB (37558667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f390b2a92aa8ce938675a24263c1e7f6b619c4c584343f3dd7a0e9d6615051d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 27 Jul 2023 23:11:23 GMT
ADD file:90cbcf9a2aaf48a433b00118dd0821eeb291092da7b7f67ce6a525ce2cba1e3f in / 
# Thu, 27 Jul 2023 23:11:27 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:45:56 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 28 Jul 2023 01:46:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:46:17 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 28 Jul 2023 01:46:19 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 28 Jul 2023 01:53:01 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 28 Jul 2023 01:53:03 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 28 Jul 2023 01:53:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 01:53:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 01:53:14 GMT
USER memcache
# Fri, 28 Jul 2023 01:53:16 GMT
EXPOSE 11211
# Fri, 28 Jul 2023 01:53:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3252778e08fa8eb67ab052ad63281284b5ef1afdc40a36021228133487ab5d52`  
		Last Modified: Thu, 27 Jul 2023 23:22:26 GMT  
		Size: 29.1 MB (29121405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63e55e013f2ab63ff93eaaf154b0debea8de9ffc8fbadaf67d3bc03851f57910`  
		Last Modified: Fri, 28 Jul 2023 01:53:46 GMT  
		Size: 1.1 KB (1082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d9a9f24853cb0188d2273603847b46ed81bd544b868ae314d609c1d9e7db7c`  
		Last Modified: Fri, 28 Jul 2023 01:53:48 GMT  
		Size: 1.9 MB (1934904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4467025968ec633fd090be17fe8c5f61d7ee738a0b34a10db006d35397e27cc`  
		Last Modified: Fri, 28 Jul 2023 01:53:51 GMT  
		Size: 6.5 MB (6500867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07da0cd083ab7d3e91ac9e7ae33d316bd7affeb2852262ff2d687be0e5c273b6`  
		Last Modified: Fri, 28 Jul 2023 01:53:46 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57f5929847506e0cf79067f8348bd883548c83f0c23defbaccf512eb17d65758`  
		Last Modified: Fri, 28 Jul 2023 01:53:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bookworm` - linux; ppc64le

```console
$ docker pull memcached@sha256:a32969620e95d4b08d5711678e6bcbd313e3bc3511d1b96cf5d08e675a90d0fb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43196803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d6a8d8d3e6746723698507be3f910bb02f0a22617da462f56031004e606edf6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 27 Jul 2023 23:23:01 GMT
ADD file:774a99e5c40757d27c981eb5ad6e03eb72970bb0c54f799eab1442624238ea3e in / 
# Thu, 27 Jul 2023 23:23:03 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:38:39 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 28 Jul 2023 03:38:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:38:51 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 28 Jul 2023 03:38:52 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 28 Jul 2023 03:42:57 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 28 Jul 2023 03:42:58 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 28 Jul 2023 03:43:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 03:43:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 03:43:01 GMT
USER memcache
# Fri, 28 Jul 2023 03:43:02 GMT
EXPOSE 11211
# Fri, 28 Jul 2023 03:43:03 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:ad974e0ada84177d519dec70d0d7d9ff6a4f468bc7306425feb8429bc276bd8a`  
		Last Modified: Thu, 27 Jul 2023 23:29:24 GMT  
		Size: 33.1 MB (33119211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ed68aff2ca1a6e8c25d8462f4b2ebbb3866c768911785569560ede6a2f053d`  
		Last Modified: Fri, 28 Jul 2023 03:43:33 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d519acbf803e11e9a1e21f396dd4e021495fa7b97a4c9df3e6f7639d8c050790`  
		Last Modified: Fri, 28 Jul 2023 03:43:33 GMT  
		Size: 2.9 MB (2891351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:097534b38ed1845470192cab29ec2d22d4e0c7a9d5f01c9948ebc1273dfe809c`  
		Last Modified: Fri, 28 Jul 2023 03:43:35 GMT  
		Size: 7.2 MB (7184700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2f9c6ce8e611c611c0bfdb7cb8ec798950618d80a9be8db98c59fdd0654825`  
		Last Modified: Fri, 28 Jul 2023 03:43:33 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d974aa6a849abcd290ae3bbfbc44f776e3928269bfa1bdbc65e2a1f11c368afe`  
		Last Modified: Fri, 28 Jul 2023 03:43:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1-bookworm` - linux; s390x

```console
$ docker pull memcached@sha256:1ab909233ee99a6798929725205b93abb2bd9a8c78ab048d925dffd359fe8cf2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35910248 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:845b0ff32d8c04c5820146361e7a2e8c8579ad2a96318fdbc7e6c669bfc27569`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 27 Jul 2023 23:47:11 GMT
ADD file:0a5e1e86b375d60637d0829f77a12085777cf2ca07495b0f6249d8efea84e958 in / 
# Thu, 27 Jul 2023 23:47:13 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 02:58:10 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 28 Jul 2023 02:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 02:58:13 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 28 Jul 2023 02:58:13 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 28 Jul 2023 03:01:19 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 28 Jul 2023 03:01:20 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 28 Jul 2023 03:01:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 03:01:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 03:01:20 GMT
USER memcache
# Fri, 28 Jul 2023 03:01:20 GMT
EXPOSE 11211
# Fri, 28 Jul 2023 03:01:21 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f4301d25bb1bea85fcc5b364aec84ff58274f714cea191ab22d9b1b1e4f78527`  
		Last Modified: Thu, 27 Jul 2023 23:52:17 GMT  
		Size: 27.5 MB (27489697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8055eb96c9dacdcc9c91194a8d4504ab82a88a0fa9f927413c1dde2e493a815`  
		Last Modified: Fri, 28 Jul 2023 03:01:51 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:040e9d91e418b36f9ea07fcd1d9db85ae7713bd99a0a17f31f41a7ef410c3423`  
		Last Modified: Fri, 28 Jul 2023 03:01:54 GMT  
		Size: 2.3 MB (2345395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a638c5b62a02bc60b52234e1556bcf148e66b74e50a0bd02d2b5f23ea2ee136d`  
		Last Modified: Fri, 28 Jul 2023 03:01:52 GMT  
		Size: 6.1 MB (6073620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c41c8e1cb6d4df65052cc47729124edceae5af653ff6a3555cf6e69a57f6de1`  
		Last Modified: Fri, 28 Jul 2023 03:01:51 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2516714a4b2b11720bd2fcf5338749e05ae2dff40f716814b7531fcbe356fdce`  
		Last Modified: Fri, 28 Jul 2023 03:01:51 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6`

```console
$ docker pull memcached@sha256:daa7eae2d45bc644f697eed288cff1460c73a7b44c291770014eb16c2ef6ff99
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
$ docker pull memcached@sha256:0c8398104f83351267e51ec72b34de06b734f2eca6637c10d246702afff814b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.0 MB (38974916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:354b899e400fa323ffaea769644cc66778676b4f4eeca0e3e1523100e8803d97`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:44 GMT
ADD file:209589a8bdb5a3788ee42ecdbccbbb561835dab96b0d8286bb5a2229d2f41be7 in / 
# Thu, 27 Jul 2023 23:24:45 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 04:03:18 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 28 Jul 2023 04:03:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 04:03:22 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 28 Jul 2023 04:03:22 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 28 Jul 2023 04:05:37 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 28 Jul 2023 04:05:37 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 28 Jul 2023 04:05:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 04:05:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 04:05:38 GMT
USER memcache
# Fri, 28 Jul 2023 04:05:38 GMT
EXPOSE 11211
# Fri, 28 Jul 2023 04:05:38 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:648e0aadf75ac2ef63c5390adc6dc14fde37a5ad88c2870ea604df0a9c0eb4e5`  
		Last Modified: Thu, 27 Jul 2023 23:29:26 GMT  
		Size: 29.1 MB (29124532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baaf8e9cef6b92919a723712ed912794373f6fc1d8dac9d5ed1d320378f657ba`  
		Last Modified: Fri, 28 Jul 2023 04:05:56 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52dca4bf886a56187b224e812b7a65f7825798dc8d536db9bb9344cb112b98e0`  
		Last Modified: Fri, 28 Jul 2023 04:05:56 GMT  
		Size: 2.7 MB (2677283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6861252b28dd75ed1a4f9accdcef6f35366a5dd59d3d7921945a20ec3f64661`  
		Last Modified: Fri, 28 Jul 2023 04:05:57 GMT  
		Size: 7.2 MB (7171562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49870ab6c52b8db6c693e18bd63b718827cd451bde693287ca70314a991cbfb6`  
		Last Modified: Fri, 28 Jul 2023 04:05:56 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da541564580ce27d2c3710f1420b22d4bc544196f1bf6536a5c58150854283d`  
		Last Modified: Fri, 28 Jul 2023 04:05:56 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; arm variant v5

```console
$ docker pull memcached@sha256:ec7dc6727737267a059c047a43864e1c5bdda0a6b8d3cdd0b49110523acfe7f7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35098422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8ce1a3d6a1d0c9162fa735664905dded291bfaa1a0398a381448950a7b9ee91`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 27 Jul 2023 23:48:29 GMT
ADD file:53cf36eb7b72a7e970f4b18af1589402b2900f12e30820cdeccc8bb0c166df80 in / 
# Thu, 27 Jul 2023 23:48:30 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 11:05:31 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 28 Jul 2023 11:05:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 11:05:37 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 28 Jul 2023 11:05:37 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 28 Jul 2023 11:08:31 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 28 Jul 2023 11:08:31 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 28 Jul 2023 11:08:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 11:08:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 11:08:31 GMT
USER memcache
# Fri, 28 Jul 2023 11:08:31 GMT
EXPOSE 11211
# Fri, 28 Jul 2023 11:08:32 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2bd6dfc5281e13a0ca9fb8d9238ac9f14a0de04489913030c8e33b9398b4a4af`  
		Last Modified: Thu, 27 Jul 2023 23:51:28 GMT  
		Size: 27.0 MB (26983508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5936d9d99182ef30677e20dad76c0549b2b7612ca100ef6c0f03c87027cee0b`  
		Last Modified: Fri, 28 Jul 2023 11:08:45 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7717a35af981145073f1343f8447ffd5b5c52de46680b1e75e4c0c11ba64bf`  
		Last Modified: Fri, 28 Jul 2023 11:08:46 GMT  
		Size: 2.3 MB (2281851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56b5203e649ffe900465b0cf521d6be756bd5dd83b5905d7ccc6aced143610b`  
		Last Modified: Fri, 28 Jul 2023 11:08:47 GMT  
		Size: 5.8 MB (5831523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6dee9c51b3b15c0179684c9c61eebfc3091a8f40afd9714ddae2728364aee4f`  
		Last Modified: Fri, 28 Jul 2023 11:08:45 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51b980bae702ef385ef2cbe3eb556c8377334b4c31c97e39cced7ed58375bc55`  
		Last Modified: Fri, 28 Jul 2023 11:08:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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
$ docker pull memcached@sha256:4b2d19d8c0d48b44b1f24b2ea0e8a62749f05db1bedbe481ff6112db44c703cc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.9 MB (37878121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c74af541d05a0758cbf5f13d5d190f1ab10b86ef5fd75112aa98b0638def7d9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 27 Jul 2023 23:43:00 GMT
ADD file:1de2ba0dc88aa343332814e19adc6b850d08e62c31589fe902b8eb2cb465934e in / 
# Thu, 27 Jul 2023 23:43:00 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 06:38:57 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 28 Jul 2023 06:39:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 06:39:01 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 28 Jul 2023 06:39:01 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 28 Jul 2023 06:41:36 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 28 Jul 2023 06:41:36 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 28 Jul 2023 06:41:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 06:41:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 06:41:37 GMT
USER memcache
# Fri, 28 Jul 2023 06:41:37 GMT
EXPOSE 11211
# Fri, 28 Jul 2023 06:41:37 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:90524f7dc01b4ce9b387992acc6cbdbcc2a9ee8c6addfd632429ca06ea18751e`  
		Last Modified: Thu, 27 Jul 2023 23:46:17 GMT  
		Size: 29.2 MB (29157226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6146d0684a3303f06ef62333440ab9aba6cab719b5762ddaee7f7b7a3a62e9ee`  
		Last Modified: Fri, 28 Jul 2023 06:42:01 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b513dbaa02d89264c8df677c8871ec60a8cba234a96d77165fc06157ed2ec1f`  
		Last Modified: Fri, 28 Jul 2023 06:42:01 GMT  
		Size: 2.5 MB (2539192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe211375d2d86acd694c377eeaf6fe900e6f57dadd07e6bd6f21809eab75c53a`  
		Last Modified: Fri, 28 Jul 2023 06:42:02 GMT  
		Size: 6.2 MB (6180162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1b4b070b2921c7d9f5349e7b258c1400ac5d0a1154df0028e634899e86fbda`  
		Last Modified: Fri, 28 Jul 2023 06:42:01 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d40396358d46edf0c2615a77e13da10249786f2546d4a9623e18ec0ce9d6aa91`  
		Last Modified: Fri, 28 Jul 2023 06:42:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; 386

```console
$ docker pull memcached@sha256:d3e70a847a7f720a3a129c6e060b3f9b3428add5e0458c1974a6a895783073e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39459484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fe4fee0ccc34611e17f9be47d4048890aa66e445397fb679f2f27edcb5de08a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 27 Jul 2023 23:38:56 GMT
ADD file:3d6e6f3e900e480a7e060fcaf57313c0f954bf906967a7fa0317567c387cf5aa in / 
# Thu, 27 Jul 2023 23:38:57 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 00:12:30 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 28 Jul 2023 00:12:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 00:12:35 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 28 Jul 2023 00:12:35 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 28 Jul 2023 00:16:17 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 28 Jul 2023 00:16:17 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 28 Jul 2023 00:16:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 00:16:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 00:16:18 GMT
USER memcache
# Fri, 28 Jul 2023 00:16:18 GMT
EXPOSE 11211
# Fri, 28 Jul 2023 00:16:18 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3a8b0c4b1a83609d978d576be6174f951ff27084d7c9aef91892b60b223a5104`  
		Last Modified: Thu, 27 Jul 2023 23:43:26 GMT  
		Size: 30.1 MB (30141788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:700ff590600873a2721ed53371f8797b79c09c48cf32c7190640b4a1d4f5755d`  
		Last Modified: Fri, 28 Jul 2023 00:16:36 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f15bfc1eebf505da6ff5a5b1b1810ad762b79725e742a9b354c57fbabd31f01a`  
		Last Modified: Fri, 28 Jul 2023 00:16:37 GMT  
		Size: 2.7 MB (2685093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80fdef0976acae3ce13d23a176fc9e9ce15eeb2ac874a0915725bbaa3108059b`  
		Last Modified: Fri, 28 Jul 2023 00:16:38 GMT  
		Size: 6.6 MB (6631063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3442227f7348458fb36b2e0d739658a8fb589ed322fd578df8e39e59fc32000d`  
		Last Modified: Fri, 28 Jul 2023 00:16:36 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5501a93139182f8a01992f6de5a5e4eaebdebaaec5a10506a07f59b936d266e6`  
		Last Modified: Fri, 28 Jul 2023 00:16:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; mips64le

```console
$ docker pull memcached@sha256:fbc5c08e8c901f9b6c9cab47733639d29f3ff1167ab861aa26fe0bb751a308d9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.6 MB (37558667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f390b2a92aa8ce938675a24263c1e7f6b619c4c584343f3dd7a0e9d6615051d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 27 Jul 2023 23:11:23 GMT
ADD file:90cbcf9a2aaf48a433b00118dd0821eeb291092da7b7f67ce6a525ce2cba1e3f in / 
# Thu, 27 Jul 2023 23:11:27 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:45:56 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 28 Jul 2023 01:46:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:46:17 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 28 Jul 2023 01:46:19 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 28 Jul 2023 01:53:01 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 28 Jul 2023 01:53:03 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 28 Jul 2023 01:53:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 01:53:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 01:53:14 GMT
USER memcache
# Fri, 28 Jul 2023 01:53:16 GMT
EXPOSE 11211
# Fri, 28 Jul 2023 01:53:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3252778e08fa8eb67ab052ad63281284b5ef1afdc40a36021228133487ab5d52`  
		Last Modified: Thu, 27 Jul 2023 23:22:26 GMT  
		Size: 29.1 MB (29121405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63e55e013f2ab63ff93eaaf154b0debea8de9ffc8fbadaf67d3bc03851f57910`  
		Last Modified: Fri, 28 Jul 2023 01:53:46 GMT  
		Size: 1.1 KB (1082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d9a9f24853cb0188d2273603847b46ed81bd544b868ae314d609c1d9e7db7c`  
		Last Modified: Fri, 28 Jul 2023 01:53:48 GMT  
		Size: 1.9 MB (1934904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4467025968ec633fd090be17fe8c5f61d7ee738a0b34a10db006d35397e27cc`  
		Last Modified: Fri, 28 Jul 2023 01:53:51 GMT  
		Size: 6.5 MB (6500867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07da0cd083ab7d3e91ac9e7ae33d316bd7affeb2852262ff2d687be0e5c273b6`  
		Last Modified: Fri, 28 Jul 2023 01:53:46 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57f5929847506e0cf79067f8348bd883548c83f0c23defbaccf512eb17d65758`  
		Last Modified: Fri, 28 Jul 2023 01:53:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; ppc64le

```console
$ docker pull memcached@sha256:a32969620e95d4b08d5711678e6bcbd313e3bc3511d1b96cf5d08e675a90d0fb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43196803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d6a8d8d3e6746723698507be3f910bb02f0a22617da462f56031004e606edf6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 27 Jul 2023 23:23:01 GMT
ADD file:774a99e5c40757d27c981eb5ad6e03eb72970bb0c54f799eab1442624238ea3e in / 
# Thu, 27 Jul 2023 23:23:03 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:38:39 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 28 Jul 2023 03:38:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:38:51 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 28 Jul 2023 03:38:52 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 28 Jul 2023 03:42:57 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 28 Jul 2023 03:42:58 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 28 Jul 2023 03:43:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 03:43:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 03:43:01 GMT
USER memcache
# Fri, 28 Jul 2023 03:43:02 GMT
EXPOSE 11211
# Fri, 28 Jul 2023 03:43:03 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:ad974e0ada84177d519dec70d0d7d9ff6a4f468bc7306425feb8429bc276bd8a`  
		Last Modified: Thu, 27 Jul 2023 23:29:24 GMT  
		Size: 33.1 MB (33119211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ed68aff2ca1a6e8c25d8462f4b2ebbb3866c768911785569560ede6a2f053d`  
		Last Modified: Fri, 28 Jul 2023 03:43:33 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d519acbf803e11e9a1e21f396dd4e021495fa7b97a4c9df3e6f7639d8c050790`  
		Last Modified: Fri, 28 Jul 2023 03:43:33 GMT  
		Size: 2.9 MB (2891351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:097534b38ed1845470192cab29ec2d22d4e0c7a9d5f01c9948ebc1273dfe809c`  
		Last Modified: Fri, 28 Jul 2023 03:43:35 GMT  
		Size: 7.2 MB (7184700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2f9c6ce8e611c611c0bfdb7cb8ec798950618d80a9be8db98c59fdd0654825`  
		Last Modified: Fri, 28 Jul 2023 03:43:33 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d974aa6a849abcd290ae3bbfbc44f776e3928269bfa1bdbc65e2a1f11c368afe`  
		Last Modified: Fri, 28 Jul 2023 03:43:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6` - linux; s390x

```console
$ docker pull memcached@sha256:1ab909233ee99a6798929725205b93abb2bd9a8c78ab048d925dffd359fe8cf2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35910248 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:845b0ff32d8c04c5820146361e7a2e8c8579ad2a96318fdbc7e6c669bfc27569`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 27 Jul 2023 23:47:11 GMT
ADD file:0a5e1e86b375d60637d0829f77a12085777cf2ca07495b0f6249d8efea84e958 in / 
# Thu, 27 Jul 2023 23:47:13 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 02:58:10 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 28 Jul 2023 02:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 02:58:13 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 28 Jul 2023 02:58:13 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 28 Jul 2023 03:01:19 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 28 Jul 2023 03:01:20 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 28 Jul 2023 03:01:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 03:01:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 03:01:20 GMT
USER memcache
# Fri, 28 Jul 2023 03:01:20 GMT
EXPOSE 11211
# Fri, 28 Jul 2023 03:01:21 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f4301d25bb1bea85fcc5b364aec84ff58274f714cea191ab22d9b1b1e4f78527`  
		Last Modified: Thu, 27 Jul 2023 23:52:17 GMT  
		Size: 27.5 MB (27489697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8055eb96c9dacdcc9c91194a8d4504ab82a88a0fa9f927413c1dde2e493a815`  
		Last Modified: Fri, 28 Jul 2023 03:01:51 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:040e9d91e418b36f9ea07fcd1d9db85ae7713bd99a0a17f31f41a7ef410c3423`  
		Last Modified: Fri, 28 Jul 2023 03:01:54 GMT  
		Size: 2.3 MB (2345395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a638c5b62a02bc60b52234e1556bcf148e66b74e50a0bd02d2b5f23ea2ee136d`  
		Last Modified: Fri, 28 Jul 2023 03:01:52 GMT  
		Size: 6.1 MB (6073620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c41c8e1cb6d4df65052cc47729124edceae5af653ff6a3555cf6e69a57f6de1`  
		Last Modified: Fri, 28 Jul 2023 03:01:51 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2516714a4b2b11720bd2fcf5338749e05ae2dff40f716814b7531fcbe356fdce`  
		Last Modified: Fri, 28 Jul 2023 03:01:51 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6-alpine`

```console
$ docker pull memcached@sha256:bb610e3fb1dcd27fa39cf120269b71ab32f1202deb4b517a2b80f17fe90beb5f
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
$ docker pull memcached@sha256:574ef430513a38925cc52ae5954677a12e0a57205fed96be5707196a180e5159
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4462428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f7da63106561ab1f7284992dad2396b234096070b4269971b23c53f2f8498ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:50:58 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Wed, 14 Jun 2023 20:50:59 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 01:07:13 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 01:07:13 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:09:21 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 01:09:21 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:09:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:09:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:09:22 GMT
USER memcache
# Wed, 21 Jun 2023 01:09:22 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:09:22 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b2b2df106c5026cd33ea4ac655b77f25410ec9f4b8a6756ebc1ceeb79fca3c7`  
		Last Modified: Wed, 14 Jun 2023 20:53:58 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed63668528d3e2159f55909c66dc48a6f746ce24c2e2f6d963b992aefaa457ce`  
		Last Modified: Wed, 14 Jun 2023 20:53:58 GMT  
		Size: 108.1 KB (108080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05536f2f26c904a5aa1b07720957a37e8b57a223725d76f8d1473dcab297a233`  
		Last Modified: Wed, 21 Jun 2023 01:10:14 GMT  
		Size: 954.8 KB (954811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e448b573a98adc8bd0a4805cb0e1b451aea0d1582f0462aa0b147799a97fad7`  
		Last Modified: Wed, 21 Jun 2023 01:10:13 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3029a709b7be20aeff1e9cebe5c6112cd1df5a0ea3efb58e61380cc75b9296e`  
		Last Modified: Wed, 21 Jun 2023 01:10:13 GMT  
		Size: 117.0 B  
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
$ docker pull memcached@sha256:eb4b801b9c9e9af6565ac003b21af39b06d55943bbc4e59a02d465fdf7f07776
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4399342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4aa99dd98a2fa001241d907951530f4afebadfd4895545c5d73f31e29b7a35fa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:57:26 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Wed, 14 Jun 2023 20:57:27 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 01:08:09 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 01:08:09 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:10:35 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 01:10:35 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:10:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:10:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:10:36 GMT
USER memcache
# Wed, 21 Jun 2023 01:10:36 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:10:36 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666588188768f19b27fb821e02d084406af8fd867cc4595b896b9eed50b2105e`  
		Last Modified: Wed, 14 Jun 2023 21:00:51 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d958a137d671266f063c0af4d7b0b6d44d9018b77fdbddb8fd412d3c0b1be3`  
		Last Modified: Wed, 14 Jun 2023 21:00:51 GMT  
		Size: 124.1 KB (124137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66841dcfe05dcef1af82648941fa1ea0e10dbdf022326916d1d74afc99885c6`  
		Last Modified: Wed, 21 Jun 2023 01:11:21 GMT  
		Size: 944.3 KB (944292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b46fdc76bcbc8fa94ae23177ac32b97a4d370a630ec7d3f52bd8aae174e75982`  
		Last Modified: Wed, 21 Jun 2023 01:11:20 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea70db1a59f508c629aef54fb39ac3ada5cfcc3aac7aa1d6ed6cde22e97d3e3b`  
		Last Modified: Wed, 21 Jun 2023 01:11:20 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; 386

```console
$ docker pull memcached@sha256:1468666da56924eda85c3bbc484ce7835f472fd27dd171a5bb32b2c929ef52b7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4283458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7cc593f180f84bb7bdbcb9e4b50cbc7d3c3bc0f5a83d2b6b9abce4758814bb0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 07 Aug 2023 19:38:26 GMT
ADD file:4b33c52e11b19fde30197c62ead0b77bde28d34edaa08346a5302cd892d3cebe in / 
# Mon, 07 Aug 2023 19:38:27 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 21:40:23 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Mon, 07 Aug 2023 21:40:25 GMT
RUN apk add --no-cache libsasl
# Mon, 07 Aug 2023 21:40:25 GMT
ENV MEMCACHED_VERSION=1.6.21
# Mon, 07 Aug 2023 21:40:25 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Mon, 07 Aug 2023 21:43:52 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Mon, 07 Aug 2023 21:43:52 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 07 Aug 2023 21:43:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 07 Aug 2023 21:43:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 21:43:53 GMT
USER memcache
# Mon, 07 Aug 2023 21:43:53 GMT
EXPOSE 11211
# Mon, 07 Aug 2023 21:43:53 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:95dc695758361a4038a2d9026959d72e1f531114edb0341be7ce47d912ef069e`  
		Last Modified: Mon, 07 Aug 2023 19:38:56 GMT  
		Size: 3.2 MB (3235144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:038b25459839e567ceb29349d695abf1d64f7664699e6ac0f4ea807603c54220`  
		Last Modified: Mon, 07 Aug 2023 21:44:17 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ed277dfdfb7162fb18aa73173b2a45185a326869f4ad568557b667d337b8b1`  
		Last Modified: Mon, 07 Aug 2023 21:44:17 GMT  
		Size: 109.5 KB (109531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e1b11e58caccee0d368106698c71335d98063d4ed22c19c716d2da506ddef4`  
		Last Modified: Mon, 07 Aug 2023 21:44:17 GMT  
		Size: 937.1 KB (937114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5f84ab2372dcf436661f4f50a1a95ec0e21e7bdb30ebb567b68f7c443dae44`  
		Last Modified: Mon, 07 Aug 2023 21:44:17 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa27df056ec91886a0dd6eb3b95024a3d02bb1b20b887da0525621d78d880a2`  
		Last Modified: Mon, 07 Aug 2023 21:44:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:ed70e3e81930652804f6d430c71ed014f9daff26aa4ad302cd37c04a8ef038de
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4454755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ddfb07c34bdda47806fc2cec7489bef9f20f0e4d6d47f4c99dbf139dbd4700d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:25 GMT
ADD file:b8cf7516cdf9487d9347da0b5b5e3a6f65f24ebcdcadf81f430adb2b2664f2d1 in / 
# Mon, 07 Aug 2023 20:16:26 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 00:46:29 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 08 Aug 2023 00:46:31 GMT
RUN apk add --no-cache libsasl
# Tue, 08 Aug 2023 00:46:32 GMT
ENV MEMCACHED_VERSION=1.6.21
# Tue, 08 Aug 2023 00:46:32 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Tue, 08 Aug 2023 00:49:28 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 08 Aug 2023 00:49:28 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Aug 2023 00:49:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Aug 2023 00:49:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Aug 2023 00:49:39 GMT
USER memcache
# Tue, 08 Aug 2023 00:49:41 GMT
EXPOSE 11211
# Tue, 08 Aug 2023 00:49:43 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:55353ca330e9474ce7b858eca6842bb540ef4a70b2981c2ed47eefb9ef4253ad`  
		Last Modified: Mon, 07 Aug 2023 20:17:20 GMT  
		Size: 3.3 MB (3346251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05163a2a65d29a4d5c99749b9902892698d3b79714d37728f6a9e2f7a2c58441`  
		Last Modified: Tue, 08 Aug 2023 00:50:16 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823f7ceea96296f95c9085f083e8083413bcc70fcd4cf20b04543ab718b3419c`  
		Last Modified: Tue, 08 Aug 2023 00:50:16 GMT  
		Size: 123.9 KB (123936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a31a6f6c857bb6d5975504a61cbdfd4142af5d54776b833e03644c98433f216e`  
		Last Modified: Tue, 08 Aug 2023 00:50:18 GMT  
		Size: 982.9 KB (982892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721f4e8ef111056d9b345692fa8573c6486de7e886c2d2333e068e0bfc6e24c2`  
		Last Modified: Tue, 08 Aug 2023 00:50:16 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c144e3114e36623a8cdb3fd49d5b274689ac0d8ac00d9e1e10c402670090de1c`  
		Last Modified: Tue, 08 Aug 2023 00:50:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine` - linux; s390x

```console
$ docker pull memcached@sha256:cd97d93e79c2345a0c10f20a912f29a0ccf5590e15c00df81596397b9567233f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4278263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f56d14fce8cfd200c86bd00cd28c95574b6bf2863bd203e7644d44a08db84ab`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 15 Jun 2023 05:18:38 GMT
ADD file:a59beca78118ebf4f86cc1685237dc3a29a519401a70668da520beaa3d29eb7a in / 
# Thu, 15 Jun 2023 05:18:38 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:27:47 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 15 Jun 2023 06:27:49 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 00:58:01 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 00:58:01 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:01:08 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 01:01:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:01:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:01:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:01:09 GMT
USER memcache
# Wed, 21 Jun 2023 01:01:10 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:01:10 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:998cc98447b44e5f0fe799dce691412796ba586ab22eb7c99aebf9d45f34833b`  
		Last Modified: Thu, 15 Jun 2023 05:29:38 GMT  
		Size: 3.2 MB (3213497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156deb87465a2c5629e5ae28c2a7251d5684baea5a930cf65ff6b478de321202`  
		Last Modified: Thu, 15 Jun 2023 06:36:33 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19020c60d58f4724218660e819b1b33b5d1428c3c5027492a2ee3c44228231df`  
		Last Modified: Thu, 15 Jun 2023 06:36:33 GMT  
		Size: 112.8 KB (112849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e76f938f015ccb0b5d2915145432efbc0af21a2f4964e0c9a67bfbbe6a577e`  
		Last Modified: Wed, 21 Jun 2023 01:01:46 GMT  
		Size: 950.3 KB (950254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b613e0a69ced3425a5949c15688d493ef10d80eb28c7bb626f0c092223fe1302`  
		Last Modified: Wed, 21 Jun 2023 01:01:46 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db4c30d38bb65cd11068e1892913b2fa04add8f27abe601485cc3b09754eb50`  
		Last Modified: Wed, 21 Jun 2023 01:01:46 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6-alpine3.18`

```console
$ docker pull memcached@sha256:8ac412315105d6fa923db09279b93ee601a4c2348b9f3fd1ccb9aa6f1562d612
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1.6-alpine3.18` - linux; amd64

```console
$ docker pull memcached@sha256:574ef430513a38925cc52ae5954677a12e0a57205fed96be5707196a180e5159
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4462428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f7da63106561ab1f7284992dad2396b234096070b4269971b23c53f2f8498ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:50:58 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Wed, 14 Jun 2023 20:50:59 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 01:07:13 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 01:07:13 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:09:21 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 01:09:21 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:09:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:09:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:09:22 GMT
USER memcache
# Wed, 21 Jun 2023 01:09:22 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:09:22 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b2b2df106c5026cd33ea4ac655b77f25410ec9f4b8a6756ebc1ceeb79fca3c7`  
		Last Modified: Wed, 14 Jun 2023 20:53:58 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed63668528d3e2159f55909c66dc48a6f746ce24c2e2f6d963b992aefaa457ce`  
		Last Modified: Wed, 14 Jun 2023 20:53:58 GMT  
		Size: 108.1 KB (108080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05536f2f26c904a5aa1b07720957a37e8b57a223725d76f8d1473dcab297a233`  
		Last Modified: Wed, 21 Jun 2023 01:10:14 GMT  
		Size: 954.8 KB (954811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e448b573a98adc8bd0a4805cb0e1b451aea0d1582f0462aa0b147799a97fad7`  
		Last Modified: Wed, 21 Jun 2023 01:10:13 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3029a709b7be20aeff1e9cebe5c6112cd1df5a0ea3efb58e61380cc75b9296e`  
		Last Modified: Wed, 21 Jun 2023 01:10:13 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:eb4b801b9c9e9af6565ac003b21af39b06d55943bbc4e59a02d465fdf7f07776
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4399342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4aa99dd98a2fa001241d907951530f4afebadfd4895545c5d73f31e29b7a35fa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:57:26 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Wed, 14 Jun 2023 20:57:27 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 01:08:09 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 01:08:09 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:10:35 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 01:10:35 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:10:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:10:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:10:36 GMT
USER memcache
# Wed, 21 Jun 2023 01:10:36 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:10:36 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666588188768f19b27fb821e02d084406af8fd867cc4595b896b9eed50b2105e`  
		Last Modified: Wed, 14 Jun 2023 21:00:51 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d958a137d671266f063c0af4d7b0b6d44d9018b77fdbddb8fd412d3c0b1be3`  
		Last Modified: Wed, 14 Jun 2023 21:00:51 GMT  
		Size: 124.1 KB (124137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66841dcfe05dcef1af82648941fa1ea0e10dbdf022326916d1d74afc99885c6`  
		Last Modified: Wed, 21 Jun 2023 01:11:21 GMT  
		Size: 944.3 KB (944292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b46fdc76bcbc8fa94ae23177ac32b97a4d370a630ec7d3f52bd8aae174e75982`  
		Last Modified: Wed, 21 Jun 2023 01:11:20 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea70db1a59f508c629aef54fb39ac3ada5cfcc3aac7aa1d6ed6cde22e97d3e3b`  
		Last Modified: Wed, 21 Jun 2023 01:11:20 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine3.18` - linux; 386

```console
$ docker pull memcached@sha256:1468666da56924eda85c3bbc484ce7835f472fd27dd171a5bb32b2c929ef52b7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4283458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7cc593f180f84bb7bdbcb9e4b50cbc7d3c3bc0f5a83d2b6b9abce4758814bb0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 07 Aug 2023 19:38:26 GMT
ADD file:4b33c52e11b19fde30197c62ead0b77bde28d34edaa08346a5302cd892d3cebe in / 
# Mon, 07 Aug 2023 19:38:27 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 21:40:23 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Mon, 07 Aug 2023 21:40:25 GMT
RUN apk add --no-cache libsasl
# Mon, 07 Aug 2023 21:40:25 GMT
ENV MEMCACHED_VERSION=1.6.21
# Mon, 07 Aug 2023 21:40:25 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Mon, 07 Aug 2023 21:43:52 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Mon, 07 Aug 2023 21:43:52 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 07 Aug 2023 21:43:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 07 Aug 2023 21:43:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 21:43:53 GMT
USER memcache
# Mon, 07 Aug 2023 21:43:53 GMT
EXPOSE 11211
# Mon, 07 Aug 2023 21:43:53 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:95dc695758361a4038a2d9026959d72e1f531114edb0341be7ce47d912ef069e`  
		Last Modified: Mon, 07 Aug 2023 19:38:56 GMT  
		Size: 3.2 MB (3235144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:038b25459839e567ceb29349d695abf1d64f7664699e6ac0f4ea807603c54220`  
		Last Modified: Mon, 07 Aug 2023 21:44:17 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ed277dfdfb7162fb18aa73173b2a45185a326869f4ad568557b667d337b8b1`  
		Last Modified: Mon, 07 Aug 2023 21:44:17 GMT  
		Size: 109.5 KB (109531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e1b11e58caccee0d368106698c71335d98063d4ed22c19c716d2da506ddef4`  
		Last Modified: Mon, 07 Aug 2023 21:44:17 GMT  
		Size: 937.1 KB (937114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5f84ab2372dcf436661f4f50a1a95ec0e21e7bdb30ebb567b68f7c443dae44`  
		Last Modified: Mon, 07 Aug 2023 21:44:17 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa27df056ec91886a0dd6eb3b95024a3d02bb1b20b887da0525621d78d880a2`  
		Last Modified: Mon, 07 Aug 2023 21:44:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine3.18` - linux; ppc64le

```console
$ docker pull memcached@sha256:ed70e3e81930652804f6d430c71ed014f9daff26aa4ad302cd37c04a8ef038de
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4454755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ddfb07c34bdda47806fc2cec7489bef9f20f0e4d6d47f4c99dbf139dbd4700d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:25 GMT
ADD file:b8cf7516cdf9487d9347da0b5b5e3a6f65f24ebcdcadf81f430adb2b2664f2d1 in / 
# Mon, 07 Aug 2023 20:16:26 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 00:46:29 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 08 Aug 2023 00:46:31 GMT
RUN apk add --no-cache libsasl
# Tue, 08 Aug 2023 00:46:32 GMT
ENV MEMCACHED_VERSION=1.6.21
# Tue, 08 Aug 2023 00:46:32 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Tue, 08 Aug 2023 00:49:28 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 08 Aug 2023 00:49:28 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Aug 2023 00:49:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Aug 2023 00:49:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Aug 2023 00:49:39 GMT
USER memcache
# Tue, 08 Aug 2023 00:49:41 GMT
EXPOSE 11211
# Tue, 08 Aug 2023 00:49:43 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:55353ca330e9474ce7b858eca6842bb540ef4a70b2981c2ed47eefb9ef4253ad`  
		Last Modified: Mon, 07 Aug 2023 20:17:20 GMT  
		Size: 3.3 MB (3346251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05163a2a65d29a4d5c99749b9902892698d3b79714d37728f6a9e2f7a2c58441`  
		Last Modified: Tue, 08 Aug 2023 00:50:16 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823f7ceea96296f95c9085f083e8083413bcc70fcd4cf20b04543ab718b3419c`  
		Last Modified: Tue, 08 Aug 2023 00:50:16 GMT  
		Size: 123.9 KB (123936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a31a6f6c857bb6d5975504a61cbdfd4142af5d54776b833e03644c98433f216e`  
		Last Modified: Tue, 08 Aug 2023 00:50:18 GMT  
		Size: 982.9 KB (982892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721f4e8ef111056d9b345692fa8573c6486de7e886c2d2333e068e0bfc6e24c2`  
		Last Modified: Tue, 08 Aug 2023 00:50:16 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c144e3114e36623a8cdb3fd49d5b274689ac0d8ac00d9e1e10c402670090de1c`  
		Last Modified: Tue, 08 Aug 2023 00:50:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-alpine3.18` - linux; s390x

```console
$ docker pull memcached@sha256:cd97d93e79c2345a0c10f20a912f29a0ccf5590e15c00df81596397b9567233f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4278263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f56d14fce8cfd200c86bd00cd28c95574b6bf2863bd203e7644d44a08db84ab`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 15 Jun 2023 05:18:38 GMT
ADD file:a59beca78118ebf4f86cc1685237dc3a29a519401a70668da520beaa3d29eb7a in / 
# Thu, 15 Jun 2023 05:18:38 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:27:47 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 15 Jun 2023 06:27:49 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 00:58:01 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 00:58:01 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:01:08 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 01:01:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:01:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:01:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:01:09 GMT
USER memcache
# Wed, 21 Jun 2023 01:01:10 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:01:10 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:998cc98447b44e5f0fe799dce691412796ba586ab22eb7c99aebf9d45f34833b`  
		Last Modified: Thu, 15 Jun 2023 05:29:38 GMT  
		Size: 3.2 MB (3213497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156deb87465a2c5629e5ae28c2a7251d5684baea5a930cf65ff6b478de321202`  
		Last Modified: Thu, 15 Jun 2023 06:36:33 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19020c60d58f4724218660e819b1b33b5d1428c3c5027492a2ee3c44228231df`  
		Last Modified: Thu, 15 Jun 2023 06:36:33 GMT  
		Size: 112.8 KB (112849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e76f938f015ccb0b5d2915145432efbc0af21a2f4964e0c9a67bfbbe6a577e`  
		Last Modified: Wed, 21 Jun 2023 01:01:46 GMT  
		Size: 950.3 KB (950254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b613e0a69ced3425a5949c15688d493ef10d80eb28c7bb626f0c092223fe1302`  
		Last Modified: Wed, 21 Jun 2023 01:01:46 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db4c30d38bb65cd11068e1892913b2fa04add8f27abe601485cc3b09754eb50`  
		Last Modified: Wed, 21 Jun 2023 01:01:46 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6-bookworm`

```console
$ docker pull memcached@sha256:a917777975a7039b6ed70ef2faab453b1e5ea7aa741899aba952d744546cc781
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1.6-bookworm` - linux; amd64

```console
$ docker pull memcached@sha256:0c8398104f83351267e51ec72b34de06b734f2eca6637c10d246702afff814b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.0 MB (38974916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:354b899e400fa323ffaea769644cc66778676b4f4eeca0e3e1523100e8803d97`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:44 GMT
ADD file:209589a8bdb5a3788ee42ecdbccbbb561835dab96b0d8286bb5a2229d2f41be7 in / 
# Thu, 27 Jul 2023 23:24:45 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 04:03:18 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 28 Jul 2023 04:03:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 04:03:22 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 28 Jul 2023 04:03:22 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 28 Jul 2023 04:05:37 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 28 Jul 2023 04:05:37 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 28 Jul 2023 04:05:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 04:05:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 04:05:38 GMT
USER memcache
# Fri, 28 Jul 2023 04:05:38 GMT
EXPOSE 11211
# Fri, 28 Jul 2023 04:05:38 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:648e0aadf75ac2ef63c5390adc6dc14fde37a5ad88c2870ea604df0a9c0eb4e5`  
		Last Modified: Thu, 27 Jul 2023 23:29:26 GMT  
		Size: 29.1 MB (29124532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baaf8e9cef6b92919a723712ed912794373f6fc1d8dac9d5ed1d320378f657ba`  
		Last Modified: Fri, 28 Jul 2023 04:05:56 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52dca4bf886a56187b224e812b7a65f7825798dc8d536db9bb9344cb112b98e0`  
		Last Modified: Fri, 28 Jul 2023 04:05:56 GMT  
		Size: 2.7 MB (2677283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6861252b28dd75ed1a4f9accdcef6f35366a5dd59d3d7921945a20ec3f64661`  
		Last Modified: Fri, 28 Jul 2023 04:05:57 GMT  
		Size: 7.2 MB (7171562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49870ab6c52b8db6c693e18bd63b718827cd451bde693287ca70314a991cbfb6`  
		Last Modified: Fri, 28 Jul 2023 04:05:56 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da541564580ce27d2c3710f1420b22d4bc544196f1bf6536a5c58150854283d`  
		Last Modified: Fri, 28 Jul 2023 04:05:56 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bookworm` - linux; arm variant v5

```console
$ docker pull memcached@sha256:ec7dc6727737267a059c047a43864e1c5bdda0a6b8d3cdd0b49110523acfe7f7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35098422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8ce1a3d6a1d0c9162fa735664905dded291bfaa1a0398a381448950a7b9ee91`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 27 Jul 2023 23:48:29 GMT
ADD file:53cf36eb7b72a7e970f4b18af1589402b2900f12e30820cdeccc8bb0c166df80 in / 
# Thu, 27 Jul 2023 23:48:30 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 11:05:31 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 28 Jul 2023 11:05:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 11:05:37 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 28 Jul 2023 11:05:37 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 28 Jul 2023 11:08:31 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 28 Jul 2023 11:08:31 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 28 Jul 2023 11:08:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 11:08:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 11:08:31 GMT
USER memcache
# Fri, 28 Jul 2023 11:08:31 GMT
EXPOSE 11211
# Fri, 28 Jul 2023 11:08:32 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2bd6dfc5281e13a0ca9fb8d9238ac9f14a0de04489913030c8e33b9398b4a4af`  
		Last Modified: Thu, 27 Jul 2023 23:51:28 GMT  
		Size: 27.0 MB (26983508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5936d9d99182ef30677e20dad76c0549b2b7612ca100ef6c0f03c87027cee0b`  
		Last Modified: Fri, 28 Jul 2023 11:08:45 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7717a35af981145073f1343f8447ffd5b5c52de46680b1e75e4c0c11ba64bf`  
		Last Modified: Fri, 28 Jul 2023 11:08:46 GMT  
		Size: 2.3 MB (2281851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56b5203e649ffe900465b0cf521d6be756bd5dd83b5905d7ccc6aced143610b`  
		Last Modified: Fri, 28 Jul 2023 11:08:47 GMT  
		Size: 5.8 MB (5831523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6dee9c51b3b15c0179684c9c61eebfc3091a8f40afd9714ddae2728364aee4f`  
		Last Modified: Fri, 28 Jul 2023 11:08:45 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51b980bae702ef385ef2cbe3eb556c8377334b4c31c97e39cced7ed58375bc55`  
		Last Modified: Fri, 28 Jul 2023 11:08:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bookworm` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:4b2d19d8c0d48b44b1f24b2ea0e8a62749f05db1bedbe481ff6112db44c703cc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.9 MB (37878121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c74af541d05a0758cbf5f13d5d190f1ab10b86ef5fd75112aa98b0638def7d9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 27 Jul 2023 23:43:00 GMT
ADD file:1de2ba0dc88aa343332814e19adc6b850d08e62c31589fe902b8eb2cb465934e in / 
# Thu, 27 Jul 2023 23:43:00 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 06:38:57 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 28 Jul 2023 06:39:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 06:39:01 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 28 Jul 2023 06:39:01 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 28 Jul 2023 06:41:36 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 28 Jul 2023 06:41:36 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 28 Jul 2023 06:41:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 06:41:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 06:41:37 GMT
USER memcache
# Fri, 28 Jul 2023 06:41:37 GMT
EXPOSE 11211
# Fri, 28 Jul 2023 06:41:37 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:90524f7dc01b4ce9b387992acc6cbdbcc2a9ee8c6addfd632429ca06ea18751e`  
		Last Modified: Thu, 27 Jul 2023 23:46:17 GMT  
		Size: 29.2 MB (29157226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6146d0684a3303f06ef62333440ab9aba6cab719b5762ddaee7f7b7a3a62e9ee`  
		Last Modified: Fri, 28 Jul 2023 06:42:01 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b513dbaa02d89264c8df677c8871ec60a8cba234a96d77165fc06157ed2ec1f`  
		Last Modified: Fri, 28 Jul 2023 06:42:01 GMT  
		Size: 2.5 MB (2539192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe211375d2d86acd694c377eeaf6fe900e6f57dadd07e6bd6f21809eab75c53a`  
		Last Modified: Fri, 28 Jul 2023 06:42:02 GMT  
		Size: 6.2 MB (6180162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1b4b070b2921c7d9f5349e7b258c1400ac5d0a1154df0028e634899e86fbda`  
		Last Modified: Fri, 28 Jul 2023 06:42:01 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d40396358d46edf0c2615a77e13da10249786f2546d4a9623e18ec0ce9d6aa91`  
		Last Modified: Fri, 28 Jul 2023 06:42:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bookworm` - linux; 386

```console
$ docker pull memcached@sha256:d3e70a847a7f720a3a129c6e060b3f9b3428add5e0458c1974a6a895783073e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39459484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fe4fee0ccc34611e17f9be47d4048890aa66e445397fb679f2f27edcb5de08a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 27 Jul 2023 23:38:56 GMT
ADD file:3d6e6f3e900e480a7e060fcaf57313c0f954bf906967a7fa0317567c387cf5aa in / 
# Thu, 27 Jul 2023 23:38:57 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 00:12:30 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 28 Jul 2023 00:12:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 00:12:35 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 28 Jul 2023 00:12:35 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 28 Jul 2023 00:16:17 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 28 Jul 2023 00:16:17 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 28 Jul 2023 00:16:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 00:16:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 00:16:18 GMT
USER memcache
# Fri, 28 Jul 2023 00:16:18 GMT
EXPOSE 11211
# Fri, 28 Jul 2023 00:16:18 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3a8b0c4b1a83609d978d576be6174f951ff27084d7c9aef91892b60b223a5104`  
		Last Modified: Thu, 27 Jul 2023 23:43:26 GMT  
		Size: 30.1 MB (30141788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:700ff590600873a2721ed53371f8797b79c09c48cf32c7190640b4a1d4f5755d`  
		Last Modified: Fri, 28 Jul 2023 00:16:36 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f15bfc1eebf505da6ff5a5b1b1810ad762b79725e742a9b354c57fbabd31f01a`  
		Last Modified: Fri, 28 Jul 2023 00:16:37 GMT  
		Size: 2.7 MB (2685093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80fdef0976acae3ce13d23a176fc9e9ce15eeb2ac874a0915725bbaa3108059b`  
		Last Modified: Fri, 28 Jul 2023 00:16:38 GMT  
		Size: 6.6 MB (6631063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3442227f7348458fb36b2e0d739658a8fb589ed322fd578df8e39e59fc32000d`  
		Last Modified: Fri, 28 Jul 2023 00:16:36 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5501a93139182f8a01992f6de5a5e4eaebdebaaec5a10506a07f59b936d266e6`  
		Last Modified: Fri, 28 Jul 2023 00:16:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bookworm` - linux; mips64le

```console
$ docker pull memcached@sha256:fbc5c08e8c901f9b6c9cab47733639d29f3ff1167ab861aa26fe0bb751a308d9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.6 MB (37558667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f390b2a92aa8ce938675a24263c1e7f6b619c4c584343f3dd7a0e9d6615051d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 27 Jul 2023 23:11:23 GMT
ADD file:90cbcf9a2aaf48a433b00118dd0821eeb291092da7b7f67ce6a525ce2cba1e3f in / 
# Thu, 27 Jul 2023 23:11:27 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:45:56 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 28 Jul 2023 01:46:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:46:17 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 28 Jul 2023 01:46:19 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 28 Jul 2023 01:53:01 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 28 Jul 2023 01:53:03 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 28 Jul 2023 01:53:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 01:53:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 01:53:14 GMT
USER memcache
# Fri, 28 Jul 2023 01:53:16 GMT
EXPOSE 11211
# Fri, 28 Jul 2023 01:53:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3252778e08fa8eb67ab052ad63281284b5ef1afdc40a36021228133487ab5d52`  
		Last Modified: Thu, 27 Jul 2023 23:22:26 GMT  
		Size: 29.1 MB (29121405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63e55e013f2ab63ff93eaaf154b0debea8de9ffc8fbadaf67d3bc03851f57910`  
		Last Modified: Fri, 28 Jul 2023 01:53:46 GMT  
		Size: 1.1 KB (1082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d9a9f24853cb0188d2273603847b46ed81bd544b868ae314d609c1d9e7db7c`  
		Last Modified: Fri, 28 Jul 2023 01:53:48 GMT  
		Size: 1.9 MB (1934904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4467025968ec633fd090be17fe8c5f61d7ee738a0b34a10db006d35397e27cc`  
		Last Modified: Fri, 28 Jul 2023 01:53:51 GMT  
		Size: 6.5 MB (6500867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07da0cd083ab7d3e91ac9e7ae33d316bd7affeb2852262ff2d687be0e5c273b6`  
		Last Modified: Fri, 28 Jul 2023 01:53:46 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57f5929847506e0cf79067f8348bd883548c83f0c23defbaccf512eb17d65758`  
		Last Modified: Fri, 28 Jul 2023 01:53:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bookworm` - linux; ppc64le

```console
$ docker pull memcached@sha256:a32969620e95d4b08d5711678e6bcbd313e3bc3511d1b96cf5d08e675a90d0fb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43196803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d6a8d8d3e6746723698507be3f910bb02f0a22617da462f56031004e606edf6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 27 Jul 2023 23:23:01 GMT
ADD file:774a99e5c40757d27c981eb5ad6e03eb72970bb0c54f799eab1442624238ea3e in / 
# Thu, 27 Jul 2023 23:23:03 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:38:39 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 28 Jul 2023 03:38:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:38:51 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 28 Jul 2023 03:38:52 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 28 Jul 2023 03:42:57 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 28 Jul 2023 03:42:58 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 28 Jul 2023 03:43:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 03:43:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 03:43:01 GMT
USER memcache
# Fri, 28 Jul 2023 03:43:02 GMT
EXPOSE 11211
# Fri, 28 Jul 2023 03:43:03 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:ad974e0ada84177d519dec70d0d7d9ff6a4f468bc7306425feb8429bc276bd8a`  
		Last Modified: Thu, 27 Jul 2023 23:29:24 GMT  
		Size: 33.1 MB (33119211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ed68aff2ca1a6e8c25d8462f4b2ebbb3866c768911785569560ede6a2f053d`  
		Last Modified: Fri, 28 Jul 2023 03:43:33 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d519acbf803e11e9a1e21f396dd4e021495fa7b97a4c9df3e6f7639d8c050790`  
		Last Modified: Fri, 28 Jul 2023 03:43:33 GMT  
		Size: 2.9 MB (2891351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:097534b38ed1845470192cab29ec2d22d4e0c7a9d5f01c9948ebc1273dfe809c`  
		Last Modified: Fri, 28 Jul 2023 03:43:35 GMT  
		Size: 7.2 MB (7184700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2f9c6ce8e611c611c0bfdb7cb8ec798950618d80a9be8db98c59fdd0654825`  
		Last Modified: Fri, 28 Jul 2023 03:43:33 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d974aa6a849abcd290ae3bbfbc44f776e3928269bfa1bdbc65e2a1f11c368afe`  
		Last Modified: Fri, 28 Jul 2023 03:43:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6-bookworm` - linux; s390x

```console
$ docker pull memcached@sha256:1ab909233ee99a6798929725205b93abb2bd9a8c78ab048d925dffd359fe8cf2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35910248 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:845b0ff32d8c04c5820146361e7a2e8c8579ad2a96318fdbc7e6c669bfc27569`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 27 Jul 2023 23:47:11 GMT
ADD file:0a5e1e86b375d60637d0829f77a12085777cf2ca07495b0f6249d8efea84e958 in / 
# Thu, 27 Jul 2023 23:47:13 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 02:58:10 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 28 Jul 2023 02:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 02:58:13 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 28 Jul 2023 02:58:13 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 28 Jul 2023 03:01:19 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 28 Jul 2023 03:01:20 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 28 Jul 2023 03:01:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 03:01:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 03:01:20 GMT
USER memcache
# Fri, 28 Jul 2023 03:01:20 GMT
EXPOSE 11211
# Fri, 28 Jul 2023 03:01:21 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f4301d25bb1bea85fcc5b364aec84ff58274f714cea191ab22d9b1b1e4f78527`  
		Last Modified: Thu, 27 Jul 2023 23:52:17 GMT  
		Size: 27.5 MB (27489697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8055eb96c9dacdcc9c91194a8d4504ab82a88a0fa9f927413c1dde2e493a815`  
		Last Modified: Fri, 28 Jul 2023 03:01:51 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:040e9d91e418b36f9ea07fcd1d9db85ae7713bd99a0a17f31f41a7ef410c3423`  
		Last Modified: Fri, 28 Jul 2023 03:01:54 GMT  
		Size: 2.3 MB (2345395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a638c5b62a02bc60b52234e1556bcf148e66b74e50a0bd02d2b5f23ea2ee136d`  
		Last Modified: Fri, 28 Jul 2023 03:01:52 GMT  
		Size: 6.1 MB (6073620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c41c8e1cb6d4df65052cc47729124edceae5af653ff6a3555cf6e69a57f6de1`  
		Last Modified: Fri, 28 Jul 2023 03:01:51 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2516714a4b2b11720bd2fcf5338749e05ae2dff40f716814b7531fcbe356fdce`  
		Last Modified: Fri, 28 Jul 2023 03:01:51 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.21`

```console
$ docker pull memcached@sha256:a917777975a7039b6ed70ef2faab453b1e5ea7aa741899aba952d744546cc781
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1.6.21` - linux; amd64

```console
$ docker pull memcached@sha256:0c8398104f83351267e51ec72b34de06b734f2eca6637c10d246702afff814b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.0 MB (38974916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:354b899e400fa323ffaea769644cc66778676b4f4eeca0e3e1523100e8803d97`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:44 GMT
ADD file:209589a8bdb5a3788ee42ecdbccbbb561835dab96b0d8286bb5a2229d2f41be7 in / 
# Thu, 27 Jul 2023 23:24:45 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 04:03:18 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 28 Jul 2023 04:03:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 04:03:22 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 28 Jul 2023 04:03:22 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 28 Jul 2023 04:05:37 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 28 Jul 2023 04:05:37 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 28 Jul 2023 04:05:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 04:05:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 04:05:38 GMT
USER memcache
# Fri, 28 Jul 2023 04:05:38 GMT
EXPOSE 11211
# Fri, 28 Jul 2023 04:05:38 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:648e0aadf75ac2ef63c5390adc6dc14fde37a5ad88c2870ea604df0a9c0eb4e5`  
		Last Modified: Thu, 27 Jul 2023 23:29:26 GMT  
		Size: 29.1 MB (29124532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baaf8e9cef6b92919a723712ed912794373f6fc1d8dac9d5ed1d320378f657ba`  
		Last Modified: Fri, 28 Jul 2023 04:05:56 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52dca4bf886a56187b224e812b7a65f7825798dc8d536db9bb9344cb112b98e0`  
		Last Modified: Fri, 28 Jul 2023 04:05:56 GMT  
		Size: 2.7 MB (2677283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6861252b28dd75ed1a4f9accdcef6f35366a5dd59d3d7921945a20ec3f64661`  
		Last Modified: Fri, 28 Jul 2023 04:05:57 GMT  
		Size: 7.2 MB (7171562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49870ab6c52b8db6c693e18bd63b718827cd451bde693287ca70314a991cbfb6`  
		Last Modified: Fri, 28 Jul 2023 04:05:56 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da541564580ce27d2c3710f1420b22d4bc544196f1bf6536a5c58150854283d`  
		Last Modified: Fri, 28 Jul 2023 04:05:56 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.21` - linux; arm variant v5

```console
$ docker pull memcached@sha256:ec7dc6727737267a059c047a43864e1c5bdda0a6b8d3cdd0b49110523acfe7f7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35098422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8ce1a3d6a1d0c9162fa735664905dded291bfaa1a0398a381448950a7b9ee91`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 27 Jul 2023 23:48:29 GMT
ADD file:53cf36eb7b72a7e970f4b18af1589402b2900f12e30820cdeccc8bb0c166df80 in / 
# Thu, 27 Jul 2023 23:48:30 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 11:05:31 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 28 Jul 2023 11:05:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 11:05:37 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 28 Jul 2023 11:05:37 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 28 Jul 2023 11:08:31 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 28 Jul 2023 11:08:31 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 28 Jul 2023 11:08:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 11:08:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 11:08:31 GMT
USER memcache
# Fri, 28 Jul 2023 11:08:31 GMT
EXPOSE 11211
# Fri, 28 Jul 2023 11:08:32 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2bd6dfc5281e13a0ca9fb8d9238ac9f14a0de04489913030c8e33b9398b4a4af`  
		Last Modified: Thu, 27 Jul 2023 23:51:28 GMT  
		Size: 27.0 MB (26983508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5936d9d99182ef30677e20dad76c0549b2b7612ca100ef6c0f03c87027cee0b`  
		Last Modified: Fri, 28 Jul 2023 11:08:45 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7717a35af981145073f1343f8447ffd5b5c52de46680b1e75e4c0c11ba64bf`  
		Last Modified: Fri, 28 Jul 2023 11:08:46 GMT  
		Size: 2.3 MB (2281851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56b5203e649ffe900465b0cf521d6be756bd5dd83b5905d7ccc6aced143610b`  
		Last Modified: Fri, 28 Jul 2023 11:08:47 GMT  
		Size: 5.8 MB (5831523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6dee9c51b3b15c0179684c9c61eebfc3091a8f40afd9714ddae2728364aee4f`  
		Last Modified: Fri, 28 Jul 2023 11:08:45 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51b980bae702ef385ef2cbe3eb556c8377334b4c31c97e39cced7ed58375bc55`  
		Last Modified: Fri, 28 Jul 2023 11:08:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.21` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:4b2d19d8c0d48b44b1f24b2ea0e8a62749f05db1bedbe481ff6112db44c703cc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.9 MB (37878121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c74af541d05a0758cbf5f13d5d190f1ab10b86ef5fd75112aa98b0638def7d9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 27 Jul 2023 23:43:00 GMT
ADD file:1de2ba0dc88aa343332814e19adc6b850d08e62c31589fe902b8eb2cb465934e in / 
# Thu, 27 Jul 2023 23:43:00 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 06:38:57 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 28 Jul 2023 06:39:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 06:39:01 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 28 Jul 2023 06:39:01 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 28 Jul 2023 06:41:36 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 28 Jul 2023 06:41:36 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 28 Jul 2023 06:41:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 06:41:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 06:41:37 GMT
USER memcache
# Fri, 28 Jul 2023 06:41:37 GMT
EXPOSE 11211
# Fri, 28 Jul 2023 06:41:37 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:90524f7dc01b4ce9b387992acc6cbdbcc2a9ee8c6addfd632429ca06ea18751e`  
		Last Modified: Thu, 27 Jul 2023 23:46:17 GMT  
		Size: 29.2 MB (29157226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6146d0684a3303f06ef62333440ab9aba6cab719b5762ddaee7f7b7a3a62e9ee`  
		Last Modified: Fri, 28 Jul 2023 06:42:01 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b513dbaa02d89264c8df677c8871ec60a8cba234a96d77165fc06157ed2ec1f`  
		Last Modified: Fri, 28 Jul 2023 06:42:01 GMT  
		Size: 2.5 MB (2539192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe211375d2d86acd694c377eeaf6fe900e6f57dadd07e6bd6f21809eab75c53a`  
		Last Modified: Fri, 28 Jul 2023 06:42:02 GMT  
		Size: 6.2 MB (6180162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1b4b070b2921c7d9f5349e7b258c1400ac5d0a1154df0028e634899e86fbda`  
		Last Modified: Fri, 28 Jul 2023 06:42:01 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d40396358d46edf0c2615a77e13da10249786f2546d4a9623e18ec0ce9d6aa91`  
		Last Modified: Fri, 28 Jul 2023 06:42:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.21` - linux; 386

```console
$ docker pull memcached@sha256:d3e70a847a7f720a3a129c6e060b3f9b3428add5e0458c1974a6a895783073e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39459484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fe4fee0ccc34611e17f9be47d4048890aa66e445397fb679f2f27edcb5de08a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 27 Jul 2023 23:38:56 GMT
ADD file:3d6e6f3e900e480a7e060fcaf57313c0f954bf906967a7fa0317567c387cf5aa in / 
# Thu, 27 Jul 2023 23:38:57 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 00:12:30 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 28 Jul 2023 00:12:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 00:12:35 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 28 Jul 2023 00:12:35 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 28 Jul 2023 00:16:17 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 28 Jul 2023 00:16:17 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 28 Jul 2023 00:16:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 00:16:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 00:16:18 GMT
USER memcache
# Fri, 28 Jul 2023 00:16:18 GMT
EXPOSE 11211
# Fri, 28 Jul 2023 00:16:18 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3a8b0c4b1a83609d978d576be6174f951ff27084d7c9aef91892b60b223a5104`  
		Last Modified: Thu, 27 Jul 2023 23:43:26 GMT  
		Size: 30.1 MB (30141788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:700ff590600873a2721ed53371f8797b79c09c48cf32c7190640b4a1d4f5755d`  
		Last Modified: Fri, 28 Jul 2023 00:16:36 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f15bfc1eebf505da6ff5a5b1b1810ad762b79725e742a9b354c57fbabd31f01a`  
		Last Modified: Fri, 28 Jul 2023 00:16:37 GMT  
		Size: 2.7 MB (2685093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80fdef0976acae3ce13d23a176fc9e9ce15eeb2ac874a0915725bbaa3108059b`  
		Last Modified: Fri, 28 Jul 2023 00:16:38 GMT  
		Size: 6.6 MB (6631063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3442227f7348458fb36b2e0d739658a8fb589ed322fd578df8e39e59fc32000d`  
		Last Modified: Fri, 28 Jul 2023 00:16:36 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5501a93139182f8a01992f6de5a5e4eaebdebaaec5a10506a07f59b936d266e6`  
		Last Modified: Fri, 28 Jul 2023 00:16:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.21` - linux; mips64le

```console
$ docker pull memcached@sha256:fbc5c08e8c901f9b6c9cab47733639d29f3ff1167ab861aa26fe0bb751a308d9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.6 MB (37558667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f390b2a92aa8ce938675a24263c1e7f6b619c4c584343f3dd7a0e9d6615051d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 27 Jul 2023 23:11:23 GMT
ADD file:90cbcf9a2aaf48a433b00118dd0821eeb291092da7b7f67ce6a525ce2cba1e3f in / 
# Thu, 27 Jul 2023 23:11:27 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:45:56 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 28 Jul 2023 01:46:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:46:17 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 28 Jul 2023 01:46:19 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 28 Jul 2023 01:53:01 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 28 Jul 2023 01:53:03 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 28 Jul 2023 01:53:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 01:53:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 01:53:14 GMT
USER memcache
# Fri, 28 Jul 2023 01:53:16 GMT
EXPOSE 11211
# Fri, 28 Jul 2023 01:53:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3252778e08fa8eb67ab052ad63281284b5ef1afdc40a36021228133487ab5d52`  
		Last Modified: Thu, 27 Jul 2023 23:22:26 GMT  
		Size: 29.1 MB (29121405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63e55e013f2ab63ff93eaaf154b0debea8de9ffc8fbadaf67d3bc03851f57910`  
		Last Modified: Fri, 28 Jul 2023 01:53:46 GMT  
		Size: 1.1 KB (1082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d9a9f24853cb0188d2273603847b46ed81bd544b868ae314d609c1d9e7db7c`  
		Last Modified: Fri, 28 Jul 2023 01:53:48 GMT  
		Size: 1.9 MB (1934904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4467025968ec633fd090be17fe8c5f61d7ee738a0b34a10db006d35397e27cc`  
		Last Modified: Fri, 28 Jul 2023 01:53:51 GMT  
		Size: 6.5 MB (6500867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07da0cd083ab7d3e91ac9e7ae33d316bd7affeb2852262ff2d687be0e5c273b6`  
		Last Modified: Fri, 28 Jul 2023 01:53:46 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57f5929847506e0cf79067f8348bd883548c83f0c23defbaccf512eb17d65758`  
		Last Modified: Fri, 28 Jul 2023 01:53:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.21` - linux; ppc64le

```console
$ docker pull memcached@sha256:a32969620e95d4b08d5711678e6bcbd313e3bc3511d1b96cf5d08e675a90d0fb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43196803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d6a8d8d3e6746723698507be3f910bb02f0a22617da462f56031004e606edf6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 27 Jul 2023 23:23:01 GMT
ADD file:774a99e5c40757d27c981eb5ad6e03eb72970bb0c54f799eab1442624238ea3e in / 
# Thu, 27 Jul 2023 23:23:03 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:38:39 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 28 Jul 2023 03:38:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:38:51 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 28 Jul 2023 03:38:52 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 28 Jul 2023 03:42:57 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 28 Jul 2023 03:42:58 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 28 Jul 2023 03:43:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 03:43:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 03:43:01 GMT
USER memcache
# Fri, 28 Jul 2023 03:43:02 GMT
EXPOSE 11211
# Fri, 28 Jul 2023 03:43:03 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:ad974e0ada84177d519dec70d0d7d9ff6a4f468bc7306425feb8429bc276bd8a`  
		Last Modified: Thu, 27 Jul 2023 23:29:24 GMT  
		Size: 33.1 MB (33119211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ed68aff2ca1a6e8c25d8462f4b2ebbb3866c768911785569560ede6a2f053d`  
		Last Modified: Fri, 28 Jul 2023 03:43:33 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d519acbf803e11e9a1e21f396dd4e021495fa7b97a4c9df3e6f7639d8c050790`  
		Last Modified: Fri, 28 Jul 2023 03:43:33 GMT  
		Size: 2.9 MB (2891351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:097534b38ed1845470192cab29ec2d22d4e0c7a9d5f01c9948ebc1273dfe809c`  
		Last Modified: Fri, 28 Jul 2023 03:43:35 GMT  
		Size: 7.2 MB (7184700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2f9c6ce8e611c611c0bfdb7cb8ec798950618d80a9be8db98c59fdd0654825`  
		Last Modified: Fri, 28 Jul 2023 03:43:33 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d974aa6a849abcd290ae3bbfbc44f776e3928269bfa1bdbc65e2a1f11c368afe`  
		Last Modified: Fri, 28 Jul 2023 03:43:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.21` - linux; s390x

```console
$ docker pull memcached@sha256:1ab909233ee99a6798929725205b93abb2bd9a8c78ab048d925dffd359fe8cf2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35910248 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:845b0ff32d8c04c5820146361e7a2e8c8579ad2a96318fdbc7e6c669bfc27569`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 27 Jul 2023 23:47:11 GMT
ADD file:0a5e1e86b375d60637d0829f77a12085777cf2ca07495b0f6249d8efea84e958 in / 
# Thu, 27 Jul 2023 23:47:13 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 02:58:10 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 28 Jul 2023 02:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 02:58:13 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 28 Jul 2023 02:58:13 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 28 Jul 2023 03:01:19 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 28 Jul 2023 03:01:20 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 28 Jul 2023 03:01:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 03:01:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 03:01:20 GMT
USER memcache
# Fri, 28 Jul 2023 03:01:20 GMT
EXPOSE 11211
# Fri, 28 Jul 2023 03:01:21 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f4301d25bb1bea85fcc5b364aec84ff58274f714cea191ab22d9b1b1e4f78527`  
		Last Modified: Thu, 27 Jul 2023 23:52:17 GMT  
		Size: 27.5 MB (27489697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8055eb96c9dacdcc9c91194a8d4504ab82a88a0fa9f927413c1dde2e493a815`  
		Last Modified: Fri, 28 Jul 2023 03:01:51 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:040e9d91e418b36f9ea07fcd1d9db85ae7713bd99a0a17f31f41a7ef410c3423`  
		Last Modified: Fri, 28 Jul 2023 03:01:54 GMT  
		Size: 2.3 MB (2345395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a638c5b62a02bc60b52234e1556bcf148e66b74e50a0bd02d2b5f23ea2ee136d`  
		Last Modified: Fri, 28 Jul 2023 03:01:52 GMT  
		Size: 6.1 MB (6073620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c41c8e1cb6d4df65052cc47729124edceae5af653ff6a3555cf6e69a57f6de1`  
		Last Modified: Fri, 28 Jul 2023 03:01:51 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2516714a4b2b11720bd2fcf5338749e05ae2dff40f716814b7531fcbe356fdce`  
		Last Modified: Fri, 28 Jul 2023 03:01:51 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.21-alpine`

```console
$ docker pull memcached@sha256:8ac412315105d6fa923db09279b93ee601a4c2348b9f3fd1ccb9aa6f1562d612
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1.6.21-alpine` - linux; amd64

```console
$ docker pull memcached@sha256:574ef430513a38925cc52ae5954677a12e0a57205fed96be5707196a180e5159
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4462428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f7da63106561ab1f7284992dad2396b234096070b4269971b23c53f2f8498ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:50:58 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Wed, 14 Jun 2023 20:50:59 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 01:07:13 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 01:07:13 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:09:21 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 01:09:21 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:09:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:09:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:09:22 GMT
USER memcache
# Wed, 21 Jun 2023 01:09:22 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:09:22 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b2b2df106c5026cd33ea4ac655b77f25410ec9f4b8a6756ebc1ceeb79fca3c7`  
		Last Modified: Wed, 14 Jun 2023 20:53:58 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed63668528d3e2159f55909c66dc48a6f746ce24c2e2f6d963b992aefaa457ce`  
		Last Modified: Wed, 14 Jun 2023 20:53:58 GMT  
		Size: 108.1 KB (108080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05536f2f26c904a5aa1b07720957a37e8b57a223725d76f8d1473dcab297a233`  
		Last Modified: Wed, 21 Jun 2023 01:10:14 GMT  
		Size: 954.8 KB (954811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e448b573a98adc8bd0a4805cb0e1b451aea0d1582f0462aa0b147799a97fad7`  
		Last Modified: Wed, 21 Jun 2023 01:10:13 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3029a709b7be20aeff1e9cebe5c6112cd1df5a0ea3efb58e61380cc75b9296e`  
		Last Modified: Wed, 21 Jun 2023 01:10:13 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.21-alpine` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:eb4b801b9c9e9af6565ac003b21af39b06d55943bbc4e59a02d465fdf7f07776
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4399342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4aa99dd98a2fa001241d907951530f4afebadfd4895545c5d73f31e29b7a35fa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:57:26 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Wed, 14 Jun 2023 20:57:27 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 01:08:09 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 01:08:09 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:10:35 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 01:10:35 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:10:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:10:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:10:36 GMT
USER memcache
# Wed, 21 Jun 2023 01:10:36 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:10:36 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666588188768f19b27fb821e02d084406af8fd867cc4595b896b9eed50b2105e`  
		Last Modified: Wed, 14 Jun 2023 21:00:51 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d958a137d671266f063c0af4d7b0b6d44d9018b77fdbddb8fd412d3c0b1be3`  
		Last Modified: Wed, 14 Jun 2023 21:00:51 GMT  
		Size: 124.1 KB (124137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66841dcfe05dcef1af82648941fa1ea0e10dbdf022326916d1d74afc99885c6`  
		Last Modified: Wed, 21 Jun 2023 01:11:21 GMT  
		Size: 944.3 KB (944292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b46fdc76bcbc8fa94ae23177ac32b97a4d370a630ec7d3f52bd8aae174e75982`  
		Last Modified: Wed, 21 Jun 2023 01:11:20 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea70db1a59f508c629aef54fb39ac3ada5cfcc3aac7aa1d6ed6cde22e97d3e3b`  
		Last Modified: Wed, 21 Jun 2023 01:11:20 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.21-alpine` - linux; 386

```console
$ docker pull memcached@sha256:1468666da56924eda85c3bbc484ce7835f472fd27dd171a5bb32b2c929ef52b7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4283458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7cc593f180f84bb7bdbcb9e4b50cbc7d3c3bc0f5a83d2b6b9abce4758814bb0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 07 Aug 2023 19:38:26 GMT
ADD file:4b33c52e11b19fde30197c62ead0b77bde28d34edaa08346a5302cd892d3cebe in / 
# Mon, 07 Aug 2023 19:38:27 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 21:40:23 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Mon, 07 Aug 2023 21:40:25 GMT
RUN apk add --no-cache libsasl
# Mon, 07 Aug 2023 21:40:25 GMT
ENV MEMCACHED_VERSION=1.6.21
# Mon, 07 Aug 2023 21:40:25 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Mon, 07 Aug 2023 21:43:52 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Mon, 07 Aug 2023 21:43:52 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 07 Aug 2023 21:43:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 07 Aug 2023 21:43:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 21:43:53 GMT
USER memcache
# Mon, 07 Aug 2023 21:43:53 GMT
EXPOSE 11211
# Mon, 07 Aug 2023 21:43:53 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:95dc695758361a4038a2d9026959d72e1f531114edb0341be7ce47d912ef069e`  
		Last Modified: Mon, 07 Aug 2023 19:38:56 GMT  
		Size: 3.2 MB (3235144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:038b25459839e567ceb29349d695abf1d64f7664699e6ac0f4ea807603c54220`  
		Last Modified: Mon, 07 Aug 2023 21:44:17 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ed277dfdfb7162fb18aa73173b2a45185a326869f4ad568557b667d337b8b1`  
		Last Modified: Mon, 07 Aug 2023 21:44:17 GMT  
		Size: 109.5 KB (109531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e1b11e58caccee0d368106698c71335d98063d4ed22c19c716d2da506ddef4`  
		Last Modified: Mon, 07 Aug 2023 21:44:17 GMT  
		Size: 937.1 KB (937114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5f84ab2372dcf436661f4f50a1a95ec0e21e7bdb30ebb567b68f7c443dae44`  
		Last Modified: Mon, 07 Aug 2023 21:44:17 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa27df056ec91886a0dd6eb3b95024a3d02bb1b20b887da0525621d78d880a2`  
		Last Modified: Mon, 07 Aug 2023 21:44:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.21-alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:ed70e3e81930652804f6d430c71ed014f9daff26aa4ad302cd37c04a8ef038de
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4454755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ddfb07c34bdda47806fc2cec7489bef9f20f0e4d6d47f4c99dbf139dbd4700d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:25 GMT
ADD file:b8cf7516cdf9487d9347da0b5b5e3a6f65f24ebcdcadf81f430adb2b2664f2d1 in / 
# Mon, 07 Aug 2023 20:16:26 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 00:46:29 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 08 Aug 2023 00:46:31 GMT
RUN apk add --no-cache libsasl
# Tue, 08 Aug 2023 00:46:32 GMT
ENV MEMCACHED_VERSION=1.6.21
# Tue, 08 Aug 2023 00:46:32 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Tue, 08 Aug 2023 00:49:28 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 08 Aug 2023 00:49:28 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Aug 2023 00:49:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Aug 2023 00:49:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Aug 2023 00:49:39 GMT
USER memcache
# Tue, 08 Aug 2023 00:49:41 GMT
EXPOSE 11211
# Tue, 08 Aug 2023 00:49:43 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:55353ca330e9474ce7b858eca6842bb540ef4a70b2981c2ed47eefb9ef4253ad`  
		Last Modified: Mon, 07 Aug 2023 20:17:20 GMT  
		Size: 3.3 MB (3346251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05163a2a65d29a4d5c99749b9902892698d3b79714d37728f6a9e2f7a2c58441`  
		Last Modified: Tue, 08 Aug 2023 00:50:16 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823f7ceea96296f95c9085f083e8083413bcc70fcd4cf20b04543ab718b3419c`  
		Last Modified: Tue, 08 Aug 2023 00:50:16 GMT  
		Size: 123.9 KB (123936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a31a6f6c857bb6d5975504a61cbdfd4142af5d54776b833e03644c98433f216e`  
		Last Modified: Tue, 08 Aug 2023 00:50:18 GMT  
		Size: 982.9 KB (982892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721f4e8ef111056d9b345692fa8573c6486de7e886c2d2333e068e0bfc6e24c2`  
		Last Modified: Tue, 08 Aug 2023 00:50:16 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c144e3114e36623a8cdb3fd49d5b274689ac0d8ac00d9e1e10c402670090de1c`  
		Last Modified: Tue, 08 Aug 2023 00:50:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.21-alpine` - linux; s390x

```console
$ docker pull memcached@sha256:cd97d93e79c2345a0c10f20a912f29a0ccf5590e15c00df81596397b9567233f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4278263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f56d14fce8cfd200c86bd00cd28c95574b6bf2863bd203e7644d44a08db84ab`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 15 Jun 2023 05:18:38 GMT
ADD file:a59beca78118ebf4f86cc1685237dc3a29a519401a70668da520beaa3d29eb7a in / 
# Thu, 15 Jun 2023 05:18:38 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:27:47 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 15 Jun 2023 06:27:49 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 00:58:01 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 00:58:01 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:01:08 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 01:01:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:01:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:01:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:01:09 GMT
USER memcache
# Wed, 21 Jun 2023 01:01:10 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:01:10 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:998cc98447b44e5f0fe799dce691412796ba586ab22eb7c99aebf9d45f34833b`  
		Last Modified: Thu, 15 Jun 2023 05:29:38 GMT  
		Size: 3.2 MB (3213497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156deb87465a2c5629e5ae28c2a7251d5684baea5a930cf65ff6b478de321202`  
		Last Modified: Thu, 15 Jun 2023 06:36:33 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19020c60d58f4724218660e819b1b33b5d1428c3c5027492a2ee3c44228231df`  
		Last Modified: Thu, 15 Jun 2023 06:36:33 GMT  
		Size: 112.8 KB (112849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e76f938f015ccb0b5d2915145432efbc0af21a2f4964e0c9a67bfbbe6a577e`  
		Last Modified: Wed, 21 Jun 2023 01:01:46 GMT  
		Size: 950.3 KB (950254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b613e0a69ced3425a5949c15688d493ef10d80eb28c7bb626f0c092223fe1302`  
		Last Modified: Wed, 21 Jun 2023 01:01:46 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db4c30d38bb65cd11068e1892913b2fa04add8f27abe601485cc3b09754eb50`  
		Last Modified: Wed, 21 Jun 2023 01:01:46 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.21-alpine3.18`

```console
$ docker pull memcached@sha256:8ac412315105d6fa923db09279b93ee601a4c2348b9f3fd1ccb9aa6f1562d612
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1.6.21-alpine3.18` - linux; amd64

```console
$ docker pull memcached@sha256:574ef430513a38925cc52ae5954677a12e0a57205fed96be5707196a180e5159
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4462428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f7da63106561ab1f7284992dad2396b234096070b4269971b23c53f2f8498ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:50:58 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Wed, 14 Jun 2023 20:50:59 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 01:07:13 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 01:07:13 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:09:21 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 01:09:21 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:09:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:09:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:09:22 GMT
USER memcache
# Wed, 21 Jun 2023 01:09:22 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:09:22 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b2b2df106c5026cd33ea4ac655b77f25410ec9f4b8a6756ebc1ceeb79fca3c7`  
		Last Modified: Wed, 14 Jun 2023 20:53:58 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed63668528d3e2159f55909c66dc48a6f746ce24c2e2f6d963b992aefaa457ce`  
		Last Modified: Wed, 14 Jun 2023 20:53:58 GMT  
		Size: 108.1 KB (108080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05536f2f26c904a5aa1b07720957a37e8b57a223725d76f8d1473dcab297a233`  
		Last Modified: Wed, 21 Jun 2023 01:10:14 GMT  
		Size: 954.8 KB (954811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e448b573a98adc8bd0a4805cb0e1b451aea0d1582f0462aa0b147799a97fad7`  
		Last Modified: Wed, 21 Jun 2023 01:10:13 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3029a709b7be20aeff1e9cebe5c6112cd1df5a0ea3efb58e61380cc75b9296e`  
		Last Modified: Wed, 21 Jun 2023 01:10:13 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.21-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:eb4b801b9c9e9af6565ac003b21af39b06d55943bbc4e59a02d465fdf7f07776
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4399342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4aa99dd98a2fa001241d907951530f4afebadfd4895545c5d73f31e29b7a35fa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:57:26 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Wed, 14 Jun 2023 20:57:27 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 01:08:09 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 01:08:09 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:10:35 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 01:10:35 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:10:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:10:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:10:36 GMT
USER memcache
# Wed, 21 Jun 2023 01:10:36 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:10:36 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666588188768f19b27fb821e02d084406af8fd867cc4595b896b9eed50b2105e`  
		Last Modified: Wed, 14 Jun 2023 21:00:51 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d958a137d671266f063c0af4d7b0b6d44d9018b77fdbddb8fd412d3c0b1be3`  
		Last Modified: Wed, 14 Jun 2023 21:00:51 GMT  
		Size: 124.1 KB (124137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66841dcfe05dcef1af82648941fa1ea0e10dbdf022326916d1d74afc99885c6`  
		Last Modified: Wed, 21 Jun 2023 01:11:21 GMT  
		Size: 944.3 KB (944292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b46fdc76bcbc8fa94ae23177ac32b97a4d370a630ec7d3f52bd8aae174e75982`  
		Last Modified: Wed, 21 Jun 2023 01:11:20 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea70db1a59f508c629aef54fb39ac3ada5cfcc3aac7aa1d6ed6cde22e97d3e3b`  
		Last Modified: Wed, 21 Jun 2023 01:11:20 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.21-alpine3.18` - linux; 386

```console
$ docker pull memcached@sha256:1468666da56924eda85c3bbc484ce7835f472fd27dd171a5bb32b2c929ef52b7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4283458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7cc593f180f84bb7bdbcb9e4b50cbc7d3c3bc0f5a83d2b6b9abce4758814bb0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 07 Aug 2023 19:38:26 GMT
ADD file:4b33c52e11b19fde30197c62ead0b77bde28d34edaa08346a5302cd892d3cebe in / 
# Mon, 07 Aug 2023 19:38:27 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 21:40:23 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Mon, 07 Aug 2023 21:40:25 GMT
RUN apk add --no-cache libsasl
# Mon, 07 Aug 2023 21:40:25 GMT
ENV MEMCACHED_VERSION=1.6.21
# Mon, 07 Aug 2023 21:40:25 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Mon, 07 Aug 2023 21:43:52 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Mon, 07 Aug 2023 21:43:52 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 07 Aug 2023 21:43:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 07 Aug 2023 21:43:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 21:43:53 GMT
USER memcache
# Mon, 07 Aug 2023 21:43:53 GMT
EXPOSE 11211
# Mon, 07 Aug 2023 21:43:53 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:95dc695758361a4038a2d9026959d72e1f531114edb0341be7ce47d912ef069e`  
		Last Modified: Mon, 07 Aug 2023 19:38:56 GMT  
		Size: 3.2 MB (3235144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:038b25459839e567ceb29349d695abf1d64f7664699e6ac0f4ea807603c54220`  
		Last Modified: Mon, 07 Aug 2023 21:44:17 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ed277dfdfb7162fb18aa73173b2a45185a326869f4ad568557b667d337b8b1`  
		Last Modified: Mon, 07 Aug 2023 21:44:17 GMT  
		Size: 109.5 KB (109531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e1b11e58caccee0d368106698c71335d98063d4ed22c19c716d2da506ddef4`  
		Last Modified: Mon, 07 Aug 2023 21:44:17 GMT  
		Size: 937.1 KB (937114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5f84ab2372dcf436661f4f50a1a95ec0e21e7bdb30ebb567b68f7c443dae44`  
		Last Modified: Mon, 07 Aug 2023 21:44:17 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa27df056ec91886a0dd6eb3b95024a3d02bb1b20b887da0525621d78d880a2`  
		Last Modified: Mon, 07 Aug 2023 21:44:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.21-alpine3.18` - linux; ppc64le

```console
$ docker pull memcached@sha256:ed70e3e81930652804f6d430c71ed014f9daff26aa4ad302cd37c04a8ef038de
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4454755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ddfb07c34bdda47806fc2cec7489bef9f20f0e4d6d47f4c99dbf139dbd4700d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:25 GMT
ADD file:b8cf7516cdf9487d9347da0b5b5e3a6f65f24ebcdcadf81f430adb2b2664f2d1 in / 
# Mon, 07 Aug 2023 20:16:26 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 00:46:29 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 08 Aug 2023 00:46:31 GMT
RUN apk add --no-cache libsasl
# Tue, 08 Aug 2023 00:46:32 GMT
ENV MEMCACHED_VERSION=1.6.21
# Tue, 08 Aug 2023 00:46:32 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Tue, 08 Aug 2023 00:49:28 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 08 Aug 2023 00:49:28 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Aug 2023 00:49:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Aug 2023 00:49:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Aug 2023 00:49:39 GMT
USER memcache
# Tue, 08 Aug 2023 00:49:41 GMT
EXPOSE 11211
# Tue, 08 Aug 2023 00:49:43 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:55353ca330e9474ce7b858eca6842bb540ef4a70b2981c2ed47eefb9ef4253ad`  
		Last Modified: Mon, 07 Aug 2023 20:17:20 GMT  
		Size: 3.3 MB (3346251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05163a2a65d29a4d5c99749b9902892698d3b79714d37728f6a9e2f7a2c58441`  
		Last Modified: Tue, 08 Aug 2023 00:50:16 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823f7ceea96296f95c9085f083e8083413bcc70fcd4cf20b04543ab718b3419c`  
		Last Modified: Tue, 08 Aug 2023 00:50:16 GMT  
		Size: 123.9 KB (123936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a31a6f6c857bb6d5975504a61cbdfd4142af5d54776b833e03644c98433f216e`  
		Last Modified: Tue, 08 Aug 2023 00:50:18 GMT  
		Size: 982.9 KB (982892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721f4e8ef111056d9b345692fa8573c6486de7e886c2d2333e068e0bfc6e24c2`  
		Last Modified: Tue, 08 Aug 2023 00:50:16 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c144e3114e36623a8cdb3fd49d5b274689ac0d8ac00d9e1e10c402670090de1c`  
		Last Modified: Tue, 08 Aug 2023 00:50:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.21-alpine3.18` - linux; s390x

```console
$ docker pull memcached@sha256:cd97d93e79c2345a0c10f20a912f29a0ccf5590e15c00df81596397b9567233f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4278263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f56d14fce8cfd200c86bd00cd28c95574b6bf2863bd203e7644d44a08db84ab`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 15 Jun 2023 05:18:38 GMT
ADD file:a59beca78118ebf4f86cc1685237dc3a29a519401a70668da520beaa3d29eb7a in / 
# Thu, 15 Jun 2023 05:18:38 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:27:47 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 15 Jun 2023 06:27:49 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 00:58:01 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 00:58:01 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:01:08 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 01:01:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:01:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:01:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:01:09 GMT
USER memcache
# Wed, 21 Jun 2023 01:01:10 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:01:10 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:998cc98447b44e5f0fe799dce691412796ba586ab22eb7c99aebf9d45f34833b`  
		Last Modified: Thu, 15 Jun 2023 05:29:38 GMT  
		Size: 3.2 MB (3213497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156deb87465a2c5629e5ae28c2a7251d5684baea5a930cf65ff6b478de321202`  
		Last Modified: Thu, 15 Jun 2023 06:36:33 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19020c60d58f4724218660e819b1b33b5d1428c3c5027492a2ee3c44228231df`  
		Last Modified: Thu, 15 Jun 2023 06:36:33 GMT  
		Size: 112.8 KB (112849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e76f938f015ccb0b5d2915145432efbc0af21a2f4964e0c9a67bfbbe6a577e`  
		Last Modified: Wed, 21 Jun 2023 01:01:46 GMT  
		Size: 950.3 KB (950254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b613e0a69ced3425a5949c15688d493ef10d80eb28c7bb626f0c092223fe1302`  
		Last Modified: Wed, 21 Jun 2023 01:01:46 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db4c30d38bb65cd11068e1892913b2fa04add8f27abe601485cc3b09754eb50`  
		Last Modified: Wed, 21 Jun 2023 01:01:46 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:1.6.21-bookworm`

```console
$ docker pull memcached@sha256:a917777975a7039b6ed70ef2faab453b1e5ea7aa741899aba952d744546cc781
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `memcached:1.6.21-bookworm` - linux; amd64

```console
$ docker pull memcached@sha256:0c8398104f83351267e51ec72b34de06b734f2eca6637c10d246702afff814b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.0 MB (38974916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:354b899e400fa323ffaea769644cc66778676b4f4eeca0e3e1523100e8803d97`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:44 GMT
ADD file:209589a8bdb5a3788ee42ecdbccbbb561835dab96b0d8286bb5a2229d2f41be7 in / 
# Thu, 27 Jul 2023 23:24:45 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 04:03:18 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 28 Jul 2023 04:03:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 04:03:22 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 28 Jul 2023 04:03:22 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 28 Jul 2023 04:05:37 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 28 Jul 2023 04:05:37 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 28 Jul 2023 04:05:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 04:05:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 04:05:38 GMT
USER memcache
# Fri, 28 Jul 2023 04:05:38 GMT
EXPOSE 11211
# Fri, 28 Jul 2023 04:05:38 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:648e0aadf75ac2ef63c5390adc6dc14fde37a5ad88c2870ea604df0a9c0eb4e5`  
		Last Modified: Thu, 27 Jul 2023 23:29:26 GMT  
		Size: 29.1 MB (29124532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baaf8e9cef6b92919a723712ed912794373f6fc1d8dac9d5ed1d320378f657ba`  
		Last Modified: Fri, 28 Jul 2023 04:05:56 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52dca4bf886a56187b224e812b7a65f7825798dc8d536db9bb9344cb112b98e0`  
		Last Modified: Fri, 28 Jul 2023 04:05:56 GMT  
		Size: 2.7 MB (2677283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6861252b28dd75ed1a4f9accdcef6f35366a5dd59d3d7921945a20ec3f64661`  
		Last Modified: Fri, 28 Jul 2023 04:05:57 GMT  
		Size: 7.2 MB (7171562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49870ab6c52b8db6c693e18bd63b718827cd451bde693287ca70314a991cbfb6`  
		Last Modified: Fri, 28 Jul 2023 04:05:56 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da541564580ce27d2c3710f1420b22d4bc544196f1bf6536a5c58150854283d`  
		Last Modified: Fri, 28 Jul 2023 04:05:56 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.21-bookworm` - linux; arm variant v5

```console
$ docker pull memcached@sha256:ec7dc6727737267a059c047a43864e1c5bdda0a6b8d3cdd0b49110523acfe7f7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35098422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8ce1a3d6a1d0c9162fa735664905dded291bfaa1a0398a381448950a7b9ee91`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 27 Jul 2023 23:48:29 GMT
ADD file:53cf36eb7b72a7e970f4b18af1589402b2900f12e30820cdeccc8bb0c166df80 in / 
# Thu, 27 Jul 2023 23:48:30 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 11:05:31 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 28 Jul 2023 11:05:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 11:05:37 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 28 Jul 2023 11:05:37 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 28 Jul 2023 11:08:31 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 28 Jul 2023 11:08:31 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 28 Jul 2023 11:08:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 11:08:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 11:08:31 GMT
USER memcache
# Fri, 28 Jul 2023 11:08:31 GMT
EXPOSE 11211
# Fri, 28 Jul 2023 11:08:32 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2bd6dfc5281e13a0ca9fb8d9238ac9f14a0de04489913030c8e33b9398b4a4af`  
		Last Modified: Thu, 27 Jul 2023 23:51:28 GMT  
		Size: 27.0 MB (26983508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5936d9d99182ef30677e20dad76c0549b2b7612ca100ef6c0f03c87027cee0b`  
		Last Modified: Fri, 28 Jul 2023 11:08:45 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7717a35af981145073f1343f8447ffd5b5c52de46680b1e75e4c0c11ba64bf`  
		Last Modified: Fri, 28 Jul 2023 11:08:46 GMT  
		Size: 2.3 MB (2281851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56b5203e649ffe900465b0cf521d6be756bd5dd83b5905d7ccc6aced143610b`  
		Last Modified: Fri, 28 Jul 2023 11:08:47 GMT  
		Size: 5.8 MB (5831523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6dee9c51b3b15c0179684c9c61eebfc3091a8f40afd9714ddae2728364aee4f`  
		Last Modified: Fri, 28 Jul 2023 11:08:45 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51b980bae702ef385ef2cbe3eb556c8377334b4c31c97e39cced7ed58375bc55`  
		Last Modified: Fri, 28 Jul 2023 11:08:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.21-bookworm` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:4b2d19d8c0d48b44b1f24b2ea0e8a62749f05db1bedbe481ff6112db44c703cc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.9 MB (37878121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c74af541d05a0758cbf5f13d5d190f1ab10b86ef5fd75112aa98b0638def7d9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 27 Jul 2023 23:43:00 GMT
ADD file:1de2ba0dc88aa343332814e19adc6b850d08e62c31589fe902b8eb2cb465934e in / 
# Thu, 27 Jul 2023 23:43:00 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 06:38:57 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 28 Jul 2023 06:39:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 06:39:01 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 28 Jul 2023 06:39:01 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 28 Jul 2023 06:41:36 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 28 Jul 2023 06:41:36 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 28 Jul 2023 06:41:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 06:41:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 06:41:37 GMT
USER memcache
# Fri, 28 Jul 2023 06:41:37 GMT
EXPOSE 11211
# Fri, 28 Jul 2023 06:41:37 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:90524f7dc01b4ce9b387992acc6cbdbcc2a9ee8c6addfd632429ca06ea18751e`  
		Last Modified: Thu, 27 Jul 2023 23:46:17 GMT  
		Size: 29.2 MB (29157226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6146d0684a3303f06ef62333440ab9aba6cab719b5762ddaee7f7b7a3a62e9ee`  
		Last Modified: Fri, 28 Jul 2023 06:42:01 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b513dbaa02d89264c8df677c8871ec60a8cba234a96d77165fc06157ed2ec1f`  
		Last Modified: Fri, 28 Jul 2023 06:42:01 GMT  
		Size: 2.5 MB (2539192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe211375d2d86acd694c377eeaf6fe900e6f57dadd07e6bd6f21809eab75c53a`  
		Last Modified: Fri, 28 Jul 2023 06:42:02 GMT  
		Size: 6.2 MB (6180162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1b4b070b2921c7d9f5349e7b258c1400ac5d0a1154df0028e634899e86fbda`  
		Last Modified: Fri, 28 Jul 2023 06:42:01 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d40396358d46edf0c2615a77e13da10249786f2546d4a9623e18ec0ce9d6aa91`  
		Last Modified: Fri, 28 Jul 2023 06:42:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.21-bookworm` - linux; 386

```console
$ docker pull memcached@sha256:d3e70a847a7f720a3a129c6e060b3f9b3428add5e0458c1974a6a895783073e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39459484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fe4fee0ccc34611e17f9be47d4048890aa66e445397fb679f2f27edcb5de08a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 27 Jul 2023 23:38:56 GMT
ADD file:3d6e6f3e900e480a7e060fcaf57313c0f954bf906967a7fa0317567c387cf5aa in / 
# Thu, 27 Jul 2023 23:38:57 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 00:12:30 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 28 Jul 2023 00:12:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 00:12:35 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 28 Jul 2023 00:12:35 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 28 Jul 2023 00:16:17 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 28 Jul 2023 00:16:17 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 28 Jul 2023 00:16:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 00:16:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 00:16:18 GMT
USER memcache
# Fri, 28 Jul 2023 00:16:18 GMT
EXPOSE 11211
# Fri, 28 Jul 2023 00:16:18 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3a8b0c4b1a83609d978d576be6174f951ff27084d7c9aef91892b60b223a5104`  
		Last Modified: Thu, 27 Jul 2023 23:43:26 GMT  
		Size: 30.1 MB (30141788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:700ff590600873a2721ed53371f8797b79c09c48cf32c7190640b4a1d4f5755d`  
		Last Modified: Fri, 28 Jul 2023 00:16:36 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f15bfc1eebf505da6ff5a5b1b1810ad762b79725e742a9b354c57fbabd31f01a`  
		Last Modified: Fri, 28 Jul 2023 00:16:37 GMT  
		Size: 2.7 MB (2685093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80fdef0976acae3ce13d23a176fc9e9ce15eeb2ac874a0915725bbaa3108059b`  
		Last Modified: Fri, 28 Jul 2023 00:16:38 GMT  
		Size: 6.6 MB (6631063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3442227f7348458fb36b2e0d739658a8fb589ed322fd578df8e39e59fc32000d`  
		Last Modified: Fri, 28 Jul 2023 00:16:36 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5501a93139182f8a01992f6de5a5e4eaebdebaaec5a10506a07f59b936d266e6`  
		Last Modified: Fri, 28 Jul 2023 00:16:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.21-bookworm` - linux; mips64le

```console
$ docker pull memcached@sha256:fbc5c08e8c901f9b6c9cab47733639d29f3ff1167ab861aa26fe0bb751a308d9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.6 MB (37558667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f390b2a92aa8ce938675a24263c1e7f6b619c4c584343f3dd7a0e9d6615051d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 27 Jul 2023 23:11:23 GMT
ADD file:90cbcf9a2aaf48a433b00118dd0821eeb291092da7b7f67ce6a525ce2cba1e3f in / 
# Thu, 27 Jul 2023 23:11:27 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:45:56 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 28 Jul 2023 01:46:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:46:17 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 28 Jul 2023 01:46:19 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 28 Jul 2023 01:53:01 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 28 Jul 2023 01:53:03 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 28 Jul 2023 01:53:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 01:53:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 01:53:14 GMT
USER memcache
# Fri, 28 Jul 2023 01:53:16 GMT
EXPOSE 11211
# Fri, 28 Jul 2023 01:53:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3252778e08fa8eb67ab052ad63281284b5ef1afdc40a36021228133487ab5d52`  
		Last Modified: Thu, 27 Jul 2023 23:22:26 GMT  
		Size: 29.1 MB (29121405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63e55e013f2ab63ff93eaaf154b0debea8de9ffc8fbadaf67d3bc03851f57910`  
		Last Modified: Fri, 28 Jul 2023 01:53:46 GMT  
		Size: 1.1 KB (1082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d9a9f24853cb0188d2273603847b46ed81bd544b868ae314d609c1d9e7db7c`  
		Last Modified: Fri, 28 Jul 2023 01:53:48 GMT  
		Size: 1.9 MB (1934904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4467025968ec633fd090be17fe8c5f61d7ee738a0b34a10db006d35397e27cc`  
		Last Modified: Fri, 28 Jul 2023 01:53:51 GMT  
		Size: 6.5 MB (6500867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07da0cd083ab7d3e91ac9e7ae33d316bd7affeb2852262ff2d687be0e5c273b6`  
		Last Modified: Fri, 28 Jul 2023 01:53:46 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57f5929847506e0cf79067f8348bd883548c83f0c23defbaccf512eb17d65758`  
		Last Modified: Fri, 28 Jul 2023 01:53:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.21-bookworm` - linux; ppc64le

```console
$ docker pull memcached@sha256:a32969620e95d4b08d5711678e6bcbd313e3bc3511d1b96cf5d08e675a90d0fb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43196803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d6a8d8d3e6746723698507be3f910bb02f0a22617da462f56031004e606edf6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 27 Jul 2023 23:23:01 GMT
ADD file:774a99e5c40757d27c981eb5ad6e03eb72970bb0c54f799eab1442624238ea3e in / 
# Thu, 27 Jul 2023 23:23:03 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:38:39 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 28 Jul 2023 03:38:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:38:51 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 28 Jul 2023 03:38:52 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 28 Jul 2023 03:42:57 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 28 Jul 2023 03:42:58 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 28 Jul 2023 03:43:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 03:43:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 03:43:01 GMT
USER memcache
# Fri, 28 Jul 2023 03:43:02 GMT
EXPOSE 11211
# Fri, 28 Jul 2023 03:43:03 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:ad974e0ada84177d519dec70d0d7d9ff6a4f468bc7306425feb8429bc276bd8a`  
		Last Modified: Thu, 27 Jul 2023 23:29:24 GMT  
		Size: 33.1 MB (33119211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ed68aff2ca1a6e8c25d8462f4b2ebbb3866c768911785569560ede6a2f053d`  
		Last Modified: Fri, 28 Jul 2023 03:43:33 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d519acbf803e11e9a1e21f396dd4e021495fa7b97a4c9df3e6f7639d8c050790`  
		Last Modified: Fri, 28 Jul 2023 03:43:33 GMT  
		Size: 2.9 MB (2891351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:097534b38ed1845470192cab29ec2d22d4e0c7a9d5f01c9948ebc1273dfe809c`  
		Last Modified: Fri, 28 Jul 2023 03:43:35 GMT  
		Size: 7.2 MB (7184700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2f9c6ce8e611c611c0bfdb7cb8ec798950618d80a9be8db98c59fdd0654825`  
		Last Modified: Fri, 28 Jul 2023 03:43:33 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d974aa6a849abcd290ae3bbfbc44f776e3928269bfa1bdbc65e2a1f11c368afe`  
		Last Modified: Fri, 28 Jul 2023 03:43:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:1.6.21-bookworm` - linux; s390x

```console
$ docker pull memcached@sha256:1ab909233ee99a6798929725205b93abb2bd9a8c78ab048d925dffd359fe8cf2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35910248 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:845b0ff32d8c04c5820146361e7a2e8c8579ad2a96318fdbc7e6c669bfc27569`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 27 Jul 2023 23:47:11 GMT
ADD file:0a5e1e86b375d60637d0829f77a12085777cf2ca07495b0f6249d8efea84e958 in / 
# Thu, 27 Jul 2023 23:47:13 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 02:58:10 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 28 Jul 2023 02:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 02:58:13 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 28 Jul 2023 02:58:13 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 28 Jul 2023 03:01:19 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 28 Jul 2023 03:01:20 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 28 Jul 2023 03:01:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 03:01:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 03:01:20 GMT
USER memcache
# Fri, 28 Jul 2023 03:01:20 GMT
EXPOSE 11211
# Fri, 28 Jul 2023 03:01:21 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f4301d25bb1bea85fcc5b364aec84ff58274f714cea191ab22d9b1b1e4f78527`  
		Last Modified: Thu, 27 Jul 2023 23:52:17 GMT  
		Size: 27.5 MB (27489697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8055eb96c9dacdcc9c91194a8d4504ab82a88a0fa9f927413c1dde2e493a815`  
		Last Modified: Fri, 28 Jul 2023 03:01:51 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:040e9d91e418b36f9ea07fcd1d9db85ae7713bd99a0a17f31f41a7ef410c3423`  
		Last Modified: Fri, 28 Jul 2023 03:01:54 GMT  
		Size: 2.3 MB (2345395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a638c5b62a02bc60b52234e1556bcf148e66b74e50a0bd02d2b5f23ea2ee136d`  
		Last Modified: Fri, 28 Jul 2023 03:01:52 GMT  
		Size: 6.1 MB (6073620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c41c8e1cb6d4df65052cc47729124edceae5af653ff6a3555cf6e69a57f6de1`  
		Last Modified: Fri, 28 Jul 2023 03:01:51 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2516714a4b2b11720bd2fcf5338749e05ae2dff40f716814b7531fcbe356fdce`  
		Last Modified: Fri, 28 Jul 2023 03:01:51 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:alpine`

```console
$ docker pull memcached@sha256:bb610e3fb1dcd27fa39cf120269b71ab32f1202deb4b517a2b80f17fe90beb5f
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
$ docker pull memcached@sha256:574ef430513a38925cc52ae5954677a12e0a57205fed96be5707196a180e5159
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4462428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f7da63106561ab1f7284992dad2396b234096070b4269971b23c53f2f8498ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:50:58 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Wed, 14 Jun 2023 20:50:59 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 01:07:13 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 01:07:13 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:09:21 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 01:09:21 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:09:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:09:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:09:22 GMT
USER memcache
# Wed, 21 Jun 2023 01:09:22 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:09:22 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b2b2df106c5026cd33ea4ac655b77f25410ec9f4b8a6756ebc1ceeb79fca3c7`  
		Last Modified: Wed, 14 Jun 2023 20:53:58 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed63668528d3e2159f55909c66dc48a6f746ce24c2e2f6d963b992aefaa457ce`  
		Last Modified: Wed, 14 Jun 2023 20:53:58 GMT  
		Size: 108.1 KB (108080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05536f2f26c904a5aa1b07720957a37e8b57a223725d76f8d1473dcab297a233`  
		Last Modified: Wed, 21 Jun 2023 01:10:14 GMT  
		Size: 954.8 KB (954811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e448b573a98adc8bd0a4805cb0e1b451aea0d1582f0462aa0b147799a97fad7`  
		Last Modified: Wed, 21 Jun 2023 01:10:13 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3029a709b7be20aeff1e9cebe5c6112cd1df5a0ea3efb58e61380cc75b9296e`  
		Last Modified: Wed, 21 Jun 2023 01:10:13 GMT  
		Size: 117.0 B  
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
$ docker pull memcached@sha256:eb4b801b9c9e9af6565ac003b21af39b06d55943bbc4e59a02d465fdf7f07776
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4399342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4aa99dd98a2fa001241d907951530f4afebadfd4895545c5d73f31e29b7a35fa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:57:26 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Wed, 14 Jun 2023 20:57:27 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 01:08:09 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 01:08:09 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:10:35 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 01:10:35 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:10:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:10:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:10:36 GMT
USER memcache
# Wed, 21 Jun 2023 01:10:36 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:10:36 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666588188768f19b27fb821e02d084406af8fd867cc4595b896b9eed50b2105e`  
		Last Modified: Wed, 14 Jun 2023 21:00:51 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d958a137d671266f063c0af4d7b0b6d44d9018b77fdbddb8fd412d3c0b1be3`  
		Last Modified: Wed, 14 Jun 2023 21:00:51 GMT  
		Size: 124.1 KB (124137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66841dcfe05dcef1af82648941fa1ea0e10dbdf022326916d1d74afc99885c6`  
		Last Modified: Wed, 21 Jun 2023 01:11:21 GMT  
		Size: 944.3 KB (944292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b46fdc76bcbc8fa94ae23177ac32b97a4d370a630ec7d3f52bd8aae174e75982`  
		Last Modified: Wed, 21 Jun 2023 01:11:20 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea70db1a59f508c629aef54fb39ac3ada5cfcc3aac7aa1d6ed6cde22e97d3e3b`  
		Last Modified: Wed, 21 Jun 2023 01:11:20 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; 386

```console
$ docker pull memcached@sha256:1468666da56924eda85c3bbc484ce7835f472fd27dd171a5bb32b2c929ef52b7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4283458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7cc593f180f84bb7bdbcb9e4b50cbc7d3c3bc0f5a83d2b6b9abce4758814bb0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 07 Aug 2023 19:38:26 GMT
ADD file:4b33c52e11b19fde30197c62ead0b77bde28d34edaa08346a5302cd892d3cebe in / 
# Mon, 07 Aug 2023 19:38:27 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 21:40:23 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Mon, 07 Aug 2023 21:40:25 GMT
RUN apk add --no-cache libsasl
# Mon, 07 Aug 2023 21:40:25 GMT
ENV MEMCACHED_VERSION=1.6.21
# Mon, 07 Aug 2023 21:40:25 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Mon, 07 Aug 2023 21:43:52 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Mon, 07 Aug 2023 21:43:52 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 07 Aug 2023 21:43:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 07 Aug 2023 21:43:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 21:43:53 GMT
USER memcache
# Mon, 07 Aug 2023 21:43:53 GMT
EXPOSE 11211
# Mon, 07 Aug 2023 21:43:53 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:95dc695758361a4038a2d9026959d72e1f531114edb0341be7ce47d912ef069e`  
		Last Modified: Mon, 07 Aug 2023 19:38:56 GMT  
		Size: 3.2 MB (3235144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:038b25459839e567ceb29349d695abf1d64f7664699e6ac0f4ea807603c54220`  
		Last Modified: Mon, 07 Aug 2023 21:44:17 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ed277dfdfb7162fb18aa73173b2a45185a326869f4ad568557b667d337b8b1`  
		Last Modified: Mon, 07 Aug 2023 21:44:17 GMT  
		Size: 109.5 KB (109531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e1b11e58caccee0d368106698c71335d98063d4ed22c19c716d2da506ddef4`  
		Last Modified: Mon, 07 Aug 2023 21:44:17 GMT  
		Size: 937.1 KB (937114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5f84ab2372dcf436661f4f50a1a95ec0e21e7bdb30ebb567b68f7c443dae44`  
		Last Modified: Mon, 07 Aug 2023 21:44:17 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa27df056ec91886a0dd6eb3b95024a3d02bb1b20b887da0525621d78d880a2`  
		Last Modified: Mon, 07 Aug 2023 21:44:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; ppc64le

```console
$ docker pull memcached@sha256:ed70e3e81930652804f6d430c71ed014f9daff26aa4ad302cd37c04a8ef038de
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4454755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ddfb07c34bdda47806fc2cec7489bef9f20f0e4d6d47f4c99dbf139dbd4700d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:25 GMT
ADD file:b8cf7516cdf9487d9347da0b5b5e3a6f65f24ebcdcadf81f430adb2b2664f2d1 in / 
# Mon, 07 Aug 2023 20:16:26 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 00:46:29 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 08 Aug 2023 00:46:31 GMT
RUN apk add --no-cache libsasl
# Tue, 08 Aug 2023 00:46:32 GMT
ENV MEMCACHED_VERSION=1.6.21
# Tue, 08 Aug 2023 00:46:32 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Tue, 08 Aug 2023 00:49:28 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 08 Aug 2023 00:49:28 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Aug 2023 00:49:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Aug 2023 00:49:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Aug 2023 00:49:39 GMT
USER memcache
# Tue, 08 Aug 2023 00:49:41 GMT
EXPOSE 11211
# Tue, 08 Aug 2023 00:49:43 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:55353ca330e9474ce7b858eca6842bb540ef4a70b2981c2ed47eefb9ef4253ad`  
		Last Modified: Mon, 07 Aug 2023 20:17:20 GMT  
		Size: 3.3 MB (3346251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05163a2a65d29a4d5c99749b9902892698d3b79714d37728f6a9e2f7a2c58441`  
		Last Modified: Tue, 08 Aug 2023 00:50:16 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823f7ceea96296f95c9085f083e8083413bcc70fcd4cf20b04543ab718b3419c`  
		Last Modified: Tue, 08 Aug 2023 00:50:16 GMT  
		Size: 123.9 KB (123936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a31a6f6c857bb6d5975504a61cbdfd4142af5d54776b833e03644c98433f216e`  
		Last Modified: Tue, 08 Aug 2023 00:50:18 GMT  
		Size: 982.9 KB (982892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721f4e8ef111056d9b345692fa8573c6486de7e886c2d2333e068e0bfc6e24c2`  
		Last Modified: Tue, 08 Aug 2023 00:50:16 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c144e3114e36623a8cdb3fd49d5b274689ac0d8ac00d9e1e10c402670090de1c`  
		Last Modified: Tue, 08 Aug 2023 00:50:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine` - linux; s390x

```console
$ docker pull memcached@sha256:cd97d93e79c2345a0c10f20a912f29a0ccf5590e15c00df81596397b9567233f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4278263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f56d14fce8cfd200c86bd00cd28c95574b6bf2863bd203e7644d44a08db84ab`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 15 Jun 2023 05:18:38 GMT
ADD file:a59beca78118ebf4f86cc1685237dc3a29a519401a70668da520beaa3d29eb7a in / 
# Thu, 15 Jun 2023 05:18:38 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:27:47 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 15 Jun 2023 06:27:49 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 00:58:01 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 00:58:01 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:01:08 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 01:01:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:01:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:01:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:01:09 GMT
USER memcache
# Wed, 21 Jun 2023 01:01:10 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:01:10 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:998cc98447b44e5f0fe799dce691412796ba586ab22eb7c99aebf9d45f34833b`  
		Last Modified: Thu, 15 Jun 2023 05:29:38 GMT  
		Size: 3.2 MB (3213497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156deb87465a2c5629e5ae28c2a7251d5684baea5a930cf65ff6b478de321202`  
		Last Modified: Thu, 15 Jun 2023 06:36:33 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19020c60d58f4724218660e819b1b33b5d1428c3c5027492a2ee3c44228231df`  
		Last Modified: Thu, 15 Jun 2023 06:36:33 GMT  
		Size: 112.8 KB (112849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e76f938f015ccb0b5d2915145432efbc0af21a2f4964e0c9a67bfbbe6a577e`  
		Last Modified: Wed, 21 Jun 2023 01:01:46 GMT  
		Size: 950.3 KB (950254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b613e0a69ced3425a5949c15688d493ef10d80eb28c7bb626f0c092223fe1302`  
		Last Modified: Wed, 21 Jun 2023 01:01:46 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db4c30d38bb65cd11068e1892913b2fa04add8f27abe601485cc3b09754eb50`  
		Last Modified: Wed, 21 Jun 2023 01:01:46 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:alpine3.18`

```console
$ docker pull memcached@sha256:8ac412315105d6fa923db09279b93ee601a4c2348b9f3fd1ccb9aa6f1562d612
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `memcached:alpine3.18` - linux; amd64

```console
$ docker pull memcached@sha256:574ef430513a38925cc52ae5954677a12e0a57205fed96be5707196a180e5159
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4462428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f7da63106561ab1f7284992dad2396b234096070b4269971b23c53f2f8498ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:50:58 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Wed, 14 Jun 2023 20:50:59 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 01:07:13 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 01:07:13 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:09:21 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 01:09:21 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:09:22 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:09:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:09:22 GMT
USER memcache
# Wed, 21 Jun 2023 01:09:22 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:09:22 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b2b2df106c5026cd33ea4ac655b77f25410ec9f4b8a6756ebc1ceeb79fca3c7`  
		Last Modified: Wed, 14 Jun 2023 20:53:58 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed63668528d3e2159f55909c66dc48a6f746ce24c2e2f6d963b992aefaa457ce`  
		Last Modified: Wed, 14 Jun 2023 20:53:58 GMT  
		Size: 108.1 KB (108080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05536f2f26c904a5aa1b07720957a37e8b57a223725d76f8d1473dcab297a233`  
		Last Modified: Wed, 21 Jun 2023 01:10:14 GMT  
		Size: 954.8 KB (954811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e448b573a98adc8bd0a4805cb0e1b451aea0d1582f0462aa0b147799a97fad7`  
		Last Modified: Wed, 21 Jun 2023 01:10:13 GMT  
		Size: 275.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3029a709b7be20aeff1e9cebe5c6112cd1df5a0ea3efb58e61380cc75b9296e`  
		Last Modified: Wed, 21 Jun 2023 01:10:13 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine3.18` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:eb4b801b9c9e9af6565ac003b21af39b06d55943bbc4e59a02d465fdf7f07776
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4399342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4aa99dd98a2fa001241d907951530f4afebadfd4895545c5d73f31e29b7a35fa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Wed, 14 Jun 2023 20:57:26 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Wed, 14 Jun 2023 20:57:27 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 01:08:09 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 01:08:09 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:10:35 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 01:10:35 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:10:36 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:10:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:10:36 GMT
USER memcache
# Wed, 21 Jun 2023 01:10:36 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:10:36 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666588188768f19b27fb821e02d084406af8fd867cc4595b896b9eed50b2105e`  
		Last Modified: Wed, 14 Jun 2023 21:00:51 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d958a137d671266f063c0af4d7b0b6d44d9018b77fdbddb8fd412d3c0b1be3`  
		Last Modified: Wed, 14 Jun 2023 21:00:51 GMT  
		Size: 124.1 KB (124137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66841dcfe05dcef1af82648941fa1ea0e10dbdf022326916d1d74afc99885c6`  
		Last Modified: Wed, 21 Jun 2023 01:11:21 GMT  
		Size: 944.3 KB (944292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b46fdc76bcbc8fa94ae23177ac32b97a4d370a630ec7d3f52bd8aae174e75982`  
		Last Modified: Wed, 21 Jun 2023 01:11:20 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea70db1a59f508c629aef54fb39ac3ada5cfcc3aac7aa1d6ed6cde22e97d3e3b`  
		Last Modified: Wed, 21 Jun 2023 01:11:20 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine3.18` - linux; 386

```console
$ docker pull memcached@sha256:1468666da56924eda85c3bbc484ce7835f472fd27dd171a5bb32b2c929ef52b7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4283458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7cc593f180f84bb7bdbcb9e4b50cbc7d3c3bc0f5a83d2b6b9abce4758814bb0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 07 Aug 2023 19:38:26 GMT
ADD file:4b33c52e11b19fde30197c62ead0b77bde28d34edaa08346a5302cd892d3cebe in / 
# Mon, 07 Aug 2023 19:38:27 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 21:40:23 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Mon, 07 Aug 2023 21:40:25 GMT
RUN apk add --no-cache libsasl
# Mon, 07 Aug 2023 21:40:25 GMT
ENV MEMCACHED_VERSION=1.6.21
# Mon, 07 Aug 2023 21:40:25 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Mon, 07 Aug 2023 21:43:52 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Mon, 07 Aug 2023 21:43:52 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Mon, 07 Aug 2023 21:43:53 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Mon, 07 Aug 2023 21:43:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 21:43:53 GMT
USER memcache
# Mon, 07 Aug 2023 21:43:53 GMT
EXPOSE 11211
# Mon, 07 Aug 2023 21:43:53 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:95dc695758361a4038a2d9026959d72e1f531114edb0341be7ce47d912ef069e`  
		Last Modified: Mon, 07 Aug 2023 19:38:56 GMT  
		Size: 3.2 MB (3235144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:038b25459839e567ceb29349d695abf1d64f7664699e6ac0f4ea807603c54220`  
		Last Modified: Mon, 07 Aug 2023 21:44:17 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ed277dfdfb7162fb18aa73173b2a45185a326869f4ad568557b667d337b8b1`  
		Last Modified: Mon, 07 Aug 2023 21:44:17 GMT  
		Size: 109.5 KB (109531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e1b11e58caccee0d368106698c71335d98063d4ed22c19c716d2da506ddef4`  
		Last Modified: Mon, 07 Aug 2023 21:44:17 GMT  
		Size: 937.1 KB (937114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5f84ab2372dcf436661f4f50a1a95ec0e21e7bdb30ebb567b68f7c443dae44`  
		Last Modified: Mon, 07 Aug 2023 21:44:17 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa27df056ec91886a0dd6eb3b95024a3d02bb1b20b887da0525621d78d880a2`  
		Last Modified: Mon, 07 Aug 2023 21:44:17 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine3.18` - linux; ppc64le

```console
$ docker pull memcached@sha256:ed70e3e81930652804f6d430c71ed014f9daff26aa4ad302cd37c04a8ef038de
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4454755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ddfb07c34bdda47806fc2cec7489bef9f20f0e4d6d47f4c99dbf139dbd4700d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:25 GMT
ADD file:b8cf7516cdf9487d9347da0b5b5e3a6f65f24ebcdcadf81f430adb2b2664f2d1 in / 
# Mon, 07 Aug 2023 20:16:26 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 00:46:29 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Tue, 08 Aug 2023 00:46:31 GMT
RUN apk add --no-cache libsasl
# Tue, 08 Aug 2023 00:46:32 GMT
ENV MEMCACHED_VERSION=1.6.21
# Tue, 08 Aug 2023 00:46:32 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Tue, 08 Aug 2023 00:49:28 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Tue, 08 Aug 2023 00:49:28 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Tue, 08 Aug 2023 00:49:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Tue, 08 Aug 2023 00:49:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Aug 2023 00:49:39 GMT
USER memcache
# Tue, 08 Aug 2023 00:49:41 GMT
EXPOSE 11211
# Tue, 08 Aug 2023 00:49:43 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:55353ca330e9474ce7b858eca6842bb540ef4a70b2981c2ed47eefb9ef4253ad`  
		Last Modified: Mon, 07 Aug 2023 20:17:20 GMT  
		Size: 3.3 MB (3346251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05163a2a65d29a4d5c99749b9902892698d3b79714d37728f6a9e2f7a2c58441`  
		Last Modified: Tue, 08 Aug 2023 00:50:16 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823f7ceea96296f95c9085f083e8083413bcc70fcd4cf20b04543ab718b3419c`  
		Last Modified: Tue, 08 Aug 2023 00:50:16 GMT  
		Size: 123.9 KB (123936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a31a6f6c857bb6d5975504a61cbdfd4142af5d54776b833e03644c98433f216e`  
		Last Modified: Tue, 08 Aug 2023 00:50:18 GMT  
		Size: 982.9 KB (982892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721f4e8ef111056d9b345692fa8573c6486de7e886c2d2333e068e0bfc6e24c2`  
		Last Modified: Tue, 08 Aug 2023 00:50:16 GMT  
		Size: 284.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c144e3114e36623a8cdb3fd49d5b274689ac0d8ac00d9e1e10c402670090de1c`  
		Last Modified: Tue, 08 Aug 2023 00:50:16 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:alpine3.18` - linux; s390x

```console
$ docker pull memcached@sha256:cd97d93e79c2345a0c10f20a912f29a0ccf5590e15c00df81596397b9567233f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4278263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f56d14fce8cfd200c86bd00cd28c95574b6bf2863bd203e7644d44a08db84ab`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 15 Jun 2023 05:18:38 GMT
ADD file:a59beca78118ebf4f86cc1685237dc3a29a519401a70668da520beaa3d29eb7a in / 
# Thu, 15 Jun 2023 05:18:38 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:27:47 GMT
RUN addgroup -g 11211 memcache && adduser -D -u 11211 -G memcache memcache
# Thu, 15 Jun 2023 06:27:49 GMT
RUN apk add --no-cache libsasl
# Wed, 21 Jun 2023 00:58:01 GMT
ENV MEMCACHED_VERSION=1.6.21
# Wed, 21 Jun 2023 00:58:01 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Wed, 21 Jun 2023 01:01:08 GMT
RUN set -x 		&& apk add --no-cache --virtual .build-deps 		ca-certificates 		coreutils 		cyrus-sasl-dev 		gcc 		libc-dev 		libevent-dev 		linux-headers 		make 		openssl 		openssl-dev 		perl 		perl-io-socket-ssl 		perl-utils 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& ./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& make test PARALLEL="$nproc" 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& apk add --no-network --virtual .memcached-rundeps $runDeps 	&& apk del --no-network .build-deps 		&& memcached -V
# Wed, 21 Jun 2023 01:01:09 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Wed, 21 Jun 2023 01:01:09 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Wed, 21 Jun 2023 01:01:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 21 Jun 2023 01:01:09 GMT
USER memcache
# Wed, 21 Jun 2023 01:01:10 GMT
EXPOSE 11211
# Wed, 21 Jun 2023 01:01:10 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:998cc98447b44e5f0fe799dce691412796ba586ab22eb7c99aebf9d45f34833b`  
		Last Modified: Thu, 15 Jun 2023 05:29:38 GMT  
		Size: 3.2 MB (3213497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156deb87465a2c5629e5ae28c2a7251d5684baea5a930cf65ff6b478de321202`  
		Last Modified: Thu, 15 Jun 2023 06:36:33 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19020c60d58f4724218660e819b1b33b5d1428c3c5027492a2ee3c44228231df`  
		Last Modified: Thu, 15 Jun 2023 06:36:33 GMT  
		Size: 112.8 KB (112849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e76f938f015ccb0b5d2915145432efbc0af21a2f4964e0c9a67bfbbe6a577e`  
		Last Modified: Wed, 21 Jun 2023 01:01:46 GMT  
		Size: 950.3 KB (950254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b613e0a69ced3425a5949c15688d493ef10d80eb28c7bb626f0c092223fe1302`  
		Last Modified: Wed, 21 Jun 2023 01:01:46 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db4c30d38bb65cd11068e1892913b2fa04add8f27abe601485cc3b09754eb50`  
		Last Modified: Wed, 21 Jun 2023 01:01:46 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:bookworm`

```console
$ docker pull memcached@sha256:a917777975a7039b6ed70ef2faab453b1e5ea7aa741899aba952d744546cc781
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `memcached:bookworm` - linux; amd64

```console
$ docker pull memcached@sha256:0c8398104f83351267e51ec72b34de06b734f2eca6637c10d246702afff814b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.0 MB (38974916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:354b899e400fa323ffaea769644cc66778676b4f4eeca0e3e1523100e8803d97`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:44 GMT
ADD file:209589a8bdb5a3788ee42ecdbccbbb561835dab96b0d8286bb5a2229d2f41be7 in / 
# Thu, 27 Jul 2023 23:24:45 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 04:03:18 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 28 Jul 2023 04:03:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 04:03:22 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 28 Jul 2023 04:03:22 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 28 Jul 2023 04:05:37 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 28 Jul 2023 04:05:37 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 28 Jul 2023 04:05:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 04:05:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 04:05:38 GMT
USER memcache
# Fri, 28 Jul 2023 04:05:38 GMT
EXPOSE 11211
# Fri, 28 Jul 2023 04:05:38 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:648e0aadf75ac2ef63c5390adc6dc14fde37a5ad88c2870ea604df0a9c0eb4e5`  
		Last Modified: Thu, 27 Jul 2023 23:29:26 GMT  
		Size: 29.1 MB (29124532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baaf8e9cef6b92919a723712ed912794373f6fc1d8dac9d5ed1d320378f657ba`  
		Last Modified: Fri, 28 Jul 2023 04:05:56 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52dca4bf886a56187b224e812b7a65f7825798dc8d536db9bb9344cb112b98e0`  
		Last Modified: Fri, 28 Jul 2023 04:05:56 GMT  
		Size: 2.7 MB (2677283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6861252b28dd75ed1a4f9accdcef6f35366a5dd59d3d7921945a20ec3f64661`  
		Last Modified: Fri, 28 Jul 2023 04:05:57 GMT  
		Size: 7.2 MB (7171562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49870ab6c52b8db6c693e18bd63b718827cd451bde693287ca70314a991cbfb6`  
		Last Modified: Fri, 28 Jul 2023 04:05:56 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da541564580ce27d2c3710f1420b22d4bc544196f1bf6536a5c58150854283d`  
		Last Modified: Fri, 28 Jul 2023 04:05:56 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bookworm` - linux; arm variant v5

```console
$ docker pull memcached@sha256:ec7dc6727737267a059c047a43864e1c5bdda0a6b8d3cdd0b49110523acfe7f7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35098422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8ce1a3d6a1d0c9162fa735664905dded291bfaa1a0398a381448950a7b9ee91`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 27 Jul 2023 23:48:29 GMT
ADD file:53cf36eb7b72a7e970f4b18af1589402b2900f12e30820cdeccc8bb0c166df80 in / 
# Thu, 27 Jul 2023 23:48:30 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 11:05:31 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 28 Jul 2023 11:05:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 11:05:37 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 28 Jul 2023 11:05:37 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 28 Jul 2023 11:08:31 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 28 Jul 2023 11:08:31 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 28 Jul 2023 11:08:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 11:08:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 11:08:31 GMT
USER memcache
# Fri, 28 Jul 2023 11:08:31 GMT
EXPOSE 11211
# Fri, 28 Jul 2023 11:08:32 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2bd6dfc5281e13a0ca9fb8d9238ac9f14a0de04489913030c8e33b9398b4a4af`  
		Last Modified: Thu, 27 Jul 2023 23:51:28 GMT  
		Size: 27.0 MB (26983508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5936d9d99182ef30677e20dad76c0549b2b7612ca100ef6c0f03c87027cee0b`  
		Last Modified: Fri, 28 Jul 2023 11:08:45 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7717a35af981145073f1343f8447ffd5b5c52de46680b1e75e4c0c11ba64bf`  
		Last Modified: Fri, 28 Jul 2023 11:08:46 GMT  
		Size: 2.3 MB (2281851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56b5203e649ffe900465b0cf521d6be756bd5dd83b5905d7ccc6aced143610b`  
		Last Modified: Fri, 28 Jul 2023 11:08:47 GMT  
		Size: 5.8 MB (5831523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6dee9c51b3b15c0179684c9c61eebfc3091a8f40afd9714ddae2728364aee4f`  
		Last Modified: Fri, 28 Jul 2023 11:08:45 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51b980bae702ef385ef2cbe3eb556c8377334b4c31c97e39cced7ed58375bc55`  
		Last Modified: Fri, 28 Jul 2023 11:08:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bookworm` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:4b2d19d8c0d48b44b1f24b2ea0e8a62749f05db1bedbe481ff6112db44c703cc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.9 MB (37878121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c74af541d05a0758cbf5f13d5d190f1ab10b86ef5fd75112aa98b0638def7d9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 27 Jul 2023 23:43:00 GMT
ADD file:1de2ba0dc88aa343332814e19adc6b850d08e62c31589fe902b8eb2cb465934e in / 
# Thu, 27 Jul 2023 23:43:00 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 06:38:57 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 28 Jul 2023 06:39:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 06:39:01 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 28 Jul 2023 06:39:01 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 28 Jul 2023 06:41:36 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 28 Jul 2023 06:41:36 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 28 Jul 2023 06:41:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 06:41:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 06:41:37 GMT
USER memcache
# Fri, 28 Jul 2023 06:41:37 GMT
EXPOSE 11211
# Fri, 28 Jul 2023 06:41:37 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:90524f7dc01b4ce9b387992acc6cbdbcc2a9ee8c6addfd632429ca06ea18751e`  
		Last Modified: Thu, 27 Jul 2023 23:46:17 GMT  
		Size: 29.2 MB (29157226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6146d0684a3303f06ef62333440ab9aba6cab719b5762ddaee7f7b7a3a62e9ee`  
		Last Modified: Fri, 28 Jul 2023 06:42:01 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b513dbaa02d89264c8df677c8871ec60a8cba234a96d77165fc06157ed2ec1f`  
		Last Modified: Fri, 28 Jul 2023 06:42:01 GMT  
		Size: 2.5 MB (2539192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe211375d2d86acd694c377eeaf6fe900e6f57dadd07e6bd6f21809eab75c53a`  
		Last Modified: Fri, 28 Jul 2023 06:42:02 GMT  
		Size: 6.2 MB (6180162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1b4b070b2921c7d9f5349e7b258c1400ac5d0a1154df0028e634899e86fbda`  
		Last Modified: Fri, 28 Jul 2023 06:42:01 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d40396358d46edf0c2615a77e13da10249786f2546d4a9623e18ec0ce9d6aa91`  
		Last Modified: Fri, 28 Jul 2023 06:42:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bookworm` - linux; 386

```console
$ docker pull memcached@sha256:d3e70a847a7f720a3a129c6e060b3f9b3428add5e0458c1974a6a895783073e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39459484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fe4fee0ccc34611e17f9be47d4048890aa66e445397fb679f2f27edcb5de08a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 27 Jul 2023 23:38:56 GMT
ADD file:3d6e6f3e900e480a7e060fcaf57313c0f954bf906967a7fa0317567c387cf5aa in / 
# Thu, 27 Jul 2023 23:38:57 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 00:12:30 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 28 Jul 2023 00:12:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 00:12:35 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 28 Jul 2023 00:12:35 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 28 Jul 2023 00:16:17 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 28 Jul 2023 00:16:17 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 28 Jul 2023 00:16:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 00:16:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 00:16:18 GMT
USER memcache
# Fri, 28 Jul 2023 00:16:18 GMT
EXPOSE 11211
# Fri, 28 Jul 2023 00:16:18 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3a8b0c4b1a83609d978d576be6174f951ff27084d7c9aef91892b60b223a5104`  
		Last Modified: Thu, 27 Jul 2023 23:43:26 GMT  
		Size: 30.1 MB (30141788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:700ff590600873a2721ed53371f8797b79c09c48cf32c7190640b4a1d4f5755d`  
		Last Modified: Fri, 28 Jul 2023 00:16:36 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f15bfc1eebf505da6ff5a5b1b1810ad762b79725e742a9b354c57fbabd31f01a`  
		Last Modified: Fri, 28 Jul 2023 00:16:37 GMT  
		Size: 2.7 MB (2685093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80fdef0976acae3ce13d23a176fc9e9ce15eeb2ac874a0915725bbaa3108059b`  
		Last Modified: Fri, 28 Jul 2023 00:16:38 GMT  
		Size: 6.6 MB (6631063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3442227f7348458fb36b2e0d739658a8fb589ed322fd578df8e39e59fc32000d`  
		Last Modified: Fri, 28 Jul 2023 00:16:36 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5501a93139182f8a01992f6de5a5e4eaebdebaaec5a10506a07f59b936d266e6`  
		Last Modified: Fri, 28 Jul 2023 00:16:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bookworm` - linux; mips64le

```console
$ docker pull memcached@sha256:fbc5c08e8c901f9b6c9cab47733639d29f3ff1167ab861aa26fe0bb751a308d9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.6 MB (37558667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f390b2a92aa8ce938675a24263c1e7f6b619c4c584343f3dd7a0e9d6615051d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 27 Jul 2023 23:11:23 GMT
ADD file:90cbcf9a2aaf48a433b00118dd0821eeb291092da7b7f67ce6a525ce2cba1e3f in / 
# Thu, 27 Jul 2023 23:11:27 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:45:56 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 28 Jul 2023 01:46:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:46:17 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 28 Jul 2023 01:46:19 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 28 Jul 2023 01:53:01 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 28 Jul 2023 01:53:03 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 28 Jul 2023 01:53:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 01:53:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 01:53:14 GMT
USER memcache
# Fri, 28 Jul 2023 01:53:16 GMT
EXPOSE 11211
# Fri, 28 Jul 2023 01:53:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3252778e08fa8eb67ab052ad63281284b5ef1afdc40a36021228133487ab5d52`  
		Last Modified: Thu, 27 Jul 2023 23:22:26 GMT  
		Size: 29.1 MB (29121405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63e55e013f2ab63ff93eaaf154b0debea8de9ffc8fbadaf67d3bc03851f57910`  
		Last Modified: Fri, 28 Jul 2023 01:53:46 GMT  
		Size: 1.1 KB (1082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d9a9f24853cb0188d2273603847b46ed81bd544b868ae314d609c1d9e7db7c`  
		Last Modified: Fri, 28 Jul 2023 01:53:48 GMT  
		Size: 1.9 MB (1934904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4467025968ec633fd090be17fe8c5f61d7ee738a0b34a10db006d35397e27cc`  
		Last Modified: Fri, 28 Jul 2023 01:53:51 GMT  
		Size: 6.5 MB (6500867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07da0cd083ab7d3e91ac9e7ae33d316bd7affeb2852262ff2d687be0e5c273b6`  
		Last Modified: Fri, 28 Jul 2023 01:53:46 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57f5929847506e0cf79067f8348bd883548c83f0c23defbaccf512eb17d65758`  
		Last Modified: Fri, 28 Jul 2023 01:53:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bookworm` - linux; ppc64le

```console
$ docker pull memcached@sha256:a32969620e95d4b08d5711678e6bcbd313e3bc3511d1b96cf5d08e675a90d0fb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43196803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d6a8d8d3e6746723698507be3f910bb02f0a22617da462f56031004e606edf6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 27 Jul 2023 23:23:01 GMT
ADD file:774a99e5c40757d27c981eb5ad6e03eb72970bb0c54f799eab1442624238ea3e in / 
# Thu, 27 Jul 2023 23:23:03 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:38:39 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 28 Jul 2023 03:38:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:38:51 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 28 Jul 2023 03:38:52 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 28 Jul 2023 03:42:57 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 28 Jul 2023 03:42:58 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 28 Jul 2023 03:43:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 03:43:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 03:43:01 GMT
USER memcache
# Fri, 28 Jul 2023 03:43:02 GMT
EXPOSE 11211
# Fri, 28 Jul 2023 03:43:03 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:ad974e0ada84177d519dec70d0d7d9ff6a4f468bc7306425feb8429bc276bd8a`  
		Last Modified: Thu, 27 Jul 2023 23:29:24 GMT  
		Size: 33.1 MB (33119211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ed68aff2ca1a6e8c25d8462f4b2ebbb3866c768911785569560ede6a2f053d`  
		Last Modified: Fri, 28 Jul 2023 03:43:33 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d519acbf803e11e9a1e21f396dd4e021495fa7b97a4c9df3e6f7639d8c050790`  
		Last Modified: Fri, 28 Jul 2023 03:43:33 GMT  
		Size: 2.9 MB (2891351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:097534b38ed1845470192cab29ec2d22d4e0c7a9d5f01c9948ebc1273dfe809c`  
		Last Modified: Fri, 28 Jul 2023 03:43:35 GMT  
		Size: 7.2 MB (7184700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2f9c6ce8e611c611c0bfdb7cb8ec798950618d80a9be8db98c59fdd0654825`  
		Last Modified: Fri, 28 Jul 2023 03:43:33 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d974aa6a849abcd290ae3bbfbc44f776e3928269bfa1bdbc65e2a1f11c368afe`  
		Last Modified: Fri, 28 Jul 2023 03:43:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:bookworm` - linux; s390x

```console
$ docker pull memcached@sha256:1ab909233ee99a6798929725205b93abb2bd9a8c78ab048d925dffd359fe8cf2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35910248 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:845b0ff32d8c04c5820146361e7a2e8c8579ad2a96318fdbc7e6c669bfc27569`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 27 Jul 2023 23:47:11 GMT
ADD file:0a5e1e86b375d60637d0829f77a12085777cf2ca07495b0f6249d8efea84e958 in / 
# Thu, 27 Jul 2023 23:47:13 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 02:58:10 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 28 Jul 2023 02:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 02:58:13 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 28 Jul 2023 02:58:13 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 28 Jul 2023 03:01:19 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 28 Jul 2023 03:01:20 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 28 Jul 2023 03:01:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 03:01:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 03:01:20 GMT
USER memcache
# Fri, 28 Jul 2023 03:01:20 GMT
EXPOSE 11211
# Fri, 28 Jul 2023 03:01:21 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f4301d25bb1bea85fcc5b364aec84ff58274f714cea191ab22d9b1b1e4f78527`  
		Last Modified: Thu, 27 Jul 2023 23:52:17 GMT  
		Size: 27.5 MB (27489697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8055eb96c9dacdcc9c91194a8d4504ab82a88a0fa9f927413c1dde2e493a815`  
		Last Modified: Fri, 28 Jul 2023 03:01:51 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:040e9d91e418b36f9ea07fcd1d9db85ae7713bd99a0a17f31f41a7ef410c3423`  
		Last Modified: Fri, 28 Jul 2023 03:01:54 GMT  
		Size: 2.3 MB (2345395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a638c5b62a02bc60b52234e1556bcf148e66b74e50a0bd02d2b5f23ea2ee136d`  
		Last Modified: Fri, 28 Jul 2023 03:01:52 GMT  
		Size: 6.1 MB (6073620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c41c8e1cb6d4df65052cc47729124edceae5af653ff6a3555cf6e69a57f6de1`  
		Last Modified: Fri, 28 Jul 2023 03:01:51 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2516714a4b2b11720bd2fcf5338749e05ae2dff40f716814b7531fcbe356fdce`  
		Last Modified: Fri, 28 Jul 2023 03:01:51 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `memcached:latest`

```console
$ docker pull memcached@sha256:daa7eae2d45bc644f697eed288cff1460c73a7b44c291770014eb16c2ef6ff99
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
$ docker pull memcached@sha256:0c8398104f83351267e51ec72b34de06b734f2eca6637c10d246702afff814b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.0 MB (38974916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:354b899e400fa323ffaea769644cc66778676b4f4eeca0e3e1523100e8803d97`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:44 GMT
ADD file:209589a8bdb5a3788ee42ecdbccbbb561835dab96b0d8286bb5a2229d2f41be7 in / 
# Thu, 27 Jul 2023 23:24:45 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 04:03:18 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 28 Jul 2023 04:03:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 04:03:22 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 28 Jul 2023 04:03:22 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 28 Jul 2023 04:05:37 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 28 Jul 2023 04:05:37 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 28 Jul 2023 04:05:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 04:05:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 04:05:38 GMT
USER memcache
# Fri, 28 Jul 2023 04:05:38 GMT
EXPOSE 11211
# Fri, 28 Jul 2023 04:05:38 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:648e0aadf75ac2ef63c5390adc6dc14fde37a5ad88c2870ea604df0a9c0eb4e5`  
		Last Modified: Thu, 27 Jul 2023 23:29:26 GMT  
		Size: 29.1 MB (29124532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baaf8e9cef6b92919a723712ed912794373f6fc1d8dac9d5ed1d320378f657ba`  
		Last Modified: Fri, 28 Jul 2023 04:05:56 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52dca4bf886a56187b224e812b7a65f7825798dc8d536db9bb9344cb112b98e0`  
		Last Modified: Fri, 28 Jul 2023 04:05:56 GMT  
		Size: 2.7 MB (2677283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6861252b28dd75ed1a4f9accdcef6f35366a5dd59d3d7921945a20ec3f64661`  
		Last Modified: Fri, 28 Jul 2023 04:05:57 GMT  
		Size: 7.2 MB (7171562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49870ab6c52b8db6c693e18bd63b718827cd451bde693287ca70314a991cbfb6`  
		Last Modified: Fri, 28 Jul 2023 04:05:56 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da541564580ce27d2c3710f1420b22d4bc544196f1bf6536a5c58150854283d`  
		Last Modified: Fri, 28 Jul 2023 04:05:56 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; arm variant v5

```console
$ docker pull memcached@sha256:ec7dc6727737267a059c047a43864e1c5bdda0a6b8d3cdd0b49110523acfe7f7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35098422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8ce1a3d6a1d0c9162fa735664905dded291bfaa1a0398a381448950a7b9ee91`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 27 Jul 2023 23:48:29 GMT
ADD file:53cf36eb7b72a7e970f4b18af1589402b2900f12e30820cdeccc8bb0c166df80 in / 
# Thu, 27 Jul 2023 23:48:30 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 11:05:31 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 28 Jul 2023 11:05:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 11:05:37 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 28 Jul 2023 11:05:37 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 28 Jul 2023 11:08:31 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 28 Jul 2023 11:08:31 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 28 Jul 2023 11:08:31 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 11:08:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 11:08:31 GMT
USER memcache
# Fri, 28 Jul 2023 11:08:31 GMT
EXPOSE 11211
# Fri, 28 Jul 2023 11:08:32 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2bd6dfc5281e13a0ca9fb8d9238ac9f14a0de04489913030c8e33b9398b4a4af`  
		Last Modified: Thu, 27 Jul 2023 23:51:28 GMT  
		Size: 27.0 MB (26983508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5936d9d99182ef30677e20dad76c0549b2b7612ca100ef6c0f03c87027cee0b`  
		Last Modified: Fri, 28 Jul 2023 11:08:45 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7717a35af981145073f1343f8447ffd5b5c52de46680b1e75e4c0c11ba64bf`  
		Last Modified: Fri, 28 Jul 2023 11:08:46 GMT  
		Size: 2.3 MB (2281851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56b5203e649ffe900465b0cf521d6be756bd5dd83b5905d7ccc6aced143610b`  
		Last Modified: Fri, 28 Jul 2023 11:08:47 GMT  
		Size: 5.8 MB (5831523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6dee9c51b3b15c0179684c9c61eebfc3091a8f40afd9714ddae2728364aee4f`  
		Last Modified: Fri, 28 Jul 2023 11:08:45 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51b980bae702ef385ef2cbe3eb556c8377334b4c31c97e39cced7ed58375bc55`  
		Last Modified: Fri, 28 Jul 2023 11:08:45 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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
$ docker pull memcached@sha256:4b2d19d8c0d48b44b1f24b2ea0e8a62749f05db1bedbe481ff6112db44c703cc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.9 MB (37878121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c74af541d05a0758cbf5f13d5d190f1ab10b86ef5fd75112aa98b0638def7d9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 27 Jul 2023 23:43:00 GMT
ADD file:1de2ba0dc88aa343332814e19adc6b850d08e62c31589fe902b8eb2cb465934e in / 
# Thu, 27 Jul 2023 23:43:00 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 06:38:57 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 28 Jul 2023 06:39:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 06:39:01 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 28 Jul 2023 06:39:01 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 28 Jul 2023 06:41:36 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 28 Jul 2023 06:41:36 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 28 Jul 2023 06:41:37 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 06:41:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 06:41:37 GMT
USER memcache
# Fri, 28 Jul 2023 06:41:37 GMT
EXPOSE 11211
# Fri, 28 Jul 2023 06:41:37 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:90524f7dc01b4ce9b387992acc6cbdbcc2a9ee8c6addfd632429ca06ea18751e`  
		Last Modified: Thu, 27 Jul 2023 23:46:17 GMT  
		Size: 29.2 MB (29157226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6146d0684a3303f06ef62333440ab9aba6cab719b5762ddaee7f7b7a3a62e9ee`  
		Last Modified: Fri, 28 Jul 2023 06:42:01 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b513dbaa02d89264c8df677c8871ec60a8cba234a96d77165fc06157ed2ec1f`  
		Last Modified: Fri, 28 Jul 2023 06:42:01 GMT  
		Size: 2.5 MB (2539192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe211375d2d86acd694c377eeaf6fe900e6f57dadd07e6bd6f21809eab75c53a`  
		Last Modified: Fri, 28 Jul 2023 06:42:02 GMT  
		Size: 6.2 MB (6180162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1b4b070b2921c7d9f5349e7b258c1400ac5d0a1154df0028e634899e86fbda`  
		Last Modified: Fri, 28 Jul 2023 06:42:01 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d40396358d46edf0c2615a77e13da10249786f2546d4a9623e18ec0ce9d6aa91`  
		Last Modified: Fri, 28 Jul 2023 06:42:01 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; 386

```console
$ docker pull memcached@sha256:d3e70a847a7f720a3a129c6e060b3f9b3428add5e0458c1974a6a895783073e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39459484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fe4fee0ccc34611e17f9be47d4048890aa66e445397fb679f2f27edcb5de08a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 27 Jul 2023 23:38:56 GMT
ADD file:3d6e6f3e900e480a7e060fcaf57313c0f954bf906967a7fa0317567c387cf5aa in / 
# Thu, 27 Jul 2023 23:38:57 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 00:12:30 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 28 Jul 2023 00:12:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 00:12:35 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 28 Jul 2023 00:12:35 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 28 Jul 2023 00:16:17 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 28 Jul 2023 00:16:17 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 28 Jul 2023 00:16:18 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 00:16:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 00:16:18 GMT
USER memcache
# Fri, 28 Jul 2023 00:16:18 GMT
EXPOSE 11211
# Fri, 28 Jul 2023 00:16:18 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3a8b0c4b1a83609d978d576be6174f951ff27084d7c9aef91892b60b223a5104`  
		Last Modified: Thu, 27 Jul 2023 23:43:26 GMT  
		Size: 30.1 MB (30141788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:700ff590600873a2721ed53371f8797b79c09c48cf32c7190640b4a1d4f5755d`  
		Last Modified: Fri, 28 Jul 2023 00:16:36 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f15bfc1eebf505da6ff5a5b1b1810ad762b79725e742a9b354c57fbabd31f01a`  
		Last Modified: Fri, 28 Jul 2023 00:16:37 GMT  
		Size: 2.7 MB (2685093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80fdef0976acae3ce13d23a176fc9e9ce15eeb2ac874a0915725bbaa3108059b`  
		Last Modified: Fri, 28 Jul 2023 00:16:38 GMT  
		Size: 6.6 MB (6631063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3442227f7348458fb36b2e0d739658a8fb589ed322fd578df8e39e59fc32000d`  
		Last Modified: Fri, 28 Jul 2023 00:16:36 GMT  
		Size: 287.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5501a93139182f8a01992f6de5a5e4eaebdebaaec5a10506a07f59b936d266e6`  
		Last Modified: Fri, 28 Jul 2023 00:16:36 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; mips64le

```console
$ docker pull memcached@sha256:fbc5c08e8c901f9b6c9cab47733639d29f3ff1167ab861aa26fe0bb751a308d9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.6 MB (37558667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f390b2a92aa8ce938675a24263c1e7f6b619c4c584343f3dd7a0e9d6615051d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 27 Jul 2023 23:11:23 GMT
ADD file:90cbcf9a2aaf48a433b00118dd0821eeb291092da7b7f67ce6a525ce2cba1e3f in / 
# Thu, 27 Jul 2023 23:11:27 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:45:56 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 28 Jul 2023 01:46:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:46:17 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 28 Jul 2023 01:46:19 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 28 Jul 2023 01:53:01 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 28 Jul 2023 01:53:03 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 28 Jul 2023 01:53:08 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 01:53:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 01:53:14 GMT
USER memcache
# Fri, 28 Jul 2023 01:53:16 GMT
EXPOSE 11211
# Fri, 28 Jul 2023 01:53:19 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:3252778e08fa8eb67ab052ad63281284b5ef1afdc40a36021228133487ab5d52`  
		Last Modified: Thu, 27 Jul 2023 23:22:26 GMT  
		Size: 29.1 MB (29121405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63e55e013f2ab63ff93eaaf154b0debea8de9ffc8fbadaf67d3bc03851f57910`  
		Last Modified: Fri, 28 Jul 2023 01:53:46 GMT  
		Size: 1.1 KB (1082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d9a9f24853cb0188d2273603847b46ed81bd544b868ae314d609c1d9e7db7c`  
		Last Modified: Fri, 28 Jul 2023 01:53:48 GMT  
		Size: 1.9 MB (1934904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4467025968ec633fd090be17fe8c5f61d7ee738a0b34a10db006d35397e27cc`  
		Last Modified: Fri, 28 Jul 2023 01:53:51 GMT  
		Size: 6.5 MB (6500867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07da0cd083ab7d3e91ac9e7ae33d316bd7affeb2852262ff2d687be0e5c273b6`  
		Last Modified: Fri, 28 Jul 2023 01:53:46 GMT  
		Size: 288.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57f5929847506e0cf79067f8348bd883548c83f0c23defbaccf512eb17d65758`  
		Last Modified: Fri, 28 Jul 2023 01:53:46 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; ppc64le

```console
$ docker pull memcached@sha256:a32969620e95d4b08d5711678e6bcbd313e3bc3511d1b96cf5d08e675a90d0fb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43196803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d6a8d8d3e6746723698507be3f910bb02f0a22617da462f56031004e606edf6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 27 Jul 2023 23:23:01 GMT
ADD file:774a99e5c40757d27c981eb5ad6e03eb72970bb0c54f799eab1442624238ea3e in / 
# Thu, 27 Jul 2023 23:23:03 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:38:39 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 28 Jul 2023 03:38:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:38:51 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 28 Jul 2023 03:38:52 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 28 Jul 2023 03:42:57 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 28 Jul 2023 03:42:58 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 28 Jul 2023 03:43:00 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 03:43:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 03:43:01 GMT
USER memcache
# Fri, 28 Jul 2023 03:43:02 GMT
EXPOSE 11211
# Fri, 28 Jul 2023 03:43:03 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:ad974e0ada84177d519dec70d0d7d9ff6a4f468bc7306425feb8429bc276bd8a`  
		Last Modified: Thu, 27 Jul 2023 23:29:24 GMT  
		Size: 33.1 MB (33119211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ed68aff2ca1a6e8c25d8462f4b2ebbb3866c768911785569560ede6a2f053d`  
		Last Modified: Fri, 28 Jul 2023 03:43:33 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d519acbf803e11e9a1e21f396dd4e021495fa7b97a4c9df3e6f7639d8c050790`  
		Last Modified: Fri, 28 Jul 2023 03:43:33 GMT  
		Size: 2.9 MB (2891351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:097534b38ed1845470192cab29ec2d22d4e0c7a9d5f01c9948ebc1273dfe809c`  
		Last Modified: Fri, 28 Jul 2023 03:43:35 GMT  
		Size: 7.2 MB (7184700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2f9c6ce8e611c611c0bfdb7cb8ec798950618d80a9be8db98c59fdd0654825`  
		Last Modified: Fri, 28 Jul 2023 03:43:33 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d974aa6a849abcd290ae3bbfbc44f776e3928269bfa1bdbc65e2a1f11c368afe`  
		Last Modified: Fri, 28 Jul 2023 03:43:33 GMT  
		Size: 121.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `memcached:latest` - linux; s390x

```console
$ docker pull memcached@sha256:1ab909233ee99a6798929725205b93abb2bd9a8c78ab048d925dffd359fe8cf2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35910248 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:845b0ff32d8c04c5820146361e7a2e8c8579ad2a96318fdbc7e6c669bfc27569`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Thu, 27 Jul 2023 23:47:11 GMT
ADD file:0a5e1e86b375d60637d0829f77a12085777cf2ca07495b0f6249d8efea84e958 in / 
# Thu, 27 Jul 2023 23:47:13 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 02:58:10 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache
# Fri, 28 Jul 2023 02:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 02:58:13 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 28 Jul 2023 02:58:13 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 28 Jul 2023 03:01:19 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V
# Fri, 28 Jul 2023 03:01:20 GMT
COPY file:bf641b13ea5b37f5830b299ebe9d72f194ee5d897db14faf8b133dc7a66a48ad in /usr/local/bin/ 
# Fri, 28 Jul 2023 03:01:20 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat
# Fri, 28 Jul 2023 03:01:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 28 Jul 2023 03:01:20 GMT
USER memcache
# Fri, 28 Jul 2023 03:01:20 GMT
EXPOSE 11211
# Fri, 28 Jul 2023 03:01:21 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f4301d25bb1bea85fcc5b364aec84ff58274f714cea191ab22d9b1b1e4f78527`  
		Last Modified: Thu, 27 Jul 2023 23:52:17 GMT  
		Size: 27.5 MB (27489697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8055eb96c9dacdcc9c91194a8d4504ab82a88a0fa9f927413c1dde2e493a815`  
		Last Modified: Fri, 28 Jul 2023 03:01:51 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:040e9d91e418b36f9ea07fcd1d9db85ae7713bd99a0a17f31f41a7ef410c3423`  
		Last Modified: Fri, 28 Jul 2023 03:01:54 GMT  
		Size: 2.3 MB (2345395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a638c5b62a02bc60b52234e1556bcf148e66b74e50a0bd02d2b5f23ea2ee136d`  
		Last Modified: Fri, 28 Jul 2023 03:01:52 GMT  
		Size: 6.1 MB (6073620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c41c8e1cb6d4df65052cc47729124edceae5af653ff6a3555cf6e69a57f6de1`  
		Last Modified: Fri, 28 Jul 2023 03:01:51 GMT  
		Size: 286.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2516714a4b2b11720bd2fcf5338749e05ae2dff40f716814b7531fcbe356fdce`  
		Last Modified: Fri, 28 Jul 2023 03:01:51 GMT  
		Size: 118.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
